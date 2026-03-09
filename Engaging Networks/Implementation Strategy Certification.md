
Onboarding Timeline Template: <https://import.cdn.thinkific.com/475908/courses/1342889/1039391_NewonboardingGanttchart_v2_2_041621-210428-143647.jpg>

### **Intro | Client Motivation**

Request an Engaging Networks demo for a client at <https://www.engagingnetworks.net/demo-request/>

Our main company website with information about our products is at <https://engagingnetworks.net>

Our support site containing in depth articles about our product is at <https://engagingnetworks.support>

Transcript: [Product Use Cases & Benefits](https://files.cdn.thinkific.com/file_uploads/475908/attachments/d0f/607/59e/1-clientmotivation-210428-134308.mp3.txt)

### Domains & SSL Certificates

**General process for clients setting up subdomains** 

1. Clients will need to provide us with the domain(s) and the intended usage (page builder/P2P)
   1. The client needs to provide EN with the subdomain they want their forms to point to - recommend using a different subdomain for donation/advocacy/p2p/events.
   2. ie. [event.4Site.com](http://event.4Site.com) [give.4site.com](http://give.4site.com) [action.4Site.com](http://action.4Site.com), etc.
2. Engaging Networks will assign the subdomains in Cloudflare
3. Clients  will add DNS records to their top level domain as below:
   [subdomain.theirdomain.org](http://subdomain.theirdomain.org)   CNAME   [ca.engagingnetworks.app](http://ca.engagingnetworks.app) (for Canada data centre)
   [subdomain.theirdomain.org](http://subdomain.theirdomain.org)   CNAME   [us.engagingnetworks.app](http://us.engagingnetworks.app) (for US data center)

There are some exceptions to this.  For clients that require a wildcard, or for peer to peer pages and sites the domains we point to are slightly different. In these instances, clients and agencies should reach out to their account manager or our support team for specific instructions

Once the client’s domain and SSL is set up it should be used as a Base URL in Engaging Networks pages. You can set this as a default under Account Preferences or amend individual page admin settings.

Transcript: [Domains & SSL Certificates](https://files.cdn.thinkific.com/file_uploads/475908/attachments/bcf/44f/fe3/3-domainsonlyedit-210428-144559.mp3.txt)