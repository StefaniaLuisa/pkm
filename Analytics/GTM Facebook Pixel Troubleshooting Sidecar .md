
**Monday, July 7**

> [!INFO]
> <https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D>
>
> [Strategy team check-in and hands-on training for implementing Facebook Pixel tracking in Google Tag Manager](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=9.0)
>
> ## Key Takeaways
>
> - [Reviewed process for troubleshooting GTM conversion tracking discrepancies](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=415.0)
> - [Implemented Facebook Pixel and conversion tracking in GTM workspace for SBCI](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=979.0)
> - [Discussed best practices for time tracking and task management between team members](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=826.0)
>
> ### GTM Conversion Tracking Troubleshooting
>
> - [Start by testing conversion events and examining tags/triggers in GTM debugger](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=1020.0)
> - [Check client assumptions and compare data from multiple sources (e.g. Engaging Networks vs GTM)](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=436.0)
> - [Look for discrepancies in page views vs conversion events](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=1244.0)
> - [Consider factors like ad blockers (typically block 20-30% of traffic)](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=1206.0)
> - [Multiple issues may compound to cause tracking discrepancies](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=1286.0)
>
> ### Facebook Pixel Implementation in GTM
>
> - [Created new workspace "Meta Pixel" in SBCI GTM container](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=1822.0)
> - [Replaced old vanilla Facebook tag with built-in GTM template](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=2425.0)
> - [Created new conversion tag and trigger for successful donations](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=2760.0)
> - [Used data layer variables for dynamic values (donation amount, currency)](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=2700.0)
> - [Tested implementation, confirmed tags firing as expected](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=3413.0)
> - [Next step: Confirm tracking in Facebook account once access is granted](https://fathom.video/share/4o32ms3ob7P8UvMmtgqa-kpsAyTGxz2D?tab=summary&timestamp=3600.0)

**VIEW RECORDING - 70 mins (5 secs of highlights)**

[@0:09](https://fathom.video/calls/344863905?timestamp=9.3) - **Sydney Moyer (4Site Studios)**

Hey, Bryan. How are you?

[@0:12](https://fathom.video/calls/344863905?timestamp=12.98) - **Bryan Casler (he/him)**

Oh, man. Siri just triggered. Have you had that problem?

[@0:18](https://fathom.video/calls/344863905?timestamp=18.3) - **Sydney Moyer (4Site Studios)**

No. No!

[@0:21](https://fathom.video/calls/344863905?timestamp=21.84) - **Bryan Casler (he/him)**

I need to enunciate better.

[@0:26](https://fathom.video/calls/344863905?timestamp=26.42) - **Sydney Moyer (4Site Studios)**

Wow. I actually, I get, I get Cindy a lot, but I don't, I don't think Siri has ever mistaken me for her.

[@0:38](https://fathom.video/calls/344863905?timestamp=38.1) - **Bryan Casler (he/him)**

Yeah. My problem to deal with. I'm glad you're not struggling with that. I mean, I know, I don't personally know, but I've heard of people named that, and like, it's a problem.

It's a consistent problem now. Like, oh, that sucks. I don't, I literally don't know what you do about that other than like, I probably I'm part.

United to Yes, Get a strong nickname to have everybody call you by.

[@1:03](https://fathom.video/calls/344863905?timestamp=63.32) - **Sydney Moyer (4Site Studios)**

Right. Or like, what if your name is Alexa? There goes that.

[@1:12](https://fathom.video/calls/344863905?timestamp=72.94) - **Bryan Casler (he/him)**

Yeah, one day we'll probably be able to name our AI's whatever we want.

[@1:18](https://fathom.video/calls/344863905?timestamp=78.16) - **Sydney Moyer (4Site Studios)**

Yeah. Not today. Dangerous.

[@1:22](https://fathom.video/calls/344863905?timestamp=82.3) - **Bryan Casler (he/him)**

Yeah, I know. I'm trying not to think too much about AI, but also think about it at the same time, I'm trying to compartmentalize it.

[@1:32](https://fathom.video/calls/344863905?timestamp=92.36) - **Sydney Moyer (4Site Studios)**

Are you in New York right now?

[@1:34](https://fathom.video/calls/344863905?timestamp=94.66) - **Bryan Casler (he/him)**

you dog-sitting? Yeah, yeah, my sister. So I came up for July 3rd, which is like the big day at a family cottage on Lake Canisius, kind of among the Finger Lakes.

And it's like a family tradition, like all the friends and friends of family members get together. And it's nice, probably had about 40, 50 people there.

It's just like a time. paying attention. you. You know chill party kind of this year's theme was pizza so everybody brought a different pizza so we had all the best pizzas that the area has to offer and then my sister though has a family friend in North Carolina and wanted to go visit her but also has two very high needs dogs and so I offer as I've done in the past offered to just set dogs for them while they're gone and these ones might bark if they do I'll go on mute and I'll just I might have to get up to get them sometimes they they work each other up and there is no end like it can go on for several minutes but they're they're sweeties they're just triggered by everything it seems yep no I know the feeling my dog is a little bit of a scaredy dog herself and she will just I think now it's just habit that she will react sometimes to you know like if she gets surprised by someone she'll just bark like she doesn't even have time to compute whether or not she's actually a she'll just right

[@3:00](https://fathom.video/calls/344863905?timestamp=180.0) - **Sydney Moyer (4Site Studios)**

She's just like, oh my god, I gotta bark.

[@3:03](https://fathom.video/calls/344863905?timestamp=183.14) - **Bryan Casler (he/him)**

Yeah, with them, you know, it was, um, one of them got into a dogfight at a dog park years ago, like, not a bad one, but they're like, we can't go to the dog park anymore.

And I was just like, every time something would happen, I think, like, they, like, siloed them a little bit more, a little bit more, and now they're just indoor dogs that stay in, like, literally, they have a fenced-in backyard, I let them out, they want to come in immediately.

Like, it's just like, okay, like, you're just inside, and everything outside gives you anxiety.

[@3:33](https://fathom.video/calls/344863905?timestamp=213.08) - **Sydney Moyer (4Site Studios)**

And it's like, alright, I know, and they're sweeties, though.

[@3:38](https://fathom.video/calls/344863905?timestamp=218.08) - **Bryan Casler (he/him)**

They were, they used to be really good, really social, and then, that's fine, though. Um, but yeah, I'll be up here until Sunday.

My partner, Angela, is, um, with me working, uh, working, uh, flying out tomorrow. So we're just meeting up with a family friend tonight.

And then, uh, yeah, they get, they all I'll back Saturday, so I'll fly out Sunday.

[@4:03](https://fathom.video/calls/344863905?timestamp=243.04) - **Sydney Moyer (4Site Studios)**

Nice! That's great, I'm glad you could be there with them at least, and help entertain, keep them calm.

[@4:09](https://fathom.video/calls/344863905?timestamp=249.98) - **Bryan Casler (he/him)**

Yeah, yeah, I like them a lot. They've come down a little bit in their old age, which is really nice, because it used to be one of them, like, obsessively licked.

Like, and I think the second part I'm about to say is still true, but it was, like, exacerbated by it.

Which is, um, I think they have memory that resets about every two to five seconds. Like, it's just, that's it.

Like, they forgot anything they were doing previously, and, like, back into lick mode, jump mode, whatever. And just, like, for the life of them, they could not, they could not, um, yeah, learn better habits.

[@4:48](https://fathom.video/calls/344863905?timestamp=288.94) - **Sydney Moyer (4Site Studios)**

Yeah, my friend's dog is like that, and she always goes for the ear, and I'm like, get there.

[@4:53](https://fathom.video/calls/344863905?timestamp=293.8) - **Bryan Casler (he/him)**

Yeah, I tried, I tried walking them, uh, time I was here, and I may still do that. While I'm here but they're very they're very dog reactive so even a dog like two blocks away it's like all hell breaks loose and I'm I feel very grateful that I'm you know I'm like an able-bodied individual and I can control them but I'm like my sister can't like my nieces couldn't like they they literally cannot take them for a walk anymore because they if they freaked out they would I don't think they'd be able to hold the leash yeah yeah yeah they their labs they look pretty big yeah ones I mean they're both one's a lab uh hound mix um let's see I guess they just like the kids playroom aww one's a lab hound mix and the other one my sister got uh she was like oh we got a lab mix and then she sent a photo I like that's a pibble I mean you got a pibble you got a tiny pibble there's five percent lab in that dog they're like shepherd mix yes yes

[@6:00](https://fathom.video/calls/344863905?timestamp=360.0) - **Sydney Moyer (4Site Studios)**

Right?

[@6:01](https://fathom.video/calls/344863905?timestamp=361.14) - **Bryan Casler (he/him)**

You get it. I was like, okay. All right.

[@6:05](https://fathom.video/calls/344863905?timestamp=365.18) - **Sydney Moyer (4Site Studios)**

They own their home, though, so they don't need to worry about, you know, renting or anything.

[@6:10](https://fathom.video/calls/344863905?timestamp=370.56) - **Bryan Casler (he/him)**

Oddly, it was not the pit bull that got into the fight, though. It was the other one. Just starting at the dog park.

[@6:18](https://fathom.video/calls/344863905?timestamp=378.76) - **Sydney Moyer (4Site Studios)**

You never know. You never know who the culprit's gonna be.

[@6:21](https://fathom.video/calls/344863905?timestamp=381.38) - **Bryan Casler (he/him)**

Okay. Let's see here. We got a bunch of fun things to talk about. We're gonna record some pixel work around GTM.

Let's save that for the end, just because that way I can have my—I know we're already recording, but I can have—let's see here.

We can have my notetaker join, and then I'll just have a clean recording to share with Steph.

[@6:50](https://fathom.video/calls/344863905?timestamp=410.12) - **Sydney Moyer (4Site Studios)**

Perfect.

[@6:54](https://fathom.video/calls/344863905?timestamp=414.1) - **Bryan Casler (he/him)**

What are these other ones here? So I was looking over your response. will now. I will read I To David, let me pull it up, I really liked it, because I also agree with it, but I really liked it, because there are a lot of vanity metrics out there, and I think you kind of struck the right tone for coming at that.

Do you have a sense, like, is this something they're already showing clients, or they want to show the client?

Like, what was that screenshot they provided?

[@7:24](https://fathom.video/calls/344863905?timestamp=444.66) - **Sydney Moyer (4Site Studios)**

I think it's, I don't know how involved David is in the creation of it, but it's just something that they want to show to their board.

Um, so I assume it's for, like, some sort of annual meeting, or, you know, packet that they'll be receiving materials, something like that.

[@7:45](https://fathom.video/calls/344863905?timestamp=465.58) - **Bryan Casler (he/him)**

Um, the only thing to possibly flag, uh, is just when we start to talk about year-over-year, I think is GA4's retention in 15 months?

I'm to remember.

[@8:00](https://fathom.video/calls/344863905?timestamp=480.0) - **Sydney Moyer (4Site Studios)**

Right.

[@8:01](https://fathom.video/calls/344863905?timestamp=481.36) - **Bryan Casler (he/him)**

More data retention. Oh, no. It's more now. Let's see here. Oh, no, it is. It's 14 months with GA4-360, a period that can be 26, 38, or 50 months.

What is GA4-360? I'm sure it's some enterprise something or other.

[@8:29](https://fathom.video/calls/344863905?timestamp=509.2) - **Sydney Moyer (4Site Studios)**

Yeah.

[@8:30](https://fathom.video/calls/344863905?timestamp=510.18) - **Bryan Casler (he/him)**

I've heard of that. Let's see here. Higher data limits, unsampled reporting, and advanced features. Yeah. starts at $150,000 a year.

Amazing. All right. Cheap. That's what we don't know about it. All right. Cool. It just sounds like they're basically doing the job for you that folks do with BigQuery.

You're just like, okay, we'll just put it all in there. Must be nice. Dave. So the only thing to flag is just that, that if they're going to do year over year, they can do one year, but if they're going to try to do multi-year, they need to set that data aside somewhere to be able to include in the future reports.

[@9:17](https://fathom.video/calls/344863905?timestamp=557.54) - **Sydney Moyer (4Site Studios)**

Yeah, that's a good thing to flag. I'm just going write that in my notes here really quick. Okay, cool.

[@9:51](https://fathom.video/calls/344863905?timestamp=591.72) - **Bryan Casler (he/him)**

Great. But yeah, feel free to send it. Um, just to repeat what I wrote in text, which is, uh, um...

You don't need to funnel anything through me unless it's something that we've talked about before, and usually there's like a good reason for it.

Or if you want a second set of eyes on, always happy. In this instance, I was just, I was really curious.

I was like, cool, like this is kind of unique. You know, there's some overlap with work we've done, but like the ask to like reflect on something they're already doing hasn't really come up before.

So I was just curious what you had put together.

[@10:27](https://fathom.video/calls/344863905?timestamp=627.1) - **Sydney Moyer (4Site Studios)**

Yeah, cool. Okay. All right. That's helpful for me to parse for as things come up.

[@10:33](https://fathom.video/calls/344863905?timestamp=633.42) - **Bryan Casler (he/him)**

Yeah. Um, and stuff like this is really easy. Like I, I, typically I don't need to task. Like if it's sub five minutes to just peek at it, um, unless I'm doing a million things or the client, uh, deserves to be billed for every second we spend on them.

Um, just a quick peek at something like this is totally fine. And especially during the ramp period, um, feel free to be over, for, uh, to, to, like,

And that needle, if you want me to look at stuff, just because I also have additional time set aside to support you, so I'll draw from that.

[@11:07](https://fathom.video/calls/344863905?timestamp=667.32) - **Sydney Moyer (4Site Studios)**

Okay, okay, cool. That makes sense. And if I were, let's say you would have spent maybe 30 minutes on that review, would I have just sent you that task that was assigned to me, or, and then you put some time to that?

[@11:21](https://fathom.video/calls/344863905?timestamp=681.72) - **Bryan Casler (he/him)**

Typically, if it ends up just being, like, ad hoc or asynchronous, I'll just log time to your task. If it's something I need to schedule for myself, or, like, I kind of want to, like, break it out for other reasons, I might just literally create a subtask or a duplicate task and then log my time there.

[@11:40](https://fathom.video/calls/344863905?timestamp=700.48) - **Sydney Moyer (4Site Studios)**

Okay. All right. So if something's maybe going to take a little bit longer, I should be doing that proactively.

[@11:45](https://fathom.video/calls/344863905?timestamp=705.02) - **Bryan Casler (he/him)**

Yeah. And for example, Fernando and I do that, we interact a lot with each other, where I'll be like, I need you, like, I need you to look at this.

And I know it's going to be 15 to 45 minutes. So like, I'll create him a task. And, you know, I say, hey.

Like, you know, either when you have time, like, I need this today, so like, you when you have time, long time there, or, you know, I'll, I'll look at the capacity report and just pick out like, oh, look, he's got time this week, or he's packed this week, next week.

Hey, hey, where are you going? Come here. Come here. Thank you. I know. It's like, trying to go under this desk, there, there's nowhere for them to fit.

Okay.

[@12:40](https://fathom.video/calls/344863905?timestamp=760.16) - **Sydney Moyer (4Site Studios)**

Hey, hey.

[@12:41](https://fathom.video/calls/344863905?timestamp=761.14) - **Bryan Casler (he/him)**

I know. I know. It's tough. Okay. Yeah. Nope. Okay. Okay. Okay. Okay. Okay. Once you're see. Okay, you want to light out?

You too, why are you both barking? Come here. Come here. Sure. Hey. Oh, no. No. You don't even know what you're barking at.

Yeah. can't even put him in the other room because my partner's on a call in there too. It's a scary world out there.

Yeah. And I'm like, they're not my dogs to correct either. So I'm just like, oh, it going be okay?

[@13:44](https://fathom.video/calls/344863905?timestamp=824.26) - **Sydney Moyer (4Site Studios)**

Really?

[@13:44](https://fathom.video/calls/344863905?timestamp=824.84) - **Bryan Casler (he/him)**

Thank you. Thank you. Okay. So, um, Fernando and I have to pass stuff back and forth to each other a lot.

So we'll, we'll create tasks. Um, it can also be informative to the PM. So if it's like unexpected support.

like, what? we're for a Okay. I'm like, I kind of want to make it more official rather than, you know, it's not like intentionally hidden, but sometimes when you log time on a task, like it's not obvious, you know, just looking at that task, why maybe a task went over on time or something.

So, you know, use your discretion there. But yeah, in your instance, I also have time set aside. Really, the judgment call for me is am I logging it as billable client time or am I chalking it up as internal onboarding time?

[@14:29](https://fathom.video/calls/344863905?timestamp=869.16) - **Sydney Moyer (4Site Studios)**

Gotcha. Okay.

[@14:30](https://fathom.video/calls/344863905?timestamp=870.96) - **Bryan Casler (he/him)**

All right. That's super helpful.

[@14:32](https://fathom.video/calls/344863905?timestamp=872.52) - **Sydney Moyer (4Site Studios)**

Nope.

[@14:34](https://fathom.video/calls/344863905?timestamp=874.32) - **Bryan Casler (he/him)**

Oceana Countries Accounts. Oceana has other Oceanas. So you think of Oceana, it's Oceana US, Oceana Canada, and I forget where the other ones are.

But in Engaging Networks, they have the ability to basically have multiple country offices, like different accounts. And so the country account is a separate Engaging Networks account.

much. much. let's bring down. then That is connected, though, and share some of the work we do for Oceana US so that there are other other national offices can use it.

The don't ask me what the relationship is, because it's it's it's murky like in some of those offices, the Oceana US does a lot to help and others that are more autonomous.

They're they're kind of proclivities and expertise and capabilities are all over the place. But Oceana Canada is the the one that comes up the most.

But even at the point where other agencies like work on our page templates that have been copied from Oceana US to Oceana Canada, for example.

So it's just it's a little it's a little murky, but we just support them whenever the request comes in of, hey, we want to do this, that or the other thing.

And usually what it means is something the US office has or offers they want. support for So And or updated to have in the other account.

[@16:04](https://fathom.video/calls/344863905?timestamp=964.78) - **Sydney Moyer (4Site Studios)**

That makes sense. Okay. I figured it was some sort of international-type branch of Oceania, but I wasn't sure it makes sense that it's actually...

[@16:13](https://fathom.video/calls/344863905?timestamp=973.74) - **Bryan Casler (he/him)**

Primarily Canada.

[@16:15](https://fathom.video/calls/344863905?timestamp=975.14) - **Sydney Moyer (4Site Studios)**

Okay, cool.

[@16:19](https://fathom.video/calls/344863905?timestamp=979.04) - **Bryan Casler (he/him)**

So troubleshooting this SBCI GTM test. Great question. So, there's a couple ways I would do this. The first is...

Oh, let's see here. Okay. So... There's a few things, which is just to... you. You One, be able to test and see conversions happening.

So usually when something like this, if I can run a test without having to make a real GIF, I'm like, okay, I'm going to go to this website, I'm going to run a test, I'm going to see the GIF, boom, done.

So it's like, Lightbox with a donation form, I run, I take that URL, I run it through the GTM debugger, so now it opens up, GTM debugger shows me everything that's happening, make a donation, and then I look for the event that's recording a transaction.

Once I do that, I make note of all the tags and triggers in play. So like, what is reporting a conversion?

And then I look at the logic that's used. I see some mention here seven days ago about they changed the logic about what does or doesn't show, switching the trigger to an element visibility when the lightbox shows the thank you page.

So like, I don't know, those are all bad ways to do that. Engaging Networks like in the markup tells you when it's a donation has been successfully made.

Like that's what you probably should be triggering on. Um, if this is not a donation, there's another way to do it, which is to, um, in a page series.

So when you have like two pages, let's say the first one you fill out your email, the last one is the thank you page.

Um, you can also in the markup, see that you're on page two of two, which now, you know, is the last page.

And you could say a conversion event has happened. So there's a bunch of different ways you can do that aren't, um, that aren't fragile.

Um, and fragile is not like a, a technical term, but really what it means is like things don't, things that might change in the page aren't gonna break other things.

So a way that you can make a fragile conversion event would be. We look for an H2 tag with the word thank you on the Engaging Networks domain.

So now it's like, hey, is that triggering on donation pages and advocacy pages? What if that gets changed to an H3?

What if this is in Spanish and it doesn't say thank you anymore? And it's like, that's fragile. So it's like it's not robust to changes that could happen without someone having knowledge that something else is dependent upon it.

So I would start by just seeing if you can make a conversion event happen and then interrogating what, oh, this looks like it's for me.

So I'm going to start by making, see if I could have a conversion event happen and interrogating what's going on there.

The second part is to check the client assumptions. So they said, you know, we actually expect there are between 16 and 23 a day.

It's like, okay, where is that coming from? Is that is that a report? I'm start by. Yeah. by. Thank

The engaging networks. Could there be something else going on there? Ad blockers will block about 20, typically about 20 to 30%.

So that doesn't explain this because it's, you know, a half to a third. So that's way, way too many.

So what else is going on there? There's other things that are much easier, which is actually to just look for page views on slash page two.

So how many of those are reported? So they say, let's say they say, Hey, we have 20 conversions according to, um, uh, engaging networks.

The conversion event says we have four conversions. And then I'm going to go, well, you have page views running on every page.

Let me run it for that URL. Oh, you have 10. Okay. Why? How could you have 10 page views, but only four conversions?

Now I found a discrepancy and I can just start to interrogate. We're like, okay, we should at least have 10.

That doesn't explain why it's not 20, but it should be in parity with this other number. And then at least you can say, like, relatively, like, hey, like, there might be something else here that unrelated to this environment specifically could be related to the way your analytics were implemented that we need to investigate kind of more broadly now.

But like finding those discrepancies and then like picking them apart. We have found in the past that it can be several things compounding.

So it may not be a single, you know, smoking gun. may not be a single thing causing the drop.

It could be a combination of, oh, you're a privacy organization and you actually 40 to 50% of your visitors run ad blockers and this has been misconfigured.

And this other thing is misconfigured and it's double reporting. And we have to solve for all three of those things to get you into something reliable.

[@21:58](https://fathom.video/calls/344863905?timestamp=1318.32) - **Sydney Moyer (4Site Studios)**

Cool. Okay. Yeah. That's really. Well, I was, I, um, just saw it come up in the production meeting earlier today, and I was like, I'm just, I'm curious about how you can go about investigating.

**ACTION ITEM: Add SBCI GTM troubleshooting to next week's agenda for Bryan's report - [WATCH](https://fathom.video/calls/344863905?timestamp=1328.9999)**

[@22:10](https://fathom.video/calls/344863905?timestamp=1330.76) - **Bryan Casler (he/him)**

Yeah. Well, if you want to add it to the agenda for next week, I can report back. Let's see here.

[@22:19](https://fathom.video/calls/344863905?timestamp=1339.72) - **Sydney Moyer (4Site Studios)**

Yeah, that would be great.

[@22:21](https://fathom.video/calls/344863905?timestamp=1341.12) - **Bryan Casler (he/him)**

Report back to Disney. All right. It's in there.

[@22:37](https://fathom.video/calls/344863905?timestamp=1357.26) - **Sydney Moyer (4Site Studios)**

Awesome.

[@22:39](https://fathom.video/calls/344863905?timestamp=1359.18) - **Bryan Casler (he/him)**

Then we're going to sidecar. So, um, as mentioned on our production call, Steph is out today, but, um, I imagine she's going to be pretty busy coming back tomorrow from a five-day weekend.

Um, though this week and next week, um, a big part of her to-do list is to start. Working on some transition plans for the retainers, really, we only need about a week, was my experience when I went on my three-week vacation.

So, yes, we're getting close to her being out, but it's not, it's not, we're not actually in a crunch period yet.

[@23:21](https://fathom.video/calls/344863905?timestamp=1401.12) - **Sydney Moyer (4Site Studios)**

Cool.

[@23:23](https://fathom.video/calls/344863905?timestamp=1403.04) - **Bryan Casler (he/him)**

All right, let me close out all the stuff I don't need. And then I'll get a, um, my Fathom going.

[@23:36](https://fathom.video/calls/344863905?timestamp=1416.62) - **Sydney Moyer (4Site Studios)**

Great. Wow, it just started pouring here, oh my god.

[@23:41](https://fathom.video/calls/344863905?timestamp=1421.74) - **Bryan Casler (he/him)**

Is it raining?

[@23:43](https://fathom.video/calls/344863905?timestamp=1423.02) - **Sydney Moyer (4Site Studios)**

Yeah, big time.

[@23:44](https://fathom.video/calls/344863905?timestamp=1424.94) - **Bryan Casler (he/him)**

Yeah, we have, uh, it's gonna be sporadic showers for the next week.

[@23:50](https://fathom.video/calls/344863905?timestamp=1430.3) - **Sydney Moyer (4Site Studios)**

Yeah. It looks like same here, I'm, I'm still on the Cape right now, and I- Oh yeah, I'm here.

The weather changes like every five minutes and, you know. You can't really, even if it says cloudy, like it was sunny all morning.

[@24:03](https://fathom.video/calls/344863905?timestamp=1443.5) - **Bryan Casler (he/him)**

Now it's boring. It's very confusing. You got sunburned? Was that the case? When you first went out there?

[@24:12](https://fathom.video/calls/344863905?timestamp=1452.46) - **Sydney Moyer (4Site Studios)**

Am I remembering correctly? Oh, I mean, I got sunburned over the weekend, that's for sure.

[@24:18](https://fathom.video/calls/344863905?timestamp=1458.22) - **Bryan Casler (he/him)**

Yes, yeah. I was thinking of you because I went grocery shopping yesterday and it was really nice out. No rush, right?

I'm just like here, dog sitting, and with my partner, and we like sat outside. They had like a hot bar, we got some food, and we just like chatted for like an hour and a half, and I got sunburn on my legs.

For reference, upstate New York has a concentration of skin cancer treatment centers due to the lack of natural sunlight.

[@24:49](https://fathom.video/calls/344863905?timestamp=1489.3) - **Sydney Moyer (4Site Studios)**

Oh man, that's tough. It's, I feel like I need like a base level burn that I, like, you know, but then we'll come tan.

And I haven't quite had that until this weekend because it's just been kind of cold and cloudy so far, but now all of a sudden it's become like hot and sunny and my skin's like, whoa, it's still winter.

[@25:14](https://fathom.video/calls/344863905?timestamp=1514.24) - **Bryan Casler (he/him)**

I just Googled it. Syracuse on average has an average per year has 56% of days where it's overcast.

[@25:24](https://fathom.video/calls/344863905?timestamp=1524.36) - **Sydney Moyer (4Site Studios)**

Wow.

[@25:25](https://fathom.video/calls/344863905?timestamp=1525.82) - **Bryan Casler (he/him)**

We crossed the 50% barrier.

[@25:27](https://fathom.video/calls/344863905?timestamp=1527.9) - **Sydney Moyer (4Site Studios)**

Oh, man, don't put that on brochures. I know.

**SCREEN SHARING: Bryan started screen sharing - [WATCH](https://fathom.video/calls/344863905?timestamp=1537.012969)**

[@25:33](https://fathom.video/calls/344863905?timestamp=1533.28) - **Bryan Casler (he/him)**

All right, so let's figure this out all in real time. And I'm going to get my Fathom to join.

All right. right. right. right.

[@27:14](https://fathom.video/calls/344863905?timestamp=1634.9) - **Sydney Moyer (4Site Studios)**

Oh, you're on mute.

[@27:17](https://fathom.video/calls/344863905?timestamp=1637.8) - **Bryan Casler (he/him)**

Let me get my bearings. All right, so Fathom is joined. We're going to look at this together, figure it out in real time.

**SCREEN SHARING: Bryan started screen sharing - [WATCH](https://fathom.video/calls/344863905?timestamp=1644.118652)**

I have too many windows open. I'm take care of that. Sydney, I'm going to collapse your window. So if you want to chat, totally fine.

But I can't see anything you're doing.

[@27:47](https://fathom.video/calls/344863905?timestamp=1667.86) - **Sydney Moyer (4Site Studios)**

Sounds good. I'll turn off my video for my fans.

[@27:55](https://fathom.video/calls/344863905?timestamp=1675.38) - **Bryan Casler (he/him)**

There we go. OK. it's Facebook Pixel, all right, let me remember what's going on here. Like the Facebook Pixel, I think this is the one where they wanted a conversion event.

mentioned the conversion API, which you had followed up with them on, and they didn't respond. So we're just going to implement this as is.

I mean, have they given, they haven't given anything else? What is it we got? I was hoping we'd have more from them.

Do you know if they've added us to Facebook?

[@28:46](https://fathom.video/calls/344863905?timestamp=1726.82) - **Sydney Moyer (4Site Studios)**

I haven't gotten a notification about it or an update from them. So'all, an you we've Google tinct.

[@28:58](https://fathom.video/calls/344863905?timestamp=1738.68) - **Bryan Casler (he/him)**

you're not going to use Google. I I I Yeah, I don't see it either. Well, it was maybe a non-starter.

We can do some prep work, though. Let me share my whole screen.

[@29:15](https://fathom.video/calls/344863905?timestamp=1755.8) - **Sydney Moyer (4Site Studios)**

Cool.

**SCREEN SHARING: Bryan started screen sharing - [WATCH](https://fathom.video/calls/344863905?timestamp=1757.568705)**

[@29:19](https://fathom.video/calls/344863905?timestamp=1759.76) - **Bryan Casler (he/him)**

Cool.

[@29:20](https://fathom.video/calls/344863905?timestamp=1760.44) - **Sydney Moyer (4Site Studios)**

Can you see my whole screen? Yep.

[@29:22](https://fathom.video/calls/344863905?timestamp=1762.78) - **Bryan Casler (he/him)**

All right. Let's go over. And access will be the thing that kills your momentum. So right now, have their account.

And we can look at their tags. We can look at their triggers. We can look at their version history.

But we want to make some changes. And we want to be able to test those changes. But also, there could be a chance where this could take a while.

Right? Like, for whatever reason. Back and forth, back and forth. It's a month from now. And somehow, in between now and then, while our changes are being worked on, they need to push a different update.

If we do the changes here, we're going to block their ability to push updates to the live environment. So instead, this is what Workspace is there for.

And so we can create a workspace. Let's call that meta. Meta. Grab that URL.

[@30:50](https://fathom.video/calls/344863905?timestamp=1850.72) - **Sydney Moyer (4Site Studios)**

Next.

[@30:51](https://fathom.video/calls/344863905?timestamp=1851.96) - **Bryan Casler (he/him)**

Now, we can do anything we want. It's not going to, one, impact their live environment. It's not going to, you

um block them from making updates and when it's ready we there's a whole merge process that they have to take in any updates they've made sense and the updates we have and then combine them together into building.

[@31:14](https://fathom.video/calls/344863905?timestamp=1874.44) - **Sydney Moyer (4Site Studios)**

Makes sense.

[@31:15](https://fathom.video/calls/344863905?timestamp=1875.46) - **Bryan Casler (he/him)**

This is wonderful. So first thing we want to do is just see do they have anything related to Meta or Facebook?

Yes, they do. All right so they have several tags here. Let's just look at how these come together. So these so you have the tag template which um basically certain services can create a template that lives in let's do this um lives in the GTM kind of environment so like all these services have a template that you can use click it you just put in a little bit of info and then it makes use of it you can also implement your own

So let's open up, uh, now let's open up all of these, oh, not going off the open, okay, alright, official, Google tag, alright.

So I'm not particularly familiar with this, I assume this just all came as is, so I'm kind of looking through what it does, okay, okay.

1 I'm gonna go over here, they have a Fundraise Up thing, we can ignore that, that'll just stop working as soon as they stop using Fundraise Up, could be helpful just to see kind of what they're doing here, may, right, there may be overlap between the same data points they want to pass in.

There's their Facebook Pixel ID. Just gonna go over here and link myself up Redcom. And it's back. So essentially making it a little easier.

Now we're here. Do those IDs match? Yep. So, I mean, to me... Yeah, this is strange. Why do they have a variable for the ID to use in QuariseUp and then have a tag, but not reference the variable?

The good news is it's the same variable, though, so that's wonderful. All right, and then now we're in conversion tracking.

Hmm. It's very strange. It's just like a hard-coded value. You would think that would be like a dynamic value.

[@34:36](https://fathom.video/calls/344863905?timestamp=2076.72) - **Sydney Moyer (4Site Studios)**

Right. That makes sense.

[@34:40](https://fathom.video/calls/344863905?timestamp=2080.26) - **Bryan Casler (he/him)**

We're using this off-site event. Okay. Yeah, so we got a whole bunch here. Okay. I'm just checking in, looks good, have this.

The one thing I keep looking at is like, where is it connected to their Facebook account? Right. Like, where is that unique ID, for example, being passed in?

So this is just the configuration, but then it just doesn't feel like it's used. Hmm. see we're, way through

All right, well, let's ignore that for a minute. Let's actually go in and see if there are... Let's click archive, yeah, so it's just custom, so it must be...

All I'm doing is trying to find out if there are, yeah, something I can leverage that's already in here.

[@36:37](https://fathom.video/calls/344863905?timestamp=2197.14) - **Sydney Moyer (4Site Studios)**

Yep.

[@36:38](https://fathom.video/calls/344863905?timestamp=2198.58) - **Bryan Casler (he/him)**

I mean, this seems pretty great. Like, I would think I want this. Is this the same thing? Facebook Archive?

[@36:46](https://fathom.video/calls/344863905?timestamp=2206.62) - **Sydney Moyer (4Site Studios)**

I think it is.

[@36:50](https://fathom.video/calls/344863905?timestamp=2210.96) - **Bryan Casler (he/him)**

Sure. All pages. We'll worry about that later. All right. All right. Facebook Archive. So it is the same. All right.

This is an unofficial search results. All right. So, it was probably updated five years ago, and it's called the Facebook Archive because it's probably the Metapixel now.

Let's see if it exists. Love Analytics Mania. They're awesome. They kind of put too much info in here. Uh, blah blah blah.

Pixel, I want to see what it looks like in GTM. Buy Facebook Archive. Okay, well that's great. They are using it.

All right. Wonderful. All right. So, let's go back. And don't know why they would have a custom pixel and also have that template set up.

So my oh, we're going to, we're going to do, we're do this. Let's clean this up now. Things. .

It's a little new. and we're gonna and we're don't need it. we have the variable, right?

[@38:59](https://fathom.video/calls/344863905?timestamp=2339.32) - **Sydney Moyer (4Site Studios)**

change it. you you you you

[@39:00](https://fathom.video/calls/344863905?timestamp=2340.0) - **Bryan Casler (he/him)**

Oh, yeah, sure. There we go. PageView, if you set consent and I need to false, that's all I'm fired, let's leave that as is, and I think that's good.

Alright, so now we're going to go back over here. We're going to pause this one.

[@39:27](https://fathom.video/calls/344863905?timestamp=2367.88) - **Sydney Moyer (4Site Studios)**

Okay.

[@39:35](https://fathom.video/calls/344863905?timestamp=2375.46) - **Bryan Casler (he/him)**

I don't know, it says... ... ... ... ... ... ... ... ... ... ... ... Back here, we disabled the old, we enabled the new, it's just going get marked with it.

All right, so now we've got a Facebook Pixel running on all the pages. using the template, and we're going to add another one, phase-bug-select-deviation-version.

I assume that's the one. here's where it's going to get complicated, though. How do we pass in the amount?

That would probably be here. Let's see here. So we have tag firing options once per event, once per page.

Really, you could only ever fire once per page.

[@41:36](https://fathom.video/calls/344863905?timestamp=2496.14) - **Sydney Moyer (4Site Studios)**

Gotcha.

[@41:50](https://fathom.video/calls/344863905?timestamp=2510.48) - **Bryan Casler (he/him)**

Oh, interesting. We can push in e-commerce. A bit of info into the data layer. All right, let's see what that might

It would look like. Nope. To get more options, I'm going check that. Interesting. I'm going back here. Yeah, this is not going to be.

Yeah, so this is just a standard event. Facebook, Excel, Donate, Event. That's Quit Looks like we probably want to purchase.

[@43:18](https://fathom.video/calls/344863905?timestamp=2598.14) - **Sydney Moyer (4Site Studios)**

Yeah.

[@43:19](https://fathom.video/calls/344863905?timestamp=2599.34) - **Bryan Casler (he/him)**

Not a donation. Let's go back. Purchase. Still don't see any addition. Let's see here. I made it a value and tag.

Must be when tag. Normally what we would want to see here is this little thing. So we could insert a dynamic.

dynamic. So right. Value. Let's just use this. We would want something like that. Let's name it enMovationAmount. Basically, we're inserting a variable that doesn't exist.

Don't even know if it's allowed or if we're doing this right, but let's save it. Oh, yeah. Must not contain references to variables.

[@44:32](https://fathom.video/calls/344863905?timestamp=2672.96) - **Sydney Moyer (4Site Studios)**

yeah. Okay.

[@44:34](https://fathom.video/calls/344863905?timestamp=2674.86) - **Bryan Casler (he/him)**

All right. All right. All right. you. don't Let's try that. Well, let's create one called Again, donation amount, it's going to be a data layer variable, so our EMGrid page template framework pushes a lot of values into the data layer, so we've got some examples in here.

This one, this is the name of it, so it's enpage.json. Page.json is the structured markup that Engaging Networks puts into the page, and then we just have underscore and the name of the value.

[@45:50](https://fathom.video/calls/344863905?timestamp=2750.16) - **Sydney Moyer (4Site Studios)**

Got it.

[@45:56](https://fathom.video/calls/344863905?timestamp=2756.98) - **Bryan Casler (he/him)**

Try that. See how that goes. I'll read it. Alright, we want to add a trigger and we need it to be on the Engaging Networks, being successful, still having it?

Yeah, I don't think so. We want it to fire on page view. When in donation amount. It's greater than zero.

So you don't have a donation amount unless you have donated. You can't donate zero dollars. exhaustion of little bit.

This I'm . And we're going to preview this. So the first thing we want to do is to see our new Facebook Pixel has fired.

We go in there. That's good news.

[@48:27](https://fathom.video/calls/344863905?timestamp=2907.46) - **Sydney Moyer (4Site Studios)**

Mhm.

[@48:29](https://fathom.video/calls/344863905?timestamp=2909.2) - **Bryan Casler (he/him)**

When you load by default, you'll be in Summary View, which shows everything that's happened. But on the left-hand side, you can actually see the individual events.

So we see all of these. We see this EN page JSON or a lot of events we fire. So that's good.

All right. Now let's go and trigger a conversion event, hopefully. and the

[@49:13](https://fathom.video/calls/344863905?timestamp=2953.34) - **Sydney Moyer (4Site Studios)**

And this is going to make a live donation, or no?

[@49:18](https://fathom.video/calls/344863905?timestamp=2958.0) - **Bryan Casler (he/him)**

use fake credit card number, and it should be a test gateway, so it should be fine. Cool. All right.

Let's go back here. We could clear this out if we wanted to, but we're at a nice round 50.

[@49:37](https://fathom.video/calls/344863905?timestamp=2977.34) - **Sydney Moyer (4Site Studios)**

Easy.

[@49:39](https://fathom.video/calls/344863905?timestamp=2979.7) - **Bryan Casler (he/him)**

Let's make a donation and see what happens. All right. Thank you, Paige. Wow, so we're at 123, so that means a lot of things just fired.

What we don't see, though, is any new pixels. So it definitely... Did not fire. I can actually show it.

That's not what we did. What did we call it? Ian Successful did it. We'll clean up that name. Interesting.

It's not in there at all. Hmm. Hmm. Thank you. So I don't know why that is. We have our renamed tags here, but we're not seeing our new tags.

Interesting. Let's go back here and actually rename those. Spock version. We can set this one in here. So that gets that, which we can at least check this.

And then to see the variables, you got to go to. don't don't Like the last, basically these are the events and when you click on one you can see what the value was at different times.

[@52:07](https://fathom.video/calls/344863905?timestamp=3127.6) - **Sydney Moyer (4Site Studios)**

Gotcha.

[@52:08](https://fathom.video/calls/344863905?timestamp=3128.44) - **Bryan Casler (he/him)**

About the page. So our variables aren't here at all. But they are here so that's good. Okay.

[@52:29](https://fathom.video/calls/344863905?timestamp=3149.44) - **Sydney Moyer (4Site Studios)**

Is this not defined as a variable in this GTM account?

[@52:36](https://fathom.video/calls/344863905?timestamp=3156.28) - **Bryan Casler (he/him)**

Yeah, let's see. It should, so here's where it got pushed as an event. And then here, yeah, it both gets pushed as an event and set as a variable, which there it is getting set.

Let's go back over here. Data layer. Variable Name, that's right. Format. We're not going to mess with that. We do have this, though, which we can key off of, which I'm going to do.

Yeah, so we have an event we fire called Successful Donation. So instead of this, what do want to do?

I want to do it off of custom event, event name, there we go. Awesome, Alright, so I'm gonna change that.

So now, instead, our trigger is listening for an event that our EM grid fires. And it's got a little bit of logic baked in there for when it does that.

But even more, what was the word I used earlier? Robust. Not fragile. Gotcha. And then in. Confirming, that's right.

Okay. So ID fires all page views, conversion. Thank you. We're missing something, so we have the universal, ah, okay, it didn't save, alright, so we replaced the tag for the all page view pixel, but our tag, it looks like for the Facebook conversion, didn't trigger.

So we have, we have the trigger, we don't have the tag that goes with it. I don't know what happened.

Let's break that again. By the way, it's looking like it's gonna storm here. Wow. After, after your comment, I'm like, oh.

[@55:51](https://fathom.video/calls/344863905?timestamp=3351.6) - **Sydney Moyer (4Site Studios)**

Moving on up. Or sideways.

[@55:55](https://fathom.video/calls/344863905?timestamp=3355.7) - **Bryan Casler (he/him)**

Yeah. So let's, let's, let's, let's And then we wanted to include this as a purchase, I think we can add a value, and then the variable here, all right, that probably explained, okay, we'll get better, let's try this test again.

So I'm just going to close everything out. Yeah, we'll try this one more time and see how far we get.

[@56:44](https://fathom.video/calls/344863905?timestamp=3404.44) - **Sydney Moyer (4Site Studios)**

Cool.

[@56:53](https://fathom.video/calls/344863905?timestamp=3413.78) - **Bryan Casler (he/him)**

We got our new pixel. Okay. $6 this time. Great news, so our pixel fired, let's look at it, did include the dynamic amount, did that record anything, who knows, because we don't have access to all the details.

Objects, probably, I don't even know. I'm using this right, so Facebook. Seems right. What could pass, let's modify it and add currency.

Usd. Wow, so yeah, let's see usd. It's cool. It's cool. Yeah, that's it. Okay. We'll just leave it as is.

Let's see if we can see any more, which would be trying to see. Sometimes you can see a little bit more info.

I can't remember how. the the the the Thank you. That was the first page, looking for anything that looks different there, no, okay, so the good news is we've now staged all this, and basically the next part is to confirm that it's tracking in Facebook as we intended.

Just to go back through one more time what we did, we replaced the old method of pixel tracking with the built-in template.

We could back out of this and go the old method, and then same for our new conversion tag, we could go the old method, but if the template is to be trusted, might as well try it.

We created a tag and a trigger by the same name to trigger when a successful donation happens. The way we trigger is the way looking.

For an event name of Ian Submission Success Donation, which is created by our IanGrid page template on a successful donation.

We then record that by passing in the value of the donation, which is also set as a custom variable on the data layer, also passed in as a data layer variable by our IanGrid page template.

And then we hard code the currency to USD.

[@1:01:30](https://fathom.video/calls/344863905?timestamp=3690.14) - **Sydney Moyer (4Site Studios)**

Is there a reason that's hard-coded versus custom?

[@1:01:34](https://fathom.video/calls/344863905?timestamp=3694.54) - **Bryan Casler (he/him)**

Yeah, don't think they offer, um, I don't think, they literally don't have the field to offer different currencies. Yeah, yeah, okay.

Um, but we could look at this. So currency, I mean, it's a, it's kind of trivial to add it in.

So let's do... What is you've got Thank So this is the currency variable, so let's do it, yen donation, currency, fix it, yeah, custom event, or custom event, it is daily there we go, and then we can, that's the robustness, I love it, we'll add it to the tag, there we go, all right, so I want to just go back and

Leave some breadcrumbs for ourselves. We created a new workspace on the SPC AI GTM Container, all meta pixel, and made the following changes.

Able Vanilla, Facebook tag, created, Facebook, Licks, Gtm tag, created Facebook, pixel, great GTM tag, And an animation, allow, stuff there, more.

So we have on- gtm trigger graded and dimensions gtm tag using the trigger and custom variables tested here and our custom our new tags varying when expected and actually you

We don't have access to their Facebook account yet, so we can't confirm that this is working as expected. There is also the chance that the Facebook template in GTM that we use, instead of the vanilla implementation, we're going to have other effects only to let them know.

And then, did I ever update the misspelling? Yeah, looks like it, yeah, all right.

[@1:06:26](https://fathom.video/calls/344863905?timestamp=3986.04) - **Sydney Moyer (4Site Studios)**

Cool.

[@1:06:30](https://fathom.video/calls/344863905?timestamp=3990.08) - **Bryan Casler (he/him)**

So figuring it out as we go, um, one part just kind of cleaning up, uh, and the other part was, um, troubleshooting, which who knows, right, if this is working, but it's probably in the ballpark.

Like, we've got all the pieces, let's say for some reason we can't disable the old vanilla, uh, uh, tag, uh, maybe the new ones causing, you know, yes, it's better, but it's also causing like now misreporting.

It's like, Hey, we can go back. And that just means we'll swap out our template tag for a custom code tag, and we'll just put in the code with the dynamic variables, and then we'll be done.

[@1:07:14](https://fathom.video/calls/344863905?timestamp=4034.14) - **Sydney Moyer (4Site Studios)**

Cool. Okay.

[@1:07:15](https://fathom.video/calls/344863905?timestamp=4035.92) - **Bryan Casler (he/him)**

There may be other things they're looking for. For example, I don't know, some people do the Add to Cart stuff.

So if someone interacts with the page, let's, you know, update that. Like, what does that look like? Um, but these are the basic ones.

You viewed the page, you converted on the page. Everything else is, is gravy.

[@1:07:33](https://fathom.video/calls/344863905?timestamp=4053.94) - **Sydney Moyer (4Site Studios)**

Yep. Makes sense. Okay. All right. That's really helpful. Um, in terms of tracking this time, I can leave a note for Heather that just says...

**ACTION ITEM: Note to Heather - FB Pixel impl work done w/ Bryan, bill both our time - [WATCH](https://fathom.video/calls/344863905?timestamp=4067.9999)**

[@1:07:47](https://fathom.video/calls/344863905?timestamp=4067.46) - **Bryan Casler (he/him)**

Let me kick, uh, kick Fathom out. Boom. Perfect. Um, and then, all right, go ahead.

[@1:07:58](https://fathom.video/calls/344863905?timestamp=4078.18) - **Sydney Moyer (4Site Studios)**

Um, I can... can... And leave a note for Heather on the test that just says, I watched you do some of this work, and so on.

[@1:08:09](https://fathom.video/calls/344863905?timestamp=4089.6) - **Bryan Casler (he/him)**

I mean, I think we'd say we did it together. Yeah. Like, you watched, but, like, you're set-carning, so.

[@1:08:16](https://fathom.video/calls/344863905?timestamp=4096.82) - **Sydney Moyer (4Site Studios)**

Yeah. Okay. All right, cool. And I'll just leave it up to her as to how she wants to build it.

[@1:08:25](https://fathom.video/calls/344863905?timestamp=4105.22) - **Bryan Casler (he/him)**

Yeah. I think she should build for both of our time. That was pretty quick, especially given that we don't have everything and we kind of just had to shoot in the dark.

[@1:08:33](https://fathom.video/calls/344863905?timestamp=4113.14) - **Sydney Moyer (4Site Studios)**

Yeah. Yeah. For sure. Okay. All right. Sounds good. Yeah. That definitely seems logical and doable. Like, it seems, too, like, kind of once you get in the flow of it, that it's pretty straightforward.

[@1:08:48](https://fathom.video/calls/344863905?timestamp=4128.9) - **Bryan Casler (he/him)**

Yeah. getting at the setup is, like, sometimes 80% of the work. Sometimes troubleshooting the setup then becomes your 80% work.

The only thing I would say is just make sure. Follow up to say, hey, like, we're ready to test as soon as we get Facebook access, and then that'll be, you know, the, that'll be the really important part that we ensure everything is tracking correctly before we tell them to start their own testing.

**ACTION ITEM: Follow up w/ Jamie re Facebook access for SBCI GTM testing - [WATCH](https://fathom.video/calls/344863905?timestamp=4150.9999)**

[@1:09:19](https://fathom.video/calls/344863905?timestamp=4159.1) - **Sydney Moyer (4Site Studios)**

Yeah. Okay. All right. Cool. I'll leave a note for Heather, and I'll write a note to Jamie just following up to get that access, and we'll go from there.

[@1:09:29](https://fathom.video/calls/344863905?timestamp=4169.1) - **Bryan Casler (he/him)**

Sounds good.

[@1:09:29](https://fathom.video/calls/344863905?timestamp=4169.92) - **Sydney Moyer (4Site Studios)**

All right, Sydney. All right.

[@1:09:31](https://fathom.video/calls/344863905?timestamp=4171.4) - **Bryan Casler (he/him)**

Thanks, Bryan. You're welcome. Take care. You too. Bye.