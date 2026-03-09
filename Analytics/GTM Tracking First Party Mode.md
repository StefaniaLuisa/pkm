
> ==🔵Tuesday, February 25==

## Sharing info on First Party Mode GA4 Article

Kinda recent news for GA4, there is now another option in how to setup tracking - "First Party Mode" (FPM), it's kinda like server-side set up lite :) and would be most helpful to clients who want to have a bit more data control and privacy but don't want to go through the full server-side setup hassle and on-going management. Here is the article - which really breaks it down well, but to make sure I really understand it, I wanted to share my own summary:

First-Party Mode is a data and privacy-focused deployment of Google tags. Instead of sending the users' data directly to Google’s servers, First-Party Mode setup routes the data directly to the website’s domain instead. The website’s infrastructure handles all requests before forwarding data to Google, this can be implemented through DNS or CDN - works by setting up a CNAME record in the DNS, which makes requests appear as if they came from the site’s domain rather than Google’s.

First-Party Mode improves tracking reliability by making Google Analytics requests appear as first-party traffic instead of third-party requests. This helps lessen the impact of ad blockers, browser privacy settings, and tracking restrictions that usually block or limit standard Google Tag Manager (GTM) tracking. Some are setup to block Google’s domains.

FPM allows for “IP obfuscation” (fun word) and overall greater control over data collection and reduces the reliance on third-party domains, enhancing data privacy overall.

As far as setup is concerned, FPM is supposedly easier - it entails configuring DNS settings to route Google tag requests through the client owned domain - the popular option seems to be using a CDN like Cloudflare, but important to note that a CDN is not required - that the FPM setup is based around updating or adding rather, a CNAME record, which can be done through a site's DNS.

Now, what are the different all the different setup options, you ask?
-Standard Client-Side Setup (Default): Your webpage loads the Google tag from a Google-owned domain (e.g., [www.googletagmanager.com](http://www.googletagmanager.com)), and tracking data is sent directly to Google’s servers.
-First-Party Mode Setup: Instead of loading Google tags directly from Google's domains, your website first processes the requests through its own domain (configured via DNS or a CDN). Data still gets to Google, but this setup allows modifications before it reaches their servers—such as “IP obfuscation” and other data modifications( which so far I have found that you can setup stripping specific URL parameters and applying custom anonymization rules…tbd on what other mods are available).
-Server-Side Setup: In a server-side setup, data is collected through a dedicated GTM Server container, hosted on a cloud platform ( Google Cloud, AWS, or some other hosting services). The server processes the data before forwarding it to Google Analytics, Facebook, or other marketing platforms.

Limitations - pretty big ones for our charity clients:
Only works on the main domain - subdomains are not tracked!!
It is still technically client-side tracking, requests are routed through the domain, but tracking is still done in the browser - This means ad blockers, Safari’s ITP, and other privacy settings can still interfere with data collection.

So, would this work for any of our clients?
Clients who only need GA4 tracking on one domain, want a low-maintenance way to improve tracking reliability, so they don’t have to worry about having the technical resources to manage a cloud server.
Would make most sense for foundations like Stupski, FPF (if they would ever approve GA4), Gambrell, DORA
Definitely not ideal for clients who use subdomains and use one GA4/GTM account to track web visits and forms interactions

That’s all folks!