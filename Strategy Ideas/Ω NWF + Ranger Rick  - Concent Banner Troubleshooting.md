---
pinned: true
Task Title: 2026 NWF & Ranger Rick  - Concent Banner Troubleshooting
Due Date: '2026-02-16'
Status:
  - waiting for client
Client:
  - National Wildlife Federation
tags:
  - NWF
  - task
  - ga4
  - data and privacy
  - 2026-Q1
  - cookie-banner
Last Edited: '2026-01-28'

---

---

Removing PII

[www.nwf.org](http://www.nwf.org)

[support.nwf.org](http://support.nwf.org)

[blog.nwf.org](http://blog.nwf.org)

[nativeplantfinder.nwf.org](http://nativeplantfinder.nwf.org)

[support.nwfactionfund.org](http://support.nwfactionfund.org)

[photocontest.nwf.org](http://photocontest.nwf.org)

[certifiedwildlifehabitat.nwf.org](http://certifiedwildlifehabitat.nwf.org)

[nwf.org](http://nwf.org)

[mayorsmonarchportal.nwf.org](http://mayorsmonarchportal.nwf.org)

[subs.rangerrick.org](http://subs.rangerrick.org)

[www.hechoonline.org](http://www.hechoonline.org)

[woobox.com](http://woobox.com)

[artemis.nwf.org](http://artemis.nwf.org)

[communitywildlifehabitat.nwf.org](http://communitywildlifehabitat.nwf.org)

---

**Details for each platform:**

**Plausible**

Plausible is a lightweight, privacy-first analytics tool that **tracks only aggregated site performance metrics without cookies or personal data.** It’s ideal for quick insights without the complexity of a traditional analytics suite.

**Pros**

- **Easy to use:** a single-page dashboard with essential metrics like unique visitors, page views, traffic sources, and simple goals.

- **No cookies / truly cookieless:** privacy built in so you don’t need intrusive cookie banners or consent prompts for analytics.

- **Lightweight and fast:** minimal impact on page performance.

- **Low barrier to adoption:** very little training required to start deriving insights.

**Cons**

- **Limited depth:** fewer metrics and no advanced tools like session recordings or detailed user flows.

- **Less flexible reporting:** not built for deep exploration or highly customized analytics needs.

**Best for:**
Teams that want **quick, compliant, easy-to-digest analytics** with minimal setup and no heavy training or maintenance.

**Matomo**
Matomo is much more complex, Google-Analytics–like platform that offers deep reporting, behavior analysis, and advanced tools. It can be self-hosted (at no software cost) or run in the cloud with support and managed updates. You keep full ownership of your data and control your hosting location.

**Pros**

- **Rich analytics and reporting:** funnels, custom reports, heatmaps, session recordings, A/B testing, etc.

- **Data ownership and compliance:** you control where data lives, which supports privacy and compliance needs.

- **No data sampling:** complete datasets (no guesswork from modeled data).

- **Flexible hosting:** choose cloud hosting or fully self-hosted on your own infrastructure.

- **Familiar interface:** looks and feels closer to Universal Analytics than simpler tools.

**Cons**

- **Higher technical overhead:** setup and maintenance require more technical involvement, especially if self-hosting.

- **More complexity:** more features means a steeper learning curve for non-technical users.

- **Potential consent requirements:** depending on configuration and data you collect, you may still need consent banners unless you configure cookieless tracking and anonymization carefully.

**Best for:**
Organizations that want **deep insights and flexibility** and have either technical support or a team comfortable navigating a robust analytics platform.

——-

Both platforms allow you to track meaningful data, but I do want to point out they serve different needs.

Along with the great resources Michael Thomas provided in his most recent comment I wanted to point out some pros and cons of each.

**Matomo**

Delivers comprehensive analytics capabilities while still supporting cookieless and privacy-compliant tracking.

**Matomo**
Matomo is the closest alternative to a full analytics suite like GA4 because it offers *deep reporting*, *data ownership*, and *privacy-first configuration options*. It can be *self-hosted* or used as a hosted cloud service depending on your preference and resources. Its advanced privacy and compliance tooling (including cookieless tracking options) makes it a strong choice for children’s content where respecting consent is essential.

- **Full analytics capability:** Includes detailed reporting, customizable dashboards, segmentation, event tracking, and other advanced metrics.

- **Data ownership & privacy:** 100% ownership of your data and strong compliance with GDPR, CCPA, and other privacy laws.

- **Cookieless tracking:** Can be configured to operate without cookies while still providing meaningful insight.

- **Flexible hosting:** Choose between self-hosting for maximal control or cloud hosting for easy management.

**Considerations**
Matomo requires more setup and administrative effort than simpler tools. It’s great if you need *longer-term depth and flexibility*, but initially it may take more configuration (especially if you self-host). That said, that upfront effort pays off if analytics are going to be a continuing priority for Ranger Rick.

**Best Fit Scenarios**

- You want a **GA-like analytics experience** with reporting depth.

- You plan to use analytics for content performance, campaigns, and audience insights.

- You have the technical capacity (internal or via partner) to maintain a more advanced platform.

**Alternate Option: Plausible Analytics**

**Overview:** Plausible is a *simple, lightweight, privacy-first analytics platform*. It focuses only on core metrics like unique visitors, page views, and basic goal tracking, and it’s designed to work without cookies or persistent identifiers.

**Pros**

- **Easy to use:** Clear, intuitive dashboard with essentials only – minimal training required.

- **No cookie consent needed:** Built to be cookieless and GDPR/CCPA compliant out of the box.

- **Fast setup and low overhead:** Quick to launch with no complex configuration or maintenance.

**Cons**

- **Limited depth:** Does not include advanced reporting, user journey analysis, or customization like Matomo.

- **Feature trade-off:** You get simplicity at the expense of insights into behaviors like funnels or segmentation.

**Best Fit Scenarios**

- You want **basic, high-level insights** quickly.

- You don’t need deep analysis or advanced metrics.

- Your priority is simplicity, minimal maintenance, and guaranteed compliance.

**Summary Recommendation**

- If Ranger Rick’s analytics needs are centered on **simple traffic awareness and compliance without consent-barrier complexity**, **Plausible** is acceptable.

- If you want a solution that can **grow with your analytics maturity, support richer insights, and replace GA4 functionality in a privacy-first way**, **Matomo** is the better long-term choice.Pro

——-

Thank you Michael Thomas! I completely agree with your recommendations!

Donna Davidovich, below I have provided some additional information about each recommended platform that I hope helps in making your decision.

**The most important question I recommend thinking about is what data or metrics do you need to see be able report on?**

**Short version and sweet overview:**

**Choose Plausible if:**

- you need a simple lightweight, privacy-first analytics platform that gives you reliable trends intutive, and a straightforward interface that anyone on your team can use.

- It focuses only on core metrics like unique visitors, page views, and basic goal tracking, and it’s designed to work without cookies or persistent identifiers.

- **Considerations:**

- **Limited depth:** Does not include advanced reporting, user journey analysis, or customization like Matomo.

- **Feature trade-off:** You get simplicity at the expense of insights into behaviors like funnels or segmentation.

**Choose Matomo if:**

- You want a **full analytics stack** that is the closest alternative to GA4 bof GA4 with deeper reporting and analysis. This is especially valuable if you anticipate needing more than just high-level traffic stats (e.g., any custom events, funnels, content performance, session behavior).

- **Considerations:** Matomo requires more setup and on-going maintence administrative effort than simpler tools. It’s a good fit if you need *detailed data and tracking flexibility*, but initially it may take more configuration.

- You want a GA4-like analytics experience with reporting depth.

- You plan to use analytics for content performance, campaigns, and audience insights.

- You have the technical capacity and resources to maintain this more advanced platform.

**Details for each platform:**

**Plausible**

Plausible is a lightweight, privacy-first analytics tool that **tracks only aggregated site performance metrics without cookies or personal data.** It’s ideal for quick insights without the complexity of a traditional analytics suite.

**Pros**

- **Easy to use:** a single-page dashboard with essential metrics like unique visitors, page views, traffic sources, and simple goals.

- **No cookies / truly cookieless:** privacy built in so you don’t need intrusive cookie banners or consent prompts for analytics.

- **Lightweight and fast:** minimal impact on page performance.

- **Low barrier to adoption:** very little training required to start deriving insights.

**Cons**

- **Limited depth:** fewer metrics and no advanced tools like session recordings or detailed user flows.

- **Less flexible reporting:** not built for deep exploration or highly customized analytics needs.

**Best for:**
Teams that want **quick, compliant, easy-to-digest analytics** with minimal setup and no heavy training or maintenance.

**Matomo**
Matomo is much more complex, Google-Analytics–like platform that offers deep reporting, behavior analysis, and advanced tools. It can be self-hosted (at no software cost) or run in the cloud with support and managed updates. You keep full ownership of your data and control your hosting location.

**Pros**

- **Rich analytics and reporting:** funnels, custom reports, heatmaps, session recordings, A/B testing, etc.

- **Data ownership and compliance:** you control where data lives, which supports privacy and compliance needs.

- **No data sampling:** complete datasets (no guesswork from modeled data).

- **Flexible hosting:** choose cloud hosting or fully self-hosted on your own infrastructure.

- **Familiar interface:** looks and feels closer to Universal Analytics than simpler tools.

**Cons**

- **Higher technical overhead:** setup and maintenance require more technical involvement, especially if self-hosting.

- **More complexity:** more features means a steeper learning curve for non-technical users.

- **Potential consent requirements:** depending on configuration and data you collect, you may still need consent banners unless you configure cookieless tracking and anonymization carefully.

**Best for:**
Organizations that want **deep insights and flexibility** and have either technical support or a team comfortable navigating a robust analytics platform.

——-

Both platforms allow you to track meaningful data, but I do want to point out they serve different needs.

Along with the great resources Michael Thomas provided in his most recent comment I wanted to point out some pros and cons of each.

**Matomo**

Delivers comprehensive analytics capabilities while still supporting cookieless and privacy-compliant tracking.

**Matomo**
Matomo is the closest alternative to a full analytics suite like GA4 because it offers *deep reporting*, *data ownership*, and *privacy-first configuration options*. It can be *self-hosted* or used as a hosted cloud service depending on your preference and resources. Its advanced privacy and compliance tooling (including cookieless tracking options) makes it a strong choice for children’s content where respecting consent is essential.

- **Full analytics capability:** Includes detailed reporting, customizable dashboards, segmentation, event tracking, and other advanced metrics.

- **Data ownership & privacy:** 100% ownership of your data and strong compliance with GDPR, CCPA, and other privacy laws.

- **Cookieless tracking:** Can be configured to operate without cookies while still providing meaningful insight.

- **Flexible hosting:** Choose between self-hosting for maximal control or cloud hosting for easy management.

**Considerations**
Matomo requires more setup and administrative effort than simpler tools. It’s great if you need *longer-term depth and flexibility*, but initially it may take more configuration (especially if you self-host). That said, that upfront effort pays off if analytics are going to be a continuing priority for Ranger Rick.

**Best Fit Scenarios**

- You want a **GA-like analytics experience** with reporting depth.

- You plan to use analytics for content performance, campaigns, and audience insights.

- You have the technical capacity (internal or via partner) to maintain a more advanced platform.

**Alternate Option: Plausible Analytics**

**Overview:** Plausible is a *simple, lightweight, privacy-first analytics platform*. It focuses only on core metrics like unique visitors, page views, and basic goal tracking, and it’s designed to work without cookies or persistent identifiers.

**Pros**

- **Easy to use:** Clear, intuitive dashboard with essentials only – minimal training required.

- **No cookie consent needed:** Built to be cookieless and GDPR/CCPA compliant out of the box.

- **Fast setup and low overhead:** Quick to launch with no complex configuration or maintenance.

**Cons**

- **Limited depth:** Does not include advanced reporting, user journey analysis, or customization like Matomo.

- **Feature trade-off:** You get simplicity at the expense of insights into behaviors like funnels or segmentation.

**Best Fit Scenarios**

- You want **basic, high-level insights** quickly.

- You don’t need deep analysis or advanced metrics.

- Your priority is simplicity, minimal maintenance, and guaranteed compliance.

**Summary Recommendation**

- If Ranger Rick’s analytics needs are centered on **simple traffic awareness and compliance without consent-barrier complexity**, **Plausible** is acceptable.

- If you want a solution that can **grow with your analytics maturity, support richer insights, and replace GA4 functionality in a privacy-first way**, **Matomo** is the better long-term choice.Pro

---

# Consent Mode - Ranger Rick vs. [NWF.org](http://NWF.org)

- **[[NWF/Ranger Rick + NWF Analytics]] - Ranger Rick - Setup to track only essential until active opt-in**

  - [GA4 Measurement ID](https://analytics.google.com/analytics/web/?authuser=0&pli=1#/a119708728p342376695/admin/streams/table/4283990941): **G-5X1JRMQ1TX**

  - [GTM: ](https://tagmanager.google.com/#/container/accounts/84656/containers/235485638/workspaces/17)**GTM-THCHXB2K**

  - Other Tag IDs attached to

    - <https://rangerrick.org/>

      - [https://subs.rangerrick.org/pubs/NF/RRK/RRK_ReDesign_12_OP_May25.jsp](https://subs.rangerrick.org/pubs/NF/RRK/RRK_ReDesign_12_OP_May25.jsp?cds_page_id=283166&cds_mag_code=RRK&id=1770863862621&lsid=60422032124056547&vid=2&cds_misc_1=offpageGoogle&cds_response_key=I5FGS0Z)

    - [G-K0CTPQ0TKW](https://www.googletagmanager.com/gtag/js?id=G-K0CTPQ0TKW) - This looks like another GA4 Account

    - G-KOCTPQOTK - This also looks like another GA4 Account Connected

    - GT-PJNV86S

```javascript
--------# Connecting option 1: this is what GTM Provides-------
GTM Snippet That should be on https://rangerrick.org/
<!-- Google Tag Manager 1 of 2 -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-THCHXB2K');</script>
<!-- End Google Tag Manager -->

This should be added right after the <body> tag
<!-- Google Tag Manager (noscript) 2 of 2 -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-THCHXB2K"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

-------------- Option 2: This is what GA4 provides ---------
SETTING UP GA4 Measurement ID: G-5X1JRMQ1TX
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-5X1JRMQ1TX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-5X1JRMQ1TX');
</script>
```

- 

# **NWF - Setup to track everything unless opted out.**

- [GA4 Measurement ID](https://analytics.google.com/analytics/web/?authuser=0&pli=1#/a119708728p317256000/admin/streams/table/3600120279): G-RLRJ1GMJC2
- [GTM](https://analytics.google.com/analytics/web/?authuser=0&pli=1#/a119708728p317256000/admin/streams/table/3600120279): GTM-KF8N

---

# 2026 NWF - GA4/GTM Audit Next Steps - PII

> [!INFO]
> Meeting scheduled by NWF to discuss the recommendation of addressing the PII compliance (called by NWF to talk through the next steps they want from the Audit we provided)

[Meeting Recording](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8) | [[NWF/2026Jan27-NWF-AnalyticsAudit-NextStep-PII - Transcripts]]

NWF - Audit Task: <https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021>

## **Key Takeaways**

- **PII Leakage:** Personal data (emails, user IDs) is leaking into GA4 via URL parameters on pages like password resets and the Garden for Wildlife certification checkout.
- **GTM Overload:** The Google Tag Manager (GTM) account is at risk of hitting its 500-event limit due to an overly granular setup and contains old, insecure Universal Analytics (UA) tags.
- **SSL Error:** An SSL certificate warning is blocking new visitors. This is a known issue with the certificate vendor and is being addressed by IT.
- **Action Plan:** 4Site will mitigate PII leaks (est. 3–5 hrs) and propose a GTM cleanup plan to improve security and prevent hitting the event limit (est. 15–20 hrs for full implementation).

---

# 2025 Q4 - NWF

[NWF Weekly Report In Productive](https://app.productive.io/2650-4site-interactive-studios-inc/task/5048848?taskActivityId=214024379)

Adenga

**Current Task:**

[#709 2025 Analytics / GTM Audit and Overhaul (15:00)](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021)

---

## Budget Notes as of Wednesday, November 5, 12:38 PM

Stef is back from leave this week and is going to begin diving into [#709 2025 Analytics / GTM Audit and Overhaul (15:00)](https://app.productive.io/2650-4site-interactive-studios-inc/task/9659021) . If you prefer that work move to January so we do not use Floater hours, please let me know — we have a lot of Floater hours so I thought it may still be OK to keep it on the books but I can adjust.

**This Quarter’s Budget Details**

- **Starting budget:** 60 hours

  - **Used:** 40.25 hours

- **Remaining:** 19.75

- [Scheduled work and meetings this quarter](https://app.productive.io/2650-4site-interactive-studios-inc/projects/39172/tasks?filter=ODY3MjM3) **(est.)**: 48 hours

  - Tasks: 39 hours

  - PM: 6 hours

  - Meetings + prep: 3 hours

- **Available quarterly budget for new requests:** 0 hours

  - 🛟 Floater hours needed: 28.25 hours

➕🛟 **TOTAL FLOATER HOURS**

- **Expire:** 8/31/2026

- **Budgeted:** 86 hours

- **Used:** 9.25 hours

- **Remaining:** 76.75 hours

- **Scheduled work using floater hours this quarter:** 28.25 hours

- **Remaining Floater Hours After Scheduled Work:** 48.5 hours