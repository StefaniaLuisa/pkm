- I wanted to share something that’s been weighing on me. We do a lot of work with progressive and DEI‑focused clients, and we talk about values a lot. With everything happening right now, it feels strange that we haven’t acknowledged it at all internally. For folks who are directly affected, that silence can feel pretty heavy.

This page is flagging that NWF’s GA4 implementation is driving a lot of volume, but the *governance* and UTM hygiene need work. In other words, the data is usable, but it is not clean or standardized enough yet for confident channel reporting and deeper analysis.

Here is what the dashboard is telling the client in plain language:

First, they have a very high number of total sessions (3.5M+ in the selected period), concentrated in a few core mediums like ‎⁠organic⁠, ‎⁠(none)⁠ (direct), ‎⁠email⁠, ‎⁠referral⁠, and ‎⁠paidsocial⁠. That is healthy and expected. However, there are also nonstandard and mes

sy mediums in the mix, such as ‎⁠null⁠, ‎⁠52515109619930⁠, and ‎⁠(not set)⁠. Those values indicate tracking or UTM issues, not legitimate marketing channels. When those appear as mediums, GA4 cannot reliably group them into default channel groupings, which leads to **“Unassigned”** traffic at the channel level and weakens any channel-based performance reporting.

Second, the account is using a *lot* of distinct session mediums (265 rows in the “How many mediums do you have?” table). Most sites should realistically sit in the 10–20 range of mediums (organic, email, cpc, social, etc.). Having hundreds implies that:

- Teams and/or vendors are inventing one-off mediums instead of using a controlled list (for example, using ‎⁠newsletter⁠ versus ‎⁠email⁠, or custom numeric values).
- Some platforms (like Engaging Networks or ad platforms) may be auto-populating UTMs in inconsistent ways.
- There is no enforced UTM taxonomy or automated normalization layer to collapse these into clean buckets.

Third, there are case sensitivity and naming consistency problems in sources and mediums. The dashboard explicitly calls out that GA treats ‎⁠Facebook_Mobile_Feed⁠ and ‎⁠facebook_mobile_feed⁠ as two different values. In the tables, you can see variants like ‎⁠fb⁠ versus ‎⁠Facebook_*⁠ for the same underlying source. That fragmentation means social traffic that should roll up under a single “Facebook” or “Paid social” line is being split across multiple rows, again making reporting noisier and less trustworthy.

Fourth, paid social tracking exists but is not fully normalized. There is a clear ‎⁠paidsocial⁠ medium in use, and multiple Facebook / Instagram placements are tagged correctly with it. That is good. At the same time, you see those same placements paired with the odd ‎⁠52515109619930⁠ medium and other nonstandard values. That suggests that some campaigns, placements, or auto-tagged links are not following the agreed tagging pattern. As a result, some paid social sessions will be correctly grouped under the Paid Social channel, while others may be ending up in “Unassigned” or “Other.”

Finally, there are early warning signs around “Unassigned” channel traffic and ‎⁠(not set)⁠ / ‎⁠null⁠ values that point to two broad configuration gaps: GA4 channel grouping and upstream tagging. When the dashboard asks “How many sessions are ‘Unassigned’?” and shows ‎⁠null⁠, ‎⁠(not set)⁠, and odd mediums in the same view, it is highlighting that some traffic cannot be mapped cleanly to GA4’s default channel groupings. That can come from:

- Missing or malformed UTMs (for example, a ‎⁠source⁠ or ‎⁠medium⁠ that does not match GA4’s default rules).
- Inconsistent capitalization or naming (for example, ‎⁠Newsletter⁠ instead of ‎⁠email⁠).
- Custom values that are not reflected in custom channel group definitions.

Taken together, the story you can tell the client is:

- Volume is strong and the core sources/mediums are present, which means GA4 is generally collecting data as expected.
- However, the current UTM and source/medium conventions are inconsistent and overly fragmented, which is causing data to split across many mediums, generate “Unassigned” traffic, and prevent clean channel-level reporting.
- To get to reliable, board-ready insights, they need a tighter UTM taxonomy, lowercase-only standards, and aligned GA4 channel group rules (or custom channels) so that all this traffic rolls up into a small, meaningful set of channels and mediums.