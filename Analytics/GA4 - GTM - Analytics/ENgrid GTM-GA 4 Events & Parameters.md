# ENgrid GTM/GA 4 Events & Parameters

#ga4 #engrid #engaingnetworks 

his is what our ENgrid Data Layer info looks like - Might be good to add to our ENgrid documentation?
1. Create a custom variable in GTM  = 'EN_PAGEJSON_CAMPAIGNPAGEID' 
{
  event: "EN_SUBMISSION_SUCCESS_DONATION",
  gtm: {uniqueEventId: 2844},
  'EN_PAGEJSON_CLIENTID': 10089,
  eventValue: false,
  'EN_PAGEJSON_CAMPAIGNPAGEID': 61451,
  'EN_PAGEJSON_CAMPAIGNID': 134379,
  'EN_PAGEJSON_PAGENUMBER': 2,
  'EN_PAGEJSON_PAGECOUNT': 2,
  'EN_PAGEJSON_PAGENAME': "4Site - EOY 2023 - Test - 61451",
  'EN_PAGEJSON_PAGETYPE': "donation",
  'EN_PAGEJSON_LOCALE': "en-US",
  'EN_PAGEJSON_REDIRECTPRESENT': false,
  'EN_PAGEJSON_SUPPORTERID': 97399947,
  'EN_PAGEJSON_COUNTRY': "US",
  'EN_PAGEJSON_GIFTPROCESS': true,
  'EN_PAGEJSON_TRANSACTIONTYPE': "FCS",
  'EN_PAGEJSON_PAYMENTTYPE': "visa",
  'EN_PAGEJSON_AMOUNT': 5,
  'EN_PAGEJSON_CURRENCY': "USD",
  'EN_PAGEJSON_DONATIONLOGID': 14501643,
  'EN_PAGEJSON_TRANSACTIONID': "pm_1OQBUHJxOh2gvObc2kdXNTN6__cus_PEen" +
                               "SmXMAgRp8U__pi_3OQBUKJxOh2gvObc1JvjlEAM",
  'EN_PAGEJSON_RECEIPTNUMBER': 4217,
  'EN_PAGEJSON_RECURRING': false
'EN_PAGEJSON_CLIENTID': 10089,
  eventValue: false,
  'EN_PAGEJSON_CAMPAIGNPAGEID': 61451,
  'EN_PAGEJSON_CAMPAIGNID': 134379,
  'EN_PAGEJSON_PAGENUMBER': 1,
  'EN_PAGEJSON_PAGECOUNT': 2,
  'EN_PAGEJSON_PAGENAME': "4Site - EOY 2023 - Test - 61451",
  'EN_PAGEJSON_PAGETYPE': "donation",
  'EN_PAGEJSON_LOCALE': "en-US",
  'EN_PAGEJSON_REDIRECTPRESENT': false,
  'EN_PAGEJSON_GIFTPROCESS': false,
  'EN_URLPARAM_MODE': "DEMO",
  'EN_URLPARAM_GTM_DEBUG': "1703262109693",
  'EN_RECURRING_FREQEUENCIES': ["ONETIME", "MONTHLY"],
  enFieldName: "supporter.address1",
  enFieldLabel: "Address",
  enFieldValue: "MzQzMSAxNHRoIFN0cmVldCBOVw==

{
  event: "EN_FASTFORMFILL_ALL_FAILURE",
  gtm: {uniqueEventId: 2978},
  'EN_PAGEJSON_CLIENTID': 10089,
  eventValue: false,
  'EN_PAGEJSON_CAMPAIGNPAGEID': 61451,
  'EN_PAGEJSON_CAMPAIGNID': 134379,
  'EN_PAGEJSON_PAGENUMBER': 2,
  'EN_PAGEJSON_PAGECOUNT': 2,
  'EN_PAGEJSON_PAGENAME': "4Site - EOY 2023 - Test - 61451",
  'EN_PAGEJSON_PAGETYPE': "donation",
  'EN_PAGEJSON_LOCALE': "en-US",
  'EN_PAGEJSON_REDIRECTPRESENT': false,
  'EN_PAGEJSON_SUPPORTERID': 97399947,
  'EN_PAGEJSON_COUNTRY': "US",
  'EN_PAGEJSON_GIFTPROCESS': true,
  'EN_PAGEJSON_TRANSACTIONTYPE': "FCS",
  'EN_PAGEJSON_PAYMENTTYPE': "visa",
  'EN_PAGEJSON_AMOUNT': 5,
  'EN_PAGEJSON_CURRENCY': "USD",
  'EN_PAGEJSON_DONATIONLOGID': 14501643,
  'EN_PAGEJSON_TRANSACTIONID': "pm_1OQBUHJxOh2gvObc2kdXNTN6__cus_PEen" +
                               "SmXMAgRp8U__pi_3OQBUKJxOh2gvObc1JvjlEAM",
  'EN_PAGEJSON_RECEIPTNUMBER': 4217,
  'EN_PAGEJSON_RECURRING': false,
  'EN_SUBMISSION_SUCCESS_DONATION': "TRUE",
  'EN_RECURRING_FREQEUENCIES': []



# DataLayer - Purchase

<script>
// datalayer push for WDS tracking
  dataLayer.push({
    event: 'purchase',
    ecommerce: {
      currency: 'USD',
      transaction_id: {{pageJson.donationLogId}},
      value: {{pageJson.amount}},
      items: [
       {
        item_id: {{pageJson.campaignPageId}},
        item_name: {{pageJson.pageName}},
        affiliation: 'Shatterproof',
        currency: 'USD',
        index: 0,
        item_category: 'EN Donation',
        item_category2: {{pageJson.recurring}},   
        item_variant: {{pageJson.recurring}},
        price: {{pageJson.amount}},
        quantity: 1
      }],   
    } // end  ecommerce
  }); // end datalayer push
</script>


Triggered on Page View Dom Ready 
giftProcess contains true



# The pageJson that is exposed on EN’s donation forms
## **/donate/1 - pageJson**
<script>var pageJson = {"clientId":10089,"campaignPageId":61451,"campaignId":134379,"pageNumber":1,"pageCount":2,"pageName":"4Site - EOY 2023 - Test - 61451","pageType":"donation","locale":"en-US","redirectPresent":false,"giftProcess":false};</script>	

## **/donate/2 - pageJson**
<script>var pageJson = {"clientId":10089,"campaignPageId":61451,"campaignId":134379,"pageNumber":2,"pageCount":2,"pageName":"4Site - EOY 2023 - Test - 61451","pageType":"donation","locale":"en-US","redirectPresent":false,"supporterId":97399947,"country":"US","giftProcess":true,"transactionType":"FCS","paymentType":"visa","amount":5.0,"currency":"USD","donationLogId":14488559,"transactionId":"pm_1OQ1bnJxOh2gvObcdxZVlGqn__cus_PEUbJDKHxAu1Uh__pi_3OQ1bqJxOh2gvObc0KTQWXbT","receiptNumber":4212,"recurring":false};</script>	