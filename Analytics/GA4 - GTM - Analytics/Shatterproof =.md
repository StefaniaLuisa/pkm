# Shatterproof =

|                                                                                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <script>var pageJson = {"clientId":10089,"campaignPageId":61451,"campaignId":134379,"pageNumber":1,"pageCount":2,"pageName":"4Site - EOY 2023 - Test - 61451","pageType":"donation","locale":"en-US","redirectPresent":false,"giftProcess":false};</script> |


| Transaction details from Shatterproof                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <script>var pageJson = {"clientId":10089,"campaignPageId":61451,"campaignId":134379,"pageNumber":2,"pageCount":2,"pageName":"4Site - EOY 2023 - Test - 61451","pageType":"donation","locale":"en-US","redirectPresent":false,"supporterId":97399947,"country":"US","giftProcess":true,"transactionType":"FCS","paymentType":"visa","amount":5.0,"currency":"USD","donationLogId":14488559,"transactionId":"pm_1OQ1bnJxOh2gvObcdxZVlGqn__cus_PEUbJDKHxAu1Uh__pi_3OQ1bqJxOh2gvObc0KTQWXbT","receiptNumber":4212,"recurring":false};</script> |



<script>
var _wds_oi = "{{transactionId}}";
var _wds_oa = “{{amount}}";		
var _wds_op = “{{transactionType}}“;
var _wds_ob = “{{pageName}}”;
var _wds_ot = "{{paymentType}}”;
</script>

**var _wds_oh = "{Insert SHIPPING Here}";**  
**var _wds_os = "{Insert SOURCE_CODE Here}";**  
**var _wds_ob = "{Insert SOURCE_TYPE Here}";**  
**var _wds_op = "{Insert PAY_METHOD Here}";**  
**var _wds_ot = "{Insert CARD_TYPE Here}";**  


pageName

“{{supporterId}}”
“{{transactionType}}”


var _wds_im = "";
var _wds_oi = "{{transactionId}}";     == order ID
var _wds_oa = “{{amount}}";		== order amount
var _wds_op = “{{transactionType}}“ == _wds_op  Payment method
var _wds_ob = “{{pageName}}”
var _wds_ot = "{{paymentType}}”.   === Credit card Type: 
var _wds_os			 ==== sournce code
“{{supporterId}}”
“{{transactionType}}”
</script>



Ocena - Data layer Variable for Donation amount:

ecommerce.value

AIUSA - DataLayer Viraible
DL - ecommerce.value = ecommerce.value
DL - ecommerce.transaction_id  = ecommerce.transaction_id


Data Layer 
en_campaign_id  = {{EN Campaign ID}}
en_transaction_amount = {{EN Transaction Amount}}
en_transaction_id = {{EN Transaction ID}}
{{Page URL}}
{{EN Donation Type}}
donation_type



function() {
  var queryString = window.location.search;
  var urlParams = new URLSearchParams(queryString);

  if (queryString.includes('ea.tracking.id')) {
    return urlParams.get('ea.tracking.id');
  } else if (queryString.includes('ea_tracking_id')) {
    return urlParams.get('ea_tracking_id'); //sometimes this form replaces . with _
  }
}

<script>
var _wds_im = "";
var _wds_oi = "{{EN Transaction ID}}";
var _wds_oa = "{{EN Transaction Amount}}";
var _wds_os = "{{ea.tracking.id}}"
var _wds_ob = "{{Page Path}}"
var _wds_ae = "{{Page URL}}"
</script>




revenue
{{EN Transaction Amount}}

order id
{{EN Transaction ID}}

campiagn Id

{{EN Campaign ID}}

{{EN Donation Type}}

{{EN Page Template Name}}

<script src="https://js.ipredictive.com/adelphic_universal_pixel.js" type="text/javascript"></script>
<script type="text/javascript">
    new AdelphicUniversalPixel(108191, 'https://ad.ipredictive.com/d/track/event',
    {
  "tn": "{{EN Transaction ID}}",
  "val": "{{EN Transaction Amount}}",
  "cust": "{{EN Donation Type}}",
  "ps": "0"
}).fire();
</script>
<noscript>
    <img src="https://ad.ipredictive.com/d/track/event?upid=108191&url={{Page URL}}&tn={{EN Transaction ID}}&val={{EN Transaction Amount}}&cust={{EN Donation Type}}&cache_buster=[timestamp]&ps=1" height="1" width="1" style="display:none" />
</noscript>



<img src="https://secure.adnxs.com/px?id=1037720&seg=14843183&order_id={{EN Transaction ID}}&value={{EN Transaction Amount}}&t=2" width="1" height="1" />