?mode=DEMO

# ENgrid One-Col Training

Created for Mike for FWW - for their EOY One-Col
Meeting Recording - Review w/ Bryan 11.14.24 - [Let's talk FWW Promotions Plugin](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg)

**Quick Link Example of a One-Col:**
[~https://oceana.org/4site-en-one-step-donation-lightbox-test/~](https://oceana.org/4site-en-one-step-donation-lightbox-test/)
Public URL: [~ENgrid Reference - Donation Page (Test Gateway)~](https://give.foodandwaterwatch.org/page/75612/donate/1) Local Dev URL: [~https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false~](https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false)

**To install ENgrid**
Copy the repo: [~https://github.com/4site-interactive-studios/engrid-fww~](https://github.com/4site-interactive-studios/engrid-fww)
npm install
npm run build

**To run a local environment**
npm valet secure
npm valet start

Once you have your local environment up, you can load the local build files on a live page by simply adding ?assets=local to the URL. This will also turn on the debugger which will visually show hidden components on the page as well as add more logs to the console. You can turn it off by adding &debug=false and then opening the debug button that will be in the bottom right corner and closing it out. After that you will be using local assets without seeing the debugger.

Local Dev URL: [~https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false~](https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false)

Definitely check out the “Developing with ENgrid” pages in the sidebar to familiarize yourself with how it all comes together: [~https://engrid.4sitestudios.com/~](https://engrid.4sitestudios.com/)

What you can likely do is copy the field setup from the most recent NPCA buildout ( [~https://support.npca.org/page/75274/donate/1~](https://support.npca.org/page/75274/donate/1) ) to this FWW page, excluding anything Premium related. Then you can add the page as a One Column Lightbox via the Promotions plugin, that’s the EN Lightbox &gt; One Column option. For this I would just use it on the 4Site website.

When added into a lightbox the page will know when it’s being embedded and add a custom data-attribute to the EN page’s body that you can key off of. For the most part a lot of the responsive layout adjustment needed for being embedded should just automatically happen.

In the end you’ll get something like this, a single column embedded donation page: [~https://oceana.org/4site-en-one-step-donation-lightbox-test/~](https://oceana.org/4site-en-one-step-donation-lightbox-test/)

—
Bryan bootstrapped the first few bits:

- Create an ENgrid Client Theme and get local dev running ( I’ll share instructions on this )
- Upload Assets to Client Library
- Create an ENgrid 1 Column Page Template pulling meta fields and other ques from their current page templates
- Create a Donation Page using the Page Template
- Set the page template to allow for embedding
- Add 18 row advanced column with ENgrid Semantic Classes to Page 1 and Page 2
- Drop in a Title and Form Block just to fill some space
- Move over some basic styles, rebuild the theme, and upload to the client account

⠀Public URL: [~ENgrid Reference - Donation Page (Test Gateway)~](https://give.foodandwaterwatch.org/page/75612/donate/1) Local Dev URL: [~https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false~](https://give.foodandwaterwatch.org/page/75612/donate/1?mode=DEMO&assets=local&debug=false)

#4site/ENgrid #4site/client/fww
#4Site/transcript

## Transcript of Meeting:

#### Let's talk FWW Promotions Plugin - November 14

###### [~VIEW RECORDING - 16 mins (No highlights)~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg)

[~@0:00~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=0.0) - **Bryan Casler (he/him)**
Um, this project is for good and water watch who runs on the run on WordPress, right stuff. we want to further end of your fundraising be able to embed one of their engaging networks pages in a single column light box, which is exactly what the promotions plugin can do.
**SCREEN SHARING: Bryan started screen sharing - [~WATCH~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=36.603965)**
we just did this for Oceana, which is included in the task description, Mike, I'll share my screen. I'll pull up this page and boom, it just shows donation page in a one column.
If I inspect this page, the way it works is basically the page detects when it's embedded and he does all the things it needs to do.
display correctly, and then everything around it is just managed by the Promotions plugin. So what we need to do is two-fold.
One, get the engaging networks page set up for food and water watch, which needs to use our EnGrid code.
And then two, to set up a promotion that shows it working in the embed. To get you started, Mike, I know you're probably getting back up to speed with the EnGrid, but I just took it upon myself to create the initial client theme.
I didn't go through all that. literally just threw some colors on the page and got all the naming and everything.
And then I uploaded it into their account and just created a page with a single field and a submit button.
So basically this is the part that's a little complicated, but It doesn't really benefit you to learn in that process or remember it or whatever.
So anyways, what ahead ended that and what is needed now is actually going into engaging our works and building out this entire page with all the fields and classes and configurations that are needed for a donation page as well as the thank you page.
And then to do any additional custom styling on the theme. To edit this page inside of engaging networks, there's a couple ways you can do it.
You can log into engaging networks and then search by the page ID. We also have this nifty little feature called p edit, which stands for page builder edit, page builder in the name of the tool.
Enging networks has to edit the page. So let me see here. Yeah, if you're not logged in, it basically breaks this a little bit.
So it'll be. We're just using your shared account stuff and then the two offices in the one password I think experienced that before.
So if I go back here and do that one more time, boom, I'll be redirected to edit the page.

[~@3:23~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=203.68) - **MichaelW**
That is very handy.

[~@3:24~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=204.52) - **Bryan Casler (he/him)**
And what you'll see is actually made back out here, all this is in this folder, sorry, in this one development, and then that's this page.
The files are all uploaded to this, so you'll just replace these files. This is the only page using it, so you don't need to worry about it, you can just upload files.
One thing to be mindful of is let's say you upload an image asset. Even though there's folders here, it's a flat file structure.
So you just want to give it a unique name that you know is not potentially somewhere else in the account.
Because it'll just override it. Also, when you upload the images, there's a built-in image compressor. And it's absolutely trash.
Do not use it. Use some other service and then uncheck that box when you upload images.

[~@4:22~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=262.62) - **MichaelW**
All right.

[~@4:25~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=265.18) - **Bryan Casler (he/him)**
But I did go ahead and so when I set this up, I also copied over all the meta tags.
I copied over the GTM, any custom code they had in their other pages. So in theory, I think you just need to literally build out the page and then theme it and then do your QA.
Obviously, building out this page, there's a lot of details. The good news is we just did a build-out for another client that I think you can effectively copy.
So I think if you, yeah, I've screwed that up. I don't know if they're on the same server, let's see.
Yeah, so they're on the same server, so they're on this US server. So what you have to do is, if you want to be able to see both at the same time, you got to open up an incognito window.
**SCREEN SHARING: Bryan started screen sharing - [~WATCH~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=317.626769)**
Let's do that here.

[~@5:31~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=331.34) - **MichaelW**
I mean, I think we get it, you only need to do all that.

[~@5:34~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=334.1) - **Bryan Casler (he/him)**
Well, I just wanted to show you the inside of the page. That was it. And then there was just one final bit for you to like.

[~@5:45~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=345.34) - **MichaelW**
It doesn't look like you'd be able to into NPCA anyways.

[~@5:48~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=348.48) - **Bryan Casler (he/him)**
Just use my, you can just use my login.

[~@5:53~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=353.0) - **MichaelW**
Is there an requirement to factor up indicate?

[~@5:56~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=356.08) - **Bryan Casler (he/him)**
Yeah, mine's in one password though. All right, so all of the content, all of the copy I should say goes in body top and you can just put in lore on it some everything below that initial copy, basically all the form elements and labels go in this section and I just put one in there just for looks.
But I would basically copy this, obviously you can ignore the upsell but just copy the structure going all the way down.
And if you see something that's not there, like maybe this source can feel that's probably unique to NPC, I just ignore it.
This is the premium block also you, not this is not a premium page, it's a regular donation page so you can ignore it.
So you go down, down, down and in the blocks, the important parts are whether it is or isn't mandatory, any custom classes added and then any swap lists that are defined.
So here's an example where The this value is set with with the swap list And that should that should be it so like if that some of these things are specific to NPC I so you'll just use your judgment and swap it out You don't need to worry about a background image because no one's viewing this page directly.
It's only going to be embedded You You can put in a banner image though, like if you wanted to you just put in an image block or a code block with an image In it in the body banner and that would appear Appear there the last thing is Or the last two things for me are just around testing so we have this test gateway and All I ever do is just search the payment gateway
pay got renamed, it's not world pay.

[~@8:02~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=482.22) - **Stef Jones (4Site Studios)**
It's Vantage? Vantage?

[~@8:06~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=486.18) - **Bryan Casler (he/him)**
It is Vantage, isn't it?

[~@8:07~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=487.88) - **Stef Jones (4Site Studios)**
I think so.

[~@8:08~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=488.96) - **Bryan Casler (he/him)**
by world pay. And then here we go. And then I have this test credit card, which 411 or 40000 work, I don't know, maybe, but if it doesn't, I usually just Google it and then find it in here.
Let's hear the auto responders need to also be copied over from their real page. And that should be, that should be everything with getting the page set up.
One last thing I wanted to point out Mike was that we have in Android when you get your, when you get your code running local,
**SCREEN SHARING: Bryan started screen sharing - [~WATCH~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=533.662728)**
Okay, we have something called the asset loader. And so if you say assets equals local, it will run and replace the CSS and JavaScript.
So it's pulled from your local server. So that way you can just do all your development locally. You don't need to keep uploading crap left and right.
So like if I open this, it just needs to be at the URL endpoint, which I have included some instructions in the task.
So it's really nice. Once you do upload the assets, Engaging Networks has like a 15 minute cache lifetime. If you wanted to force Engaging Networks to load the most recent assets, you can do assets equals flush, which just appends an arbitrary URL argument, or sorry, an arbitrary number to the end of the string path and that forces it to be the latest assets.

[~@9:54~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=594.8) - **MichaelW**
Yep, Going back to here, when you, oh.

[~@10:00~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=600.0) - **Bryan Casler (he/him)**
load assets local. You see all the hidden fields and this debugger. If you don't see that, you can then also say debug equals false, which will turn it off.
This debugger stays open until you close it. It's just cookie didn't here. As an example, one of the cool things about the debugger and this only shows up when you're also loading assets local is this branding HTML.
This may or may not be useful for you, but if you click it, it copied in a bunch of markup.
Some of this is outdated, but it basically copies in a bunch of markup so you can just see how different things are being styled.
Like right now, we can tell checkboxes and radio selects aren't being styled, but these things are, sorry, yeah, the native checkboxes and radio selects aren't being so you know, your mileage may vary.
would probably just build out the page and then theme that if it were me. But, let's say you close this out, sorry, end bug, and then refresh the page.
You won't even get that. The very last thing is, let's say, because when debug mode is on, you get a bunch of helpful console logs.
If you do want the logs, but not the debug interface, you can just do debug log. And, like, we see we already got something going on here, but.
Then you get the full output of everything. That's it. So that's everything on my end that I just wanted to share and debrief with you.
Steph, do you have anything to add to all of this?

[~@11:45~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=705.12) - **Stef Jones (4Site Studios)**
I mean, that's pretty much everything that needs to happen. Just be sure that you're matching the branding and everything from their current pages, which is not, we didn't design those.
It looks like they're kind of. on an Eingrid Shell, though. I've seen Eingrid code in the templates that Monbilt, but that's the styling we need.
So really love on Donate to Oceana, that it's got that image and Donate to Oceana kind of above that.
But if there's any questions with that, we can ask Angie if she wants a design change, if something isn't fitting correctly in how you're laying it out, like that's about it.

[~@12:26~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=746.98) - **Bryan Casler (he/him)**
Yeah, I should add. So the reason their pages look like they're built on Eingrid is because they kind of are.
So the Breein flexible templates, which are the templates we designed and developed for engaging Oce, are just Eingrid without a client theme.
So it's like a dumb down version of it. So yeah, some of it might be applicable. You might just be able to like copy their styles wholesale, paste it in there and be like, it's good to go.

[~@12:54~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=774.88) - **Stef Jones (4Site Studios)**
I always wondered about that. So with engaging networks, Because I do think a lot of people do use that the templates we created are those like up to date or like are we constantly adding anything to that?
Or is it like this template and it does, you know, the bare minimum, but it has like the different column properties and things you can update it and kind of retrofit any of our stuff.

[~@13:20~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=800.68) - **Bryan Casler (he/him)**
The answer is no, we're not constantly updating it. It doesn't include any JavaScript, all the cool functionality that is required for JavaScript is done there.
And then we've updated it twice since then basically. The biggest difference is the structure of the page where we take extra time to build out the 18 semantic.
columns, whereas we kind of think the funk and put those most columns in the template rather than in the page.
And basically, you are only in one column in the free and flexible templates. So it'll get the job done, but it's not necessarily future proof.
The reason we do that is that everything is compartmentalized. So in the future, we can move it to code rather than having to go page my page and move it.

[~@14:29~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=869.36) - **Stef Jones (4Site Studios)**
That's freaking awesome. I don't think we get enough credit from engaging networks on providing them with that, absolutely not, which is me off more and more than more I find out about how much we've done for them.

[~@14:43~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=883.56) - **Bryan Casler (he/him)**
Yeah, yeah, welcome to the club. Mike, will spare you more and talk. If you don't have any questions right now, feel free to share any to come up later today.

[~@14:54~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=894.2) - **MichaelW**
so the easiest thing to do is just copy and PCA. Yep.

[~@14:59~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=899.2) - **Stef Jones (4Site Studios)**
And then go from there. One last thing. Sorry. I'm sorry to throw one last thing before you finish, Mike, I'm going to send you the GTM and GA4 code to just slap in the template you're using.

[~@15:11~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=911.58) - **MichaelW**
Okay.

[~@15:12~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=912.72) - **Stef Jones (4Site Studios)**
Oh, that probably in a sub task or something.

[~@15:15~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=915.6) - **Bryan Casler (he/him)**
Mike, what when you're copying it over, one of the things you do need to move is the, we call it the give by select that's where you're selecting the credit card.
Payback, whatever it might be. You need to move over the images that are used. So engaging that reflects you just like use images from anybody's server.
But every time we create a new account, copy the image, those are already optimized. you just upload them and update the URL path.
Okay.

[~@15:46~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=946.6) - **MichaelW**
That's it. Sounds good.

[~@15:54~](https://fathom.video/share/qXdXhbvzKNdka2dF_x3yHssJFsz9sRVg?timestamp=954.44) - **Bryan Casler (he/him)**
All right. All Thank you.