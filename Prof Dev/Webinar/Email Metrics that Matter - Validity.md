---
Title: Webinar - Validity Email Metrics Webinar Notes
Date: '2025-12-10'
Recording Duration (mins): 60
tags:
  - webinar
  - email
  - resources
  - 2025-Q4

---

> **Webinar Date: Wednesday, December 10 11:06 AM**
>
> Voice Memo Recording:

- Define specific, measurable business results from email.
- Shift success metrics from email opens to valuable recipient actions (e.g., clicks, purchases).
- Distinguish B2C (immediate conversions) from B2B (long- term lead nurturing) goals.
- Identify key metrics that directly quantify and prove business value.
- Connect subscriber engagement behaviors (clicks, activity) to the bottom line.
- Analyze foundational technical metrics like deliverability and sender reputation.
- Diagnose issues by connecting these three layers of data. Metrics proving worth to stakeholders

## Ai Summary

# My Notes

## List Growth

• The Metric: The rate at which your list is growing net of churn (unsubscribes and bounces). • The Formula:

| New Subscribers - (Unsubscribes + Hard Bounces) * 100 Total List Size

• Why It Matters: A stagnant list is a dying list. You must acquire new leads faster than you lose old ones to natural decay.

• Diagnostic Use:

relevance). Negative Growth: Diagnose your churn sources (frequency fatigue, content

• Flat Growth: You are only replacing churn; investigate new acquisition channels.

• Benchmark: A healthy list grows by roughly 2.5% per month (according to a study conducted by the Data & Marketing Association).

## Subscriber Lifetime Value (SLV)

Subscriber Lifetime Value (LTV)

• The Metric: The average revenue a single subscriber generates for your business during their entire time on your list (active emails only). • The Formula:

• (Monthly Revenuc from Email) * Average Lifespan (in Months) Total Subscribers

Why It Matters: This defines your "ceiling" for acquisition costs. You cannot spend more to get a subscriber than they are worth.

Diagnostic Use:

- Budgeting: Use LTV to determine your maximum Cost Per Acquisition (CPA).

Investment: Use high LTV to justify budget increases for retention and personalization tools.

Benchmark: • Aim for a 3:1 LTV-to-CPA Ratio. • You should earn $3 for every $1 spent acquiring a customer.

## Other Metrics to Track:

<https://cln.sh/qF9rDRS6>

## Valuing the "Non-Revenue" Action

• In B2B, emails rarely generate immediate cash. They generate conversations.

• Measure Pipeline Contribution, not just closed deals.

• How to Value "Non-Revenue" Actions:

- If 1 in 10 Webinars leads to a $10k deal, then 1 Webinar Registration = $1,000 (Weighted Value).
- Key Metrics to Watch:
  - Marketing Influenced Revenue: Revenue from deals where email touched the prospect during the journey.
  - Pipeline Velocity: How much faster do deals close when the prospect is engaged with email content?
  - MQL to SQL Conversion: The rate at which email leads are accepted by Sales.
  - MQL = Marketing

## Engagement Metrics

BROKEN Metrics:

→ Open Rate

(Total Opens/Delivered Emails) * 100

• The Metric:

The percentage of delivered emails that loaded the tracking pixel.

Apple Mail Privacy Protection (MPP):

- Apple pre-fetches (downloads) email images via proxy servers, regardless of whether the user touches the phone.
- This triggers a "False Open" for nearly every Apple user.
- Open rates are artificially inflated (often by 30% - 50%).
- "Open Time" and "Device Data" are obscured (geo- location is generic).

New Reality:

- The Open Rate is now a directional signal, not an absolute truth. It's useful for trendlines, but dangerous for segmentation (e.g., "Resend to non-openers" now misses people).

## Measuring Interest: CTR, CTOR, and Attention

These are the VITAL Mertics for Engagement

→ Click-Through Rate (CTR) Total Clicks (Delivered Emails) * 100

Insight: Measures overall campaign performance (Subject Line + Content) Benchmark: Average is 2.0% - 2.3% (HubSpot). Top performers hit 5%

→ Click-to-Open Rate (CTOR)

- 100 Unique Opens / Insight: Measures the effectiveness of the content itself, stripping out subject line performance Benchmark : Average is \~6%, but healthy programs aim for 10% - 15% (Mailerlite)

→ Read Rate / Dwell Time Percentage of emails viewed for 8+ seconds Insight: Measures if content was consumed or just "loaded". Benchmark : Aim for &gt; 60% Read Rate (Litmus)

<https://cln.sh/QsW9S88n>

## The Good Goodbye:

<https://cln.sh/0vJZX2ny>

→ Unsubscribe Rate

(Total Unsubscribes/Delivered Emalls) * 100

• The Metric: The percentage of recipients who choose to opt-out of your communications •

Insight: Unsubscribes are not the enemy; they are organic list hygiene.

Benchmark: Litmus recommends keeping this under 1% - 2%. High-performing lists often see rates below 0.5%

Danger Zone: A sudden spike (&gt;1%) indicates "List Fatigue" (sending too often) or a breach of trust (content mismatch)

Best Practice: Never hide your unsubscribe link. If a user can't find the exit, they will force their way out by clicking "Mark as Spam" - which is far more damaging.

# Deliverability & Reputation Metrics

<https://cln.sh/DKGQF5yc>

Delivery vs.→ Bounce Rate **NEEDS to KEEP under 2%**

(Tallene Emails *100 Total Sent Emails The Metric: The percentage of sent emails rejected by the receiving server (Gateway). Source: Your ESP. Insight: High bounces indicate blocking, poor list hygiene or invalid addresses. Benchmark: Keep below 2% → Delivery Rate Total Sent - Total Bounced* 100 Total Sent The Metric: The percentage of emails successfully accepted by the receiving server. Source: Your ESP. Insight: "Delivered" only means "Accepted", it does not confirm the email went to the Inbox. → Inbox Placement Rate (IPR) Total Sent - Total Bounced * 100 Total Sent

The Metric: The percentage of emails that land in the Primary Inbox rather than the Spam folder. Source: Requires Validity's Litmus, Everest, or Sender Certification. Insight: This is the only metric that confirms visibility. Your ESP cannot see this data.

## Reputation Signals

<https://cln.sh/8fkGXFp6>

0.1 user complaint rate - more than 1 complaint per 1,000 emails - inbox providers start dinging you

.3 or more - Google will start sending your emails to Spam

## SRD:

Microsoft proactively marks emails as Spam

Google Postmaster Tools (GPT) Microsoft SNDS * 100 • URL: [postmaster.google.com/](http://postmaster.google.com/) • URL: • explicitly clicked. "Re

• Domain and IP Reputation: sendersupport.olc.protecti h Google/Yahoo)

High/Med/Low/Bad, this will go away consiste om/snds/

at the end of 2025.

• Compliance Dashboard: The single o source of truth for Gmail delivery. It now tracks 8 specific requirements • Filter Result: Your "Traffic l • Green: Good, Spam &lt; 10% • Yellow: 10% &lt; spam &lt; 909 spamme Red: &gt;90% sent to Spam.

Authentication: SPF, DKIM. DMARC, and From: header alignment. ins Complaint Rate: Rounds to see 0.2%, you have a critic Unsubscribe: Checks for both "One- click" and "Honor unsubscribe" Junk Votes Trap Hits: Shows raw coun compliance. (lotal Junk otal Not Junk vol"Pristine" vs. "Recycled" tr Spam Rate: Checks against the 0.3% soft asks random users 'Did you think this. is threshold. Status: Goal is all Green ("Compliant"). "Needs Work" indicates a blocking risk ativ

## Reputation Visibility: Where to Look

### Google Postmaster Tools (GPT)

• URL: [postmaster.google.com](http://postmaster.google.com)

==🔴• Domain and IP Reputation: High/Med/Low/Bad, this will go away at the end of 2025.==

• ==🔴Compliance Dashboard: The single source of truth for Gmail delivery. It now tracks 8 specific requirements: • Authentication: SPF. DKIM. DMARC. and From: header alignment. • Unsubscribe: Checks for both "One- click" and "Honor unsubscribe" compliance. • Spam Rate: Checks against the 0.3% threshold. • Status:==

Goal is all Green ("Compliant"). "Needs Work" indicates a blocking risk.

### Microsoft SNDS

• URL: [sendersupport.olc.protection](http://sendersupport.olc.protection).outlook.c om/snds/

THIS will only work on owned IP address -will not work on shared ID

• Filter Result: Your "Traffic Light" status: • Green: Good, Spam &lt; 10% • Yellow: 10% &lt; spam &lt; 90% • Red: &gt;90% sent to Spam.

• Complaint Rate: Rounds to 0.1%. If you see 0.2%, you have a critical problem.

• Trap Hits: Shows raw count of "Pristine" vs. "Recycled" trap hits. S

### Sender Score

• URL: [senderscore.org](http://senderscore.org)

• What it is: A global "Credit Score" for your IP (0-100).

Ideal above 80 score

• Tiers: • 0-70 (Poor): Reputation needs repair. • 70-80 (Fair): Functional, but risky. • 80-100 (Good): Healthy sending habits.

## Diagnosing with Data

<https://cln.sh/NNW6HrQ0>

## Litmus

<https://cln.sh/MR3snGXs>

## Key Takeaways: Your Measurement Checklist

• Measure Value, Not Volume • Focus on Conversion Rate and LTV to prove business impact. • Stop reporting vanity metrics (Open Rates) to leadership.

• Monitor the "Real" Engagement • Switch from Open Rate to Read Rate (Dwell Time) to deal Apple MPP issues.

Watch CTOR to ensure your content delivers on your subject line's promise.

Secure Your Access

Don't trust "Delivered." Measure Inbox Placement Rate (IPR).

Check Google Postmaster Tools weekly for Compliance/Spam Rate (&lt;0.1%).

&gt;Next Steps

Audit your current reporting dashboard against this checklist.

Download the Litmus State of Email Report for deeper benchmarks.

# Validty Email Metrics - Webinar Transcript

What's up that we look good? We're ready to go. Just another drama. You know, that's a live show. It's showbiz. There you go. Uh, we will give people just one more minute of seeing these numbers tick off. All right. I think we're ready to get started. You ready, Raphael? I am. Awesome. Oh, we have a thumbs up. Sounds great. Looks great. Thanks, Steph. Awesome Okay, well, let's kick it off. I'm Jessica. and Validity's director of brand and content for the next 30 minutes. We are going to talk about all things, email, marketing metrics, uh, including which metrics to track, which to take with the grain of salts, um, and how to prove the real value of your email program, which I know is top of mind for a lot of us, with 2026 planning happening. Before we get started, just a few quick reminders. If you have any questions throughout the session, just enter them using the chat or the Q and A buttons. We love to see a lot of live discussion going on. So don't be shy. Um, and we'll definitely save time at the end for any questions that don't get answered. Also note that everyone will receive a recording of the session by email within the next few days. We always get that question a bunch of times, but yes, you'll be getting this deck. Um, and without further ado, let's meet our speaker. Raphael. As a senior email strategist at validity, Raphael helps companies all over the world overcome challenges related to email marketing strategy, deliverability, platform migration, segmentation, and email journeys. Did I miss anything, Raphael? It's quite a rap sheet. I'm presenting. There's that too. Yeah, webinar star. forgot about that one. Do you want to take us through what we're covering today? Yeah, well, hi, everyone. Well, thank you for joining us. I know how packed our calendars are right now with uh, yeah, a lot going on. A lot of you, I know, are in the middle of planning mode and looking to set your goals and strategy for next year. And I think that's the perfect moment for us to pause and ask. Are we actually measuring the right things? Because, I mean, the definition of success in email is shifting right under our feet. We know that digital markers were many hats, and we must focus on our limited time and attention on actions that actually drive measurable business results. So we're moving away from the, the, the vanity metrics, like open rates, and we're now focusing on ensuring that every email sent be specific to take a valuable step. And we need to recognize that that valuable step looks different for everyone. In B to C, right? You push for it, you need conversions. Where in B is B to B, you focus on the nurturing and advancing the business evaluation process. But regardless of your industry, you need the data that reflects these skills. So today, We have structured this discussion on this specific order here, where we'll start at the top. By defining business impact metrics and how to measure the success, improve your worth to the stakeholders. Next, we'll talk about the engagement metrics and pretty much the subscriber behaviors that drive the revenue. And finally, we'll uncover delivability and reputation metrics, which are the technical foundation that makes everything else possible. So by the end of the session, you possess the ability to diagnose email problems by looking at these 3 layers of data. All right. So we'll begin our deep dive at the top of the pyramid, which is business impact metrics. So these are the numbers that translate your daily work to the only language that your stakeholders and boss, truly speak, which is revenue, growth, and oral. So before you optimize a single subject lines, you must define what success actually looks like on the balance sheet. So zooming in at this very important metric that your boss is like a hawk into this, right? is conversion rate. This is your ultimate source of truth. It doesn't matter how many people pay email. And how many people completed the desired outcome, right? Whether that's buying a product, registering for a webinar, like this one, or downloading a resource. This is the final measurement of your email's revenue potential. And to calculate this, you divide the number of people who completed the action by the number of delivered emails. And while benchmarks are out there, they vary so much by the different industry. usually hovering between one and 5%. Your goal should be your own historic package. And also, if you see high click rates and low conversions, the email that is child, but maybe your landing page is faint. Maybe the form is too long or the offer isn't quite clear, but it's both of them click and the conversions are low. There's likely happening, there's some disconnect within the email itself. So the conversion rate isolates exactly where the friction is in your phone, okay? All right, next, let's look at list growth free. Many marketers, they make the mistake of accounting just the new signups, but that's just like a vanity metric. We need to understand that beer growth accounts for the people leaving too. or the child. I mean, email list they naturally decay about 25% every year. So it, I mean, it helps to think of the list as a leaky bucket. You know, people naturally change their jobs, they abandon their email, unsubscribe. That is just the normal decay. To find the real growth, the true growth, you need to subtract or unsubscribes and you heart bounce from the new subscribers and divide that by the total list size. If you see a result that is negative, then you're listening shrinking, and your revenue petition's also shrinking. So your goal is to outpace that natural decay. A healthy program usually sees at 2.5% month over month net growth. So if you aren't hitting that, then you need to investigate your position sources immediately. All right, this metro here speaks the loudest to a finance team. Subscriber Lifetime Fad. This tells you exactly what one email address is worth. And you calculate this by multiplying your average monthly email attribute of revenue per subscriber by the average number of months they stay on your list. So your goal is to hit the golden rule of a 3 to one ratio. That means that for every dollar you spend to get a subscriber, you make $3 back. Um, and Y 3 to one? Well, the consensus is that the 1st dollar that you, that you, that you get, it pays for the ad, and the 2nd covers your overhead and your salaries. And the 3rd is your actual profit. So you sort of below this, you're likely losing money, but if you're above it, then you're not spending enough to grow. All right, before we leave the business impact metrics sections, we have to address a scary reality. We can see here from this source, the state of email by Litmus. Industry data is showing one in 5 marketing leaders have absolutely no idea what the email ORI is. And this is a massive blind spot. So if you aren't on that 21% there, you're vulnerable. So when your budget gets cut next year, the 1st the 1st program is to go or the ones that can't prove their word. So you need to close that gap immediately and understand your ROI per email. And to do that, these formulas here will give you that help. So for ROI, you can, well, you can look at at the big picture, like the ROI for the whole year, but it can also drill down to specific campaign. And the same goes for revenue per email. I recommend calculating the revenue per email per campaign, right? Because I mean, per email, it makes sense. And this let, this specific metric, the revenue per email, that helps you see if, for example, if you choose a newsletter, if that one is more efficient than your Friday promo. Regardless of the list side, right? So it's a very useful metric to use as well. There's also customer acquisition costs or CAC, CAC. I give you when I line that with your with your budgeting cycle, which is usually monthly or quarter, the form is over there. And finally, track your average organ society. month over month. This helps you spot season a trend, like people spending more per card in November versus July, which tends to be the case because of Black Friday. But the key here for all of these metrics is time frame alignment. You have to ensure your revenue and your cost, they align with the exact same period. Whatever period you choose to calculate with. Now, I know that many of you out there are thinking, I'm in B to B. I don't have a shopping card. My emails don't generate, you know, cash instantly. And you're right. For you, revenue isn't an event. It's just part of the process, right? So that doesn't mean, though, that your email isn't worth zero. I mean, you need to shift from measuring direct revenue to measuring pipeline contribution. And you do that by assigning a weighted value to non-venue actions. So an easy math to do this is if you know that one out of 10 people who attend your webinars eventually sign a contract of, let's say, a $1000, then your webinar registration isn't free. It's worth $1000 to your pipeline. So you must report that number to your leadership. If you just look at the final click, look, you know, at the marketing influence beverage. Like, for example, it's that CEO that read your email 3 months before signing that deal, if he read it, then yes, your email gets that credit too. So in B to B, basically your goal isn't just to sell. It's just to accelerate that deal through the pipeline, and it can assign metrics to that. That will help you along the way too. All right, so now that we have established the financial destination, we need to look at the vehicle that gets us there. And the business impact. Think of it as the result that we just went through. And the engagement metrics are like the cause, right? You can't get a high conversion rate or high lifetime value, unless your subscribers are actively interacting with your content. So let's have a look at those metrics. That will help us tell us if your audience is actually listening. All right, so before we talk about clicks, we need to talk about open rates, right? For decades, this has been our sort of North Star, but today is effectively broken. And the big reason behind that is that Apple Mail privacy product, male privacy protection, or MPP. And similar image proxies that exist out here. So whenever you send an email for those that don't know, whenever you send an email to someone that has Apple email address, uh, at [iCloud.com](http://iCloud.com) or has even like a Gmail address configured in their Apple device. Apple will tell its proxy service to download all of the images for you. And that will include the tracking pixel. So, you know, and that happens even before they use a picks up their phone to have a look. So, This data to your ESP or your email service provided your platform that you use, right? It will tell you that that is a real human. It looks like a human that opened it. But in reality, that isn't the case. That isn't a subscribe. Someone hasn't seen it. So the results will be, your open rates will get inflated, often about 30 to 50%. So that basically means you can't just trust blindly that raw number, right? The good old tact of just sense those that open recently, like trying to get them to purchase something because they're showing that interest. Well, that can now potentially harm you. That's because you're likely sending to people that are not interested, because they're matched by Apple and it's a privacy proxy. So moving forward, treat opens as a sort of directional train, not a hard fact. Okay? That's why the next set of metrics that I'm going to show here are so vital. All right, so let's start by cleaning up the confusion between click through rate and click to open rate. CTR or click through rate? This is a more high-level view. It takes clicks, divided by deliver emails, and according to some benchmarks, the global average sits about 2.3%. Now, CTOR is sort of a content auditor. It takes the clicks divided by the opens, and it tells you of the people that saw the design. How many clicked on something? Well, the average of this is around 6%, healthy programs should aim for 10 to 15. Okay. And there's also be rate or through all time. This tracks how long the email was open to be read. Limits has this definition of read as of anything that was open for more than 8 seconds to be read. Um, and the only way, this is amazing because it's the only way to know if your cop is actually being consumed by people, not just the lady or skin. If you see high opens, but low well time, mostly below 2 seconds, then your subject line worked, but your content is failing to deliver. Um, and that is a signal. Maybe you have to shorten your copy or even improve your design hierarchy altogether. And finally, for the engagement section, we must look at the unsubscribing. Many markers they usually panic when they exceed these numbers grow up. But I want to invite you to ship that mindset a bit. I mean, the unsubscribers are sort of a good goodbye. right? It's the user telling you, like, hey, this isn't for me anymore. And just leaving your lips, volunteer, right? They help me clean the list for you. And we suggest keeping this metric, uh, very low, either below one or two. I usually recommend Amy for it under 0.5 or anything lower than that. And if you see a spike, don't ignore that, even though that we know that that Google is doing, um, they have a recent update for their uh, managed subscription, that leverages uh, the list of subscribe header. And a lot of folks are have been reporting spikes because of this. Uh, you still have to have a closer look because that could be a clear signal of the list of team. Maybe you're emailing too often people are trying to unsubscribe. So if you set or maybe you're sending some content that doesn't match that that expectancy that they had when they signed up for. So all of that to say, just ensure that you make your unsubscribe links easy to find. If a frustrated user can't find the exit door, they will create one by hitting the spam button. And you don't want that. Right? For centers that have the list of subscribe that I've recommended. Gmail will naturally nudge you. see here in the the screenshot. Gmail nudges their users to do the unsubscribed value than report spent. And that's a good thing, right? Because, I mean, at the end of the day, the lesson here is, I know a non-subscribe hurts your ego, but a spam complaint, that will hurt your deliverability. So always choose the unsubscribed path. All right, so we talked about how to measure value. We talked about how to measure engagement, but none of that matters if your email never beaches the inbox. So now we're gonna peel back the technical layer and understand a little bit of the mobility. And the difference between just sending the message and then and between actually arriving on the inbox. All right, so we need to do that by breaking down the 3 distinct metrics that define your access to the subscriber. The 1st one is bound straight. This measures the percentage of email that were rejected by the receiving service. And this data comes directly from your platform from your ESP. You need to keep this under 2%. Anything above that, that is a clear signal that your list is not great. It has poor data. Maybe your collection process is not doing great or If you if you get list from 3rd party for some reason, maybe Dallas isn't great. So having, if you see a high number there, that's a, that's a bread flag, okay? The 2nd one here is delivery rate. This is pretty much the opposite of the the boundary because this measures the percentage of emails accepted by the service. Bounce is being rejected. This is accepted. But again, this state is also available by you are speaking, and the format is just your sent emails minus the bounces. Okay? And one thing that that is key here that we need to remember, that deliver or deliverability that you also that you often see in your platform. That only means that the server that received the message said, okay, I got it. It never tells you if your user saw that message of the inbox. Right? And to get that, that brings us to the 3rd metric here. And it's the most critical one, which is the inbox basement. This measure how many emails actually landed the inbox versus being sent to the spam folder. And there's a big distinction here. I mean, your ESP can't provide this data because they lose visibility once the email leaves their service. You often need a 3rd party tool, like, like our own litmus or efforts to help you measure this. Or even our certification, because we also get direct data from some mailbox providers from that product as well. Without any of that, honestly, you were just blind to whatever, uh, weather in the inbox or the junk folder. You're not going to be able to get that date, unfortunately. And your reputation is basically built on trust and there are 3 ways to break it, basically. 1st with is the spam complaint, right? We talked about that a bit, right? People marking in span. So when a user activity clicks on that spam button, that data is often sent back to you, the sender, but within your email sending platform via something called Feedback Loop. Not all mailbox providers have feedback poop. Gmail doesn't have one. For example, but Yahoo, Microsoft, and some other bigger ones, they do have. So they send that data back. And ideally, they want you to do something with it, not just get the data. They want you to monitor and remove those that are complaining from your list. But also monitor the rate, right? Memorize this number, 0.1. And when I say [0.one](http://0.one) is the user complaint rate. So that means that if you exceed more than one complaint for a 1000 emails that landed in the inbox, Your reputation can take a hit. And if you hit 0.3, I mean, 3 out of a 1000 emails. Google and Yahoo will likely start sending your messages to this band folder directly. So pay close attention to this metric. It's it's very important. And you can get this metric from Google at Google Postmaster Tours, okay? The 2nd one here would be Spentraps. These are decoy email addresses that look real. look like real people's addresses, but they don't actually belong to real humans. So if you're sending to spend trap addresses, it's kind of like you're stepping on a trip wire, right? Because in some ways, it tells the the companies that the handle these fan traps, that you're either buying this or feigning to clean your old data. Um, and in order to understand where, if you're hitting spam traps, you will need a 3rd party tool that has access to that. Okay? And finally, the Simon Killer here, which is specific to Outlook and Hotmail, which is S-R-D, or send a reputation data. So for those that don't know, Microsoft goes down the route of not just waiting for complaints to come in, they actively pull their users and ask them, hey, from this that you received on your inbox, did you do you want it? Do you think this junk? If the user says, no, I don't want it. I think it's John. Uh, Even if they don't click, this is spam, your reputation will take a hit, right? Because in their interpretations that if there's a lot of people saying, hey, this is likely expand, and I don't want it in my inbox. They will take that into consideration. This data, unfortunately, is not widely available. It's exclusive to our validity center certification data. But, you know, talk to us if you want to know them a little bit more about it. All right, so like I said, you can't fix what you can't see and right now your platform, your ESP is completely blind to most of the numbers that I talked about. And these are numbers that will determine your fate. Google and Microsoft, they are constantly creating, if you don't know where to find that report card, then you were just guessing. Like I said before, Google postmatch the tools, that is the place to go for. For getting data directly from Google. You should be using the compliance status page on their, on their V2, uh, postmaster tools to get the, the information if you're passing their 8 critical checks. If you see any needs work status in there, that's a big red flag and you got to work on that immediately if you want to get to the inbox. You know, so they launched a version 2 of Google Postmaster Tools. And that means that they're going to officially retire the old domain and IP reputation grass from version one. So all of that high medium and low chart that you have right now, that'll be gone soon. So your new North Star will be the compliance status and the spam rate. Um, and if you go to Google Postmaster Tools and go to Spam, uh, use a reported spam rate, you see a big graph which has shown the previous line. this one here. So you see that grass that will be, you know, it's very detailed and it shows the threshold lines over there and you have to watch that like a hawk. Remember, stay below [0.one](http://0.one)%. If you hit 0.3, Google, send you a message to the spam, uh, it's fair like to spend, to send more messages that you're sending to them, to the spam folder. So, again, this, combined with the status, the complaint status, that, with the needs working, that is your new report. Okay? Next one where you can get more visibility to uh, mailbox provided data would be Microsoft SNDS. It works kind of like the same way, but it gives you more of a traffic light signal for your IP. So this is specifically for those that have dedicated IP. If you're on a shared IP, this is not gonna work. And remember, the, for Microsoft, the complaint rate rounds up. So if you see 0.2%, then you were in trouble. 7 0.1. And finally, we also have sender score. This is our tool. I mean, since Google, uh, doesn't have a, will not have in the future, uh, their reputation valuation. You can use center sports, kids knew that grading. So you get over there 0 to 100 sort of credit score. And I did, you want to aim to something above 80 because that's when we see healthy, sending habits happening. So, that great update the above, that's where you got to aim for. All right, now that we have defined every layer of that pyramid that I showed in the beginning, it's time to put them to work. So I added this section here, well, to teach you how to be a sort of email detective and, you know, try to look for common symptoms, like, The open range, port conversion, and we'll use some of the metrics that we saw here today to help you pinpoint what is happening. Alright. Like, for example, let's say you have the mystery of why am I open rates low? Most marketers will immediately blame the subject line. But you have to be smarter than that. I mean, 1st you have to look at your inbox placement rate. If Everest, for example, if you're using Everest to measure that, if Everest is telling you that a specific mailbox provider is showing uh, uh, inbox placement rate that is below 80%, I mean, rewriting the subject like won't help. I mean, your deliverability is having a problem. You were landing this manfolder. But so you got to deal with that specific. You gotta do things to get you out of this handfolder. But let's say your inbox placement is high, 90% or above, but your opens are still low. Then like they have a creative problem. I mean, your subject lines isn't resonating. Um, What else next? Oh, yeah. The CTR. If people open, but they are not clicking with the CTR under 10%, then like they have a content mismatch or subject mind made a promise that your email body didn't keep. So work on that too. On the flip side, if you have high clicks, but 0 perversion, then stop tweaking the email, the email worked perfectly. The problem is likely with your manly page. Maybe the form is too long or the page is loading too slowly. Got to go down that path. And finally, to see high bounces or block listing, That is like that data hygiene fader. So don't, for that one, just know riding your way out, like doing a different subject line, a different copy. You need to stop sending, clean your list, remove span traps. You know, fix the root cause before you send any new message. That is the only way. So, I know. A lot of stuff, but how do you keep track of all of that? Like how do you turn the lights on? Well, 1st we have Lema's email, analytics, that solves engagement blind spot, problem, instead of relying on the broken open rate that I talked about before. Litnus will show you the beefing. Will tell you if your subscribers are glancing, that means that you looked at the emails for less than 2 seconds. We're actually reading that they read for along with the exact. It will help you measure true attention, even after with MPP and all of that, because we focus on the other ones too. Second, we will, I mean with this tool, we have solved the deliverability mystery as well. We have a spam testing tool that allows you to run the skin before you launch. We'll send you, we send your email to VOC addresses at Gmail at Outlook at Yahoo and and all of the corporate filters as well as well. And that will tell you, um, if if it will land on the inbox or like the expand of the spam folder. So you do all of that before you send and schedule your campaign. And finally, you can protect your conversions. If you worked hard to get those clicks. So don't lose it because, I mean, your, you know, you don't want your message to be broken because something's missing over there. So test your message across 100 plus devices instantly. So that way with this platform, um, you get the data that will give you that information that delivered actually means delivered perfect. Okay? All right, so to wrap up, here's our checklist for your meeting tomorrow when you get to your job. It's like, okay, I saw this amazing webinar. lets talk about it. So first, shift the conversation with your leadership. Stop reporting opens, start reporting conversions and lifetime values and things that are valuable to the business, right? Second, update your engagement definition. You can use ReVay, click to open rates, all of that, you know, to see the truth behind the pixel. And finally, secure a foundation. I mean, check inbox basement, monitor Google Postmaster Tools, daily, weekly, if you must. If you're not looking at these numbers, then you're flying blind. Okay? So we, I know we have covered a lot here today, and we'll be sending this this entire deck as a PDF reference guide for you to keep. And I really appreciate you spending your time here with us. I know that we have few minutes left, must spend, send this back to Jess, see if there's anything else that we can talk about. Test. Ooh, that was a lot rough, but ton of great information. I hope everyone's feeling good about setting some good benchmarks for 2026 and making their bosses happy, as you said. That's what we're all about. Um, so if anyone's looking for any more tips on how to make the most use of your marketing data, check out these free resources. Again, this will be coming to us via email for the next few days. Um, and now let's get into some questions. The chat has been going wild. So thank you all for being so engaged. I saw that. Yeah, I love seeing everyone help each other out in there. Um, so if you the, the recurring ones that I saw, um, we can get started, but let's see. We had a couple people asking about spam rate. What do we do if we see this Bam rate hit .one%? Does this wear off over time? That's a good question. I mean, with family, I mean, let me go back to that graph because I think it, But Google is the one that we usually talk about spam rates being being a little bit high. Go back, here it is. So this graph here shows Google's spam rate. We can see that red line there. And the yellow eyes. So the red line there, that is the 0.3 and the yellow line 0.1. So if you see anything above the yellow line, that is a warning. Like, hey, something is happening on my side that is getting people annoyed. But if you see some spikes like the ones that we're seeing over there, that is a red flag. Ideally, what I usually recommend is one pinpoint, whatever was sent on those days that you see the spikes, need to know what was sent exactly. Because from that, not only you know the content, but you also know the audience, depending on the audience that you are sending that content to, maybe it doesn't resonate. Maybe you sent it then the day before, so it's too much, usually or are those? It's related to expectancy. They're not expecting or it doesn't match what they were expecting or to frequent and content not valuable. So try to pinpoint the days in what was sent to try to cover these things that I mentioned, to see, they, they do match. Awesome. Thank you for that. Does that answer? That could go on. No, it was a very thorough answer. Thank you. Um, and a few questions about click to open rate. People asking if it is now unreliable due to MPP. Well, Let's put it this way. Like I said, with MPP, you would likely see the inflated opens with at [iCloud.com](http://iCloud.com) addresses, right? So for those, it's kind of hard to pinpoint which ones are the real humans, which ones are not. But for the other ones, You can count for those. I mean, we Google when someone opens, That will track the open with Gmail. Um, So you can you can isolate that across the providers that don't use any sort of proxy opens and give that, you know, a general idea. I know it's not going to be the true picture. Not everyone is doing the opens, but at the very least, it gives you a sense of how their content is resonating with people. If they're opening and you know that, hey, this is, there's no MPP here. Then you should be able to do the calculation on top of the ones that are not part of it. And at the very least, that's that's a thermometer on itself. So, yeah. those more directional metrics. How do we combat privacy scanner unsubscribe clicks? Oh, that is a good question. Um, Yeah, there's, I know like freezer wind litmus, right? We test the links within the emails. Um, In a way, we would click on every, visit every link within the email, but there's a way for us to inform within the HCML, like, hey, don't follow this link. Unfortunately, that there isn't one specific adopted parameter or attribute that you can add to links that would inform the mailbox providers like, hey, don't follow this. Um, So, yeah, we can't. We truly can't. But the good news is that most platforms they would not let the unsubscribe go through automatically. They're able to understand like, hey, this is coming from unlikely auto open or thoughts click type of situation and try to prevent that. So if you don't, if you want to know more, I would recommend talking to your ESP and ask them about how they manage these things. But yeah, that can be a problem. It doesn't happen very often, but that can be a problem for some, especially for in a B to B space. Awesome. Great advice. We'll do one more because we're unfortunately out of time. Um, but someone wanted to know, when you say spending enough to grow, can you clarify exactly what that code or should look like? Is it investing in headcount for lifecycle or is it purchasing lists? Oh. I mean, Purchasing list is not a good idea in general because, I mean, if you're, depending, you, you're going to be dependent on whoever is at point of those email addresses to do the correct thing and validate those email addresses, right? So, If you're spending that way, yes, that is one way to grow. But you also need to calculate your growth rate based off of that. Like I said, unsubscribes is one way, but if you clean your list automatically, like we always recommend, like clean your list by removing those that are not engaging. Consider those as part of your list growth calculation, as if you were if they were unsubscribed. And do that per source. So that way, you know, like if we're growing less by acquiring from this source, What is the churn? What is the growth rate that, you know, accounting for the new ones? plus the ones that we're leaving, or even plus the ones that we're, we're removing intentionally because of lack of engagement. You need to consider those and do that per source. And to that point, I mean, for spending on that source, X amount of dollars and that is growing X or bringing Y of revenue. And the other one, which is more organic, which tends to be more, more successful, and that one you have the source labeling and you know how much your list is growing and you have these measurements, that will give you that information. That's what I said, 3 to one. I mean, if you've not seen that ratio, for whatever source that is, something is wrong. Awesome. We have a few people in the chat saying how tough it is in the B to B space. We totally hear you guys. So it will do a separate webinar for these folks someday. Um, but that is unfortunately all the time that we have for today. So thank you all so much for joining us. Our last validity webinar of the year. I can't believe it. Um, but hopefully we'll get guys in the new year. So thanks to you and Rafael. Yes. Thanks, everyone. Thank you for listening.