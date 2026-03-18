EN Account - Marketing Tools &gt; Email Suppressions

[https://spamchecker.mailreach.co/tests/398690d6e396cabd50b5c?_gl=1*1vft8f3*_up*MQ..*_gs*MQ..&gclid=CjwKCAiAqprNBhB6EiwAMe3yhl9XsVzRASmJBrCeue589sLx6w9PvGK1EGaQItQY7D29GDRXN3lm3hoCfX8QAvD_BwE&gbraid=0AAAAABp-tfPk06j2i9pmmTUr8-MuVi7l7](https://spamchecker.mailreach.co/tests/398690d6e396cabd50b5c?_gl=11vft8f3_upMQ.._gs*MQ..&gclid=CjwKCAiAqprNBhB6EiwAMe3yhl9XsVzRASmJBrCeue589sLx6w9PvGK1EGaQItQY7D29GDRXN3lm3hoCfX8QAvD_BwE&gbraid=0AAAAABp-tfPk06j2i9pmmTUr8-MuVi7l7)

<https://us.engagingnetworks.app/index.html?ddthymfjrdrljs3zd5xb6uqkgm=n36RQimQPLV5_W5rlPit0aUeTh-ofus1EwPVj-nZHCyydtDcvXAXDcSbnJxzEj0MOb9w8kom#/emailsuppression>

- I would export and remove (keep a copy)
  - Hard-bounces from your account
  - Complaints
- Then I would export your soft bounces - take a look for spelling errors or anything eggregious that sometimes can happen.
  - I would segment these out of your best performance sends

## TEST: Email Delivarbility

All great

DNS Record Status
Source
Status
DMARC

SPF

DKIM

## Test: DMARC

All looks great: <https://cln.sh/NKQtvkB1>

## Test 2: Ran audit on domain: clf.org

<https://cln.sh/nzNxHtms>

Results:

- SOA Serial Number Format is Invalid -
  - We will issue a warning if your serial is either invalid by being outside of the allowed range or if it does not conform to this format.

It means the domain’s SOA serial number is malformed, which can break or delay DNS updates, but it does **not**directly block email; it can indirectly cause issues if DNS changes are not propagating correctly.

Here is what is going on in plain language.

The page is flagging the **“DNS SOA Serial Number Format”** problem. Every DNS zone has an SOA (Start of Authority) record. One of the fields in that record is the **serial number**, which is just a 32‑bit integer that should be between 1 and 4,294,967,295. Name servers use this number to decide when there is a newer version of the zone. When you change DNS, you are supposed to bump that number so secondaries know to pull the new data.

MXToolbox is warning that the SOA serial number for this domain is either:

- Outside the valid range (less than 1 or greater than 4,294,967,295), or
- Not in the expected “date-based” format (YYYYmmddss), which is a common convention.

In practice, many DNS providers use the date format so humans can read it, but DNS itself does not require that format. What DNS does require is that the serial be a valid 32‑bit unsigned integer and that it increase when the zone changes.

For your email domain, the implications are:

1. If the serial is truly invalid (for example 0 or something bigger than allowed), some secondary DNS servers may refuse to transfer the zone, or think it never updates. That can mean:
   - MX records or other DNS changes you make do not propagate correctly.
   - Remote mail servers might see stale or missing MX records, SPF records, or other DNS data.
2. If the serial is valid but just not in the “YYYYmmddss” pattern, MXToolbox will still complain, but operationally email can work fine as long as:
   - The serial increases when changes are made.
   - All authoritative name servers are in sync.

So from an email perspective:

- It is **not a direct deliverability blocker** like a bad MX or missing SPF/DMARC.
- It **is a hygiene/configuration issue** that can cause subtle, hard‑to‑diagnose issues if DNS changes are not being picked up by all name servers.

How I’d approach fixing / evaluating risk:

1. Look up the SOA for the domain with `dig` or your DNS host’s UI and note the serial number.
2. Confirm that:
   - It is a positive integer in range.
   - All authoritative name servers for the domain show the same serial.
3. If it is invalid or stuck:
   - Update it to a proper date‑style serial like `2026030301` in your DNS management interface, or
   - If your provider manages it automatically, open a ticket and reference the SOA serial warning.
4. After fixing, re‑run the MXToolbox test to confirm the warning clears, then verify that MX, SPF, DKIM, and DMARC records are all still intact.

Recap: This error is telling you “the zone’s version number is not in a good shape.” It is primarily a DNS zone‑management issue. It can indirectly affect email if DNS changes to MX/SPF/etc. are not reliably propagating, so it is worth cleaning up, but it is not on its own proof that email for the domain is broken.