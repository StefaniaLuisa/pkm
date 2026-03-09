
<https://us.dmarcian.com/domain-overview/>

## DMARC

- [x] **DMARC Inspector is Valid - with recommendations**

> DNS Query
>
> _[dmarc.ran.org](http://dmarc.ran.org)
>
> Record
>
> `v=DMARC1; p=none; rua=mailto:dmarc_agg@vali.email,mailto:7e2e779f13ec471fbfa57ae1ad62e9f3@dmarc-reports.cloudflare.net`

### DMARC Inspector Improvements

DMARC record is currently setup under both "[ran.org](http://ran.org)" and "_[dmarc.ran.org](http://dmarc.ran.org)". The DMARC record at "[ran.org](http://ran.org)" should be removed.

- DMARC record "p" tag is set to "none", which does not prevent abuse on your domain.
  - The policy that will be applied to emails that fail DMARC. Acceptable values are: “none”, “quarantine”, or “reject”.
  - "none" is used to collect reports without impacting email flow.
  - “quarantine” informs receivers (Yahoo, Gmail, etc.) to treat email that fails DMARC as suspicious (deliver to spam folder).
  - “reject” informs receivers to reject any email that fail DMARC.

- [x] **DMARC Validator - Passed**

- [x] **SPF - Record is valid - Passed**

> **SPF Record**
> ****v=spf1 include:%{i}._ip.%{h}.ehlo.%{d}.[spf.vali.email](http://spf.vali.email) \~all**

- [x] **DMARC Issues: [ran.org](http://ran.org)**

> **WARNING**A DMARC record was detected under`ran.org`. DMARC records must be located at`_dmarc.ran.org`: and not directly at`ran.org`. If DMARC was set up as a wildcard record, that should be removed and placed only at the domain level.

## Domain Overview - DMARCIAN

- Your domain has a DMARC record. The next step is to add your account's reporting address for dmarcian to that record.

  **Your current record:**`v=DMARC1; p=none; rua=mailto:dmarc_agg@vali.email,mailto:7e2e779f13ec471fbfa57ae1ad62e9f3@dmarc-reports.cloudflare.net`

#### How do I update my DMARC record?

You'll need access to your domain's DNS. Then you need to update the existing TXT Record at the Location/Target provided below.

##### TXT Record to Update in DNS

`v=DMARC1; p=none; rua=mailto:ghzteq6t@ag.us.dmarcian.com, mailto:dmarc_agg@vali.email,mailto:7e2e779f13ec471fbfa57ae1ad62e9f3@dmarc-reports.cloudflare.net;`

##### Location/Target

`_dmarc`

- So that the record is created at `_dmarc.ran.org`

#### 

## TLS & MTA-STS Inspector

- [ ] TLS Recrod - None found

- [ ] MTA-STS Record - Not found

- [ ] MTA STS Policy - Not found

  Increase email security with MTA-STS and TLS reporting

  <https://support.google.com/a/answer/9261504?hl=en>

## SMPT

Connecting to 141.193.213.10 - this is DNS Record IP Address

6/9/2025 4:34:54 PM Connection attempt #1 - Unable to connect after 15 seconds. [15.01 sec]

- LookupServer [smtp:[ran.org](http://ran.org)] 15005ms

## SPF Surveyor

- [x] SPF Record Valid

> v=spf1 include:%{i}._ip.%{h}.*ehlo.%{d}.*[spf.vali.email](http://spf.vali.email) \~all

## DKIM

- [x] DKIM Record Valid -[ Troubleshoot DKIM Issues](https://support.google.com/a/answer/11612790?sjid=17825932167043976241-NC#setup)

[ran.org](http://ran.org) | Google

google._[domainkey.ran.org](http://domainkey.ran.org)

`v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAuW4Uq9noTm2OYdEEfGkGaWMaRc4osVc2LYzWeRP/YmA8iEeKfB4LEadh73KAQjedKBNBkUVTYJ7wi/Hf8EkYTnTPN4XSJGIoYNv9P3Q/lu0EKPMYATPF9Nmhb7QdPMF5qz8W6UaiqAPfiAiH4KtvyherQdh/WbcPMTyf1ZQCk+j+Da7aSCd1B6Zn0xlteQHZksAXaMCX+NdfhmF2QtTSjzKfAXTAOABE9AMqcbVB9jGokXKBYGlBlucJywu3chWo2y18/QJFzHNAsU4XawIgwoILf4PzPP4p0yhboYQ3YVXd7t5TZcK7lu2UQVzaEivhloyyKajGKue4bvxpbn6LFwIDAQAB`

## *Error*

Domain must have at least one mail server.

[*help_outline*](https://support.google.com/a/answer/174125)

[Help center article](https://support.google.com/a/answer/174125)

*warning*

DKIM is not set up.

[*help_outline*](https://support.google.com/a/answer/174124)

[Help center article](https://support.google.com/a/answer/174124)

*warning*

DMARC is not set up.

[*help_outline*](https://support.google.com/a/answer/2466580)

[Help center article](https://support.google.com/a/answer/2466580)

*warning*

MTA-STS DNS Record.

---

## Google Admin Toolbox

### Check MX:

**he Google Workspace MX record value is** `smtp.google.com`.

### <https://toolbox.googleapps.com/apps/checkmx/check?domain=ran.org&dkim_selector=>

### **Set up MX records for Google Workspace**

<https://support.google.com/a/answer/16004259?visit_id=638850947299904171-1971580508&rd=1>

### Set up DKIM

<https://support.google.com/a/answer/174124>

### Set up DMARC

<https://support.google.com/a/answer/2466580>

---

Email Domains being used in EN account

[info@ran.org](mailto:info@ran.org)

[membership@ran.org](mailto:membership@ran.org)

[donoralerts@ran.org](mailto:donoralerts@ran.org)

[organizing@ran.org](mailto:organizing@ran.org)

[organizinghelp@ran.org](mailto:organizinghelp@ran.org)

[events@ran.org](mailto:events@ran.org)

MX Toolbox

MX Audit: <https://mxtoolbox.com/SuperTool.aspx?action=mx:ran.org&run=toolpage>

<https://cln.sh/w7y7XmCy>

<https://cln.sh/PbPJ6tjX>

Issue:

Test:

DMARC Policy Not Enabled Result
Result:

DMARC Quarantine/Reject policy not enabled

DMARC Policy details: More Information About Dmarc Policy Not Enabled

This Warning indicates that the DMARC record for this domain is not currently protected against phishing and spoofing threats. To resolve this Warning you will need to set a Quarantine or Reject policy on the domain's DMARC record. Setting a Quarantine or Reject value will prevent fraudsters from spoofing the domain as mail servers will Quarantine or Reject messages that fail authentication tests.

*Note: It is advised to not set a Quarantine or Reject policy until you have evaluated your DMARC reports to make sure you don't have any legitimate senders that have email delivery problems.

### DMARC Email Delivery Reporting

**Monitor, detect and fix real world problems with your SPF and DKIM configuration**