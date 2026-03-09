
# SCAN Analytics | GA4-GTM

#GA4 

GA4 Measurement ID: G-2GBTND94Q6

GTM ID: GTM-52HZVMW

When a site visitor fills out any of the on-page subscription forms:

Key Event “form_submit” fires

The Tag is ID40 = “Form Submit” send this event to GA4

4Site: SCAN V2 Website Sign Up

NVSignupForm1820335

div#[NVSignupForm1820335.at-form.at](http://NVSignupForm1820335.at-form.at)-mode-person

div#[NVTag2.ngp-form.at](http://NVTag2.ngp-form.at)

---

## SCAN Lead Gen - GA4/GTM Form Listener

Here’s the *exact* Custom JavaScript you can paste into your new GTM variable (Variables → New → User-Defined → Custom JavaScript). I’ve pulled the footer’s block ID straight from your page and added a placeholder for your banner wrapper—just replace `'.YOUR_BANNER_WRAPPER_SELECTOR'` with the selector for that top-of-page banner container:

```plaintext
javascript
```

CopyEdit

`function() { var form = {{Form Element}}; if (!form) return undefined; // FOOTER instance if (form.closest('[data-block-id="block_c3e8869f74e757a01f758f15200c147a"]')) { return 'footer'; } // BANNER instance (replace this with your banner’s actual wrapper selector) if (form.closest('.YOUR_BANNER_WRAPPER_SELECTOR')) { return 'banner'; } return 'unknown'; }`

**What you need to do:**

1. **Create** a new User-Defined Variable in GTM of type **Custom JavaScript**.

2. **Name** it something like /s`JS – Newsletter Form Location`.

3. **Paste** the code above into the editor.

4. **Replace** `'.YOUR_BANNER_WRAPPER_SELECTOR'` with the actual CSS selector of the banner wrapper (e.g. `.promo-newsletter-banner` or the `[data-block-id="…"]` that it lives in).

5. Save.

Now you can use `{{JS – Newsletter Form Location}}` as a parameter in your GA4 tag (or in trigger filters) to distinguish **banner** vs. **footer** submissions.

---

```plaintext
gtag("event", "form_submit", {
```

```plaintext
  form_id: "ykRray-B-UOKrwkLch_JVw2",
```

```plaintext
  form_name: "4Site: SCAN V2 Website Sign Up",
```

```plaintext
  form_submit_text: "Contribute",
```

```plaintext
  form_category: "SignupForm",
```

```plaintext
  user_properties: {'': ""},
```

```plaintext
  send_to: "G-2GBTND94Q6"I
```

Steps Version 2:

Here’s a crystal-clear, step-by-step walkthrough to build your “Newsletter Lead” form-submit trigger and GA4 event tag in Google Tag Manager (GTM) and Google Analytics 4 (GA4).

---

- **Enable Built In Variables**

1. In GTM, click **Variables** in the left menu.

2. Click **Configure** (top right).

3. Under **Forms**, check **Form ID** and **Form Classes**.

4. Under **Page Variables**, ensure **Page URL** and **Page Title** are checked.

---

### 2. Create the “Newsletter Form Submit” trigger

- Go to **Triggers** → **New** → name it `Newsletter Form Submit`.

- Named it “[4Site] form_submit | footer subscribe “

- Click **Trigger Configuration** → choose **Form Submission**.

- Tick **Wait for Tags** and set **Timeout** to `2000 ms` (2 s).

- Tick **Check Validation** (ensures only successful, HTML5-validated submits fire).

- Under **This trigger fires on**, select **Some Forms** and add two conditions:

  - **Form ID** equals `NVSignupForm1820335`

  - **OR** **Form Classes** contains `at-form`

- (Optional) Under **This trigger fires on**, add **Page URL contains** `savethechildrenactionnetwork.org` to scope it only to your main site.

- Save the trigger.

> **Why these conditions?**
>
> - The placeholder `<div class="ngp-form">…</div>` is replaced by an injected `<form id="NVSignupForm1820335" class="at-form">…</form>` when EveryAction’s `at.js` runs.
>
> - Watching **Form ID** covers the static ID; watching **Form Classes** covers any future ID changes as long as the `at-form` class remains.

Saved trigger: [4Site] form_submit | footer subscribe

<https://cln.sh/tvy2RNBb>

Footer successful - but need to figure out a way to differentiate the banner from the footer form

---

### 3. Build the GA4 “Newsletter Lead” event tag

1. Go to **Tags** → **New** → name it `GA4 Event – Newsletter Lead`.

2. Click **Tag Configuration** → choose **Google Analytics: GA4 Event**.

3. Under **Configuration Tag**, select your existing GA4 Configuration tag.

4. In **Event Name**, enter:

   ```plaintext
   Nginxpag
   ```

   CopyEdit

   `newsletter_lead`

5. Under **Event Parameters**, click **Add Row** and configure:

   Parameter NameValue`form_id{{Form ID}}page_location{{Page URL}}page_title{{Page Title}}`

6. In **Tag Firing** choose the **Newsletter Form Submit** trigger.

7. (If using Consent Mode) under **Advanced Settings** → **Tag Sequencing**, or **Firing Options**, add an Exception trigger that checks **Consent – Analytics Storage** equals `denied`.

8. Save the tag.

---

### 4. Mark the event as a conversion in GA4

1. In GA4, go to **Admin** (⚙️) → **Events**.

2. Find `newsletter_lead` in the list (or wait for it to appear after your first test).

3. Toggle **Mark as conversion** to **On**.

---

## Next Steps

1. **Preview & test** in GTM: use GTM’s Preview mode, submit the footer form, and confirm the `GA4 Event – Newsletter Lead` tag fires once.

2. In GA4 **DebugView**, verify the `newsletter_lead` event shows up with correct `form_id`, `page_location`, and `page_title`.

3. In GA4 **Realtime → Conversions**, confirm your conversion count increments on each test submit.

4. **Publish** the GTM container when you’re satisfied.

---

### Quick-check audit list

- Trigger fires only on the footer form (Form ID or `at-form`).

- GA4 tag fires **after** the 2 s wait, but only on successful submits.

- Event parameters populate correctly in DebugView.

- Conversions toggle registers under GA4 → Events.

- Consent Mode blocks the tag when analytics_storage is denied.

### 

---