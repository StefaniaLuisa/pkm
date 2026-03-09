---
pinned: false
external_files:
  - 1.6. Module recap.pdf

---


## [Diagram for how to capture the nested event](https://)

---

- **Engaging Networks (EN):** Shows higher page views because it counts every hit, including bots, refreshes, and even technical glitches. EN does not filter out most non-human traffic.

- **Google Analytics 4 (GA4):** Usually reports lower numbers. It *filters out* known bots and won’t count users who block cookies, use ad blockers, or don’t accept your cookie banner.

**2. Why This Impacts Your Conversion Rate**

- Conversion rate = Submissions ÷ Page Views.

- If EN is your source, your page view count is probably too high, so your conversion rate looks artificially low.

- If GA4 is your source, your count is lower, so your conversion rate looks higher than reality.

- Neither number is “perfect”—transparency is key!

**3. How To Get the Most Accurate Page View Count**

- **Use GA4 as your “source of truth”** because it’s the industry standard and filters out most bot traffic.

  - Accept that GA4 may undercount some visitors due to privacy tools and cookie consent requirements.

- **Track the difference (“gap”) between GA4 and EN:** Regularly compare the numbers. If GA4 is always around 60% of EN, you can use this to explain differences to your team or board.

- **Improve your GA4 tracking:**

  - Make sure your GA4 tags load early on the page.

  - Use Google’s Consent Mode so at least basic views are counted, even for users who don’t consent.

  - Double-check that bot filtering is enabled in GA4 (it is by default).

That is a great idea Christian, knowing the average data gap can help understand the difference and help explain the differences and make decisions.

Laura, unfortunately, no analytics platform will ever be 100% accurate, but there are a couple of ways your can feel a little better about the data you are seeing,

I usually recommend GA4 as your more accurate source (again never is 100%) - but this is only when setup with default bot filters and consent mode is Advanced, not basic. If your consent mode is setup as Advanced page_views will still be captured, so if you know that info, that might help fell that number is closer to accurate. However, If your Consent Mode is setup using its Basic mode, no data will be tracked until consent is given.

There are a couple of ways you can check which mode is installed, most CMPs have a section that states what mode is used, and some even have a general number of overall page-views which can be another resource to see which platform is providing you with the most accurate page_view number.

---

- 

That is a great idea Christian! Laura, I would even continue to keep track of the difference between GA4 and EN form page views over time, it can be a huge help to explain variances and get a better idea what the average gap looks like between the platforms.

Even though neither platform will ever be 100% accurate, I do think but there are a couple of ways your can feel a little better about the data you are seeing, I usually recommend GA4 as your more accurate resource, mostly because it is indurstry standard and does audomatically block bots (unless default settings have been updated)

There are also a couple things you can check to know what data you are getting in your GA4 accoun. First, I would check what consent mode you are using,if you are using the "Advanced" mode you are actually still collecting page_views and will be somewhat more accurate. However, if your consent Mode is setup using its "Basic" mode, no data will be tracked until consent is given.

There are a couple of ways you can check which mode is installed, some CMPs have an Advanced Settings section where you can chose this configuration. I would also check if you can see any metrics in your CMP dashboard, some do show pageviews - not by page but by total amount but can still be helpful to check against GA4 for accuracy.

Something else that came to mind, this is just an idea that would need to be tested, but if you setup a “form_view” event you should be able to track every time a visitor actually sees your donation form

Basic Consent Mode: Google tags only fire if a user consents to cookies (analytics, ads, etc.) and no data is sent until consent is given.
Advanced Consent Mode: Google tags can send “cookieless pings” even before the user consents, and page_view is captured, a cookie is only stored when/if consent is given. This might be overkill