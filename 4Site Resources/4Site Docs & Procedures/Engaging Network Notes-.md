# Engaging Network Notes:

#4Site #engaingnetworks 

This is to be a repository of notes on EN oddities or processes. Mostly documentation of the convos that happen in the EN Slack channels and Bryan provides his insight because he is brilliant! 

——————————————————————————————--------------

## 12.11.23 Regarding Stripe gateway update: 
 [https://4site.slack.com/archives/C02G2293F5W/p1702321234648399](https://4site.slack.com/archives/C02G2293F5W/p1702321234648399)
**Marcie Lenaghan - EN Rep**
Happy Monday! 
 Has anyone used the Stripe gateway update where mobile wallet data should be pulled into the users Supporter Record automatically? If you've tested this on a live page, please let me know. Thanks! (edited) 

**Bryan Casler**
I thought everyone was when the product update was made. We have done a bunch of testing and have a few related support tickets. Anything in particular you’re looking for? (edited) 
looking for? (edited) 

**Marcie Lenaghan** 
Yes, sorry -- poor wording on my part! I meant more like has anyone rearranged the donor experience to be able to test the update. I just want to see if anyone has had any issues with it, or if it's functioning as expected. I know you had said you ran into some problems with it, so I wanted to see if anyone else was experiencing similar trouble.

**Bryan Casler**
Challenges so far
* 		Default selection on forms (e.g. selecting country based on IP address) getting blended when other fields are left blank and more address details are returned from Stripe
* 		Phone numbers not pulling in ( we’re still working through this one )
* 		And Digital Wallets returning address data that the client does not want in their database because they have an expectation of what X might be in Y field (e.g. Region). This is mostly related to systems syncing data to external databases. And they no longer have control over what that data could be.
(edited)

**Marcie Lenaghan** 
My understanding from Marta is that these have been (or are being) addressed 


——————————————————————————————--------------

### [REST API to submit a page in EN](https://4site.slack.com/archives/C02G2293F5W/p1702312034510329): 12.11.23
**John Siemiatkoski - EN Guy** 
Can anyone share an example of a client page using the EN REST API to submit the page?
**Bryan Casler**
[@John](https://4site.slack.com/team/UB18E9XMG)
 Email signup form in the footer: [https://oceanconservancy.org/](https://oceanconservancy.org/)
It submits to a service we set up ( to keep a static IP)  that then submits via the rest api
Same for the inline email sign up forms you see on their blogs: [https://oceanconservancy.org/blog/2023/12/07/what-sand-dune/](https://oceanconservancy.org/blog/2023/12/07/what-sand-dune/)

——————————————————————————————--------------

### Donation amount passing through cookie or custom supporter field

**Ryan Baillargeon**
  [11:34 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402488467309)
Quick Q - our client has a multi-page donation form - and they select the donation amount on the first page. How can I present the selected amount on page 3 of the form in a summary. The donation amount isn’t in pagejson at this point - and I can’t add Donation Amount through a hidden field - as its on the first page already. I feel like there is an easy answer I’m missing. 
[@alex](https://4site.slack.com/team/UBRBM6H0V)

**Bryan Casler**
  [11:36 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402573064649)
Cookie or a custom supporter field you then reference as a merge tag

**GT**
**glyn**
  [11:38 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402691295239)

**Ryan Baillargeon**
  [11:40 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402840634959)
Thank you 
[@glyn](https://4site.slack.com/team/U02QC9X6W3V)
 - that worked!

**Ryan Baillargeon**
  [11:41 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402886228209)
i should have scrolled down that support page further - amount-total isn’t in the insert tool -

**Ryan Baillargeon**
  [11:41 AM](https://4site.slack.com/archives/C02G2293F5W/p1702402911037719)
and I’ve really only built mutli-step forms with javascript - not pages. ! thanks.

**Bryan Casler**
  [11:46 AM](https://4site.slack.com/archives/C02G2293F5W/p1702403184419969)
Damn, I’m so scorn I didn’t even think of that

**Michael Thomas**
  [11:47 AM](https://4site.slack.com/archives/C02G2293F5W/p1702403238942739?thread_ts=1702402886.228209&cid=C02G2293F5W)
replied to a thread:
**i should have scrolled down that support page further - amount-total isn’t in the insert tool -**

——————————————————————————————--------------


 



