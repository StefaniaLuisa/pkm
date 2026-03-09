# GTM & GA4 for 4Site Studios

#4sitemarketing #4Site #gtm #ga4 

[4Site Tracking Doc](https://docs.google.com/spreadsheets/d/1bX3UaCVA1I4Kh3F7yNjBt-I7z2lIF-m1lI3ZD9UG41I/edit#gid=0)


The forms are not hubspot they are Gravity Forms


[https://www.youtube.com/results?search_query=Track+Gravity+forms+with+GTM](https://www.youtube.com/results?search_query=Track+Gravity+forms+with+GTM)

[Gravity Forms TRacking Blog](https://www.analyticsmania.com/post/track-gravity-forms-with-google-tag-manager/)

How to setup your own Event Listeners: [https://www.simoahava.com/analytics/simple-custom-event-listeners-gtm/](https://www.simoahava.com/analytics/simple-custom-event-listeners-gtm/)



<script type="text/javascript">
  jQuery(document).ready(function() {
   jQuery(document).bind("gform_confirmation_loaded", function(event, formID) {
    window.dataLayer = window.dataLayer || [];
    window.dataLayer.push({
     'event': 'formSubmission',
     'formID': formID
    });
   });
  });
</script>
