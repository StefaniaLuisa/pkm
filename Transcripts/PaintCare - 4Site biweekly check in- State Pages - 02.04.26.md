# PaintCare + 4Site biweekly check in: State Pages  - February 04

[**VIEW RECORDING - 37 mins (No highlights)**](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4)

[@0:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=0.0) - **Stef Jones (4Site Studios)**

Ten book-a-roonies. I love Depop, and it's a problem. I need to start selling on Depop to, like, make the difference up.

But what a steal of a deal. I love it.

[@0:12](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=12.98) - **Sebrinia Welch**

That's awesome.

[@0:13](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=13.88) - **Stef Jones (4Site Studios)**

I've never heard of that. Oh, so it's an app, and it's like a marketplace. However, it's more, like, clothing-based and not so many things.

[@0:24](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=24.84) - **Heather Schneider (she/her)**

Yeah, I use Poshmark. I haven't used Depop.

[@0:27](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=27.3) - **Stef Jones (4Site Studios)**

Well, Poshmark, I have a friend who used that one. I don't know why I haven't used it. I forgot about Poshmark.

Don't get me started.

[@0:34](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=34.46) - **Sebrinia Welch**

to start it up before, too.

[@0:35](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=35.9) - **Stef Jones (4Site Studios)**

Yeah.

[@0:36](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=36.94) - **Heather Schneider (she/her)**

I sell on there sometimes. I'm much better at buying than selling.

[@0:42](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=42.24) - **Stef Jones (4Site Studios)**

I, so my parent, my mom's, where we, my mom's a hoarder, hoarder, hoarder. And so every time I've been going there, I've been, like, taking things out of the basement.

And, like, I've just started taking photos, but, like, my goal is to start selling something. I told my dad I'd give him a cut.

TBD and how that goes. My mom is like, everything in here means so much to me. like, all these trinkets?

[@1:14](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=74.68) - **Heather Schneider (she/her)**

It's a real thing.

[@1:15](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=75.34) - **Stef Jones (4Site Studios)**

Yeah, just talking about the millennial and Gen X inheritance. Yeah, it's fun. But I was just talking, Sabrina and I have the same kind of sweatshirts.

And I bought mine off of Depop, which I just love, like it's a resale for clothing. Oh. Yeah, and it's an app.

And I got it for 10 bucks. And I just, I'm shopping too much. So I need to weigh out the pros and cons.

[@1:49](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=109.08) - **Heather Schneider (she/her)**

Well, good morning, Chelsea. We are excited because we are going to take you through the state pages today. So the development is complete.

It's been thoroughly QA-ed. By the team, so Mike is going to walk you through, show you what the front end looks like, and then we can dive into how the back end works so that we can get you set up to start doing your own testing.

[@2:11](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=131.56) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay, sounds great.

[@2:13](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=133.62) - **Heather Schneider (she/her)**

All right, Mike, over to you. And Sabrina, Stef, as you see things, I know that there's some topics you wanted to touch on with some of the design aspects, so feel free to jump in.

**SCREEN SHARING: Michaelw started screen sharing - [WATCH](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=141.673325)**

[@2:28](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=148.16) - **MichaelW**

Okay, so there's a new custom post type on staging right now, the state. And let's see, it's separate from the existing states.

We're keeping around the existing states for now, just for reference purposes, much like how the events, the old events are still there.

I should probably go ahead and remove the old events, actually, when I do the next deploy. Let's just show you what the states kind of look like.

We'll start with California as an example. So here we have the centered hero image, title appears over here on this little paint splash background.

We have program details with this information slider that kind of gives you kind of like a heads-up view of all the most important facts about what you guys have done in California.

We have the drop-off paint site locator. We have some informational columns about the large volume pickup service, what kind of products you accept.

Here are some example events. These aren't actually real events because I just, I don't think you guys have any real events right now that are live.

So I just temporarily made these live just so you can see what these look like on California or on a state.

Here we have the fees and funding section that kind of gives you an overview of how much, what the cost are associated with the different sizes are quantities of paint.

We have the official document section, which we're . Here you have your annual reports that are specific to the state that you currently live on, like the official documents page for each state.

These are moved here now and we have the resources which gives you links to the information for California retailers and the brochure materials ordering page.

We have the sidebar menu that automatically assembles itself based upon the content that's here on the right side. So it assembles itself from the headings and from the accordions.

So that's California. Let's look at some of the other states. have some of the other blocks that are featured.

Here in Maryland, for example, we have a video block with single video on it. Here on this test state page, we have a video block with multiple videos on it, and you can see how it lets you select from.

beizers into All the videos below it, sort of go through like a list. Here in Colorado, we have an example of the door-to-door pickup service, which is here.

Gonna use the information about that. We also have a feed block with additional details because it gives you a price change as of an effective date here, which should be April 1st.

Let's see what else. I think that was the highlights of all the major sections. So now let's talk about how this thing is built.

Let's go back to California, Edipa State. Here you have the default Gutenberg editor because custom blocks are loading. So here's what the information center kind of looks like.

So... So It gives you kind of like the details and brief summaries of what's been done in California, and you can add as many of these as you want.

This is the Site Locator. This is the Events for State shortcode, which automatically loads the events if there are any.

And the Official Documents section, which is some accordions that you maintain manually, much like you do currently with the Official Documents page, except that instead of maintaining a separate page, it's all here on the same page as California.

One thing to note in the Gutenberg Editor, just a reminder that this table of contents is really handy when it comes to building things.

So if you click this, it shows you the overview and lets you easily select these different blocks. One thing that's also really useful with this table of contents here,

Is that if you click the blue button and you click patterns, we've created some patterns that represent, that they're used in the state pages so that you can very easily just sort of like, you know, drop, drag and drop things into the document with some, basically some personal information which you can then update whenever you're creating a new state.

So here we have the new program information section, here we have the door-to-door pickup service, the fees and funding with the single row, program details, official documents, etc.

So whenever it comes around, comes time to like actually create more states, you'll probably find this handy so that you can very quickly get up to speed and get everything kind of dropped into place and then you would go back and edit it.

Let's take a look at some of the other blocks. So this is the custom block, the information slider. If there's loads, and it's shown here, the fee block, which is here, and you can sort of like go through here and update the different prices as they're updated, or you can add price schedules, future price changes, by adding a row and then putting in a different value for the future.

Let's say the five-gallon was going to go to $2 in California. Oops. And that's how you would kind of add those additional prices for the future.

[@8:52](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=532.881) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

For the fee with the, when we have like the two different fee charts, like you're referencing... How do you get the color difference?

[@9:03](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=543.58) - **MichaelW**

It happens automatically. So, yeah, the first row is blue and the first row is purple. Yeah, right. The additional rows are all purple.

And by the way, you can add as many future price changes as you like. You can stack 10 of them if you wanted, if you happen to have that information.

So maybe this goes to $2.25 on April 1st and maybe gets up to $4 in, I don't know, 20, 30.

[@9:34](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=574.0) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah.

[@9:34](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=574.96) - **MichaelW**

You can stack all that information up, so it just gives them a heads-up view.

[@9:39](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=579.68) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay. And then you showed me the short code for the events. Is that something that we should just have, like, be there the whole time?

[@9:49](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=589.16) - **MichaelW**

Like, is it still functioning the same way where it won't show unless there's actively an event? That's correct.

[@9:54](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=594.84) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay. So we should just, like, leave the short code there and it will do its thing.

[@9:58](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=598.14) - **MichaelW**

Mm Okay.

[@9:58](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=598.48) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@10:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=600.001) - **MichaelW**

They're forever, and any time you have events, it'll automatically show up here.

[@10:03](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=603.641) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@10:06](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=606.141) - **MichaelW**

See, here we have an example video block with a single video. Because there's only one video, it doesn't give you the slideshow underneath of it.

So it just doesn't show that whole slideshow bit underneath. It just shows a single video. And I'll show you what that video block looks like on the back end.

So here we have the new program information. And this is a video block. And, yeah, you just pop in the URL.

There's a thumbnail. It's optional. You don't need it for YouTube videos because it automatically pulls in, you know, the YouTube thumbnail.

But this video block does support Vimeo, YouTube, and MP4 videos that are uploaded to the site manually. So Note that the title and the content are required.

Technically, I mean, it's not really required, but if you want it to look correct, you'd want to put that information in.

Otherwise, the video will expand to fill the entire width of the area. In fact, I can show you what I mean.

So here we had the video, and you can see it has a title, has some content in the video itself.

But if I were to come back and actually delete those. I'm just pasting this into my text editor so I lose them.

And then save. Then refresh. And you see it just, it just expands to fill the entire, the entire width.

The block, so because it doesn't have that text information, but it does tell you that it's required because we kind of wanted to try to maintain the same ratio across all the different slides.

So it's kind of weird, like if this one has text, this one has text, this one has text, and this one, we're to fill the entire section.

It's a little bit weird, so. But technically, if you don't have text, you don't have to put it there, but it's preferable.

Just for the way it looks. Let's see, that was the video for the single. This is how the video looks, there's like four of them or more.

Header text field. Ah, yes. So this bit here that says get started by finding a drop-off site, this is actually free form text area.

So you can put anything you want there. By default, it just. Drops in this link, it says get started by finding a drop-off site and links to the site locator, but you can actually put anything there that you want.

So if you come back over here to the test state, scroll down to the bottom, and this is where that lives.

Not that you'd ever really need a certain need to put anything else down here, but you can if you want to.

**ACTION ITEM: Set bottom CTA default text color to white - [WATCH](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=819.9999)**

Okay. Actually, probably should. That should probably default to being white color because this is a blue splash paint background.

So Well then Yeah, so I'll make sure I'll make a note of that. Oh, and this image here, this is the featured image.

So if you open up the state sidebar in the editor, that's where you set that image. So you're probably going to want to make sure and set that, like, a rectangular landscape-oriented image for every state that you create.

Of course, I've already set those for all of the existing states already, but future states. Oh, and you might see here this title shortcode.

That's just a little shortcode I created just that automatically inserts the name of the page, wherever that's found. And that's just because I was copying and pasting a lot of these blocks in the different states, and I didn't like having to keep continually, you know.

Re-update the name of the state and all these different blocks. So I just put in a title and it automatically fills itself out on the front end.

So this bit here, paid care offers drop-off sites throughout Colorado, that's actually a title sort code. It just pulls that directly from the name of the page.

So if you see that inside the editor, that's what that's doing. Uh, so I think that's pretty much it.

Uh, it seems, I think it should be pretty straightforward. Uh, there's a few new blocks, the video block, um, the info slider block, the fee block.

And, uh, this button here that looks a very particular way. It's just, uh, it's just a singular button that, um, looks like this and looks like this on hover.

Just to show you what that looks like. It gets not much to it, really. really. really. It You But it is a custom block because we wanted a button that looked a very particular way so that we'd match the aesthetics of the state pages, which is here.

So, any questions about how to, you know, maintain these state pages?

[@16:34](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=994.942) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Not that I can think of right now. I might need to, like, click around.

[@16:45](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1005.64) - **Heather Schneider (she/her)**

And I put a note in the chat that we'll be replacing the links in the navigation to go to the new state pages as well.

Although, actually, the URLs will stay the same when we launch, right? The state pages?

[@17:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1020.0) - **MichaelW**

The URL actually is subtly different. So you can see here, it's, this is slash state slash Colorado. The original state is slash states slash Colorado.

So it's subtly different. However, when it comes time to deploy, what it will do is I'll set up some redirects.

So the old states URLs automatically redirect to the new state URL. That way they completely replace it. I'll also update all the links in the states page and in the states menu.

And further, we'll also take the official documents page and then replace these links with redirects to the new sections on the new pages.

So for example, annual ports for the old Colorado goes to this page. However, annual ports for Colorado in the new style would come down here.

So I would actually just take the, take Take these links and set up some redirect patterns, so the old links automatically redirect to the new links, and I'll be sure to update all the existing links on the site currently with the new link style.

That way, even if somebody somehow has a link to the old states sitting around in their, I don't know, their favorites or their bookmarks or something, they'll still wind up at the correct place, which is here.

So any questions, concerns, or feedback?

[@18:42](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1122.18) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Can you show me how the annual report image is in the, I guess it's the accordion menu? Yeah.

[@18:51](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1131.68) - **MichaelW**

Yep. So it's right here. And this... This a what's called a media and text block. This is one of the default Gutenberg blocks.

So it lets you set an image, and this image has been set to 30% of the width, and then it has on the right side the text.

So this is just a standard Gutenberg block, and currently it's only being used in the state pages in this particular location of the accordion, where you can provide the latest report details.

[@19:38](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1178.48) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@19:49](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1189.36) - **MichaelW**

So you can come in here and easily replace the infographic with a new infographic if you need to. So that is are saying, you doing to to see.

let's taking the the bottom. give see talking about of one. And You So, yep. Any other concerns about that?

[@20:10](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1210.96) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

No, I think that makes sense.

[@20:12](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1212.66) - **MichaelW**

just was curious.

[@20:14](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1214.06) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

And then, to go back to what you were saying earlier, I forgot what the section is called, where you kind of have, they're not like templates, but you have like the example of like the, if we were like recreate the state of patterns.

[@20:27](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1227.64) - **MichaelW**

Yeah.

[@20:28](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1228.8) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

So, yeah, we had this paint care state category of block patterns. Under patterns. Yeah. And is that something that, you said that those have been like created and I could like drag them over?

Is that how that works? Sure.

[@20:47](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1247.74) - **MichaelW**

Yeah. I'll show you real quick.

[@20:49](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1249.26) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay. I just wanted to clarify.

[@20:50](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1250.92) - **MichaelW**

We can do that. I'm going to edit my test state. And then we'll go ahead and just delete everything.

everything. Thank Okay. And then we'll add some patterns. And we'll start with the... Here we go. Program details. So here, I've clicked on it, and it automatically inserts this information here.

And this is sort of like what's currently there on the California page. I use the California page for a lot of the black patterns.

But we can change the black patterns to be, you know, to have different information if you wanted. But this is just what gets inserted by default.

So there's the program details. Next, maybe we want official documents. Again, it comes in with some just default information that you can update.

And then maybe we want to put something above the official documents. So we'll before. And let's see. Fee and file.

file. There you go. And automatically inserts this information here. So by using the blocks, you can very quickly get up speed is the bottom line when creating a new state.

[@22:11](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1331.44) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

No, that's helpful. Yeah.

[@22:15](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1335.2) - **MichaelW**

So it just puts in some default information that you then correct for the state that you're currently building and then you save and that's it.

[@22:27](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1347.96) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

And do you have any guidance for the, um, I noticed that these are, these images are kind of different sizes and shapes and they kind of became uniform on the live page.

Is there a specific size or shape we should be looking for when, when I update these images?

[@22:47](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1367.14) - **MichaelW**

No, doesn't really matter what size images you use. They're automatically going to get resized to a particular height.

[@22:53](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1373.22) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

That's what I thought it like looked like. I was just verifying.

[@22:56](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1376.92) - **MichaelW**

Yeah. So come over here. So we added these, these images here.

[@22:59](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1379.58) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah. And then you see they're all being forced to the same height. Yeah, and I can tell from the original one that they're not all the same height.

[@23:07](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1387.14) - **MichaelW**

So, okay, that's helpful too.

[@23:09](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1389.88) - **Stef Jones (4Site Studios)**

The goal with this section and the icons really are to keep icons, because even looking at, I think with the mock-up, we had more graphic images that had a number on it, which really don't work for these so much.

You can see the, the California, you really want to, you can't even read the 99.44%.

[@23:33](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1413.58) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, I mean, I, I imagine when I, I, I meet with the graphic designer on this, we'll, we'll, we're gonna, I mean, we're gonna update our annual report graphic, and then they'll inform this.

So then, like, the number will just be changing throughout the year and not.

[@23:47](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1427.54) - **Stef Jones (4Site Studios)**

Yeah.

[@23:48](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1428.18) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

The actual graphic itself.

[@23:49](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1429.74) - **Stef Jones (4Site Studios)**

Yep. Then that's exactly goes into one of the things. Sabrina, think you like, like, I will.

[@23:56](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1436.48) - **Sebrinia Welch**

I was like, I'm muting and ready to jump in.

[@23:59](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1439.44) - **Stef Jones (4Site Studios)**

Yeah. I'll Sabrina. Karina, jump in.

[@24:01](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1441.1) - **Sebrinia Welch**

Yeah, so I mean, the goal of that, of course, with that block is to be able to add anything, really.

It's supposed to be, you know, very flexible to say, here's some sort of imagery, here is a big data point and a label.

And you'll see on, like, different test pages that we had the California, what I took from that, the mock-up, was from the annual report or, you know, the infographic.

But what Mike did for the rest of the states was actually pull in the program details, which is a little bit different.

So you get to decide, you know, what information you want to pull if it is truly from, you know, the infographic.

But we did want to show, like, what does three cards look like versus what does five cards or, you know, five data points look like.

But yeah, ultimately, we wanted to reach out to you all, because I knew you had a graphic designer, to lean into those kind of visuals that allow for your brand to also ensure that it looks aligned to

[@25:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1500.0) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Not just like little clips that I made for the sake of the mock-up from the- no, no, until, I mean, we, we had this on our radar that they, Tiffany's the name of the graphic designer, she's going through and like updating a lot of our materials right now, um, so that's, that this is all helpful for that.

[@25:20](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1520.68) - **Sebrinia Welch**

Perfect.

[@25:23](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1523.08) - **MichaelW**

I just, uh, to highlight one other thing, uh, about the sidebar menu, so it, it keys itself based upon these headings.

So if I were to add another heading somewhere, anywhere, it's automatically going to get picked up, um, so we'll go ahead and just add another heading up here.

[@25:46](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1546.72) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

And is it like the H2 heading specifically, or?

[@25:50](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1550.44) - **MichaelW**

No, any heading.

[@25:51](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1551.88) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

heading, okay.

[@25:52](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1552.46) - **MichaelW**

Yep. No. In here. you. So here, it's there. So that shows up at the sidebar as you create them.

Also, the official documents accordion area, that is kind of a special case in that the accordion items, the headings of the accordion items get automatically pulled in underneath of the title preceding it.

So here, we have official documents as a heading, and then we have this accordion with all the accordion items.

And so the headings are automatically pulled in as children of the prior headings. So just taking note of that is that whenever you create an accordion, you'll want to have like a title for the entire section above it.

That way you notice how to organize itself. So, that's lot information about. That's It's It's lot. It's a lot.

It's a You see here, for this accordion, we have these three accordion headings named annual reports, law, and sales tax, and then resources, and those automatically get pulled in as children under the preceding title.

So this is actually, so I guess what I'm trying to say is official documents is not an actual part of the accordion at all.

It's just a loose title that's positioned just before the accordion.

[@27:26](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1646.62) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay, yeah, that makes sense.

[@27:28](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1648.8) - **MichaelW**

Okay. So, all right, any other questions, concerns, or feedback?

[@27:42](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1662.26) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Um, where's the drop-off paint title being pulled from? Because I noticed that the title looks different for the site locator section.

I'm just curious.

[@27:55](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1675.14) - **MichaelW**

So, site locator is here. It's just a short code. And so, um... You specify what state it is via the abbreviation, and then you give the entire thing a title if you want to, which is what, I think if you take away the title, I think I have it currently not providing that blue box, so you don't even necessarily need to block.

If you were to remove the title, the blue box would go away.

[@28:20](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1700.26) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay, and then in theory it wouldn't show up on the menu?

[@28:24](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1704.12) - **MichaelW**

I mean, yeah, correct, because the title...

[@28:26](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1706.72) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

was just curious, okay.

[@28:28](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1708.4) - **MichaelW**

Right. Let's just see what happens if I take this away. Been a while, so I tested this.

[@28:34](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1714.68) - **Stef Jones (4Site Studios)**

And we're not able to style that in the same way, or like the font?

[@28:40](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1720.26) - **MichaelW**

No.

[@28:40](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1720.98) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

because it's part of the existing locator, right? Like that's...

[@28:51](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1731.52) - **Heather Schneider (she/her)**

Maybe that's... When we finish this site locator project, will it be styled better to align with the new design?

[@28:58](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1738.58) - **Stef Jones (4Site Studios)**

Yeah. Oh, that's kind of...

[@29:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1740.0) - **MichaelW**

Right. So because I took away the title, now it just shows the locator without the title and without that blue box surrounding it.

[@29:06](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1746.98) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@29:09](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1749.12) - **MichaelW**

But I'm going to put it back now.

[@29:10](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1750.58) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah. mean, like, I think we want it there.

[@29:11](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1751.78) - **MichaelW**

I was just curious because it looks different. Yeah. And then what you can, mean, if you want to take away the title, maybe you don't want the blue box anymore, but you still want it to be in the menu.

You may try to just add a title add a title box. Yeah.

[@29:24](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1764.66) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@29:27](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1767.14) - **Stef Jones (4Site Studios)**

Yeah, that looks actually, I like, oh, that looks a little more, uh, sleek.

[@29:38](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1778.9) - **MichaelW**

All right. So what next? Uh, Chelsea.

[@29:45](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1785.56) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Um, I don't know. Like I said, I think I need to, I'll need to like, play around. don't know if have any more questions this moment, but, um.

[@29:52](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1792.74) - **MichaelW**

Okay. Okay.

[@29:53](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1793.44) - **Heather Schneider (she/her)**

And Chelsea, do you have access to log into the back end of the staging site?

**ACTION ITEM: Send Chelsea staging links (old vs new) + recording; request Bugherd feedback by Feb 13 - [WATCH](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1794.9999)**

[@29:58](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1798.36) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

I put the link in. think. So I haven't tried it in a while, but I can.

[@30:03](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1803.52) - **Heather Schneider (she/her)**

Okay. I have all the links in a task ready to go for you. That links also to each of the current state pages and the new state pages, so you can look at them side by side if you want.

Do you think now through the end of next week, so the 13th, is enough time for you to do testing?

[@30:23](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1823.78) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, that should be fine.

[@30:26](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1826.1) - **Heather Schneider (she/her)**

Okay, wonderful. Mike is on vacation next week, so when he gets back on the 17th, and we have time set aside to do any improvements, but if anything is blocking you as you're doing your testing, just let us know, and we could, Steph or Sabrina can jump in and support while Mike is out.

And I will share the link to this recording in case you want to review anything from there, but we are excited to get your feedback.

[@30:56](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1856.0) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, mean, it looks, it looks good.

[@30:57](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1857.54) - **Heather Schneider (she/her)**

I'm, I'm excited. Awesome. Awesome. Awesome. Does anyone have anything else to chat about?

[@31:04](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1864.6) - **Stef Jones (4Site Studios)**

I feel good about everything, Chelsea. We are chugging along, working on the site locator, but I feel good. Sabrina?

[@31:14](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1874.68) - **Sebrinia Welch**

Pretty good. I noticed in Figma that there were some comments dropped, so appreciate that.

[@31:22](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1882.06) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, we have very minimal feedback other than the comments that we made, I think, at this point. And I'm getting some icons that we've already used from our graphic designer to see if they can be helpful at all.

I don't know if we're looking for, like, the exact icons we want to use or, like, inspiration, but we can work together on that if I do not have what you're looking for.

[@31:50](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1910.3) - **Sebrinia Welch**

Yeah, absolutely. Did you, I guess another thing that I would be curious about, if there's any sort of, I guess, flow?

Those or things that aren't reflected or like actual tasks that the user would do that are reflected, that would be also great to know.

One thing that came up to mind as we were preparing for this was just realizing that the frame or I guess the column in which our state pages is narrower because we have that floating table of contents on the left.

So that's something that I kind of want to, I do want to process is that, you know, if we do narrow our map for the maps that are embedded on the state pages, it's going to be, as you see, as you saw there, but like, it'll be, the width is quite considerably less than a full width desktop.

So processing potentially, is there something we need to do differently for the state pages due to, um, that, that floating table of contents is something that I might want to process out as well.

[@33:00](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=1980.0) - **Stef Jones (4Site Studios)**

I actually kind of liked and would love to hear your thoughts on, you know, removing that outline did make it look, it doesn't make it much bigger, but I wonder if just having that so it's not boxed, I don't know, could be something that just makes this area look a little sleeker, but again, that can happen.

[@33:21](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2001.5) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Like having the title, just the title that matches the other ones and then remove the blue box.

[@33:25](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2005.66) - **Stef Jones (4Site Studios)**

Yeah. And then I wonder if there is a little room for it to be a little wider because we were kind of removing that outer, that outer layer.

Um, I don't think it's terrible that it's this little, I'm just trying to think it's because it's especially on a state, you know, I think I would be more concerned if this was like how it showed, you know, uh, for the whole entire state, but that's just my subjective opinion.

I think, um, I would love to hear how the rest of your team feels about that. And maybe, you

You this view right now is pretty high up. I wonder, do we go a little further into the state to, you know, like, zoom in just so you're really just looking at the state, yeah.

[@34:13](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2053.94) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, and, like, not seeing the states, which in this example are particular or not are states.

[@34:20](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2060.42) - **Stef Jones (4Site Studios)**

Yeah, and so, like, right here, I think this is a really nice view, and especially as we put the new site locator, which will show the out, the other states, even if they're not.

**ACTION ITEM: Mock embedded locator on state page + main locator page for Chelsea review - [WATCH](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2067.9999)**

Yeah. So I think an increased view would be good.

[@34:38](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2078.82) - **Sebrinia Welch**

That's just, like, in the next revision, I might just mock up what the embedded map looks like on the state page so that we just have a point conversation.

[@34:48](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2088.36) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Or, like, yeah, because I know that the examples we're looking at now for the new locator, it's sort of, it is taking up the entire, like, fake desktop.

So it might be helpful because it is going to exist. in the next field. Like within like a page on a browser, so like what it would look like on the actual, or this page, and then the main locator page.

[@35:12](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2112.77) - **Sebrinia Welch**

Yep.

[@35:13](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2113.93) - **Stef Jones (4Site Studios)**

Which leads me to, do we want to just leave this as is right now, because we're going to end up doing the work to, like, I don't want to, you know, waste your time of trying to fix this site locator, if we're going to just end up, re-adding those and making sure that it, you know, is exactly what you want.

So just something to be cognizant of.

[@35:38](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2138.97) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, I mean, I don't know if we just spent a lot of time messing with the current one. Yeah.

Yeah. And we're going to update it, too.

[@35:44](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2144.91) - **Stef Jones (4Site Studios)**

Yeah, I agree. I wouldn't want you to spend your time on that. We should spend time. This is a great kickoff to how we want to make it look with the site locator.

Yeah, kind of the same, but yeah, just savings use some time.

[@36:05](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2165.99) - **Heather Schneider (she/her)**

All righty. So I'll share all the links with you in a task and you can test away. Oh, and I added you to Bugherd for this project so you could collect feedback that way.

We've used Bugherd before.

[@36:20](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2180.29) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Yeah, okay. So this is like previously, we'll go through the...

[@36:24](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2184.85) - **Heather Schneider (she/her)**

Yeah, you just start tagging places.

[@36:26](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2186.69) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Make comments on Bugherd.

[@36:28](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2188.51) - **Heather Schneider (she/her)**

Yeah. Ideally, that would be great. If you have any challenges with that, let us know and then, you know, you could collect it other ways.

But I think it's probably just easier for you just to click a button, log your feedback, and then we can get that over to Mike with all of the screen and recording information that comes with it.

[@36:47](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2207.31) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Okay.

[@36:48](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2208.67) - **Heather Schneider (she/her)**

All righty, everyone. have a great rest of your day.

[@36:51](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2211.41) - **Stef Jones (4Site Studios)**

Thank you.

[@36:52](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2212.47) - **Chelsea Tufarolo ([paint.org](http://paint.org))**

Thanks, you too.

[@36:53](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2213.29) - **Sebrinia Welch**

Bye.

[@36:54](https://fathom.video/share/yPfUzztnJXV7xPX3HRDnT4DgeyuD8ez4?timestamp=2214.11) - **Stef Jones (4Site Studios)**

Bye.