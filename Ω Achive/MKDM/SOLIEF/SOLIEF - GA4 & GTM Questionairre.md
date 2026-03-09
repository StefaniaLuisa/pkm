
---

Marketing Highlight:
Project Highlight: [Statue of Liberty-Ellis Island Foundation](https://www.statueofliberty.org/) – GA4/GTM Analytics Audit

The Statue of Liberty-Ellis Island Foundation, in partnership with MKDM, approached us with a critical need; to ensure their analytics setup could accurately measure and support their paid digital marketing efforts for their client. As our first collaboration with MKDM, this project set the stage for a partnership we hope has long-term potential. 

Our process for this audit started with reviewing the Foundation’s main site and subdomain, identifying gaps and opportunities in their existing GA4 and GTM configurations. Within the scope of this audit, we focused on setting up Key lead tracking events and easy to pull attribution reporting, ensuring that MKDM will easily be able to show the value of their paid channels. The result gives both the Foundation and MKDM actionable insights to inform thier strategy, while providing us opportunity to recommend continued optimizaiotion of their analytics based on our findings.

This engagement delivered improvements in understanding what data is being tracked, and how to report on while also opened the door to ongoing collaboration with MKDM—expanding our impact beyond analytics into broader digital strategy support.

---

# Introduction

Below are a series of questions that we will review with you at our kickoff meeting. We kindly ask that you complete and return this form in advance to ensure we use our time effectively. This information will directly support our GA4/GTM audit and implementation for SOLEIF.

We understand that SOLEIF is focused on expanding visibility of its passenger search database and improving analytics tracking to support campaign performance and future digital investments including a website redesign.

**4Site Project Team**

- Stef Jones, Director of Strategy

- Heather Schneider, SVP of Creative Operations

**MKDM / SOLEIF**

- Eliza Slone

## Background

1. Please provide a brief background on the Statue of Liberty-Ellis Island Foundation (SOLEIF) and its website objectives.


1) What are the primary goals and objectives of their website (s)?


1. Inform people about the Statue of Liberty, Ellis Island and the Foundation. This includes providing accurate information to people planning a visit, as well as just general educational information.

2. Allow people to research their family and other immigration history through facilitating online access to the Passenger Search Database (currently around 60 million immigration records; soon to expand to around 120 million). Note that email registration IS required to access full resources so this is both a programmatic/mission goal AND a lead generation source to support fundraising goals.

3. Secure donations to support the work of the Foundation, through these primary channels:

- 

1. Membership (<https://www.statueofliberty.org/donate/>)

2. Wall of Honor Inscriptions (<https://www.statueofliberty.org/support/wall-of-honor/>)

3. Special contributions to key projects, including:


1) Statue of Liberty Museum / Founders Registry (last major capital project; <https://www.statueofliberty.org/support/wall-of-honor/>)

2) Ellis Island Museum Reimagined (current major capital project; <https://www.statueofliberty.org/ellis-island/supportellis/>)


1. Secondary / smaller goals:

- 

1. General email collection (not through passenger search). Email collection box in page footers (this can and should be better - in the future!)

2. Shop - primarily for reproductions of historical documents available through the passenger search (<https://www.statueofliberty.org/shop/>)


1) Can you provide any background on the current GA4 and GTM setups? Who implemented them, and when?

NEEDED/REQUESTED - 2023?

1. Please provide all of the domain/subdomains associated with SOLEIF.

- 

1. [https://www.statueofliberty.org](https://www.statueofliberty.org/)

2. [https://heritage.statueofliberty.org](https://heritage.statueofliberty.org/passenger)

3. Are there any others?

- 

1. <https://libertyellisfoundation.org/> (redirects to [statueofliberty.org](http://statueofliberty.org))

2. [ellisisland.org](http://ellisisland.org/) (redirects to [statueofliberty.org](http://statueofliberty.org/))

3. [soleif.org](http://soleif.org) (redirects to [statueofliberty.org](http://statueofliberty.org/))


1) What is the most important data to capture for each domain?

- 

1. What metrics are most important to capture for [https://www.statueofliberty.org](https://www.statueofliberty.org/)


1) Site visitation basics - sources, interactions, behavior

2) Donations - Possibly with some breakout by category, but we’d take counsel about how much granularity to embed in GA4 (possibly just 1x vs. monthly?)

- 


- [1x Membership](https://www.statueofliberty.org/membership)

- [Monthly Membership](https://www.statueofliberty.org/membership)

- [1x Donation ](https://www.statueofliberty.org/donate/)

- [Monthly Donation](https://www.statueofliberty.org/donate/)

- [EIMR Donations](https://www.statueofliberty.org/steward)

- [Founders Registry](https://www.statueofliberty.org/liberty/) (Limited utilization)

 1. Wall of Honor Inscriptions ([Wall of Honor Inscription](https://www.statueofliberty.org/inscribe-a-name/))

 2. Email registrations

 3. What metrics are most important [https://heritage.statueofliberty.org](https://heritage.statueofliberty.org/passenger)

 4. Initiate passenger search (visit <https://heritage.statueofliberty.org/passenger>, <https://heritage.statueofliberty.org/full-passenger-search>, enter data, click results). Potentially split between these two pages (full passenger vs. /passenger page search)

 5. Create account to view passenger search results

 6. Add to cart

 7. Store purchases

 8. Log-In to view passenger search results

 9. Possibly save image to account/profile

10. What are the overall issues being seen with the current configuration and data that is being gathered in the current GA4/GTM setup?

- 

1. Many pages appear to be missing tags (1000+, primarily on [heritage.statueofliberty.org](http://heritage.statueofliberty.org))

2. Lack of cross domain configuration

3. Potentially use of legacy UA tags

4. Lack of confidence in event/key event definition accuracy and setup


1) Are there any compliance or regulatory concerns with how the accounts are currently configured (e.g., CPRA, GDPR, other state or federal laws)?

Yes. Cookie Yes was recently implemented by the SOLEIF internal team for [statueofliberty.org](http://statueofliberty.org/); ensuring that this setup is accurate is required. They have been attempting to implement Cookie Yes on [heritage.statueofliberty.org](http://heritage.statueofliberty.org/) as well but this is not yet live to our understanding.

1. Are you aware of any custom events or conversions currently being tracked? Any reason to be cognizant of legacy tags from Universal Analytics still being live?

Yes. Currently at least 26 custom events are being tracked. However, a decent number of the key events appear not to be working correctly (no/low number of events counted in the last year for actions we understand to be happening on site). Legacy tags UA appear to be in place still to some extent.

## Current Utilization

- How is SOLEIF currently measuring the success of their digital initiatives? What metrics are being currently tracked?

- 


- What data, if any, has been most helpful?

Limited digital fundraising initiatives to date. Email performance tracked primarily through Pardot (Salesforce Marketing Cloud Account Engagement) reporting. Google Grant performance tracked through Google Grant ad account.

- What tracking challenges currently exist, and what are you hoping to resolve? What is currently unavailable?

Given limited organizational experience to date with digital ads, difficult to determine. We are seeking to create a reasonable framework for the scope of digital ad planned.

One known issue are the conversions currently utilized in Google Grant account (these appear misaligned with organizational goals). This is more related to campaign optimization that measurement, however.

- What data or specific reports would make MKDM or SOLEIF feel confident in the decisions they are making based on the data?

Reporting that provides clarity about the value of marketing efforts. Specifically:

- Traffic/engagement resulting from marketing campaigns by source

- Number of new registrations (primarily passenger search, but also other registrations) resulting from paid search vs. meta va. grant vs. other sources

- Value of new registrants

- Donations resulting from paid search vs. meta va. grant vs. other sources

- Wall of honor inscriptions resulting from paid search vs. meta va. grant vs. other sources

- How frequently is data being reviewed? What would the ideal frequency for reviewing site data be?

To be determined. Likely at least weekly during active campaigns / pilot phase if not more frequently.

- Do MKDM or SOLEIF use or intend to use Google Ads, Search Console, or other Google products that need to be linked with GA4?

Yes. Planning for running both Google Paid Ads account and Google Grant Ads (both should be linked with GA4 already). Search Console is linked but data appears to be flawed / inaccurate. If we’re able to improve this within scope, great. If not, Google Console is not a high priority.

## Marketing & Audience

- Who is your primary digital audience? (e.g., demographics, behaviors)

- Which platforms or channels drive the most traffic or conversions? (e.g., Google Ads, Meta Ads)

- Are you currently segmenting your audience for marketing purposes? If so, how?

## Tracking Setup & Measurement

- What are the primary goals for this analytics initiative? (e.g., enhancing data accuracy, supporting marketing campaigns, ensuring compliance)

Creating solid platform for a successful launch of a digital marketing pilot program consisting of Google Grant, Google Paid Ads, Meta campaigns, as well as potentially display campaigns and postal retargeting. Objectives will include both lead generation and donation.

- For this initial audit and configuration, what campaigns, channels and/or platforms must be tracked for MKDM’s current paid initiatives.

- 


- Are there any active or planned marketing campaigns that this analytics setup should support?

Yes:

- Meta Lead Generation (via passenger search and potentially also using meta forms).

- Meta Donation / Wall of Honor.

- Google Paid Ads with lead generation and donation objectives.

- Google Grant. Google Grant campaign has been ongoing for several years now but objective and conversions will be revisited to better align with SOLIEF marketing goals as possible.

- Possibly, display ads, although may be executed via google/pmax

- Postal retargeting

- Are UTMs being used to track shared URLs? If there is any documentation for this, please provide.

UTM codes have been used in Google Grant program (sample template: {lpurl}?utm_source=google&utm_medium=cpc&utm_campaign=statue-of-liberty&utm_term={keyword}. No additional documentation. Planning to implement UTMs globally and would accept recommendations for specific formats.

- Are there any other form of tracking being put when running a campaign?

- What data are you looking to see on a regular basis?

- Are there specific metrics or KPIs that are most important for making decisions

- What are the most important actions that  you wish to track? (e.g., form submissions, donations, searches)

- 


- Are there specific events or interactions on your website that you want to track (like video views, scroll depth, link clicks, etc)?

## Cookie Consent & Compliance

Hoping that answering of the questions in this section will fall under the scope of work on this project. Setup may be complete (not setup on heritage) and not confident of the internal knowledge used to execute setup.

- How is the cookie consent banner configured? (e.g., opt-in, opt-out)

- Has CookieYes been integrated with advertising platforms to ensure consent is properly honored?

- Is the consent banner configured to display based on the user's location?

- Are third-party cookies (e.g., from Google Ads, Meta) blocked until consent is given?

## Testing

- Can you provide sample or test forms for validation?

- Is there any specific process we should follow when testing contact forms, subscription forms, donation forms or any other interactive site element?

## Platform Access

Please add [goog@4site.tv](mailto:goog@4site.tv)  to the accounts listed and notify [stef@4sitestudios.com](mailto:stef@4sitestudios.com)  once access has been granted.

*Please also note any additional platforms or integrations in use (e.g., Salesforce Pardot, CMS), and the appropriate access contacts (full tech echo system)*

**Platform**

**Access Type**

GA4 Property (for both domains)

Admin

GTM Container(s)

Admin

CookieYes (or another Consent Tool, if applicable)

Edit/Admin

Meta Pixel & Meta Business Event Manager

Partner/Admin via Meta Business Manager

## Timeline & Process

1. Timeline

Now - June 11

- Conduct GA4 Audit: Events, Conversions,ecommerce, referral exclusions

- Review GTM Container: Tags, Triggers, Variables

- Evaluate Tracking for all relevant Channels/Sources

June 12

- Presentation of recommendations

June 12-16:

- MKDM review of recommendations and consolidated feedback

June 17-20:

- Implement tracking improvements

- 4Site Self-QA of work

- Documentation

June 23:

- Walkthrough of implementation

- Project Completion

1. Are there any upcoming events that will affect the timeline, such as time off, staff retreats, annual meetings, or board meetings?

2. [Productive](https://app.productive.io/2650-4site-interactive-studios-inc/projects/690668)