---
Title: >-
  GA4-GTM Donor Journey - AI Prompt for a Donor Journey for NWF | Analytics
  Audit
Client: National Wildlife Federation
Status:
  - In Progress
tags:
  - NWF
  - aiprompt
  - analytics

---



### Ai Prompt for a Donor Journey for NWF

#NWF 

We have a non-profit client that would like to be able to track the customer journey a bit better on their site and on their donation forms. They want to be able to extract more data from their donor's journey especially so that it can be better recognized and captured in GA4. Here is what our client said they want to figure out. "We are running into Google Ads and other PPC don’t understand nonprofit ecommerce - we would like to figure out how to better standardize Donor ecommerce journey through our site and donation forms, where google would recognize that a donor started but not complete. These supporters have intent but didn’t make it through the journey. Or if card was denied and they gave up - something like this. " Please recommend the best way to achieve this for our clients. Provide detailed step by step instruction and exactly what to do, what strategy to implement and the exact Events and triggers to setup

- Double the Donation - delay in both of these - could they be included?

- Chariot/DAFpay - delay in both of these - could they be included?

## Answer from Chat:

You’ll get what they want by treating donations *exactly* like ecommerce in GA4, then tracking each step of the funnel (start → form view → fields filled → payment submitted → success / fail) with clear events that Google Ads can bid on and build audiences from.

Below is a concrete, “just do this” plan.

---

## 1. Strategy: Standardize the donation funnel as ecommerce

**Goal:** Make every donation path look like a clean ecommerce checkout to GA4 & Google Ads so we can:

- See *where* donors drop off (PPC vs organic, etc.).

- Build audiences of “started but not completed.”

- Measure declines/errors separately.

**We’ll model the funnel like this:**

1. **Donation intent** → `donate_click`

2. **Form loaded** → `view_item` or `view_donation_form` (custom)

3. **Checkout started** → `begin_checkout`

4. **Payment details submitted** → `add_payment_info`

5. **Purchase complete** → `purchase`

6. **Card declined / error** → `payment_error` (custom)

We’ll stick as closely as possible to GA4’s **recommended ecommerce events** (`begin_checkout`, `add_payment_info`, `purchase`) so they auto-feed Monetization reports and ecommerce funnels. ([Google for Developers](https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?utm_source=chatgpt.com))

---

## 2. Prereqs: Make sure foundation is solid

1. **Confirm GA4 + GTM (Google Tag Manager) setup**

   - GA4 property is live and receiving data.

   - GA4 configuration tag is deployed via GTM on:

     - Main site (`www.example.org`)

     - Donation forms (subdomain, directory, or third-party if allowed).

2. **Cross-domain tracking** (if forms are on another domain, e.g. `donate.example.org` or vendor domain)

   - In GA4 Admin → Data streams → Web stream → **Configure tag settings** → **Configure your domains**.

   - Add rules like:

     - `example.org`

     - `donate.example.org`

     - Vendor domains if you can support client-side tagging & link decoration.

   - Ensure GTM GA4 configuration tag has **“Allow linker”** enabled (if using gtag template, this is automatic once GA4 domain linking is configured).

3. **Decide: data layer vs. scraped DOM**

   - **Best:** donation platform exposes a **data layer** object with transaction data (`items`, `value`, `currency`, `transaction_id`, error codes).

   - **Fallback:** use CSS selectors / URL patterns to identify key steps; later evolve to a data layer when possible.

---

## 3. Event architecture: what we will track

Here’s the canonical event set I recommend for nonprofits:

### 3.1 Funnel “spine” (recommended events)

1. `donate_click` **(custom but simple)**

   - Fired when someone clicks any primary Donate CTA.

   - Parameters:

     - `button_location` (header, homepage_hero, appeal_page, etc.)

     - `campaign` (if specific: giving_tuesday, year_end, etc.)

2. `begin_checkout` **(GA4 recommended)**

   - Fired when the actual donation form loads with a visible amount field.

   - Parameters:

     - `items`: array with at least one object:

       - `item_name`: "Donation"

       - `item_category`: "Donation"

       - `price`: default pre-selected amount (if any)

       - `currency`: "USD" (or appropriate)

     - `campaign` (optional, but useful)

   - This marks “they actually started the donation process.”

3. `add_payment_info` **(GA4 recommended)**

   - Fired when the donor clicks the “Donate/Submit payment” button (after filling name/card fields), *regardless*of success.

   - Parameters:

     - Same `items` array as above (but now with chosen amount).

     - `value`: full donation amount.

     - `payment_type`: e.g. `credit_card`, `paypal`, `ach`.

   - This is your “strong intent” signal to import as a **secondary conversion** into Google Ads (for optimization and remarketing) without conflating with actual donations. ([ayudante.asia](https://ayudante.asia/sparkline-blog/ga4-how-to-understand-the-ecommerce-performance-on-google-analytics-4?utm_source=chatgpt.com))

4. `purchase` **(GA4 recommended)**

   - Fired only on successful completion (thank-you page OR success callback).

   - Parameters:

     - `transaction_id`: unique donation ID.

     - `value`: final donation amount.

     - `currency`: "USD" etc.

     - `items`: same array with donation as the “product.”

   - This populates Monetization → Ecommerce in GA4. ([Google for Developers](https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?utm_source=chatgpt.com))

### 3.2 Error / abandonment helpers

5. `payment_error` **(custom)**

   - Fired when the platform returns a declined card / gateway error.

   - Parameters:

     - `error_code`: technical code from gateway if available (e.g. `card_declined`, `insufficient_funds`).

     - `error_message_short`: sanitized, non-PII message category (e.g. `validation_error`, `gateway_timeout`).

     - `value`: donation value attempted.

   - This lets you quantify “they *tried* but failed.”

6. `donation_form_abandon` **(custom, optional)**

   - Fired if user reaches `begin_checkout` but never hits `add_payment_info` within a time window (e.g. 30+ seconds and navigates away).

   - This is a bit more advanced (often done via GTM timers or GA4 audiences, see below).

---

## 4. GTM build: tags & triggers step by step

I’ll assume web GTM. Adjust names to your conventions.

### 4.1 Create base GA4 configuration tag

1. In GTM → **Tags** → **New** → *GA4 Configuration*.

2. Measurement ID: from GA4 → Admin → Data Stream.

3. Trigger: **All Pages** across main + donation domains.

4. Save & publish (or at least ready to test in Preview).

### 4.2 `donate_click` event tag

**Trigger strategy:** click trigger on main Donate buttons.

1. **Create a click trigger**

   - Triggers → New → *Click – All Elements* (or *Just Links*).

   - Choose “Some Clicks.”

   - Condition examples:

     - `Click Text` contains “Donate”

     - OR `Click Classes` contains `btn-donate`

     - Or precise selector as needed.

   - Name: `Click – Donate CTA`.

2. **Create event tag**

   - Tags → New → *GA4 Event*.

   - Configuration tag: your GA4 config.

   - Event name: `donate_click`.

   - Event parameters:

     - `button_location` → Variable (e.g. custom JS or DOM variable, or a constant for now).

     - `campaign` → Variable (read from data attribute or URL `utm_campaign`).

   - Trigger: `Click – Donate CTA`.

### 4.3 `begin_checkout` event tag

**Trigger strategy:** page view of the main donation form step (URL or dataLayer flag).

1. **Create trigger**

   - If forms live on URL like `/donate`:

     - Trigger type: *Page View – DOM Ready*.

     - Some page views:

       - `Page Path` equals `/donate`

       - Or `Page URL` contains `/donate`.

   - If using embedded iframe / EN / Classy, might be:

     - Custom event (e.g. `en_form_loaded`, `classy:formReady`) from vendor’s data layer.

   - Name: `PV – Donation Form`.

2. **Create event tag**

   - Tag type: GA4 Event.

   - Event name: `begin_checkout`.

   - Event parameters:

     - `items` → Data Layer variable that returns the GA4 ecommerce `items` array, or:

       - Use Constant/JS variable with minimal object:

       ```js
       [{
         item_name: 'Donation',
         item_category: 'Donation',
         currency: 'USD'
       }]
       
       ```

     - `campaign` → from UTM or hidden field (Variable).

   - Trigger: `PV – Donation Form`.

### 4.4 `add_payment_info` event tag

**Trigger strategy:** click submit on donation form **before** API/gateway response.

1. **Create trigger**

   - If regular HTML form:

     - Trigger type: *Form Submission* OR *Click* on the submit button.

     - Filter to donation forms only:

       - `Form ID` equals `donationForm`

       - or `Page Path` contains `/donate`.

   - If vendor exposes custom event (e.g. `donation_submission_started`), use that.

   - Name: `Form – Donation Submit Click`.

2. **Create event tag**

   - Tag type: GA4 Event.

   - Event name: `add_payment_info`.

   - Event parameters (from data layer or inputs):

     - `value` → Variable `dlv.donationValue` or derived from field.

     - `currency` → "USD" or from data layer.

     - `payment_type` → variable from gateway or selected option.

     - `items` → same array as `begin_checkout` but with `price` set to chosen amount.

   - Trigger: `Form – Donation Submit Click`.

### 4.5 `purchase` event tag

**Trigger strategy:** thank-you page OR vendor success callback.

**Option A: Thank-you page URL**

1. **Trigger**

   - Type: *Page View – DOM Ready*.

   - Some page views:

     - `Page Path` equals `/donate/thank-you` (or vendor’s confirmation URL).

   - Name: `PV – Donation Thank You`.

2. **Tag**

   - Type: GA4 Event.

   - Event name: `purchase`.

   - Event params:

     - `transaction_id` → Data layer or querystring param.

     - `value` → donation amount.

     - `currency` → "USD".

     - `items` → donation item array.

   - Trigger: `PV – Donation Thank You`.

**Option B: Data-layer success event**

If the platform pushes something like:

```js
dataLayer.push({
  event: 'donation_success',
  ecommerce: {
    transaction_id: '12345',
    value: 50,
    currency: 'USD',
    items: [{ item_name: 'Donation', price: 50 }]
  }
});
```

1. Trigger type: *Custom Event* → `donation_success`.

2. Tag: GA4 Event → `purchase`.

3. Map parameters from `ecommerce` object via variables.

### 4.6 `payment_error` event tag

**Trigger strategy:** data layer event when gateway returns an error OR DOM observer that sees error message element.

**Data-layer example:**

```js
dataLayer.push({
  event: 'donation_error',
  error_code: 'card_declined',
  error_message_short: 'card_declined',
  attempted_value: 100,
  currency: 'USD'
});
```

1. Trigger

   - Type: Custom Event.

   - Event name: `donation_error`.

   - Name: `CE – Donation Error`.

2. Tag

   - GA4 Event.

   - Event name: `payment_error`.

   - Parameters:

     - `error_code` → `{{dlv.error_code}}`

     - `error_message_short` → `{{dlv.error_message_short}}`

     - `value` → `{{dlv.attempted_value}}`

     - `currency` → `{{dlv.currency}}`

   - Trigger: `CE – Donation Error`.

---

## 5. Identifying “started but did not complete”

You’ve now got a clean funnel: `begin_checkout` → `add_payment_info` → `purchase` / `payment_error`.

To specifically flag *“intent but no completion”*:

### 5.1 GA4 audiences

In GA4:

1. Admin → **Audiences** → New audience.

2. Define an audience like **“Donation Started – No Purchase”**:

   - Include users who:

     - `event_name` = `add_payment_info`

   - AND **exclude** users who:

     - `event_name` = `purchase` (within N days, e.g. 7).

3. Publish.

Link GA4 → Google Ads (if not already) and **import this audience** to Ads. ([Google Help](https://support.google.com/nonprofits/answer/9841491?hl=en&utm_source=chatgpt.com))

Now Ads can remarket to people who tried to donate but didn’t finish.

### 5.2 Audience for “Card declined / error”

Same idea:

- Include: `event_name` = `payment_error`.

- Exclude: `purchase` within 1–7 days.

Use this for softer messaging, “Having trouble finishing your donation?” etc.

---

## 6. Connect to Google Ads the *right* way

1. In GA4 → Admin → **Product Links** → Google Ads → Link account.

2. In GA4 → **Advertising** → Conversion Management:

   - Mark `purchase` as a **key event**.

   - Also consider marking `add_payment_info` and/or `begin_checkout` as key events (for upper-funnel measurement). ([Adswerve](https://adswerve.com/blog/google-ads-ga4-conversions-best-practices-recommendations?utm_source=chatgpt.com))

3. In **Google Ads**:

   - Tools & Settings → Conversions → New conversion action → **Import** → GA4.

   - Import:

     - `purchase` (core conversion; consider also a native Ads tag if you want maximum accuracy, but for Grants it’s often fine to use GA4 import).

     - `add_payment_info` as a **secondary** conversion (bid on or use mainly for optimization insights).

---

## 7. Handling “supporters with intent but didn’t complete”

Once events & audiences are live, you can:

1. **See drop-off in GA4**

   - Use **Explore → Funnel exploration**:

     - Step 1: `begin_checkout`

     - Step 2: `add_payment_info`

     - Step 3: (`purchase` OR `payment_error`)

   - Break down by:

     - `session_default_channel_group` (PPC vs email vs organic).

     - Campaign (`session_campaign` or UTM).

2. **Build PPC strategies**

   - Remarketing campaigns targeting:

     - Audience: `add_payment_info` but no `purchase`.

     - Audience: `payment_error` but no `purchase`.

   - Adjust ad copies & landing pages specific to these groups.

3. **Optimize the journey**

   - Look at:

     - Device (mobile vs desktop).

     - Form length.

     - Payment types with highest `payment_error` rates.

---

## 8. Implementation checklist (non-dev vs dev responsibilities)

**Non-Dev / Strategy-side**

1. Approve event names & parameters with the client.

2. Document:

   - All donation URLs / flows (one-time vs monthly, campaign vs general).

   - Expected thank-you URLs.

3. Define naming for:

   - `button_location`

   - `campaign` taxonomy.

**Dev-side**

1. Ensure data layer pushes on:

   - Donation form view.

   - Submission start.

   - Success.

   - Error.

2. Add any custom events needed from the vendor platform.

3. Implement GTM tags/triggers described above.

4. Validate in:

   - GTM Preview.

   - Browser Network tab.

   - GA4 Realtime & DebugView. ([Google for Developers](https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?utm_source=chatgpt.com))

---

## 9. Next Steps + Quick-check audit list

**Next Steps for you / your team**

1. Map the client’s current donation flows (URLs, vendors, steps).

2. Decide where a data layer can be added (or confirm existing pushes).

3. Implement the 5 core events via GTM: `donate_click`, `begin_checkout`, `add_payment_info`, `purchase`, `payment_error`.

4. QA everything in GTM Preview + GA4 DebugView using test donations.

5. Create at least two GA4 audiences:

   - “Donation Started – No Purchase”

   - “Payment Error – No Purchase”

6. Link GA4 ↔ Google Ads and import `purchase` + `add_payment_info` as conversions; sync audiences for remarketing.

**Quick-check audit list**

- GA4 config tag firing on **all** main + donation pages.

- Cross-domain tracking configured under GA4 → Data stream → Configure domains.

- `begin_checkout` fires on every donation form load.

- `add_payment_info` fires when donor clicks submit.

- `purchase` fires only on successful gifts, with `transaction_id`, `value`, `currency`, `items`.

- `payment_error` fires with error code when card fails.

- GA4 audiences for non-completers created and populating.

- Conversions imported into Google Ads & visible in campaign reports.

If you want, next step we can tailor this to a specific platform (Engaging Networks, Classy, EveryAction, etc.) and I’ll give you the **exact** dataLayer schema and GTM variables to use for that stack.

---

# **1. When different teams own the C3 and C4 properties**

### **When different teams own the C3 and C4 properties**

If the C3 and C4 are run by completely different departments (different digital teams, different data owners, different reporting structures), it’s very common to see **separate GA4 properties** — one for each entity.
This creates a very clear data boundary and helps satisfy internal governance requirements.
*The tradeoff:* you cannot track the supporter journey across both sites as a single person or session, because the systems are intentionally separated.

When one group oversees both the C3 and the C4, we’ve seen many organizations use **one GA4 property with cross-domain tracking** for all domains.
This setup allows:

- A single supporter to be recognized as the same user across both sites

- Consistent attribution

- Unified journeys (e.g., someone signs an advocacy action on the C4 and later reads a blog or donates on the C3)

- Cleaner reporting and less fragmentation of traffic and engagement data

Then, for compliance, the reporting simply filters by domain or URL path when needed.

### **3. What likely makes the most sense for NWF**

Based on everything we’ve seen so far, it seems like NWF’s teams work across both domains and want continuity in reporting. If the sites are maintained by the same digital/marketing/analytics group, the most effective setup is:

**→ One GA4 property, with cross-domain tracking enabled for C3 + C4 + any subdomains.**

This preserves the supporter journey as a single user and avoids treating the same person as “new” every time they move between sites.

If the two entities were placed in separate GA4 properties, there would be no technical way to stitch the journey back together. Attribution, sessions, and user counts would all fragment, which makes high-level reporting and PPC optimization much harder.

### **4. Final note (and a legal caveat)**

The analytics platform *can* unify the journey; the question is simply whether your legal team is comfortable with shared data governance between the C3 and C4. We’ll follow whatever guidance they provide.

Once you receive the legal clarification, we can fully align the GA4 setup to meet both compliance and reporting needs.