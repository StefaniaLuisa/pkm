---
Client: National Wildlife Feferation
Title: NWF - 2025 Analytics / GTM Audit and Overhaul
Due Date: '2026-01-07'
Task Details: See if NWF wants to move forward with any of the recommendations
Link: https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021
File: >-
  https://docs.google.com/spreadsheets/d/1DWv2ZOm-yRS0-C56KMU6--k33aXFQtU-eZiCDi6bWT8/edit?usp=sharing
Status:
  - follow-up
  - waiting for client
tags:
  - NWF
  - GA4
  - GTM
  - tracking

---

















## Related Links

Internal:

> [!INFO]
> [[Analytics/GA4-GTM Donor Journey]] (Notes on the donor journey NWF wants accomplished)
>
> [[NWF/NWF - GA4 Audit Plan]] (Audit plan, I used for the task)

External Files

*OG: [NWF - 2025 Analytics / GTM Audit and Overhaul](https://docs.google.com/document/d/15k9QVELL4pQX2diXD4ErbHXUOJVhxr7uIaDkDPbw7ek/edit?usp=sharing) - Bryan’s Proposal*

> [!INFO]
> [2025 NWF - GA4/GTM Audit - Analytics Questionairre](https://docs.google.com/document/d/1CprY-wttfh3Wd2bg4fCgtCJjlMvd3JfsVf7UJmt7v-o/edit?usp=sharing)
>
> [2025 NWF - GA4/GTM - Tracker](https://docs.google.com/spreadsheets/d/1DWv2ZOm-yRS0-C56KMU6--k33aXFQtU-eZiCDi6bWT8/edit?usp=sharing)
>
> [2025 Analytics / GTM Audit and Overhaul (15:00) - Productive.io](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021)

# Google Tag Manager Account

There are hundreds of custom GA4 event tags, many with one-off, descriptive names like CTBDH2‑CertifyYourHabitat‑CertifyYourGardenToday, EPMEchecklist, and EPTPshop. These are often tied to specific pages or campaigns.

Legacy Universal Analytics events and third-party vendor tags (e.g., Snap, Floodlight, multiple Facebook pixels, and Google Ads conversion tags) are still active, increasing noise and risk of duplicate firing.

Tags are being used to track individual buttons or pages instead of using one canonical event with parameters (like click text or page title). Many events are ungrouped in GTM ("Unfiled Items"), with overlapping or unused triggers and no clear deprecation process in place.

This tab is an inventory of GTM tags across the client’s container. It mixes GA4 event tags, legacy Universal Analytics events, multiple ad pixels (Facebook, Snap, Bing, Floodlight, Google Ads), and many one‑off, page‑ or CTA‑specific events. In short: it’s a sprawling, historical container without consolidation.

Why this is a problem:

- It inflates distinct GA4 event names. GA4 allows about 500 unique event names; dozens of bespoke names like “CTBDH2‑CertifyYourHabitat‑CertifyYourGardenToday,” “EPMEchecklist,” and “EPTPshop” burn through the cap quickly and fragment reporting.
- Legacy UA and duplicate vendor tags add noise and risk double‑firing, making debugging harder and data less trustworthy.
- Campaign/page‑specific event naming hides insight. Instead of one canonical event with rich parameters, you get hundreds of low‑value event names that are hard to analyze and maintain.
- Governance gaps. Many “Unfiled items,” overlapping triggers, and old tags suggest no deprecation process, which increases bloat and the chance of errors.

Here’s how I’d fix it:

- Consolidate to a small, canonical GA4 event set (e.g., click, form_submit, generate_lead, purchase), and move specificity into parameters like link_text, component_name, form_id, donation_amount.
- Map existing bespoke names to those canonical events using GA4 Modify events and GTM lookup transforms; normalize to lowercase.
- Retire UA and stale pixels; keep one verified pixel per vendor, documented in folders.
- Standardize triggers for sitewide link clicks and form tracking with CSS selectors, so CTAs don’t create new event names.
- Maintain an event dictionary and register only essential custom definitions; monitor distinct event count and set alerts well below the cap.

Recap: this tab shows an overgrown GTM container that will push GA4 toward its event‑name limit and degrade data quality. Consolidation, parameterization, and deprecation will protect the cap and make reporting clearer.

Roadmap to fix:

Google Tag Bloat issues and recommendations

**What I’m seeing**

**Consolidate event names, push detail into parameters, retire legacy**

 1. Canonical event set

    - Define a tight list of GA4 event names used across the property. Aim for ≈ 15–30 max. Examples:

      - click, view_item, select_item, generate_lead, begin_checkout, add_payment_info, purchase, sign_up, login, view_promotion, select_promotion.

    - Resist creating new event names per campaign or page. Use parameters for context.

 2. Parameterize context instead of naming new events

    - Add rich parameters to your canonical events:

      - link_text, link_url, link_domain, cta_id, cta_location, component_name, page_section.

      - For donation flows: donation_amount, donation_frequency, upsell_shown, upsell_accepted, form_id, transaction_id.

    - Replace events like “CTBDH2‑CertifyYourHabitat‑CertifyYourGardenToday” with one event: click, and pass cta_id=“certify_garden_today”, component_name=“CTBDH2”.

 3. Transform and dedupe incoming names

    - GA4 Admin → Modify events: map near‑duplicate or campaign‑specific names to your canonical set.

    - GTM → Use a Lookup Table or Custom JS Variable to translate legacy event names before send.

    - Turn on lowercase normalization for event names and key parameters to avoid case splits.

 4. Retire UA and rogue tags

    - Disable or remove Universal Analytics tags in GTM. They add noise and can double‑fire behaviors.

    - Remove unknown GA4 tags and duplicate vendor pixels. Keep a single, documented pixel per vendor.

    - Group deprecated tags into a “_Archive” folder in GTM for traceability, then publish the removal.

 5. Standardize click and form tracking

    - Use GTM Link Click triggers plus CSS selectors for nav, CTA buttons, promo modules, quizzes.

    - Emit click with link_text, cta_id, component_name. Stop emitting unique event names per CTA.

    - For forms, consistently emit form_start, form_submit, and generate_lead where appropriate, with form_id and form_name.

 6. Donation and subscription flows

    - Keep purchase reserved for true donations. Ensure value, currency, transaction_id, items are set.

    - Add generate_lead for subscription successes. Avoid creating “subscribe/2” specific event names.

    - Use cookies or data layer values you already set, but pass them as parameters on canonical events, not new event names.

 7. Channel and attribution hygiene

    - Normalize UTMs to lowercase and standard mediums (paidsocial vs social) so you don’t need event‑name variants to find campaign performance.

    - Configure cross‑domain so journeys don’t fragment and you aren’t tempted to mint new event names to patch attribution.

 8. Governance in GTM

    - Folders: GA4 Events, GA4 Config, Ads & Pixels, Deprecated, Utilities.

    - Naming: Tag [GA4] Event: click | CTA, Trigger: Click | CTA buttons, Var: CSS Selector | CTA buttons.

    - A “New Event Checklist”: justify parameter use, confirm it isn’t a duplicate, align with canonical list, add to dictionary.

 9. Event dictionary and custom definitions

    - Maintain a dictionary: event_name, description, parameters, owner, trigger, business goal.

    - Register only high‑value parameters as custom dimensions. Keep under GA4 limits (50 event‑scoped custom dimensions).

    - Build one Looker Studio chart to monitor distinct event names weekly. Alert if &gt; 300 to trigger cleanup.

10. Workspace and rollout

- Create a “Consolidation” workspace. Migrate 5–10 high‑volume bespoke events first to prove the pattern.

- Publish in stages. Use DebugView and GTM Preview to confirm parity.

- Document changes in a change log. Note any Modify events mappings in GA4 Admin.

## Audit Notes:

Our work is dependent upon the NWF team working on [#1375 Confirm Metrics for GA4/GTM Audit](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625719) so I can always adjust our tasks if you need more time for that work.
Timeline as it stands now, but it can be adjusted if you need more time for the metrics confirmation.

November 5-10:

- NWF [#1375 Confirm Metrics for GA4/GTM Audit](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625719) - Waiting for some answers

November 12-14

- [x] [#1374 1. Analytics discovery: GA4/GTM/Consent Configuration Audit](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625714)

- [x] [#1373 2. Analytics discovery: GA4 Property & Events Audit](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625704)

- [x] [#1376 3. Analytics discovery: GTM Container Audit](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625755)

- [x] [#1370 4. Analytics discovery: Data Validation via DebugView & Preview](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625657)

- [x] [#1371 5. Analytics discovery: Cross-Domain & Attribution Testing](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625663)

- [x] [#1377 6. Analytics discovery: Donation/Subscription Event Mapping](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625783)

November 24-25

- [#1378 7. Analytics discovery: Findings & Data Improvement Roadmap/Scope](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/task/14625789)

  # Current Setup

  ### [Account Details -](https://analytics.google.com/analytics/web/?authuser=0&pli=1#/a119708728p317256000/admin) Everything filled out nicely: All of the below accepted:

  Basic Settings

  **Account Id:** 119708728

  **Account Name:** NWF - NB

  **Country of Business: United States**

- [x] Modeling contributions & business insights Enable

- [x] Technical support

- [x] Recommendations for your business

- [x] Data Processing Terms: The Data Processing Terms for this account were accepted on May 22, 2018.

### Property Settings:

Property details:

- Property name (required) GA4 - NWF Holistic (All Subdomains) - GA4
- Reporting time zone: United States - (GMT-05:00) New York Time
- Currency displayed as US Dollar (S)

**~🔴Business details (NEEDS ACTION)~**

- Industry (required): Law & Government
- Business size (required): Not filled out
- Business objectives (required): Not filled out
- Select one or more business objectives: Not filled out

# Data streams

Two data streams are setup:

1. NB - NWF Holistic (All Subdomains) - GA4 <https://www.nwf.org/> - Receiving traffic in past 48 hours.
2. NWF Eco Leaders (GA4) <https://www.nwfecoleaders.org/home> — No data received in past 48 hours. **~🔴(Remove and add as a domain to cross-track)~**

# Web Stream details

[**NB - NWF Holistic (All Subdomains) - GA4**](https://analytics.google.com/analytics/web/?authuser=0&pli=1#/a119708728p317256000/admin/streams/table/3600120279)

STREAM URL: [**https://www.nwf.org/**](https://www.nwf.org/)

STREAM ID: **3600120279**

MEASUREMENT ID: **RLRJ1GMJC2**

---

## Events

### **Enhanced measurement (all turned on)**

- [x] Page views

- [x] File downloads

- [x] Scrolls

- [x] Outbound

- [x] clicks

- [x] Form interactions

- [x] Site search

- [x] Video engagement

~🟠Recommendation: Form internactions does not always work as expected, turn off if not seeing the correct data~

### Modify Events

No modified events

### Create custom events:

1. Custom event name : [EN_PAGE_VIEW](https://cln.sh/hg0DDzhJ)
   1. Matching conditions: event_name equals EN_PAGE_VIEW

### Measurement Protocol API secrets:

No API secrets yet

### Redact data:

**No data set to be redacted**. Redact specific data collected by website events before it's sent from your website to Google Analytics. Redacted values will show up as "(redacted)". [Learn more about data redaction](https://support.google.com/analytics/answer/13544947?hl=en_US&utm_id=ad)

#### Choose what to redact:

1. Email: Redact most email addresses from event data

   URL query parameters

2. Redact URL query parameters from specific event parameters

---

## Google Tag

### Configure tag settings

**Your Google tag - Tag Name:** NB - NWF Holistic (All Subdomains) - GA4

**Tag ID:** G-RLRJ1GMJC2

**Destinations 2 Destinations have this tag:**

1. NB - NWF Holistic (All Subdomains) - GA4 - G-RLRJ1GMJC2
2. [www.nwf.org/EcoLeaders](http://www.nwf.org/EcoLeaders) - G-LHOLDCZBST
   1. ~🔴This is a seperate GA4 account under the “[www.cleanearthchallenge.com](http://www.cleanearthchallenge.com)” property as a data stream: [https://cln.sh/Rfd0ngDN](https://cln.sh/Rfd0ngDN)~
   2. ~🔴is this a specific landing page that’s data is important to bring into the [cleanearthchallenge.com](http://cleanearthchallenge.com)? Not sure I understand this property setup~

**Additional settings:** Ignore duplicate instances of on-page configuration ~🟠(recommended to turn on)~

#### Tag Quality

- Tag coverage summary: All the pages that this is not on [[tag-coverage-G-RLRJ1GMJC2 (1).csv]]

### Manage connected site tags

### View tag instructions