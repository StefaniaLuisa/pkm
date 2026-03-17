---
pinned: true
Client:
  - 4Site
Title: Client Ideas
Due Date: '2026-01-05'
Task Details: 'Ask Fernando Questions about Regive - Add pushdown & regive to FWW agenda. '
Status:
  - In Progress
tags:
  - Ideas
  - projectIdeas
  - fww
  - engagement
Last Edited: '2025-12-28'

---

## **Enable Yoast SEO Schema Aggregation - Est \~30 minutes** 

Yoast just released a new opt-in feature called Schema Aggregation as part of Yoast SEO 27.1 (so we would need to make sure your plugin is updated to this version to enable).

What this does is adds a new endpoint to your site that publishes your entire structured data (articles, authors, posts) and organizational information into an format called, "schemamap.” that is optimized for AI search engines to recieve all of your site’s content in one go and see the connected “picture”, rather than adhoc based on what has been scraped/crawled recently or not.
**Our Recommendation: Enable this feature**
We do recommend enabling Schema Aggregation for your site. It is a low-risk, forward-looking change that helps make sure  your content is accurately represented as AI becomes a bigger part of how people find your org’s content and information online.

**What are the Pros?**

- It is completely opt-in and free, available on all Yoast SEO plans.
- It does not change your existing schema or affect how your site appears in traditional search results, the same data is simply organized and served more efficiently.
- It is built with a privacy-first approach and respects your existing Yoast privacy settings.
- It eliminates duplicate entities (e.g., the same author mentioned across many posts) and presents a clean, connected view of your site!
- It uses cached responses and is designed to handle server load efficiently, so it should have no impact on site performance.
- The feature was tested across real-world client sites before launch.


**What are the Cons?**
This does create a new public endpoint:

- Enabling Schema Aggregation adds a URL to your site (e.g., /wp-json/yoast/v1/schema-aggregator/get-xml) that exposes your site's full structured data graph to anyone,  including AI systems, who requests it. For most sites, this is simply a more organized version of information already publicly available. However, if your site contains content you intentionally restrict from broad indexing or AI use, you should evaluate whether this is a good decision and aligns with your organization’s goals and content strategy before enabling it.
- From what we are aware and know of your site’s content and structure you do not have many pages if any that are set to no-index so that search engines and Ai do not currently crawl.

It’s new and in an early stage:

- Like most of ai,  “Schema Aggregation” is a new the format not finalized or universally adopted yet, but its Microsoft so we do think that it will be a matter of time before wider adoption will take place
- All of Agentic Search actively consuming schemamaps is still developing
- It launched in March 2026. Yoast tested it in controlled environments with agency partners, it has not yet had a long track record in the wild.
  - We can schedule this task for 3-4 months from now to give it some time to mature



Please let us know if this is something you would like us to enable, if not now in a couple of months?

# CLF

<https://app.productive.io/2650-4site-interactive-studios-inc/tasks/15569234>

# Engaging Networks Quiz

- Demo Page: [~https://protect.worldwildlife.org/page/87293/survey/1~](https://protect.worldwildlife.org/page/87293/survey/1)

- Full Documentation: [~https://docs.google.com/document/d/199scy9pKuSDMAC-4JCSbLLiAXpmxPNcfezbz_khODOU/edit?usp=sharing~](https://docs.google.com/document/d/199scy9pKuSDMAC-4JCSbLLiAXpmxPNcfezbz_khODOU/edit?usp=sharing)

- <https://4site.slack.com/archives/C090PFE7TV0/p1768420532355129>

# Sitewide Redirect

#redirect

Recorded the National Trust for Historic Preservations sitewide redirect today ( [~https://cln.sh/P4xgdPtv~](https://cln.sh/P4xgdPtv) ) using code we developed that you can deploy on GTM + the target EN page.[~https://github.com/4site-interactive-studios/4site-nthp-eoy-redirect~](https://github.com/4site-interactive-studios/4site-nthp-eoy-redirect)

Might be good for anyone really - anyone that uses GTM

---

# Regive

#regive

Past project - Est = 12 Actual 18.5

But now that it has been developed what would the estimate be?

- AIUSA

- FWW

- NWF

- Shatterproof

Anyone that uses EN

**Could this be done for SCAN? - They use EveryAction -**

- [ ] **Ask Fernando how long would it take to implement regive to other EN/ENgrid clients. Could this be adapted for EveryAction - SCAN**

Resources:

[Regive: Turn Your “Thank You” Page into a Second Gift](https://www.4sitestudios.com/blog/regive-turn-your-thank-you-page-into-a-second-gift-with-just-one-click/)

[Donate Now and Help Protect the Planet | Rainforest Action Network - Fighting for People and Planet](https://act.ran.org/page/90804/donate/1?val&chain)

[Thank You Pages That Give Back | Portfolio | 4Site Studios](https://www.4sitestudios.com/portfolio/thank-you-pages-that-give-back/)

---

# Unsubscribe Page/ Options

I went to unsubscribe from SCAN and was sent to this page and really liked what it offers the donor - could use some design update: [https://cloud.alerts.savethechildren.org/preferencecenter?sfmcEmail=stefjones1024@gmail.com&cid=Email:SFMC:Annual_End_of_Year_5x:New_Leads_Coop_E6:122725&s_subsrc=|||266585||](https://cloud.alerts.savethechildren.org/preferencecenter?sfmcEmail=stefjones1024@gmail.com&cid=Email:SFMC:Annual_End_of_Year_5x:New_Leads_Coop_E6:122725&s_subsrc=%7C%7C%7C266585%7C%7C)

<https://cln.sh/tqRb3wLH>

---

# Multistep ENgrid Donation Form Embedd - Promo-Plugin Pushdown

#4site/client/fww #fww #PromoPlugin #client-ideas

*Monday, December 22 9:19 PM*

Inspired by FWW’s Donation Pushdown (however, button click, the donor is taken off-page to the full donation form) my version would keep on site. <https://cln.sh/qldQbDdd>

**Optimized User Flow:**

On a visitor’s first site visit, the page loads with a pushdown containing an embedded donation form (any ENgrid form):

[[Example - FWW - Embedded Multistep - Pushdown - Promo-Plugin_User Flow 1 of 2.png]]

The visitor can complete the entire action directly on the page. The embedded form is multi-step, and the visitor is never taken off the site or redirected to another domain.

Once the action is completed and the donation is made, the pushdown will no longer display for that visitor.

If the visitor bypasses the embedded form and takes no action, the pushdown will respond to scroll behavior by collapsing into a smaller pushdown CTA banner.

[[Example - FWW - Embedded Multistep - Pushdown - Promo-Plugin.jpg]]

At any point, the visitor can click the banner—either the CTA link or anywhere within the banner itself, similar to an accordion interaction—and the pushdown will smoothly expand back into the full embedded form. This ensures the donor can return to the form and take action on-page at any time, without worrying that they’ve missed their opportunity.

---

# Projects mentioned in ABM - Q4 2025

- **Human Detection Fraud Prevention** (Project mentioned in today’s ABM Meeting ( glad I stay on)

  - What other prep for Holiday audits, review can we offer?

    - Clean lists?

    - Review segmentation

    - Review email copy and strategy

    - A/B testing

  # Post-Holiday Stewardship

  [[4Site/Webinar/Post Holiday Stewardship Webinar - 11.2025]]

- **Post holiday donor stewardship -** mentioned this in the [~NWF slack~](https://4site.slack.com/archives/CP444T4CB/p1762450005193059?thread_ts=1762449008.308229&cid=CP444T4CB) - Helping to provide a strategy for our clients and recommend some communication can make a big impact.

  - Here are a few automation ideas that could be great to pitch or plan for January:

    - **1. A custom post-holiday gift Welcome Series for New Donors (Nov–Dec gifts)**

      - A short series thanking them, sharing what NWF was able to accomplish last year and that they are joining a community trying to do X, previewing what’s ahead in the new year possibly and putting in an “if” scenario where if the donor made a larger gift - end the series with a monthly ask - if lower gift amount

    - **2. One-Time Donors**
      Send a thank-you and impact update in January, mentioning that they have supported in the past - then follow up in February with a soft upsell to monthly giving.

    - **3. High-Dollar Donors**
      A more “personal” email from the President/CEO, thanking them directly and inviting deeper engagement, such as DAF giving? Attending/sponsor upcoming events, or tailored opportunities.