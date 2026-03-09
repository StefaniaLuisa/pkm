
---

### GA4/GTM Notes: - Sunday, April 6 #NWF #GA4 #GTM

So many events are firing twice: <https://cln.sh/vWmG7YLR>

UA Tags need to be removed! Asap!

Events are duplicating <https://cln.sh/9z6c4Lsc>

- To fix this, I would recommend turning this on: Ignore duplicate instances of on-page configuration (recommended) under Tag Details

- Configure domains correctly: <https://cln.sh/9nPcm5pF>

  - Property settings &gt; Property Data collection and modifications &gt; Data streams &gt; Configure Tag Settings

  - Important Note: “Your tag is sending data to multiple destinations. Changes to your Google tag will affect all connected destinations.”

    **Dismiss[Learn more](https://support.google.com/tagmanager/answer/12002338#Destination)**

**Active Tags:**

GA4 Destination: G-RLRJ1GMJC2 **(“NB - NWF Holistic (All Subdomains) - GA4” This is the correct account )**

GA4 Destination: G-LHOLDCZBST - **No idea**

GA4 Destination: G-5X1JRMQ1TX - **Ranger Rick**

UA Account: G-NXP8DRT4NM

UA GTM: UA-119708728-1

Main Tag Container: GTM-KF8N

### **Unique Main Domains:**

<https://nwf.org/>

<https://www.shopnwf.org/> - this should be a seperate property under NWF in GA4

<https://nwfactionfund.org/>

### Subdomains:

[mayorsmonarchportal.nwf.org](http://mayorsmonarchportal.nwf.org) - Mayor’s Monarch Pledge

[support.nwf.org](http://support.nwf.org) - Donation forms

<https://support.nwfactionfund.org/page/79875/action/1> - Petition/NWF Action Fund

<https://legacy.nwf.org/> - Estate Planning

[keepitpublic.nwf.org](http://keepitpublic.nwf.org) - <https://keepitpublic.nwf.org/2019/01/how-the-shutdown-impacts-national-parks-wildlife/> Seems like a miscrosite not sure where it is being hosted

---

EN Page Template Name

## NWF - GA4 - Task to track 4Site Template - en_page_template_name

Productive Task:[ Troubleshoot into Looker Studio Report](https://app.productive.io/2650-4site-interactive-studios-inc/tasks/11584103)

**This is setup really weird and more confusing than it needs to be**

### **Issues I ran into:**

They need to[ add their subdomain](https://cln.sh/PGy6prqN)s their GA4 account setup for proper tracking:

Adding Subdomains here: <https://cln.sh/q9jHH1Jm>

They are still running tags for UA and a GTM tag that looks like it is was setup for UA - <https://cln.sh/ggm8Kltc>

## Current Setup To Track 4Site Template Name

### In GA4:

**Event Created:** en_page_template_name : <https://cln.sh/l1d89FL1>

**Custom Dimension also created:** EN Page Template Name —— Parameter = en_page_template_name

<https://cln.sh/7f53gWdv>

### In GTM

- EN - Page Template - DataLayer Variable = [enPageTemplateName](https://cln.sh/YzhFQk7d)

Attached to:

- [EN - Has Page Template Name](https://cln.sh/BJvvffMh) (Trigger)

---

Recommend to Delete - Not doing anything :

### Trigger Configuration: [EN - Has Page Template Name](https://cln.sh/BJvvffMh)

**Trigger Type** = Page View

**This trigger fires on**= *EN - Page Template Name* **matches** *RegEx.+*

**References to this Trigger:**

- *EN - Record Page Template Name as GA4 Event (Tag)*

---

Recommend to Delete - Not doing anything :

### Tag Configuration: [EN - Record Page Template Name as GA4 Event](https://cln.sh/4dvY6rdN)

**Event Name:** en_page_template_name

<table>
<tbody><tr><td colspan="1" rowspan="1"><p><strong>Parameter</strong></p></td><td colspan="1" rowspan="1"><p><strong>Value</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p>Page Template Name</p></td><td colspan="1" rowspan="1"><p>{{EN - Page Template Name}}</p></td></tr></tbody>
</table>

Triggering on

- **EN - Has Page Template Name Page View (this is the Regex+)**

---

# New Setup

New Event in GA4 = EN_PAGE_VIEW

Custom Definition Update in GA4 = <https://cln.sh/ZZVn3Zsf>

Created New Tag in GTM = [[4Site] EN_PAGE_VIEW](https://cln.sh/BKL9kxPm)

**Event Name:** EN_PAGE_VIEW

<table>
<tbody><tr><td colspan="1" rowspan="1"><p><strong>Parameter</strong></p></td><td colspan="1" rowspan="1"><p><strong>Value</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p>EN - Page Template Name</p></td><td colspan="1" rowspan="1"><p>{{EN - Page Template Name}}</p></td></tr></tbody>
</table>

Trigger On = All [Page Views](https://cln.sh/cHMxFR4D)

Recommendation for GTM: <https://cln.sh/yHbJsnmz>

Custom Definition Update = <https://cln.sh/ZZVn3Zsf>