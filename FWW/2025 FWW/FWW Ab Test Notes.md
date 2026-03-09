
C. Ablocker - 13832

B. Multistep - 13831

A. One-Col - 13830

```javascript
<script>

// Template Code for Running A/B tests in 4Site's Promo Plugin - Follow comments to know what needs to be updated. 
// Designate your promos for easy copy/paste code update:
// Promo Varation A (CONTROL) = Find 4A4A4A and replace with Variation A Promo ID 
// Promo Varation B (TEST) = Find 4B4B4B and replace with Variation B Promo ID 
// Promo ADBLOCKER = Find 4C4C4C and replace with ADBLOCKER Variation



function checkForAdblocker() {

  document.body.insertAdjacentHTML(
    "beforeend",
    '<ins data-adBlockTest class="adsbygoogle ad-zone ad-space ad-unit textads banner-ads banner_ads" style="display: block !important; width:1px !important; height: 1px !important; visibility: hidden !important;"></ins>'
  );
  const testAd = document.querySelector("[data-adBlockTest]");

  if (testAd) {
    const testAdWidth = testAd.offsetWidth;
    if (testAdWidth == "1") {
      console.log("########################################");
      console.log(
        "No adblocker detected, will run Control Promotion"
      );
      triggerPromotions();
    } else if (testAdWidth == "0") {
      console.log("########################################");
      console.log(
        "Adblocker detected, won't run any of the Multivariate Promotions"
      );
      console.log(
        "Triggering Promotion: ADBLOCKER "
      );
      console.log("########################################");
      window.triggerPromotion(13832); // Replace with ADBLOCKER Promo ID

    }
  }
}

function triggerPromotions() {

  const gtPromotions = ["multistep", "spinner",];

  if (gtPromotions) {
    const myPromotion =
      gtPromotions[Math.floor(Math.random() * gtPromotions.length)];
    if (myPromotion == "multistep") {
      console.log(
        "Triggering Promotion #13830" 
      );
      console.log("########################################");
      window.triggerPromotion(13830); 
      window.dataLayer.push({
        event: "promotion_seen",
        promotionName:
          "Promotion #13830", //Replace with Variation A (CONTROL) Promo ID
      });
    } else if (myPromotion == "spinner") {
      console.log(
        "Triggering Promotion #13831" //Replace with Variation B (TEST) Promo ID
      );
      window.triggerPromotion(13831); //Replace with Variation B (TEST) Promo ID
    }  else {
      console.log(
        "The promotion chosen is outside the array and nothing was triggered"
      );
      console.log("########################################");
    }
  }
}

checkForAdblocker();



</script>
```