
**Phase 4: Event and parameter validation via DebugView (3.0h)**

- Test flows and capture:

  - Site arrival and navigation on [nwf.org](http://nwf.org), including clicks that were reported as not tracking into GA4.

  - Donation funnel: landing, amount select, form interactions, submit/thank you on [support.nwf.org](http://support.nwf.org); watch for UA gtag conflicts and double page_view firing.

  - Advocacy funnel: landing, form interactions, submit/thank you.

- Validate each event’s schema and parameters (page_location, page_referrer, session_source/medium, form interactions, purchase-like conversions), including Enhanced Measurement consistency between Google tag and GA4 stream settings.

- Output: Event dictionary covering observed events, conditions, parameters, destinations, and gaps vs KPIs.

Deliverable: Source‑of‑truth spreadsheet with sampled tags, trigger logic, destinations, status, and deprecation candidates—plus naming convention gaps and doc hygiene issues.

- **Donation/e‑commerce mapping to KPIs (1.0h)**

- Map donation events to target KPIs: revenue, item/value parameters, transaction IDs, attribution to campaigns/UTMs, and funnel conversion.

- Flag where GA4 purchase or custom conversion is missing or mis-specified and estimate effort to standardize.

**Phase 8: Reporting alignment review (0.8h)**

- Trace Looker Studio metric definitions back to GA4 dimensions/events to spot mismatches that drive stakeholder confusion.

- Capture a short list of “report‑breaking” issues: double pageviews, missing events on clicks, no data for specific stream, attribution gaps.

**Phase 9: Risk register and remediation roadmap (1.5h)**

- Risk register: Document systemic risks from legacy UA tags, over‑complex GTM, centralized knowledge, and lack of documentation. Include privacy/regulatory drift risks and GA3→GA4 transition remnants.

- Remediation roadmap:

  - Sequenced steps to stabilize measurement, reduce noise, and modernize tags using templates, with effort ranges and prerequisites.

  - Cross‑domain setup, Enhanced Measurement standardization, legacy UA removal plan, GA4 event schema standard, naming conventions, documentation, and ownership plan.

- Include “fast wins” vs “heavy lifts,” with recommended sprint sizing for Q1–Q2 and dependencies.

**Phase 10: Readout and refined scope (0.7h)**

- Prepare a concise findings deck and updated scope with time/phasing estimates for the overhaul.

- Internal review and edit pass so the document is client‑ready and implementation teams have clear next steps.

**Deliverables**

- **GA4 settings checklist:** Properties, data streams, tag connections, Enhanced Measurement, filters, exclusions.

- **GTM tag inventory (sampled):** Tags, triggers, destinations; deprecation targets; naming convention recommendations.

- **Event dictionary:** Observed events and parameters for site, donation, advocacy; gaps vs KPIs.

- **Attribution and cross‑domain validation notes:** Evidence of session continuity or fragmentation; domain list to include.

- **Risk register:** Prioritized risks with impact/likelihood and mitigation.

- **Remediation roadmap:** Sequenced actions with effort ranges, dependencies, and QA guidance.

- **Findings deck + refined SOW:** Scope and estimates for audit implementation and modernization.

**Assumptions and constraints**

- No production changes during audit; all testing via GTM preview and GA4 DebugView.

- Access provided to GA4, GTM, Google tag settings, and the relevant Looker Studio reports.

- The audit does not include writing or deploying new tags; it identifies and sizes the work.

**Why this structure works**

It balances breadth and depth in a complex, legacy‑heavy environment. We’ll confirm the foundations first, then focus time where tracking breaks stakeholder KPIs: site interactions, donation and advocacy funnels, session continuity, and report alignment. The outputs give implementation teams a clear, safe order of operations, with realistic effort ranges so NWF can budget and schedule.

**GA4 Audit Plan: 13 hours**

The steps below outline the work that will make up the two phases that were laid out in the SOW:

1. Discovery Phase: Conduct an initial audit to document the current setup, identify pain points, and assess opportunities. A critical component will be identifying and prioritizing KPIs.


1) Roadmap Development: Use findings from the discovery phase to create a detailed plan for the overhaul.

To accomplish the discovery phase I’ll be leaning on the GA4 DebugView mode, GTM preview, and test flows across [nwf.org](http://nwf.org), as well as the donation, and advocacy forms.

1. **GA4/GTM/Consent Configuration Audit - (1h)**

- Assess the technical setup of the property(s).

  - Review GA4 config

  - GTM configuration

  - Consent mode configuration

2. **GA4 property settings & events, dimensions audit (2h)**

   - GA4 settings checklist:

     - Check and verify their data streams, measurement IDs, Google tag connections, Enhanced Measurement, internal traffic filters, referral exclusions, and data retention.

     - Check Enhanced Measurement and Google tag

       - Compare Enhanced Measurement toggles in GA4 streams against Google tag configuration, and make sure they match .

3. **GTM container audit (2 h)**

   - Taking an Inventory of their GTM - cataloging triggers/tags variables that feed GA4.

4. **Data validation (3 hrs)**

   - Using the debugger & GTM Preview to test different visitor flows and capture the data /

     - Test flows and capture / variables passing into GA4

     - Because of time constraints Focusing on:

       - Site arrival and navigation on [nwf.org](http://nwf.org), including clicks that were reported as not tracking into GA4.

       - Donation funnel: landing, amount select, form interactions, submit/thank you on [support.nwf.org](http://support.nwf.org); watch for UA gtag conflicts and double page_view firing.

       - Advocacy funnel: landing, form interactions, submit/thank you.

     - **Cross‑domain and attribution testing (1.0h)**

       - Confirm whether cross‑domain measurement is configured for journeys from [nwf.org](http://nwf.org) to EN-hosted forms and other relevant subdomains.

5. **Donation/Subscription testing (1.0h)**

   1. Map donation and subscription events - providing findings on revenue, item/value parameters, transaction IDs, attribution to campaigns/UTMs, etc.
   2. Flag where GA4 purchase or custom conversion is missing or mis-specified and estimate what it would take to standardize.


1) **Findings & Data Improvement roadmap (1.5h)**

   1. Capture issues: double pageviews, missing events on clicks, no data for specific stream, attribution gaps.
   2. We will provide notes of risks from legacy UA tags, over‑complex GTM, centralized knowledge, and lack of documentation. Include privacy/regulatory drift risks and GA3→GA4 transition remnants.
   3. Provide measurement and data Improvement roadmap:
      1. Provide steps and a plan to improve data and measurement accuracy.
      2. Include “fast wins” vs “heavy lifts,” with recommendations on what should be prioritized.

**Deliverables**

- **GA4 & GTM source of truth & tag inventory spreadsheet:**

  - Properties, data streams, tag connections, Enhanced Measurement, filters, exclusions.

  - Tags, triggers, destinations; deprecation targets; naming convention recommendations.

  - dictionary of events, the observed and tested events (cannot confirm all - based on time constraints) and parameters for site, donation, advocacy

- **Findings and prioritized recommendations to move towards the cleanest most accurate data possible.**