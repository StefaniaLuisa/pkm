---
NWF

---

---

# NWF

## **Thursday, February 12 Work**

### **NWF.org GTM Updates**

- Consent Management is now on

- I updated the custom variable - [it is no longer a lookup table](https://cln.sh/SBdWk0pg), it is now much more reliable. Also, since I just updated the config of this variable, no other updates to the [connected tags need to be made. ](https://cln.sh/GZmSc09c)already in use custom variable no other updates to the connected tags need to be made.

- Updated [GA4 Configuration](https://cln.sh/MGVz309d) Tag. I have configured it for consent (which is important to do on your other tags) and updated the trigger - this will make sure the connection fires immediately upon page entry.

Cookie Consent is now functioning as expected on the NWF.org site & EN forms:

- Confirming that when a new visitor or new browser session has visited the NWF Website that all cookies are set to “granted” it is not until the visitor updates these consent options do they deny tracking.

  - [Cookies upon visit - Banner showing ](https://cln.sh/2Ph0t2T6)- All Cookies are being tracked and data is passing into GA4

  - To test I turned off:

    - [Performance Cookies turned off](https://cln.sh/qH2fhKSD) = https://cln.sh/3WDtpZLz

    - [Opting out of targeting cookies](https://cln.sh/5yKT2F4N) =<https://cln.sh/0xx50kcm>

    - Functional Cookies turned off, opted out of all consent options = <https://cln.sh/HZswxgBl> (Please note that security storage cookie was not opted out of - this is considered a necessary cookie - so no issue there)

Please review - noted issues I ran into:

- [NWF.org - Triple Tracking ](https://cln.sh/PkXcbGZW)Issue

  - [These depreciated tags ](https://cln.sh/1PKhQdW8)need to be removed from nwf.org & your EN forms

---

# Ranger Rick

1. GA4 Settings
   1. Updated the Enhanced Measurement
   2. Updated Monitored Domains
      1. [rangerrick.com](http://rangerrick.com)
      2. [rangerrick.org](http://rangerrick.org)
      3. [www.rangerrick.org](http://www.rangerrick.org)