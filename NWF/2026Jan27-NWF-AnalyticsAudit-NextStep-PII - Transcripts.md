# GTM Action Plan Review - <https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021> (4Site & NWF) - Stephanie Waggys - January 27

[**VIEW RECORDING - 29 mins (No highlights)**](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8)

## Meeting Purpose

[Review audit findings and plan GTM/GA4 compliance actions.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=75.0)

## Key Takeaways

- [**PII Leakage:** Personal data (emails, user IDs) is leaking into GA4 via URL parameters on pages like password resets and the Garden for Wildlife certification checkout.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=273.0)
- [**GTM Overload:** The Google Tag Manager (GTM) account is at risk of hitting its 500-event limit due to an overly granular setup and contains old, insecure Universal Analytics (UA) tags.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1105.0)
- [**SSL Error:** An SSL certificate warning is blocking new visitors. This is a known issue with the certificate vendor and is being addressed by IT.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=384.0)
- [**Action Plan:** 4Site will mitigate PII leaks (est. 3–5 hrs) and propose a GTM cleanup plan to improve security and prevent hitting the event limit (est. 15–20 hrs for full implementation).](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1608.0)

## Topics

### PII Leakage in GA4

- [**Problem:** Personal data is being captured in GA4 via URL parameters.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=273.0)
- [**Identified Sources:**](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=273.0)
  - [Password reset pages (e.g., ](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=304.0)`.../reset-password?email=...`[)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=304.0)
  - [Garden for Wildlife certification checkout (flagged by Facebook pixel)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=161.0)
  - [URLs containing email addresses (e.g., ](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=823.0)`.../states/massachusetts/di-paolan@nwf.org`[)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=823.0)
- [**Solution:** Redact PII from historical data and configure GA4 to exclude it from future tracking.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=652.0)
  - [**Method 1 (Page-Specific):** Exclude specific pages or apps.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=791.0)
  - [**Method 2 (Parameter-Specific):** Exclude any URL parameter containing PII.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=681.0)
- [**Goal:** Prevent future leaks without losing valuable tracking data.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=780.0)

### Google Tag Manager (GTM) Overload

- [**Problem:** The GTM account is at risk of hitting its 500-event limit due to an overly granular setup.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1251.0)
  - [**Example:** A separate event for each donation amount ($10, $20) instead of a single ](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1332.0)`value`[ event with a dynamic parameter.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1332.0)
- [**Security Risk:** Old, unused Universal Analytics (UA) tags create security vulnerabilities and cause reporting errors.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1105.0)
- [**Solution:** Consolidate events and remove old tags to improve security, performance, and data integrity.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1105.0)

### SSL Certificate Error

- [**Problem:** An SSL certificate warning is blocking new visitors, likely causing a drop in traffic and donations.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=384.0)
- [**Cause:** A known issue with the certificate vendor that triggers an error 30 days before expiration.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=583.0)
- [**Status:** IT is aware and will update the certificate this week or next, coordinating with CRM and SLAM server updates.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=583.0)

### GA4 Reporting Inconsistencies

- [**Problem:** Inconsistent URL naming conventions (e.g., mixed case) cause GA4 to treat identical pages as unique, fragmenting data and making reporting difficult.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1008.0)
- [**Solution:** Standardize all URLs to lowercase to ensure consistent, accurate reporting.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1020.0)

## Next Steps

- [**4Site:**](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1459.0)
  - [Mitigate PII leaks in GA4 (est. 3–5 hrs).](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1608.0)
  - [Propose a GTM cleanup plan (est. 15–20 hrs for full implementation).](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1500.0)
  - [Send Kelly McGinnis the URL and screenshot of the SSL error.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1702.0)
- [**NWF:**](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1586.0)
  - [Provide 4Site with URLs of known PII-leaking pages (e.g., password resets) to expedite discovery.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1647.0)
  - [Review 4Site's proposals and confirm next steps.](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?tab=summary&timestamp=1586.0)

## Action Items

- **Review NWF GTM; draft cleanup plan (UA removal, consolidation, click event)** - [WATCH (5 secs)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1489.9999)
- **Email Stef PII URLs (password reset, CWH app, redirects); then Stef implements GA4 redactions** - [WATCH (5 secs)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1636.9999)
- **Email Kelly SSL error page URL + screenshot + cert details** - [WATCH (5 secs)](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1691.9999)

---

# Transcript

# GTM Action Plan Review - <https://app.productive.io/2650-4site-interactive-studios-inc/tasks/9659021> (4Site & NWF) - Stephanie Waggys - January 27


[**VIEW RECORDING - 29 mins (No highlights)**](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8)

[@0:05](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=5.96) - **Stef Jones (4Site Studios)**

Can any, can everyone hear me?

[@0:08](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=8.2) - **Donna Davidovich (National Wildlife Federation)**

Yeah, I gotcha. Yeah, I can hear you. So far, so good. A little snowy and cold, but otherwise, okay.

[@0:17](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=17.52) - **Stef Jones (4Site Studios)**

Yeah, I think we're all feeling that. We're doing okay. We're, you know, we're waking up in the morning, so we're getting there.

And how is it not February yet? I know. January always feels like the longest month of the year, you know, it's a whole year in one month, truly.

[@0:35](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=35.3) - **Donna Davidovich (National Wildlife Federation)**

Yes, true. We are getting there.

[@0:38](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=38.28) - **Stef Jones (4Site Studios)**

We are getting there.

[@0:40](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=40.44) - **Donna Davidovich (National Wildlife Federation)**

Is that your cat?

[@0:42](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=42.02) - **Stef Jones (4Site Studios)**

Yes, his name is Winston. He's the brains behind the operation, so.

[@0:48](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=48.7) - **Donna Davidovich (National Wildlife Federation)**

Love it.

[@0:50](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=50.2) - **Stef Jones (4Site Studios)**

Yeah, he's my, he's an older boy. He's 15, so he's my little, he's my baby, my little salt cat.

Um, well, is everyone here that. Matt is attending this meeting.

[@1:03](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=63.66) - **Stephanie Waggy (National Wildlife Federation)**

It looks like we're just waiting on Matt, but with the crunch for time, would say let's go ahead and kind of get started and I can catch him up with anything else later.

[@1:14](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=74.4) - **Stef Jones (4Site Studios)**

Sure. So I saw that you guys all looked at the audit, the recommendations, and wanted to focus on PII compliance, so like personal identifiable information and making sure that we're removing that, but I wanted to make sure to let me know what about that section you're like, okay, I want to focus on, because PII could be, it's a whole thing.

know there are aspects where you're bringing in some users' data, like emails, so we definitely want to redact those, but is there anything else when you're thinking about addressing PII and compliance that you want to make sure we're hitting?

[@2:00](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=120.0) - **Stephanie Waggy (National Wildlife Federation)**

I guess, Connie, can you speak to a little bit more of that, by chance?

[@2:09](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=129.76) - **Connie Hannigan-Franck (National Wildlife Federation)**

In PII compliance, that's more web space and removal of pixel information from people's personal when they come to us.

So that was not advertising. That is more a data collection entry point.

[@2:35](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=155.14) - **Stephanie Waggy (National Wildlife Federation)**

Okay. Yeah, I thought that there was, you could speak to what you were seeing where these issues were, but no worries.

[@2:41](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=161.7) - **Connie Hannigan-Franck (National Wildlife Federation)**

The one, the only, one point that I've seen in the past is when Facebook has said that the Garden for Wildlife certification page was shooting personalized information over the URL when people check out.

But that was the only issue that I have seen. But I'm not quite sure how to correct that on my end.

That would be probably web-based.

[@3:12](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=192.3) - **Stef Jones (4Site Studios)**

And that's something we can look through, like, at what content is being gathered, especially if you have the URL that is being used and that Facebook ad and, like, where that pixel.

I could look in your GTM to see how that pixel is set up. Oh, no, no.

[@3:27](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=207.3) - **Connie Hannigan-Franck (National Wildlife Federation)**

It's not my ad. It's just that it's detecting that the data is being, coming across. Yeah. see. The is seeing it.

Yeah. So it's not collecting the data from that URL, I guess, if that makes sense.

[@3:43](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=223.52) - **Stef Jones (4Site Studios)**

Okay.

[@3:43](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=223.98) - **Connie Hannigan-Franck (National Wildlife Federation)**

Because we just have the site-wide page view. Yeah. And Facebook's like, wait a minute, I'm seeing this, so I'm not collecting it.

[@3:51](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=231.48) - **Stef Jones (4Site Studios)**

Yep. Okay.

[@3:52](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=232.86) - **Connie Hannigan-Franck (National Wildlife Federation)**

Okay.

[@3:53](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=233.38) - **Stef Jones (4Site Studios)**

That's perfect to know that it's not, like, a honed-in URL that you're sending around. It's your Facebook pixel that's...

Yeah. Addressing the whole website and saying, no, there's some information that's being gathered that is not in compliance with their terms of service.

Gotcha. Okay. We could definitely make sure that we are looking at your Facebook pixel. And, I mean, it kind of goes along with there are some other areas of the site that we need to redact data based on, you know, PII.

But knowing specifically to address any issues with your pixels not firing can do that. Was there anything else? Because there, I can show you what I'm seeing and what you're gathering right now.

**SCREEN SHARING: Stef started screen sharing - [WATCH](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=281.119821)**

So looking in your account, but really looking at this audit dashboard is kind of like the best way to see what you're gathering.

Because, yeah, you can go through a lot of your report. And, And kind of lose yourself in there. But this kind of gets, are you collecting any personal information?

So what we're seeing here, and I just put the report from, you know, six, over six months, or it's about six months.

And what we're seeing is when someone is resetting their password to come in, and again, I'm not familiar with, you know, reset password and your carrier news at [pwcs.edu](http://pwcs.edu).

I'm looking, so the audit is reviewing your holistic GA4. So knowing exactly where someone can reset their password like this would be helpful to me so I can make sure that no, that this data, because right now, what we can do is confirm email change, and it's actually putting the email change.

We can say, do not track anything after this, oh gosh, parameter. was like, what is the, so we can say like.

later. Do not, when there's a parameter of, like, we can make sure no user IDs, but just knowing the exact page, so I'm not making any assumptions of where this might be at the moment.

So where people are resetting their passwords, their account, looks like there's a lot of reset passwords, [buildgrantsat.gov](http://buildgrantsat.gov). So this is kind of a weird one that's, like, programs, and if I grab this, and this audit page isn't, it's an audit report, so something like this, I just want to make sure, is this correct that this is an issue, or is this how the URL should be?

Yeah, we're having, this is an issue with PII as well, that the SSL certificate is not up to date, so.

Sorry, it was. I thought maybe I heard someone say something. So this is an issue for anyone trying to get to your site.

If they have not already been to your site and have said, you know, proceed, they're thinking that this could be a, like a spam site.

So if you have seen, you know, a drop-in donations or a drop-in viewers in a little bit, this could be an issue.

But I think what I saw is that the certificate, it actually looked kind of weird. If we look at the information for the certificate, if we go to council, we can actually see that.

I think there's like, this is worth looking into a little further. Go to developer tools. And if we look at, now it's going to be, we have,

We can see your SSL certificate in here. Of course, now I'm going to forget how to find it. Here we go.

And it might not even be showing up anymore to see, but there is a way you are able to see, like, when your SSL certificate is going to expire.

And when I went to go look at that for your URL, it looked like it was just, like, on the brink of expiration.

Like, something was off. And, of course, right now, everyone looking at me, where is it? But I can make sure I provide that to you and give you any information that I am seeing on the back end.

Which, even here, I feel like it should be showing up. You know, override overview here. There it is. I was like, oh, I'm making things up.

View certificate. So it's not trusted. So I don't know where it was bought. Something is up with, because here it says expires by Friday, February 13th, 2026.

So there's time, like this shouldn't be happening. And I did test this on Chrome. I did test this on Safari, and it is showing up if you're not, if you've never been to the site before, like clearing cookies.

So a person could say always trust, but you want that to be done right away. Whoever bought the SSL and whoever set it up might be just worth looking at the configuration.

It's good to know. Oh, Kelly? Sorry. Oh, no worries.

[@9:43](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=583.261) - **Kelly McGinnis (National Wildlife Federation)**

So just for the benefit of this group, John, who is our networking guy, he is aware of the certificate expiring in February.

For whatever reason, this certificate, when it's like 30 days out from expiring, Hiring, it triggers an error because it falls below a certain threshold that is, I don't understand the complexities about it in the backend, but he is aware and this is being updated, I think, I think actually this week or Monday of next week, because we've got to make those same updates on our CRM and SLAM servers.

So I know they're all interconnected.

[@10:26](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=626.541) - **Stef Jones (4Site Studios)**

Gotcha. Okay. Well, yeah, I don't want to waste your time with that. Yeah, that's a bummer. If there's a different, because SSL, you could pretty much buy from your favorite vendor that sells them.

I don't think that's common to have kind of this issue 30 days out, but I could be wrong. You know, I would follow your IT's recommendations.

Okay. With that, just looking at, again, this is the private data that you do want to. And one of the things I will do is I'll go through your Google Analytics account.

And what we can do is redact, like we have your data deletion requests. So we can focus on some of the data deletion.

And we can also look at other areas that we can redact data. And we would only focus on taking out those parameters.

So anything that's after the question mark that holds any email or any personal PII, we can just remove it.

That way, if there's any issue with it removing any significant or important data, I will flag that and let you know.

But we should be able to remove just the data that is not PII compliant. Are there any questions on that?

next time. you you time. So we'll So

[@12:03](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=723.321) - **Stephanie Waggy (National Wildlife Federation)**

I guess, Matt, did you have any other specifics with the PII stuff that we wanted to look into?

[@12:10](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=730.901) - **Matthew Kehres (National Wildlife Federation)**

I mean, I think we've talked about a few of the specific points that came up in the audit, like some of the password reset things, some of the data that we think is getting passed from, I believe, the Certified Wildlife Habitat app, or to other, you know, I think a lot of it is showing up there.

Like, basically, it's sort of the question that was posed earlier. It's like, is there a specific area we can find where it's like, just do not track after a specific URL parameter?

Or can we just ignore this type of page?

[@12:56](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=776.561) - **Stef Jones (4Site Studios)**

Yeah. And yeah, we can definitely do that. So Just to ensure that we don't run into this again because, of course, we can redact, but it would be best just to make sure that that doesn't get tracked in the future.

And again, so if this is an app or, again, because I'm not familiar with every aspect of the website, providing where this is happening would be really, really helpful because then we can see, do we need to say, okay, don't track this one page?

Or do we need to say, don't track after the parameter? You know, we can kind of do this a different way where we can be explicit about not tracking data.

And if it's multiple pages, again, we can do something similar.

[@13:42](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=822.721) - **Matthew Kehres (National Wildlife Federation)**

That makes sense. I guess the other one question I had is, it looked like in one of the examples you provided in the audit that, I don't know if it's like, it looked like it was like an email address that was showing.

And it's, I guess, is that something we need to be telling, I don't know, program teams or others that are developing their own pages or providing content like that, that like naked email address links in content can flag this, or is there something we can do to like avoid those getting like picked up?

[@14:26](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=866.521) - **Stef Jones (4Site Studios)**

Yeah, I mean, it's definitely, these are getting picked up outside of your website. That's the thing, like they're getting picked up when they're being taken to these pages, you know, and so that's kind of interesting, like this is States, Massachusetts, and then it has a at [nwf.org](http://nwf.org).

So I'm assuming this is someone who might work there, like Di Paolan. And so that to me is like, is there something, an internal, like.

Even a, like, gosh, Outlook or Microsoft has, like, an internal site that a lot of corporations and organizations use, and then it links out to different things.

Is that happening where, does that sound familiar or anything? Because I'm trying to see a lot of these. It is kind of weird why it's appended to, like, a URL.

[@15:28](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=928.581) - **Matthew Kehres (National Wildlife Federation)**

So, it's interesting, the formulation here, I'm wondering if these are on our blog, and maybe we had guest authors or something?

I can check one of these real quick.

[@15:42](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=942.681) - **Stef Jones (4Site Studios)**

Yeah, and through the work that I'll do to look at how to redact and make sure that we are blocking this from getting tracked in the future, I can also, you know, look at where these are coming from and spend some discovery time, because I'm going to need to make sure that I'm covering all my bases.

But it is like just looking at it and what I've seen, it is kind of interesting that there's a mix of [nwf.org](http://nwf.org) email addresses, but then there are Gmail.

So I just, if you guys knew off the top of your head, like what might be passing people's information through, is there a, is there a form that's redirecting people?

If there's someone who's like signing up and then it's taking them somewhere else, like their data is getting passed through somehow, you know?

So anything like that helps me like hone it down and save time.

[@16:34](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=994.101) - **Matthew Kehres (National Wildlife Federation)**

Yeah.

[@16:36](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=996.261) - **Stef Jones (4Site Studios)**

But we could definitely make sure it doesn't get tracked in the future. And if we can't find the exact area, we'll do it by parameter instead of like by page or app.

The other thing is kind of looking at you're not found, like all of this kind of does go into making sure your, your compliance isn't.

I think there are a little bit of inconsistencies with how page paths are set up, which can, you know, I think the biggest thing there is that it's just hard for your reporting when Google Analytics 4 or Google Analytics in general does not see case all the same.

So if you have an uppercase one time and a lowercase another time, it's going to see it as two separate pages or two separate reporting or tracking.

So that's something to note as you do create new pages in the future or even your current pages to really look at what you are currently doing and keep it consistent.

So now that you do, you kind of do have this like sentence case going on, if you're using that in like, like sharing on Google or sharing on, you know, social, make sure that it is, it does match this cadence.

Um, or naming convention. Uh, Google does prefer everything lowercase. Lowercase just makes it all consistent and you kind of just, the more consistency you can give Google, the better, and just kind of making a standard of every URL lowercase, every, uh, tracking parameter lowercase just makes it easy to keep consistent moving forward.

Um, I think kind of going through that, I do also know, uh, there's a lot, I think what I noticed is that your GTM looks scarier than it really is.

And the reason why is it because there's so many old tags and things like that do cause a security risk.

When you have tags that are not being used and they're depreciated. Those are like weak points, um, that people can figure out how to take advantage of.

There's. Those old UA, Universal Analytics tags, those can cause reporting issues, duplication. And again, those are weak points. I almost think of it as with WordPress, you always need to keep up your plugins.

And the reason why you want your plugins to work well, but they also, if you have older versions of your plugins, they're all security risks.

Because there's a reason why they need to update it. Those are just like your weak points. And so having, you have a lot of tags and variables in your GTM account that are not being used.

And if they are, it would be advantageous to look through. And anyone who does actively use Google Tag Manager, GA4, to really sit through and look at and be like, which one of these can we really need?

Which can be consolidated? Because I did notice there are multiple, very granular events being created for each click or button.

And really, that could be all merged into one event. Because one event, you can just set up a click event.

You're gathering every click that's done on the website. And from that click event, you will start getting the pages that are being clicked automatically.

automatically, you can make sure the copy that the link is will pass through. And that way, you do need to report on it.

You would take your report that would be your click event. And then you can show, OK, what was the copy that was clicked?

What was the URL that page was on? You're almost at capacity with how many events you can even have before Google will not allow you to create anymore.

says, if haven't below. And So I think you're at the point where if you needed any more events, you would not be able to create any more very shortly.

So cleaning up GTM will help. Insecurity, I have no doubt. It doesn't have so much to do with PII, but just making sure that your data is coming through correctly and you have no security risks on any of your data that you're collecting, especially having to do with GA4 and GTM.

And I can provide if that, because it can be overwhelming, I can provide what I recommend a way to go through that.

I think it does start with whomever uses these platforms the most and really doing, and I could join and help if wanted, but really like looking through what is being used and what's not.

And I do have, I did provide what is I do because when That Tracker, so this is a repository of all of your, these are all of them.

So here's your tags, so your triggers, and like all of these, this, a lot of these can be consolidated, where instead of it being a report that's a line item for each money, each dollar amount being donated, you would be able to get any information, and you are kind of like digging deeper into a like value event.

would be like what Engaging Networks, Lightbox, value, and then you would be able to see, okay, they gave $10 or they gave $20.

So the reporting would be a little different, and the benefit of that is not having, not reaching that limit that you guys are almost at.

So point? There's nothing inherently wrong with how this is being set up. It is very granular, and if you're used to it, but you are running a risk of it moving very slow.

It could be one of the reasons why you're getting more data than you intended, and you will max out how many events that Google allows you to have, which is 500.

So any questions, I can recommend some next steps just based on what we've talked about right now and kind of like what I've laid out in the recommendation, but I want to make sure I'm not missing anything.

[@24:07](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1447.14) - **Stephanie Waggy (National Wildlife Federation)**

Stef, if you'd like to share, yeah, kind of what you think next steps. I know Kelly has a quick question at the very end, but we can get that in here.

[@24:13](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1453.36) - **Kelly McGinnis (National Wildlife Federation)**

Yeah, sorry. I was holding off until we were fully done with the agenda because I don't want to monopolize time.

[@24:18](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1458.34) - **Stef Jones (4Site Studios)**

Yeah, yeah. You know, I want to follow through with, you know, looking at your PII risks. I'll go through, you know, case and parameters.

I can dive a little bit more into the variations and what I recommend and how you can move forward in keeping consistency just based on what I'm seeing.

But I will look through the page paths, like, you know, shown here, and I will make the choice of either making sure these pages are excluded, or we just exclude the parameters that are bringing in the personal information.

**ACTION ITEM: Review NWF GTM; draft cleanup plan (UA removal, consolidation, click event) - [WATCH](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1489.9999)**

So we can go a different couple ways with that and what we need to do. So we'll follow those.

Another thing that I would love to recommend is I'll write out some plans on how I would audit your audit, like how I would go through your triggers and your tags, and I can lay out some recommendations I have.

I have not changed anything. This audit was to gather all of your information to better understand it, and what I really saw was a lot of these are so granular that there is a lot of opportunity to combine, and there's a lot of old events.

And definitely anything that's under universal analytics needs to be removed, depreciated, and I would be happy to work with whomever sets these up and kind of show them how I would recommend.

Like I don't have to do all the like combining and merging. I can show whomever and recommend a way that just building it a little different.

And again, this isn't the wrong way to do it. It just caps you out, especially with all your sites, especially if you're using a GTM for so many different sites and you're being so granular, that's where it becomes an issue.

So I can write out some steps that I recommend, how to look through it, how I can help, or showcase how to just merge a couple things.

Does that sound good?

[@26:26](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1586.62) - **Stephanie Waggy (National Wildlife Federation)**

Yeah, that sounds good. I'll get with the team and get back to you here. Probably today or tomorrow, specifically kind of our thoughts after this.

[@26:33](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1593.24) - **Stef Jones (4Site Studios)**

So thank you for walking through everything. Of course, if there was anything I missed, I think, you know, please let me know.

just wanted to make sure that if there was anything outside of, you know, the PII risks that I labeled here, that I'm definitely hitting.

And I think to start off, just an estimate of what something like this would look like. And I don't remember if I added an estimate already.

Alright. Thank

[@27:01](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1621.92) - **Stephanie Waggy (National Wildlife Federation)**

I think he did. I think it did too.

[@27:06](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1626.08) - **Stef Jones (4Site Studios)**

This is the consolidation, so right here. And yeah, that would be for all of this. So would you like, oops, because I thought you just wanted the PII mitigation.

**ACTION ITEM: Email Stef PII URLs (password reset, CWH app, redirects); then Stef implements GA4 redactions - [WATCH](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1636.9999)**

So 15, 20 hours is everything that's laid out right here.

[@27:25](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1645.36) - **Stephanie Waggy (National Wildlife Federation)**

Okay, perfect.

[@27:27](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1647.02) - **Stef Jones (4Site Studios)**

So I would say like the PII mitigation, I would give like three to five hours just to make sure.

And I think the more you can give me up front of like telling me where the, if you can even send me the URLs that you even think, because the discovery is, I don't want to waste time, you know, trying to find where these things are.

Of course, I'll do my due diligence and look for it. But if you already know, please send those over.

And, and anytime I don't use, I'm not going to use, you know, so, but just a three to five hours because Google Analytics likes to just.

Be fun and not be easy, but.

[@28:03](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1683.74) - **Stephanie Waggy (National Wildlife Federation)**

Of course, right? That makes sense.

[@28:05](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1685.32) - **Stef Jones (4Site Studios)**

Yeah. No. Okay.

[@28:07](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1687.32) - **Stephanie Waggy (National Wildlife Federation)**

Well, I'll catch up with everybody internally because I know we're out of time and then I'll let you know for our next steps what we want to go forward.

**ACTION ITEM: Email Kelly SSL error page URL + screenshot + cert details - [WATCH](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1691.9999)**

So thank you for walking through everything.

[@28:14](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1694.96) - **Stef Jones (4Site Studios)**

Of course. Of course. I will reiterate everything in the task and I'll hear from you guys soon.

[@28:20](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1700.22) - **Stephanie Waggy (National Wildlife Federation)**

And Stef, just really, really quick.

[@28:22](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1702.5) - **Kelly McGinnis (National Wildlife Federation)**

Can you please confirm for me what page you were on when you saw that SSL cert error?

[@28:28](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1708.62) - **Stef Jones (4Site Studios)**

Yeah. Yeah. I, uh, it looks like I was going to, uh, here, I will share that with you right now.

[@28:37](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1717.24) - **Kelly McGinnis (National Wildlife Federation)**

Perfect. And if you have a screenshot you could send me, um, yeah, either via email or however, that would be super helpful.

[@28:44](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1724.82) - **Stef Jones (4Site Studios)**

Yes, I will do that. And that's no problem. I can even, um, that certificate that had the error and stuff, can get that to you as well.

[@28:52](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1732.78) - **Kelly McGinnis (National Wildlife Federation)**

Perfect. Thank you so much.

[@28:54](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1734.5) - **Stef Jones (4Site Studios)**

Of course. Of course. Everyone have a great day.

[@28:56](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1736.94) - **Kelly McGinnis (National Wildlife Federation)**

Thank you. Thank you.

[@28:58](https://fathom.video/share/_bSdMg5HzLKXoYQxbyh8d5HiquU-cnK8?timestamp=1738.22) - **Stephanie Waggy (National Wildlife Federation)**

Bye guys.