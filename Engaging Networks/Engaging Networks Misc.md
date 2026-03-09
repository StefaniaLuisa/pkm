<https://client.engagingnetworks.academy/>

<https://agency.engagingnetworks.academy/enrollments>

Supportal: <https://knowledge.engagingnetworks.net/?l=en>

## Pre-Populating Forms:

<https://knowledge.engagingnetworks.net/youraccount/pre-populating-form-fields>

Example:

[https://secure.charity.org/page/20145/donate/1?**supporter.appealCode=NY%20S-001&transaction.donationsAmt=2**](https://secure.charity.org/page/20145/donate/1?supporter.appealCode=NY%20S-001&transaction.donationsAmt=2)

<https://meyerweb.com/eric/tools/dencoder/> = **URL-encoder Tool** - turning spaces and special characters into things like `%20`, `%3A`, etc.) or take already-encoded text and convert it back into normal readable text. The author mentions it is useful, for example, for turning “encoded JavaScript URLs from complete gibberish into readable gibberish.”

### EN tagged fields & Parameters

| Tagged Field | URL Parameter (Case Sensitive) |
| --- | --- |
| Tribute Options | `transaction.trbopts` |
| Tax Deductible | `transaction.taxdeductible` |
| Shipping Title | `transaction.shiptitle` |
| Shipping Region | `transaction.shipregion` |
| Shipping Postcode | `transaction.shippostcode` |
| Shipping Notes | `transaction.shipnotes` |
| Shipping Last Name | `transaction.shiplname` |
| Shipping First Name | `transaction.shipfname` |
| Shipping Enabled | `transaction.shipenabled` |
| Shipping Email Address | `transaction.shipemail` |
| Shipping Country | `transaction.shipcountry` |
| Shipping City | `transaction.shipcity` |
| Shipping Address 2 | `transaction.shipadd2` |
| Shipping Address 1 | `transaction.shipadd1` |
| Recurring Start Date | `transaction.recurrstart` |
| Recurring Payment | `transaction.recurrpay` |
| Recurring Frequency | `transaction.recurrfreq` |
| Recurring End Date | `transaction.recurrend` |
| Recurring Day | `transaction.recurrday` |
| Recurring Count | `transaction.recurrcnt` |
| Recurring Period | `transaction.recurprd` |
| Recognize Gift | `transaction.recnzegft` |
| Payment Type | `transaction.paymenttype` |
| Payment Currency | `transaction.paycurrency` |
| In Memoriam | `transaction.inmem` |
| Inform Region | `transaction.infreg` |
| Inform Postcode | `transaction.infpostcd` |
| Inform Name | `transaction.infname` |
| Inform Email | `transaction.infemail` |
| Inform Country | `transaction.infcount` |
| Inform City | `transaction.infcity` |
| Inform Address 2 | `transaction.infadd2` |
| Inform Address 1 | `transaction.infadd1` |
| Honoree Name | `transaction.honname` |
| Gift Reason | `transaction.gftrsn` |
| Fee cover | `transaction.feeCover` |
| Donation Amount | `transaction.donationAmt` |
| Direct Gift | `transaction.dirgift` |
| Additional Comments | `transaction.comments` |
| Credit Card Expiration Date | `transaction.ccexpire` |
| Title | `supporter.title` |
| Region | `supporter.region` |
| Postcode | `supporter.postcode` |
| Phone Number | `supporter.phoneNumber` |
| Middle Name | `supporter.middleName` |
| Last Name | `supporter.lastName` |
| First Name | `supporter.firstName` |
| Email Address | `supporter.emailAddress` |
| Supporter Birthday | `supporter.dateOfBirth` |
| Card Holder Name | `supporter.creditCardHolderName` |
| Country | `supporter.country` |
| City | `supporter.city` |
| Bank Routing Transit Number | `supporter.bankRoutingNumber` |
| Bank Account Type | `supporter.bankAccountType` |
| Bank Account Number | `supporter.bankAccountNumber` |
| Appeal Code | `supporter.appealCode` |
| Anonymous Donor | `supporter.anonymousDonor` |
| Address 3 | `supporter.address3` |
| Address 2 | `supporter.address2` |
| Address 1 | `supporter.address1` |
| Credit Card Number | `Sensitive data shouldn't be passed over a URL` |
| Credit Card Verification Value | `Sensitive data shouldn't be passed over a URL` |

### **How to find other URL parameters**

To find out the name of a field, it is best to look at the HTML of the page in your browser:

Enlarges the table by opening it in a full screen dialogOpen

1. Right-click on the field or question and select Inspect

![image-20251028-164259.png|215](https://knowledge.engagingnetworks.net/__attachments/39092764/image-20251028-164259.png?inst-v=856f9ade-517f-4441-9abc-66306bb4367a)

2. Find the corresponding input tag and name attribute in the HTML

![image-20251028-170041.png|283](https://knowledge.engagingnetworks.net/__attachments/39092764/image-20251028-170041.png?inst-v=856f9ade-517f-4441-9abc-66306bb4367a)

| i. In this example`,` the name attribute for inclusion in the URL is: `supporter.questions.42761` |  |
| --- | --- |

![image-20251028-164610.png|257](https://knowledge.engagingnetworks.net/__attachments/39092764/image-20251028-164610.png?inst-v=856f9ade-517f-4441-9abc-66306bb4367a)

| ii. As this is an opt-in question*, it would be added into the query string with either a Y or N value. This could be the query string starting with`&`:<br>`https://secure.charity.org/page/20145/donate/1?supporter.appealCode=NY%20S-001&transaction.donationsAmt=20&supporter.questions.42761=N` |
| --- |

It’s not recommended to use an opt-in question as URL parameters