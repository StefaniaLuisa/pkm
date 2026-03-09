# FWW EN Template - GA4/GTM 
#4site

For Food & Water Watch
Add this code after the <head> tag 
```
<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-W399T6');</script>
<!-- End Google Tag Manager -->

    <!-- START: 4Site custom code to surface the referring URL to the EN pages -->
    <script>
        const firstReferrer = {user_data~First Referrer};
    </script>
    <!-- END: 4Site custom code to surface the referring URL to the EN pages -->
	
	<!-- Start Google Tag Manager Data Layer Initialization Script -->
	<script>
	 window.dataLayer = window.dataLayer || [];
	</script>
	<!-- End Google Tag Manager Data Layer Initialization Script -->

	<!-- Google Analytics 4 -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-X09714MWYF"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-X09714MWYF');
    </script>
 <!-- End Google Analytics 4 -->
```


#4site/client/fww

