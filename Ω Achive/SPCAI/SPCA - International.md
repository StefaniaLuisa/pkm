
---

### Lapsed Donor List

- Pardot Export = 9, 936
  - Donor Status = Current Donor\~Lapsed Donor\~Not a Donor
- EN Export = 17,226
  - Donor Status = Lapsed Donor
- 4Site Subscriber List Export = 17229

### Active Recurring:

Donor Status = Active Recurring

- Pardot Export = 5,550
- Engaging Networks - Export = [6,250](https://cln.sh/kS42QrLZ)
- 4Site Subscriber List Export = 15,4108

### Active Audience - This is a mix of supporter records via donor status

Donor Status = Active Recurring\~Current Donor\~New Donor\~Not a Donor

- **Current Donor =** 10662
- **Active Recurring =** 5599
- **New Donor =** 4597
- **Not A Donor =** 18
- Pardot Export= **20873**

### Current Donor List

Donor Status = Current Donor

- EN Export = 11,531
- 4Site Subscriber List Export =9,067

### Inactive Donor

Donor Status = Inactive Donor

- EN Export = **41010**
- 4Site Subscriber List Export = 20359

### **NON-Opens in the last 6 months - How was this calculated**

Donor Status =Active Recurring\~Current Donor\~Inactive Donor\~Lapsed Donor\~New Donor\~Not a Donor\~Not a Donor;Not a Donor

“Pardot_2025_Non_Opens_6m_” = Count: 58,0186

---

### SPCA - Supporter List Discrepancy

- Thursday, April 24 11:20 AM

There is a discrepancy between what SalesForce (and a Pardot export) shows for the supporter list compared to what Engaging Networks is showing and SPCA International cannot get list to populate in EN the same way they are pulling into SalesForce.

Of subscriber list, have 20,000 active donors on the email list but if run that report in SF can get it to match in Pardot original export but running those same parameters in EN the numbers are way off.

Emma Kronish to provide us with:

1. Expectations for what the lists shoudl have

2. Examples of some supporters that are in one list but not the others

3. Any other data related to the discrepancy to help us troubleshoot

Related task #26 4Site Onboarding

We have 5 email segments

- Prospect - Never donated (\~200,000)
- Lapsed -12-24mo since last donation (\~20,000)
- Active - Donations made in &lt;365 days (\~20,000)
- Recurring Donor - Monthly donor (\~5,000)
- Non-Openers - Haven’t opened an email in 6+ months (\~500,000)

Our total subscriber list is in the ballpark of 800,000 but we really only actively email about 250,000-300,000 (we suppress the non-openers).

The [lists were exported from Pardot](https://spcai.box.com/s/enzxdb8r9asgyae7wvoxfecc69dv8z0k). Using their Dynamic lists we generated the segements out of the list titled 2025 Subscriber List.

Attached is a screenshot of the Active and Lapsed lists when run in Salesforce.

[[Lapsed_Donors.png]][[Active_Donors (1).png]]