
FWW was having issues with their digital wallets not showing up on Desktop, and not showing up for FWA. 

Fernando Recommend making sure they have whitelisted their domains

## How to whitelist Domains in Stripe Account:

In Stripe, whitelist domains by adding them under Payment method domains and verifying them.

- In the Stripe Dashboard, go to **Payments: Payment method domains**. Take note of what “mode” you are on, you will need to make sure the domains are added for both “test” and “live” mode to work properly. ([See how to tell here](https://cln.sh/V8W8kR7g))
- Click **Add a new domain**. Enter the root domain only (example: [**example.org**](http://example.org)). Do not include protocol (https://) or paths (/donate). Add each subdomain separately if you use them (e.g., [**donate.example.org**](http://donate.example.org)). Wildcards aren’t supported (*)
- Domains here allow payment methods in **Elements** that require domain registration: **Apple Pay, Google Pay, Link, PayPal, Amazon Pay, Klarna**. Stripe uses this to authorize your site to show and use those methods.
- **Verify Apple Pay (extra step required):**
  1. After adding the domain, download the **Apple verification file** from Stripe.
  2. Host it at this exact path on your site: **/.well-known/apple-developer-merchantid-domain-association** (no redirects).
  3. Ensure it’s publicly accessible over HTTPS, then click **Verify** in Stripe. Status should turn **Enabled**.
- **Google Pay, Link, PayPal, Amazon Pay, Klarna:**
  - No file placement is typically required. Ensure your Elements integration loads on the added domain and that the domain is reachable over HTTPS. Stripe will mark the domain **Enabled** when checks pass.
- **Common gotchas to avoid:**
  - Make sure you are adding all domains and subdomains to both **Live** and **Test** modes. 
    - For example, if the site is [**www.nonprofit.org**](http://www.nonprofit.org) but donations run at [**donate.nonprofit.org**](http://donate.nonprofit.org) 
    - Add **every subdomain** you’ll use Elements on; adding the root (.[nonprofit.org](http://nonprofit.org)) doesn’t cover subdomains.
    - Don’t include protocol or paths (https://). Add [**nonprofit.org**](http://nonprofit.org) or [**donate.nonprofit.org**](http://donate.nonprofit.org), not <https://nonprofit.org/donate>.

Dev heavy info if helpful

- Serve over **HTTPS** and avoid redirects for the Apple file.
- If you use a headless CMS or proxy/CDN, confirm the verification file is served by your checkout domain, not just the CMS domain.


- **Optional via API (Apple Pay domains):** You can register Apple Pay domains programmatically after hosting the verification file. - this would be something Killian would do or us if provided the access. 

## [Domains & IP Address](https://docs.stripe.com/ips#stripe-domains)

Here is how that is done through the API (more technical)

Whitelist Your Domain for Stripe Integration

Here's a step-by-step guide to whitelist your domain for use with Stripe:

For API Communication

1. Identify which Stripe domains need to be whitelisted:

   - Check the [**list of Stripe domains**](https://docs.stripe.com/ips#stripe-domains) needed for your integration
   - Common domains include `api.stripe.com`, `js.stripe.com`, and `checkout.stripe.com`

2. Access your firewall or network security settings:

   - Log into your server, hosting provider, or network administration panel
   - Navigate to the security settings, allowlist, or firewall configuration

3. Add Stripe domains to your allowlist:

   - Add all required Stripe domains
   - Ensure you include all subdomains listed in the Stripe documentation
   - Don't block any of the fully qualified domain names used by Stripe

For Payment Methods

1. Register your domain with Stripe:

   - Go to the [**Payment method domains page**](https://dashboard.stripe.com/settings/payment_method_domains) in your Stripe Dashboard
   - Click **Add a new domain**
   - Enter your domain name (e.g., example.com)
   - Click **Save and continue**

2. Register all necessary domains and subdomains:

   - Repeat the process for all subdomains (e.g., www.example.com, shop.example.com)
   - Remember to register domains for both testing and production environments

3. For local testing:

   - Use a tool like [**ngrok**](https://ngrok.com/) to get an HTTPS domain
   - Register this temporary domain in your Stripe Dashboard

For Custom Email Domain (Optional)

1. Add your domain in the Stripe Dashboard:

   - Navigate to [**Customer email**](https://dashboard.stripe.com/settings/emails) settings
   - Add the domain you want to send customer emails from

2. Verify your domain:

   - Configure DNS records as provided in the Dashboard
   - Add the TXT and CNAME records to your DNS provider
   - Wait up to 72 hours for verification to complete

3. Set up a DMARC policy for your domain:

   - Create a TXT record with name `_dmarc`
   - Use a value like `v=DMARC1; p=none; rua=mailto:report@example.com`

For Custom Checkout Domains (Optional)

1. Add a custom domain for Checkout:
   - Go to [**Dashboard settings**](https://dashboard.stripe.com/settings/custom-domains) for custom domains
   - Follow the instructions to set up your custom subdomain for Checkout pages

Remember to test your configuration after completing these steps to ensure everything works correctly.