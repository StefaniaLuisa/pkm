
&lt;Form Header&gt;

<https://act.savethechildrenactionnetwork.org/a/congress-keep-promises-kids-fa-6-25-1>

```css
Header {
    font-family: "Oswald", sans-serif;
    font-size: 48px;
    text-transform: uppercase;
    font-weight: 500;
    line-height: 1.25em;
    margin: 0;
    padding: 24px 0px 0px 0px;
    text-align: left;
}

Read More {
    color: #da291c;
    font-family: "Oswald", sans-serif;
    font-weight: 500;
    text-decoration: underline;
    text-transform: uppercase;
    cursor: pointer;
}

Body Copy {
 font-family: "Lato", sans-serif;
  font-weight: 400;
  font-size: 1rem; /*which is 18px */
    line-height: 1.5em;
    padding: 24px 0px 24px 0px;
    margin: 0;
}
```

p

```css
* {
  box-sizing:border-box;
}

:root {
  --main-font-family:"Lato", sans-serif;
  --secondary-font-family:"Oswald", sans-serif;
  --glyphicons-font-family:"Glyphicons Regular";
  --main-text-color:#000;
  --main-white:#fff;
  --main-red:#da291c;
  --main-pale-blue:#9ab3d5;
  --main-orange:#fc4c02;
  --main-tan:#d6cebd;
  --main-yellow:#fc0;
  --main-dark-grey:#676767;
  --main-grey:#808184;
  --main-biscuit:#e8e3d4;
  --main-light-grey:#e5e7eb;
  --main-rgb-biscuit:232,227,212;
  --main-rgb-white:255,255,255;
  --default-box-shadow:0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  --alpha: 0.33;
  --alpha2: 0;
}

html {
  font-size:18px;
}


/* Body */
body.background-white {background-color:var(--main-white);}
body.background-biscuit {background-color:var(--main-biscuit);}

body {
  background-repeat:no-repeat;
  color:var(--main-text-color);
  font-family:var(--main-font-family);
  font-size:18px;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  font-weight:400;
  line-height:1.5em;
  margin:0;
  text-rendering:optimizelegibility;
}

main {
  margin:0 auto;
  width:100%;
}

main.theme-content a,
main.theme-content a:hover {
  font-weight:700;
  color:var(--main-red);
  text-decoration:underline;
}

/* Theme Header */
figure.branding {
  display:flex;
  line-height:0;
  margin:0 auto;
  max-width:1240px;
}

figure.branding a {
  display:block;
  padding:24px 0px;
}

figure.branding img {
  height:61px;
  width:280px;
}

figure.branding img.stacked  {
  display:none;
}

header.theme-header section.header-image {
  background-position:50% 33%;
  background-size:cover;
  height:200px;
  margin:0;
}

main article section.article-content {
  padding: 48px 20px 60px 20px;
  width:100%;
}

article .article-content > .branding,
article .article-content .inline-image {display:none;}

/* FastAction */
article .at.ngp-form .FastAction {
  margin:0;
  padding:0;
}

article .at.ngp-form .FastAction .fastAction {
  background: rgba(var(--main-rgb-biscuit), var(--alpha));
  padding:10px;
  border-radius:0px;
}

body.background-biscuit article .at.ngp-form .FastAction .fastAction {background: rgba(var(--main-rgb-white), var(--alpha));}

article .at.ngp-form .FastAction p a {
  font-weight:400;
  color:var(--main-text-color);
  text-decoration:underline;
}

article .at.ngp-form .FastAction p a:focus,
article .at.ngp-form .FastAction p a:hover {text-decoration:underline;}

article .at.ngp-form .FastAction p {
  align-items:center;
  display:flex;
  font-size:16px;
  justify-content:space-between;
  line-height:1.25em !important;
  margin:0;
  padding:0 5px;
}

article .at.ngp-form .FastAction .profile-link {
  background:#fff;
  border: 1px solid var(--main-light-grey);
}

article .at.ngp-form .FastAction p > span {
  font-family:var(--primary-font-family);
  color:var(--main-text-color) !important;
  margin:0;
  padding:5px;
}

article .at.ngp-form .FastAction .fa-cta span a {
  color:#fff;
  text-decoration:none;
}

article .at.ngp-form .FastAction .fa-lead {
  display:block;
  order:1;
}

article .at.ngp-form .FastAction .fa-lead b {font-weight:700;}

article .at.ngp-form .FastAction .fa-lead i {font-family:var(--secondary-font-family);}
  
article .at.ngp-form .FastAction .fa-lead br {display:none;}

article .at.ngp-form .FastAction .fa-cta {order:2;}

/* Form */
article .at.ngp-form {
  width:100%;
  margin: 0 40px 0 auto;
}

article .at.ngp-form.multistep-layout {
  max-width:600px;
  overflow:unset;
  min-width:320px;
}

main section.at-inner {background:none;}

article .at.ngp-form form {padding:0px;}

article .at.ngp-form .at-form * {color:var(--main-text-color);}
article .at.ngp-form .at-form span[style*="color"] * {color:unset;}

article .at.ngp-form form a {text-decoration:none;}

article .at.ngp-form header.at-title {
  font-family:var(--secondary-font-family);
  font-size:48px;
  text-transform:uppercase;
  font-weight:500;
  line-height:1.25em;
  margin:0;
  padding:24px 0px 0px 0px;
  text-align:left;
}

article .at.ngp-form header.HeaderHtml {
  font-size:1rem;
  line-height:1.5em;
  padding:24px 0px 24px 0px;
  margin:0;
}

article .at.ngp-form header.MeterHtml + header.HeaderHtml {padding-top:16px;}

article .at.ngp-form header.HeaderHtml h2,
article .at.ngp-form .content.thankYou h2 {
  font-size:1.5rem;
  font-weight:700;
  line-height:1.5em;
  margin:0 0 15px;
}

article .at.ngp-form p,
article .at.ngp-form header.HeaderHtml p,
article .at.ngp-form .content.thankYou p {
  margin:0 0 15px;
  padding:0;
}

article .at.ngp-form header.HeaderHtml strong,
article .at.ngp-form header.HeaderHtml b {font-weight:700;}

article .at.ngp-form.multistep-layout header.HeaderHtml p {
  font-size:1rem;
  line-height:1.5em;
}

article .at.ngp-form header.HeaderHtml p:last-child,
article .at.ngp-form .content.thankYou p:last-child {margin:0;}

article .at.ngp-form .content.thankYou {
  margin:0 auto;
  max-width:840px;
  padding:20px;
  width:100%;
}

article.two-columns .at.ngp-form .content.thankYou {max-width:unset;}

article .at.ngp-form header.HeaderHtml a,
article .at.ngp-form .at-markup a,
article .at.ngp-form .content.thankYou a {
  color:var(--main-red);
  font-weight:700;
}

article .at.ngp-form header.HeaderHtml a:hover,
article .at.ngp-form .content.thankYou a:hover {text-decoration:underline;}

article .at.ngp-form .content.thankYou table {width:100%;}

article .at.ngp-form .content.thankYou button.btn-social {
  color:#fff;
  font-weight:700;
  margin:0 15px 0 0;
}

article .at.ngp-form .ngp-deactivation-message {
  padding:20px 20px 0;
  text-align:center;
}

article .at.ngp-form .ngp-deactivation-message p  {
  line-height:24px;
  margin:0 0 15px;
}

article .at.ngp-form .at-inner h2 {
  font-size1.5rem;
  font-weight:700;
  line-height:1.5em;
  margin:20px 0 5px;
}

article .at.ngp-form header.HeaderHtml p.disclaimer {
  font-size:.777778rem;
  font-style:italic;
}

/* Read More Styles */
article .at.ngp-form header.HeaderHtml > span.show-full-body {display:none;}

/* Blockquote Stuff */
article .at.ngp-form  .HeaderHtml blockquote {
  border-top:2px solid var(--main-red);
  border-bottom:2px solid var(--main-red);
  margin:20px 0;
  padding:20px 0;
}

article .at.ngp-form .HeaderHtml blockquote > *:not(blockquote) {display:none;}

article .at.ngp-form .HeaderHtml blockquote.expanded > *:not(blockquote) {display:block;}

article .at.ngp-form .HeaderHtml blockquote h2 {
  color:var(--main-red);
  display:flex;
  flex-direction:row-reverse;
  font-family:var(--secondary-font-family);
  font-size:1.333333rem;
  font-weight:400;
  justify-content:space-between;
  line-height:1.2em;
  margin-bottom:0;
}

article .at.ngp-form .HeaderHtml blockquote.expanded h2 {
  display:flex;
  margin-bottom:15px;
}

article .at.ngp-form .HeaderHtml blockquote h2:before {
  content:"\f055";
  font-family:var(--font-awesome-solid);
  font-size:1.25rem;
  font-weight:700;
  padding-left:20px;
}

article .at.ngp-form .HeaderHtml blockquote.expanded h2:before {content:"\f056";}

article .at.ngp-form .HeaderHtml .square-image-with-text {
  gap:20px;
  grid-template-columns:100px 1fr;
  margin:0 0 16px;
}

article .at.ngp-form .HeaderHtml .square-image-with-text:last-child {margin:0;}

article .at.ngp-form .HeaderHtml .expanded .square-image-with-text {display:grid;}

article .at.ngp-form .HeaderHtml .square-image-with-text figure {margin:0;}


/* Form Steps */

article .at.ngp-form ol.at-steps {
  background:#fff;
  border-radius:0;
  border:1px solid var(--main-biscuit);
  display:grid;
  grid-template-columns:1fr 1fr 1fr;
  margin:0;
  padding:0px;
}

body.background-biscuit article .at.ngp-form ol.at-steps {
  background:var(--main-biscuit);
  border:1px solid var(--main-white);
}

article .at.ngp-form ol.at-steps:before,
article .at.ngp-form ol.at-steps:after {display:none;}

article .at.ngp-form ol.at-steps li.at-step {
  border:0;
  color:var(--main-dark-grey);
  margin:unset;
  padding:0;
  position:relative;
  width:100%;
}

article .at.ngp-form ol.at-steps li.at-step.active {background-color:var(--main-biscuit);}

body.background-biscuit article .at.ngp-form ol.at-steps li.at-step.active {background-color:var(--main-white);}

article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before,
article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {
  border-style:solid;
  border-width:36px 0 36px 12px;
  border-color:transparent transparent transparent var(--main-biscuit);
  content:"";
  display:block;
  height:0;
  position:absolute;
  top:0;
  width:0;
}

article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before {left:0;}
article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {right:-12px;}

article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before,
body.background-biscuit article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {border-color:transparent transparent transparent #fff;}
body.background-biscuit article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before {border-color:transparent transparent transparent var(--main-biscuit);}

article .at.ngp-form ol.at-steps li.at-step a,
article .at.ngp-form ol.at-steps li.at-step b {
  align-items:center;
  display:grid;
  font-size:.666667rem;
  height:72px;
  line-height:2em;
  padding:15px 12px 9px 12px;
  text-align:center;
  text-transform:uppercase;
  width:100%;
}

article .at.ngp-form ol.at-steps li.at-step a:before,
article .at.ngp-form ol.at-steps li.at-step b:before {
  background:var(--main-text-color);
  border:0;
  border-radius:50%;
  display:flex;
  font-size:.666667rem;
  font-weight:700;
  height:24px;
  justify-content:center;
  left:unset;
  line-height:2em;
  margin:0 auto;
  padding:0;
  position:relative;
  right:unset;
  top:0;
  transform:none;
  width:24px;
}

article .at.ngp-form ol.at-steps li.at-step a span.step-title {
  display:flex;
  height:24px;
  justify-content:center;
}

/* Progress Meter Stuff */
article .at.ngp-form header.MeterHtml {
  margin:0;
  padding:0 20px;
  width:100%;
}

article .at.ngp-form header.at-title + header.MeterHtml {padding-top:12px;}

article .at.ngp-form header.MeterHtml iframe {display:none;}

article .at.ngp-form figure.progress-meter {
  margin:0;
  padding:0;
}

article .at.ngp-form figure.progress-meter strong {
  display:block;
  font-size:1rem;
  font-weight:700;
}

article .at.ngp-form figure.progress-meter progress {
  appearance:none;
  background:var(--main-biscuit);
  border:0;
  border-radius:15px;
  display:block;
  height:30px;
  margin:0 0 10px;
  padding:0;
  position:relative;
  -webkit-appearance:none;
  width:100%;
  box-shadow:unset;
  z-index:3;
}

article .at.ngp-form figure.progress-meter progress::-webkit-progress-bar {
  background:var(--main-biscuit);
  border:0;
  border-radius:15px;
}

article .at.ngp-form figure.progress-meter progress::-moz-progress-bar {
  background-color:var(--main-red);
  border-radius:15px;
}

article .at.ngp-form figure.progress-meter progress::-webkit-progress-value {
  background-color:var(--main-red);
  border-radius:15px;
}

article .at.ngp-form figure.progress-meter p.progress-meter-details {
  display:grid;
  gap:10px;
  grid-template-columns:auto 1fr auto;
  margin:0;
  text-transform:uppercase;
}

article .at.ngp-form figure.progress-meter p.progress-meter-details span {
  font-size:.777778rem;
}

article .at.ngp-form figure.progress-meter p.progress-meter-details span.progress-meter-submitters {
  grid-column:1 / 2;
}

article .at.ngp-form figure.progress-meter p.progress-meter-details strong {
  font-size:.888889rem;
  text-transform:initial;
}

article .at.ngp-form figure.progress-meter p.progress-meter-details span.progress-meter-goal {
  grid-column:3 / 4;
  padding-left:10px;
  text-align:right;
}

/* Form Elements */
article .at.ngp-form fieldset.at-fieldset {
  padding:0px;
  min-width:unset;
}

article .at.ngp-form fieldset.AdditionalInformation.hide-additional-information legend {display:none;}

article .at.ngp-form fieldset.ContributionInformation {padding-top:10px !important;}

article .at.ngp-form.multistep-layout fieldset.Interests {padding-top:0 !important;}
article .at.ngp-form fieldset.at-fieldset.PaymentMethodSection {padding-top:20px;}

article .at.ngp-form legend.at-legend {
  display:flex;
  font-family:var(--secondary-font-family);
  font-size:24px;
  font-weight:400;
  line-height:28px;
  margin:0 10px;
  padding:20px 0 10px;
  text-transform:uppercase;
}

article .at.ngp-form fieldset.ContributionInformation legend.at-legend {padding-bottom:0;}

article .at.ngp-form .at-row label,
article .at.ngp-form fieldset.TicketInformation label {
  color:var(--main-text-color);
  font-size:18px;
  line-height:1.5em;
  margin:0 10px 10px;
}

article .at.ngp-form fieldset.TicketInformation label {margin:0;}

article .at.ngp-form fieldset.TicketInformation label span {color:var(--main-text-color);}

article .at.ngp-form .at-row label input,
article .at.ngp-form .at-table label input,
article .at.ngp-form .at-row label select,
article .at.ngp-form .at-table label select,
article .at.ngp-form .at-row label .select2-selection,
article .at.ngp-form .at-row label textarea,
article .at.ngp-form .at-row label .vgs-input-container iframe {
  border:1px solid var(--main-text-color);
  border-radius:6px;
  font-size:1rem;
  font-weight:400;
  height:44px;
  line-height:46px;
  margin:5px 0;
  padding:8px 16px;
}

article .at.ngp-form .at-row label .intl-tel-input {margin:5px 0 15px;}

article .at.ngp-form .at-row label .intl-tel-input input {padding-left:46px;}

article .at.ngp-form .at-row label select,
article .at.ngp-form .at-table label select {
  background-position:right 15px center;
  padding:0 15px;
}

article .at.ngp-form .at-recurring label select {
  border-width:2px;
  height:36px;
  margin:0 5px 0 0;
  padding:0 20px 0 5px;
}

article .at.ngp-form .at-row label .select2-selection {
  color:var(--main-text-color);
  padding-top:10px;
  text-transform:none;
}

article .at.ngp-form .at-row label .select2-selection__rendered {color:var(--main-text-color);}

article .at.ngp-form .at-row label textarea {
  height:auto;
  line-height:1.5em;
  min-height:100px;
}

article .at.ngp-form .at-row label small,
article .at.ngp-form .at-table label small,
article .at.ngp-form .at-row label a.at-whatsthis {
  color:var(--main-text-color);
  font-size:16px;
  line-height:1em;
}

article .at.ngp-form .at-row.PostalCode.City.StateProvince label {
  flex:1 120px;
  min-width:120px;
}

article .at.ngp-form .at-row.FirstName.LastName label,
article .at.ngp-form .at-row.Country.PostalCode.City.StateProvince label  {
  flex:1 150px;
  min-width:150px;
}

article .at.ngp-form .at-row label.at-cc-expiration {
  flex:1 140px;
  min-width:140px;
}

article .at.ngp-form .at-row.EmailAddress.HomePhone label,
article .at.ngp-form .at-row.EmailAddress.MobilePhone label {
  flex:1 180px;
  min-width:180px;
}

article .at.ngp-form .at-row.Prefix.FirstName.LastName label.Prefix,
article .at.ngp-form .at-row.FirstName.LastName label.custom-prefix {
  flex:1 120px;
  min-width:120px;
}

article .at.ngp-form input::placeholder {opacity:.5;}

article .at.ngp-form hr {border-bottom:1px solid var(--main-grey);}

/* Checkboxes */
article .at.ngp-form label.at-check,
article .at.ngp-form .at-markup.UpdateMyProfile {margin:5px 10px;}

article .at.ngp-form .at-recipient-msg label.at-check.NotificationSendCopy {margin:7px 0 10px;}

article .at.ngp-form .at-row .UpdateMyProfile b {font-weight:700;}

article .at.ngp-form .updateMyProfileSection > label {margin:0;}
  
article .at.ngp-form label.at-check .at-checkbox-title-container:before,
article .at.ngp-form label.at-check .at-checkbox-title-container:after,
article .at.ngp-form .UpdateMyProfile label > span:before,
article .at.ngp-form .UpdateMyProfile label > span:after,
article .at.ngp-form label.at-check.authorize-payment-label > span:before,
article .at.ngp-form label.at-check.authorize-payment-label > span:after {
  border:1px solid var(--main-text-color);
  border-radius:6px;
  height:24px;
  left:0;
  top:0;
  width:24px;
}

article .at.ngp-form input[type="checkbox"]:focus + span:before {
  box-shadow:unset;
  border-color:var(--main-dark-grey);
}

article .at.ngp-form label.at-check .at-checkbox-title-container:before,
article .at.ngp-form .UpdateMyProfile label > span:before,
article .at.ngp-form label.at-check.authorize-payment-label > span:before {background:none;}

article .at.ngp-form label.at-check .at-checkbox-title-container:after,
article .at.ngp-form .UpdateMyProfile label > span:after,
article .at.ngp-form label.at-check.authorize-payment-label > span:after {
  background-color:var(--main-red);
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/BSA/BSA/1/116731/images/themes/check-mark-white.svg);
  background-position:center;
  background-repeat:no-repeat;
  background-size:14px 14px;
  border-color:var(--main-text-color);
  content:"";
  font-size:16px;
  line-height:16px;
  text-align:center;
}

article .at.ngp-form label.at-check .at-checkbox-title-container,
article .at.ngp-form .UpdateMyProfile label > span,
article .at.ngp-form fieldset.ContributionInformation label.at-select.SelectedFrequency span.at-select,
article .at.ngp-form label.at-check.authorize-payment-label > span {
  display:block;
  font-size:1rem;
  line-height:1.333333em;
  margin:0;
  padding-left:35px;
  text-transform:none;
}

article .at.ngp-form fieldset.ContributionInformation label.at-select.SelectedFrequency span.at-select {padding-left:0;}

article .at.ngp-form label.at-check .at-checkbox-title,
article .at.ngp-form label.at-check .at-cover-costs-info,
article .at.ngp-form label.at-select .select-collapse,
article .at.ngp-form .UpdateMyProfile label span {
  color: var(--main-text-color);
  font-size:18px;
  font-weight:400;
  line-height:24px;
}

article .at.ngp-form .at-row label.multi-select .select2-selection {
  height:auto;
  line-height:30px;
  min-height:40px;
  padding:0;
}

article .at.ngp-form .at-row label.multi-select .select2-container--default .select2-selection--multiple {margin:0;}

article .at.ngp-form .select2-container--default .select2-selection--multiple .select2-selection__choice {
  line-height:30px;
  white-space:normal;
}

article .at.ngp-form .at-row label.multi-select .select2-container--default li.select2-search--inline input {
  border:0;
  height:30px;
  margin:0;
  padding:0;
}

article .at.ngp-form fieldset.ContributionInformation label.at-select.SelectedFrequency,
article .at.ngp-form fieldset.ContributionInformation label.at-select.SelectedDuration {margin:0 0 0 4px;}

article .at.ngp-form fieldset.ContributionInformation label.at-select.SelectedFrequency.select-collapse {margin:5px;}

article .at.ngp-form fieldset.ContributionInformation .at-recurring {
  display:flex;
  flex-wrap:wrap;
  font-size:1rem;
  line-height:20px;
  margin:0 0 10px;
  padding:0 10px;
}

article .at.ngp-form fieldset.ContributionInformation.forced-recurring .at-recurring {display:none;}

article .at.ngp-form .at-recurring label {
  font-size:1rem;
  line-height:20px;
}

article .at.ngp-form .at-recurring label.IsRecurring {
  display:flex;
  margin:5px 0;
}

article .at.ngp-form .at-recurring label.IsRecurring span {
  display:block;
  font-size:1rem;
  line-height:24px;
}

article .at.ngp-form .at-recurring label select,
article .at.ngp-form .at-recurring label input {
  border:1px solid var(--main-grey);
  border-radius:0;
  color:var(--main-text-color);
  font-size:56px;
  font-weight:700;
  height:34px;
  line-height:22px;
  margin:0 5px 0 0;
  padding:0 20px 0 5px;
}

article .at.ngp-form fieldset.ContributionInformation .at-recurring .at-check {
  display:block;
  margin-right:0;
}

article .at.ngp-form fieldset.AdditionalInformation .other-option > label.at-text {
  margin:-1px 10px 0 0;
  flex-grow:1;
  flex-basis:unset;
}

article .at.ngp-form fieldset.AdditionalInformation .other-option label.at-text input {
  height:34px;
  line-height:34px;
  margin:0;
}

article .at.ngp-form .at-row.SmsLegalDisclaimer {
  margin:0;
  padding:0 10px;
}

article .at.ngp-form .at-row.SmsLegalDisclaimer.at-indented {padding-left:45px;}

article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer,
article .at.ngp-form .at-row.LegalHeaderHtml .at-markup.LegalHeaderHtml {
  color: var(--main-text-color);
  margin:0;
  padding:0;
  font-size: 18px;
}

article .at.ngp-form .at-row.LegalHeaderHtml .at-markup.LegalHeaderHtml {
  margin-top:10px;
}

article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer p,
article .at.ngp-form .at-row.LegalHeaderHtml .at-markup.LegalHeaderHtml p {
  font-size:16px;
  line-height:1.142857rem;
  margin:0 0 10px;
}

article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer p a {
  font-weight:700;
  text-decoration:underline;
}

article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer p a:focus,
article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer p a:hover {text-decoration:underline;}

article .at.ngp-form .at-row.SmsLegalDisclaimer .at-markup.SmsLegalDisclaimer p:last-child {margin-bottom:10px;}

/* Radio Buttons + Toggle */
article .at.ngp-form .radios label input[type="radio"] {
  -moz-appearance:none;
  -webkit-appearance:none;
  border:2px solid var(--main-dark-grey);
  border-radius:50%;
  content:"";
  display:block;
  height:24px;
  left:0;
  margin:0;
  padding:0;
  outline:none;
  position:absolute;
  width:24px;
}

article .at.ngp-form .radios label input[type="radio"]:checked {
  background:var(--main-white);
  border:6px solid var(--main-red);
}

article .at.ngp-form .form-item-selectedfrequency .radios {
  display:flex;
  flex-wrap:wrap;
}

article .at.ngp-form.multistep-layout .form-item-selectedfrequency .radios {margin:10px 0 0;}

article .at.ngp-form .form-item-selectedfrequency .radios label {
  color:var(--main-text-color);
  display:block;
  font-size:.888889rem;
  font-weight:600;
  line-height:1.5em;
  height:34px;
  margin:0 0 0 10px;
  padding:5px 10px 5px 30px;
  position:relative;
  text-decoration:none;
}

article .at.ngp-form .form-item-selectedfrequency .radio-description {
  color:var(--main-red);
  display:block;
  font-size:18px;
  font-style:italic;
  font-weight:700;
  line-height:1.5em;
  margin:0px 10px 5px 12px;
  padding:0;
  width:100%;
}

article .at.ngp-form .form-item-selectedfrequency .radio-description-value-0 {
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/arrow-red.png);
  background-repeat:no-repeat;
  background-size:24px 30px;
  padding:13px 0 5px 30px;
}

/* Form Control Buttons */
article .at.ngp-form .at-form-submit {
  display:block;
  margin:10px 0 0;
  padding:0px;
}

article .at.ngp-form .at-form-submit:before {display:none;}

article .at.ngp-form:not(.multistep-layout) .at-form-submit,
article .at.ngp-form .at-form-submit .step-prevNext,
article .at.ngp-form.faux-multistep-layout .at-form-submit {
  display:grid;
  gap:20px;
  grid-template-columns:auto 1fr auto;
  grid-template-rows:auto auto;
  width:100%;
}

article .at.ngp-form:not(.multistep-layout, .faux-multistep-layout) .at-form-submit {grid-template-columns:1fr auto 1fr;}

article .at.ngp-form .at-form-submit .step-prevNext {padding:0;}

article .at.ngp-form .at-form-submit .step-prevNext:has(.secure-processing-div[style*="display: none;"]),
article .at.ngp-form .at-form-submit:has(.secure-processing-single-step-div[style*="display: none;"]) {row-gap:0;}

article .at.ngp-form .at-form-submit .step-prevNext .prevNext {padding:0;}

article .at.ngp-form .at-form-submit .step-prevNext:before,
article .at.ngp-form .at-form-submit .step-prevNext:after {display:none;}

article .at.ngp-form .at-form-submit .step-prevNext .next,
article .at.ngp-form.faux-multistep-layout .at-form-submit > .btn-at-primary {
  grid-column:3 / 4;
  grid-row:1 / 2;
}

article .at.ngp-form .at-form-submit .back-link.at-submit,
article .at.ngp-form .at-form-submit .step-prevNext .prev {
  grid-column:1 / 2;
  grid-row:1 / 2;
}

article .at.ngp-form .at-form-submit .at-submit,
article .at.ngp-form .at-form-submit .step-prevNext .btn-at,
article .at.ngp-form legend.at-legend-with-submit input,
.lightbox-modal.at-modal button.lightbox-accept-button,
article .at.ngp-form .at-ecards button.at-preview-ecard {
  align-items:center;
  background-color:var(--main-red);
  border:1px solid var(--main-red);
  border-radius:6px;
  color:#fff;
  display:flex;
  float:none;
  font-family:var(--secondary-font-family);
  font-size:24px;
  font-weight:700;
  height:auto;
  justify-content:center;
  letter-spacing:1.44px;
  line-height:1.2em;
  margin:0;
  order:2;
  padding:16px;
  text-align:center;
  text-transform:uppercase;
  transition:.2s ease-out;
  white-space:normal;
  width:auto;
}

article .at.ngp-form:not(.multistep-layout, .faux-multistep-layout) .at-form-submit {
  grid-column:2 / 3;
  grid-row:1 / 2;
}

article .at.ngp-form .at-form-submit .step-prevNext .btn-at {
  margin:0;
  padding:16px;
  width:unset;
}

article .at.ngp-form .at-form-submit .step-prevNext .btn-at-primary::after {
  content: url("https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/chevron-right.svg");
  display: inline-block;
  width: auto;
  height: 24px;
  padding-left:12px;
}

article .at.ngp-form:not(.faux-multistep-layout) .at-form-submit > .at-submit,
article .at.ngp-form.faux-multistep-layout .at-form-submit > .btn-at-primary {
  background-image:url("https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/chevron-right.svg");
  background-position:center right 12px;
  background-repeat:no-repeat;
  background-size:16px 28px;
  padding-right:40px;
}

article .at.ngp-form .at-form-submit .step-prevNext .prev .btn-at,
article .at.ngp-form .at-form-submit .back-link.at-submit {
  background-color:#fff;
  border:0px;
  color:var(--main-text-color);
  text-decoration:underline;
  font-size:18px;
  font-weight:500;
}

article .at.ngp-form .at-form-submit .back-link.at-submit {
  grid-column:1 / 2;
  grid-row:1 / 2;
}

body.background-biscuit article .at.ngp-form .at-form-submit .step-prevNext .prev .btn-at,
body.background-biscuit article .at.ngp-form .at-form-submit .back-link.at-submit {background-color:var(--main-biscuit);}

article .at.ngp-form .at-form-submit .step-prevNext .prev .btn-at::before,
article .at.ngp-form .at-form-submit .back-link.at-submit::before {
  content: url("https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/chevron-left.svg");
  display: inline-block;
  width: auto;
  height: 18px;
  padding-right:8px;
}

article .at.ngp-form.multistep-layout .at-form-submit .secure-processing-div,
article .at.ngp-form .at-form-submit .secure-processing-single-step-div  {
  float:none;
  grid-column:1 / 4;
  grid-row:2 / 3;
  margin:0;
  width:100%;
}

article .at.ngp-form .at-form-submit .secure-processing-single-step-div {
  grid-column:1 / 4;
  text-align:left;
}

article .at.ngp-form.multistep-layout .at-form-submit .secure-processing-div label,
article .at.ngp-form .at-form-submit .secure-processing-single-step-div label {
  color: var(--main-text-color);
  display:flex;
  font-family:var(--main-font-family);
  font-size:18px;
  font-weight:400;
  justify-content:flex-end;
  line-height:24px;
  width:100%;
}

article .at.ngp-form .at-form-submit .secure-processing-single-step-div label {
  flex-direction:row-reverse;
  justify-content:center;
}

article .at.ngp-form .at-form-submit .secure-processing-single-step-div label .glyphicons-lock {margin:0 8px 0 0;}

/* Contribution Buttons */
article .at.ngp-form fieldset.ContributionInformation .at-radio {margin:0 -10px;}

article .at.ngp-form fieldset.ContributionInformation .at-radios {
  display:grid;
  gap:16px;
  grid-template-columns:1fr 1fr;
  margin:16px 20px 16px;
}

article .at.ngp-form fieldset.ContributionInformation .at-radios:before,
article .at.ngp-form fieldset.ContributionInformation .at-radios:after {display:none;}

article .at.ngp-form fieldset.ContributionInformation label.label-amount {
  align-items:center;
  border-radius:28px;
  color:var(--main-white);
  float:none;
  font-family:var(--secondary-font-family);
  font-size:24px;
  text-transform: uppercase;
  font-weight:500;
  height:60px;
  justify-content:center;
  letter-spacing:.5px;
  line-height:1em;
  margin:0;
  padding:16px;
  text-shadow:unset;
  width:100% !important;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount.incrediblyLong,
article .at.ngp-form fieldset.ContributionInformation label.label-amount.veryLong,
article .at.ngp-form fieldset.ContributionInformation label.label-amount.tooLong {
  font-size:1.333333rem;
  font-weight:500;
  height:80px;
  line-height:1.166666em;
  white-space:normal;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount.chosen-option {
  border-color:var(--main-red);
  color:#fff;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount input[name="SelectAmount"] {
  height:0 !important;
  left:0;
  position:absolute;
  top:0;
  width:1px !important;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount a,
article .at.ngp-form fieldset.ContributionInformation label.label-amount a:hover,
article .at.ngp-form fieldset.ContributionInformation label.label-amount:hover a {
  background:#000;
  border:0px solid;
  border-radius:6px;
  height:58px;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount input:checked + a {
  background-color:var(--main-red);
  border-color:var(--main-red);
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount.label-otheramount {
  background:transparent;
  border:unset;
  font-size:0;
  grid-column: span 2;
  height:auto;
  line-height:60px;
  margin-bottom:10px;
  padding:0;
  position:relative;
}

article .at.ngp-form fieldset.ContributionInformation label.label-amount.label-otheramount.error {padding-bottom:20px;}

article .at.ngp-form fieldset.ContributionInformation .at-radios.recurring-options label.label-otheramount:after {
  content:"";
  font-size:0;
}

article .at.ngp-form fieldset.ContributionInformation input.edit-otheramount,
article .at.ngp-form fieldset.ContributionInformation input.edit-otheramount:required::selection {
  background:#fff;
  border-radius:6px;
  font-family:var(--secondary-font-family);
  font-size:24px;
  font-weight:500;
  height:60px;
  width:600px;
  letter-spacing:unset;
  line-height:60px;
  margin:0;
  padding: 8px 24px;
  position:absolute;
  top:0;
  transition:background-color .25s ease-in-out, border-color .25s ease-in-out;
  width:100% !important;
}

article .at.ngp-form fieldset.ContributionInformation input.edit-otheramount::placeholder {
  color:var(--main-text-color);
  font-weight:700;
}

article .at.ngp-form fieldset.ContributionInformation input:checked + input.edit-otheramount {
  background-color:var(--main-red);
  border-color:var(--main-red);
  color#fff;
  padding:0 20px 0 25px;
}

article .at.ngp-form fieldset.ContributionInformation input:checked + input.edit-otheramount:required,
article .at.ngp-form fieldset.ContributionInformation input:checked + input.edit-otheramount::placeholder {color:#fff;}

article .at.ngp-form fieldset.ContributionInformation label.label-otheramount span,
article .at.ngp-form fieldset.ContributionInformation input.edit-otheramount:required + span {
  border:0;
  color:#fff;
  display:flex;
  font-family:var(--secondary-font-family);
  font-size:1.166667rem;
  font-weight:700;
  height:60px;
  justify-content:space-between;
  line-height:60px;
  padding:0 0 0 12.5px;
  width:100px;
}

article .at.ngp-form fieldset.ContributionInformation label.label-otheramount span {color:var(--main-text-color);}

article .at.ngp-form fieldset.ContributionInformation label.label-otheramount .error {
  color:red;
  display:block;
  font-size:.888889rem;
  font-weight:600;
  left:0;
  line-height:1.25em;
  margin:0;
  padding:5px 0 0;
  position:absolute;
  top:60px;
}

/* Payment Method Buttons */
article .at.ngp-form fieldset .at-payment-method-buttons label.at-btn-radio.large {
  border:1px solid var(--main-text-color);
  border-radius:6px;
  font-family: var(--secondary-font-family);
  font-weight: 500;
  letter-spacing: 1.08px;
  line-height: 18px;
  text-transform: uppercase;
}

/* In Honor / Memory of */
article .at.ngp-form fieldset.at-fieldset.TributeGift {padding:0 20px !important;}

article .at.ngp-form fieldset.TributeGift label.EnableTributeGift {margin:5px 0;}

article .at.ngp-form .at-tribute-gift,
article .at.ngp-form .at-tribute-gift label {
  line-height:20px;
  margin:0;
}

article .at.ngp-form .at-check.IncludeRecipient {margin:5px 10px;}

article .at.ngp-form fieldset.RecipientInformation {padding:0 10px !important;}

article .at.ngp-form .form-item-inhonororinmemoryof {margin:5px 0;}

article .at.ngp-form .form-item-inhonororinmemoryof > label {
  font-weight:700;
  margin:10px 0;
  width:100%;
}

article .at.ngp-form .form-item-inhonororinmemoryof .radios label {font-size:1rem;}

article .at.ngp-form fieldset .radios {
  display:flex;
  flex-wrap:wrap;
  margin:0;
}

article .at.ngp-form fieldset.ContactInformation .radios,
article .at.ngp-form fieldset.AdditionalInformation .radios {padding:10px;}

article .at.ngp-form fieldset.AdditionalInformation .radios {flex-direction:column;}

article .at.ngp-form .radios label {
  display:block;
  flex-wrap:wrap;
  line-height:24px;
  margin:5px 10px 5px 0;
  padding-left:32px;
  padding-right:10px;
}

article .at.ngp-form fieldset.ContactInformation .radios label,
article .at.ngp-form fieldset.AdditionalInformation .radios label {
  flex:unset;
  min-width:50px;
  padding-right:0;
}

article .at.ngp-form.form-item-inhonororinmemoryof .radios label label input {
  flex:unset;
  margin:0;
  min-width:30px;
}

article .at.ngp-form fieldset.RecipientInformation .at-recipient-info .at-title {
  font-size:1rem;
  font-weight:700;
  margin:10px 10px 0;
}

article .at.ngp-form fieldset.RecipientInformation .at-markup.RecipientInfoHeaderHtml {
  font-size:1rem;
  line-height:1.411765em;
  margin:10px;
}

article .at.ngp-form fieldset.RecipientInformation label.notificationsenddate,
article .at.ngp-form fieldset.RecipientInformation label.NotificationMessage {margin:0;}

/* Additional Information / Custom Stuff */
article .at.ngp-form fieldset.AdditionalInformation .at-markup h2 {
  font-size:1.25rem;
  font-weight:700;
  margin:10px 0;
}

article .at.ngp-form fieldset.AdditionalInformation .at-markup p {line-height:1.25em;}

article .at.ngp-form fieldset.AdditionalInformation .at-row-full > label.at-text,
article .at.ngp-form fieldset.AdditionalInformation .at-row-full > label.at-check,
article .at.ngp-form fieldset.AdditionalInformation .at-row-full > label.at-select,
article .at.ngp-form fieldset.AdditionalInformation .at-row-full > div > label.checkbox-list-label,
article .at.ngp-form fieldset.AdditionalInformation .at-row-full > .form-unit-radio > label {
  font-weight:500;
  margin-top:10px;
}

article .at.ngp-form fieldset.AdditionalInformation label.at-area {margin-top:10px;}

article .at.ngp-form fieldset.AdditionalInformation label.at-area textarea {margin-top:10px;}

article .at.ngp-form fieldset.AdditionalInformation .at-row-full > label.at-check {margin-top:5px;}

article .at.ngp-form fieldset.AdditionalInformation .radios label {margin:5px 15px 5px 0;}

article .at.ngp-form fieldset.AdditionalInformation .radios label[title="Other"],
article .at.ngp-form fieldset.AdditionalInformation .other-option label.at-check {
  display:flex;
  margin-right:0;
}

article .at.ngp-form fieldset.AdditionalInformation .radios label[title="Other"] label.at-text,
article .at.ngp-form fieldset.AdditionalInformation div.other-option label.at-text {
  margin-top:0;
  padding-left:10px;
  flex-grow:1;
}

article .at.ngp-form fieldset.AdditionalInformation .radios label[title="Other"] label.at-text {margin:-5px 0;}

article .at.ngp-form fieldset.AdditionalInformation .radios label[title="Other"] label.at-text input,
article .at.ngp-form fieldset.AdditionalInformation div.other-option label.at-text input {
  height:34px;
  line-height:34px;
  margin:0;
}

article .at.ngp-form .at-fields.interests-fields {margin:0;}

article .at.ngp-form fieldset.ContributionInformation .gift-support {margin-top:10px;}

article .at.ngp-form fieldset.Interests .InterestsHeaderHtml p {margin-top:0;}

article .at.ngp-form fieldset.ContributionInformation .gift-designation select,
article .at.ngp-form fieldset.ContributionInformation .other-designation input {margin-bottom:5px;}

article .at.ngp-form fieldset.ContributionInformation label.other-designation.hidden {display:none;}

article .at.ngp-form fieldset.TicketInformation .at-fields {padding:0 10px;}

article .at.ngp-form fieldset.TicketInformation table {
  background:none;
  border-collapse:collapse;
}

article .at.ngp-form fieldset.TicketInformation table tr {background:none;}

article .at.ngp-form fieldset.TicketInformation table th,
article .at.ngp-form fieldset.TicketInformation table td {padding:15px;}

article .at.ngp-form fieldset.TicketInformation table.at-table th,
article .at.ngp-form fieldset.TicketInformation table.at-table tr.ticketTotals td,
article .at.ngp-form fieldset.TicketInformation table.at-table tr.ticketTotals td b {
  background:var(--main-rgb-biscuit);
  color:var(--main-grey);
  font-size:1rem;
  font-weight:700;
  line-height:1.333333em;
}

article .at.ngp-form fieldset.TicketInformation table tr td {border-bottom:1px solid var(--main-rgb-biscuit);}

article .at.ngp-form fieldset.TicketInformation table tr.ticketTotals td {border:0;}

article .at.ngp-form fieldset.TicketInformation table td select {margin:0;}

article .at.ngp-form footer.FooterHtml {
  margin:0;
  padding:0;
  width:100%;
}

article .at.ngp-form footer.FooterHtml p {
  font-size:.75em;
  margin:0 0 15px;
}

article .at.ngp-form footer.FooterHtml p:last-child {margin:0;}

/* Advocacy Stuff */
article .at.ngp-form section.logo-container + section.logo-container,
article .at.ngp-form .inline-elements + .inline-elements,
article .at.ngp-form .inline-elements + figure.progress-meter {display:none;} 

/* Advocacy Override */
article .at.ngp-form fieldset.at-fieldset.AdvocacyFields {padding:0 10px 20px;}

article .at.ngp-form fieldset.AdvocacyFields .at-legend-with-submit {
  display:flex;
  flex-direction:column;
  padding:20px 0 10px 0;
  width:calc(100% - 20px);
}

article .at.ngp-form fieldset.AdvocacyFields .at-legend-with-submit .at-secondary-submit {
  margin:0 0 20px;
  order:0;
  width:auto;
}

article .at.ngp-form fieldset.AdvocacyFields .Subject0 .Subject {
  border-top:1px solid var(--main-grey);
  font-weight:700;
  margin-top:10px;
  padding-top:20px;
  font-size: 18px;
}

article .at.ngp-form fieldset.AdvocacyFields .Subject0 .Subject:before {
  content:"Subject:";
  padding-right:5px;
}

article .at.ngp-form .at-targets {background-color:var(--main-rgb-biscuit);}

article .at.ngp-form .at-targets {padding:10px;}

article .at.ngp-form .at-targets figure {margin:10px;}

article .at.ngp-form .at-targets .at-target-image {border-radius:0;}

article .at.ngp-form fieldset.AdvocacyFields .Message0 textarea {
  background:var(--main-white);
  padding:15px;
}

/* Impact Statements */
article .at.ngp-form fieldset.ContributionInformation .form-type-radios.form-item-selectamount {width:100%;}

article .at.ngp-form .explainers {
  padding:0 10px;
  width:100%;
}

article .at.ngp-form .explainers .explainer {
  background:var(--main-red-gradient);
  color:#fff;
  display:none;
  font-size:1.111111rem;
  font-weight:600;
  line-height:1.4em;
  padding:20px;
  position:relative;
  text-align:center;
  width:100%;
}

article .at.ngp-form .explainers .explainer strong {
  color:#fff;
  font-size:1.333333rem;
  font-weight:700;
}

article .at.ngp-form .explainers .explainer.displayed {display:block;}

/* eCard Stuff */
article .at.ngp-form .at-ecards .at-ecard {
  border:0;
  border-radius:0;
  display:block;
  height:unset;
  margin:0 0 20px;
  width:100% !important;
}

article .at.ngp-form .at-ecards .at-ecard .at-ecard-img {
  border:5px solid var(--main-dark-grey);
  border-radius:0;
  height:auto;
  overflow:auto;
}

article .at.ngp-form .at-ecards .at-ecard.selected .at-ecard-img {
  border:5px solid var(--main-red);
}

article .at.ngp-form .at-ecards .at-ecard-img img {
  left:unset;
  max-height:unset;
  position:relative;
  top:unset;
  transform:none;
  width:100%;
}

article .at.ngp-form .at-ecards .at-ecard input {
  display:none;
}

article .at.ngp-form .at-ecards button.at-preview-ecard {
  font-size:1rem;
  margin:0 0 20px;
  min-height:48px;
  width:100%;
}

/* EFT Section */
article .at.ngp-form fieldset.PaymentInformation .at-eft-accepted-here {
  display:flex;
  flex-wrap:wrap;
  margin:0;
}

article .at.ngp-form fieldset.PaymentInformation .at-eft-accepted-here > label,
article .at.ngp-form fieldset.PaymentInformation .at-eft-accepted-here > label.authorize-payment-label {width:100%;}

article .at.ngp-form fieldset.PaymentInformation .at-eft-accepted-here select.eft-input {width:100% !important;}

article .at.ngp-form .at-row label a.at-whatsthis {line-height:20px;}

/* Payment Method Buttons */
article .at.ngp-form .PaymentMethodSection .at-payment-method-buttons .at-btn-radio-wrapper label {
  align-items:center;
  display:flex;
  justify-content:center;
}

article .at.ngp-form .PaymentMethodSection .at-payment-method-buttons .at-apple-pay-button-wrapper label {border:0;}

/* Error States */
article .at.ngp-form label small.error {
  color:red;
  font-size:.875rem;
  font-weight:500;
  line-height:1.285714em;
  margin-bottom:10px;
  padding:0;
}

article .at.ngp-form label.error select,
article .at.ngp-form label.error input:required::placeholder {color:var(--main-grey);}

/* Pages Content */
article .at.oa-page {width: 100%;}

/* Lightbox */
.lightbox-modal.at-modal .at-modal-inner {
  border-radius:25px;
  max-width:600px !important;
}

.lightbox-modal.at-modal header a.lightbox-close {
  display:block;
  top:5px;
  right:10px;
}

.lightbox-modal.at-modal .at-modal-inner header > div {
  color:var(--main-text-color);
  font-size:1.5rem;
  font-weight:700;
  line-height:1.125em;
  max-width:100%;
  padding:20px 35px;
  text-align:center;
}

.lightbox-modal.at-modal .at-lightbox-content-wrapper p {
  font-size:1rem;
  line-height:1.5em;
  margin:0 auto 15px;
  text-align:center;
}

.lightbox-modal.at-modal button.lightbox-accept-button {
  font-weight:700;
  margin:0 auto;
  max-width:300px;
  padding:10px 20px;
  text-transform:none;
}

.lightbox-modal.at-modal .at-modal-inner footer .at-footer-content {padding:10px 20px;}

.lightbox-modal.at-modal footer a.lightbox-decline-button,
.lightbox-modal.at-modal .at-modal-inner footer div.lightbox-footer {color:var(--main-text-color);}

.lightbox-modal.at-modal footer a.lightbox-decline-button {font-weight:700;}


/* Footer */
footer.theme-footer {
  background-color:var(--main-text-color);
  color:var(--main-white);
  padding:0;
  position:relative;
  width:100%;
}

footer.theme-footer .footer-container {
  margin:0 auto;
  padding:0px;
  position:relative;
  width:100%;
  z-index: 1;
}

footer.theme-footer .footer-container.extended {background-color:var(--main-biscuit)}

body.background-biscuit footer.theme-footer .footer-container.extended {background-color:var(--main-white)}

footer.theme-footer .footer-container:before {
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/footer-decoration-black.svg);
  background-repeat:repeat-x;
  background-position:top center;
  background-size:cover;
  content:"";
  display:block;
  height:100px;
  position:absolute;
  top:-20px;
  width:100%;
  z-index: 0;
}

footer.theme-footer .footer-container.extended:before {
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/footer-decoration-biscuit.svg);
}

body.background-biscuit footer.theme-footer .footer-container.extended:before {
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/footer-decoration-white.svg);
}

footer.theme-footer .footer-container .footer-container {
  margin:0 auto;
  max-width:840px;
  padding:0px;
  position:relative;
  width:100%;
}

footer.theme-footer p.attribution {font-style:italic;}

footer.theme-footer figure.branding {
  margin:0 auto;
  width:200px;
}

footer.theme-footer figure.branding a {text-decoration:none;}

footer.theme-footer figure.branding img {
  height:auto;
  width:200px;
}

footer.theme-footer figure.branding img.horizontal {display:none;}

footer.theme-footer figure.branding img.stacked {display:block;}

footer.theme-footer figure.branding figcaption {
  color:var(--main-red);
  font-weight:600;
  font-size:22px;
  line-height:30px;
  padding-top:8px;
  text-decoration:none;
}

footer.theme-footer p {
  font-size:16px;
  line-height:1.5em;
  margin:0 auto 16px;
}

footer.theme-footer p.disclaimer {text-wrap:balance;}

footer.theme-footer p strong {font-weight:700;}

footer.theme-footer p.privacy-policy {margin-bottom:8px;}

footer.theme-footer p.privacy-policy a {font-weight:700;}

footer.theme-footer p a {
  color:var(--main-white);
  text-decoration:underline;
}

footer.theme-footer p a:focus,
footer.theme-footer p a:hover {
  cursor:pointer;
  text-decoration:underline;
}

footer.theme-footer .social-media-links {
  display:flex;
  flex-wrap:wrap;
  gap:12px;
  justify-content:center;
  margin-bottom:16px;
}

footer.theme-footer .social-media-links a.icon {
  background-position:center;
  background-repeat:no-repeat;
  display:block;
  font-size:0;
  height:32px;
  margin:24px 20px;
  width:32px;
}

footer.theme-footer .social-media-links a.icon.facebook {background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/facebook-white.svg);}
footer.theme-footer .social-media-links a.icon.instagram {background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/instagram-white.svg);}
footer.theme-footer .social-media-links a.icon.x {background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/x-white.svg);}

footer.theme-footer .share-icons span a:hover,
footer.theme-footer .share-icons span a:focus {text-decoration:none;}

footer.theme-footer p.links a {
  font-weight:700;
  text-decoration:underline;
}

footer.theme-footer p.copyright {
  font-size:.777778rem;
  line-height:1.428571em;
}

/* Extended Footer */
footer.theme-footer .footer-container .content-container {
  background:var(--main-text-color);
  color:var(--main-white);
  margin: 0 auto;
  max-width:840px;
  padding: 60px 40px 60px 40px;
  width:100%;
  position: relative;
  text-align: center;
}

footer.theme-footer .footer-container.extended .content-container {
  background:var(--main-biscuit);
  color:var(--main-text-color);
  text-align:start;
}

body.background-biscuit footer.theme-footer .footer-container.extended .content-container {background:var(--main-white);}

footer.theme-footer .footer-container.extended .content-container p {font-size:18px;}

footer.theme-footer h2.extended-footer-title {
  font-family:var(--secondary-font-family);
  font-size:48px;
  font-weight:500;
  line-height:1.333333em;
  margin:0 0 32px 0;
  text-align:center;
  text-transform:uppercase;
}

footer.theme-footer figure.icon-container {
  margin:0 auto;
  max-width:400px;
  padding:0;
  text-align:center;
  width:100%;
}

footer.theme-footer figure.icon-container a {
  text-decoration:none;
}

footer.theme-footer figure.icon-container span {
  color:var(--main-text-color);
  display:block;
  font-size:2rem;
  margin:0 auto 16px;
}

footer.theme-footer figure.icon-container figcaption p {
  color:var(--main-text-color);
  font-size:.888889rem;
  margin:0;
  text-decoration:none;
}

footer.theme-footer figure.icon-container p.caption-title {
  font-family:var(--secondary-font-family);
  font-size:1.333333rem;
  font-weight:400;
  line-height:1.2em;
  margin:0 0 4px;
  text-underline-offset:2px;
}

footer.theme-footer figure.icon-container a:hover p.caption-title,
footer.theme-footer figure.icon-container a:focus p.caption-title {text-decoration:underline 1px;}

footer.theme-footer .extended-footer-container:before {
  background-image:url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/pre-ex-footer.svg);
  background-repeat:repeat-x;
  background-position:top center;
  background-size:contain;
  content:"";
  display:block;
  height:100px;
  position:absolute;
  top:-20px;
  width:100%;
}

/* Accordion Paragraphs */
section.footer-container.extended .accordion body-content {
  display: flex;
  flex-direction: column;
  gap: 24px;
  margin:0 auto;
  max-width: 840px;
  width:100%;
}

section.footer-container.extended .accordion details {
  border:0;
  border-bottom:2px solid var(--main-text-color);
  border-top:2px solid var(--main-text-color);
  margin:24px 0px;
  padding:24px 0;
  width:100%;
  display: grid;
}

section.footer-container.extended .accordion details summary {
  font-family:var(--secondary-font-family);
  font-size:28px;
  line-height:1.333333em;
  padding:0;
  text-transform:uppercase;
  width:100%;
}

section.footer-container.extended .accordion details summary {
  display:grid;
  gap:20px;
  grid-template-columns: 1fr 48px;
  position:relative;
}

section.footer-container.extended .accordion details summary:after {
  background-image: url(https://nvlupin.blob.core.windows.net/images/van/TSM/TSCAN/1/98937/images/standard_theme_25/chevron-right.svg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: 10px;
  background-color: black;
  content:"";
  cursor: pointer;
  display:block;
  height:48px;
  transform:rotate(90deg);
  width:48px;
}

section.footer-container.extended .accordion details[open] summary {margin:0 0 12px;}

section.footer-container.extended .accordion details[open] summary:after {transform:rotate(-90deg);}

section.footer-container.extended .accordion details summary::marker,
section.footer-container.extended .accordion details summary::-webkit-details-marker {
  content:url();
  background-color:var(--main-text-color);
}

section.footer-container.extended .accordion details[open] .accordion-item-content {
  margin:0 auto;
  max-width:760px;
}

section.footer-container.extended .accordion details[open] .accordion-item-content :last-child {margin-bottom:0;}

/* Fonts */
article .at.ngp-form .at-form *,
.lightbox-modal.at-modal * {
  font-family:var(--main-font-family);
  font-weight:400;
}

article .at.ngp-form .at-form strong,
.lightbox-modal.at-modal strong {font-weight:700;}

article .at.ngp-form .at-form .glyphicons {font-family:var(--glyphicons-font-family);}

/* Read More Option */
article .has-read-more .at.ngp-form header.HeaderHtml > *,
article .has-read-more .at.ngp-form header.HeaderHtml.show-all span.show-full-body {display:none;}

article .has-read-more .at.ngp-form header.HeaderHtml.show-all > *,
article .has-read-more .at.ngp-form header.HeaderHtml > p:first-child,
article .has-read-more .at.ngp-form header.HeaderHtml > span.show-full-body {display:block;}

article .has-read-more .at.ngp-form header.HeaderHtml > span.show-full-body:nth-last-child(2) {display:none;} 

article .has-read-more .at.ngp-form header.HeaderHtml > span.show-full-body {
    color:var(--main-red);
    font-family:var(--secondary-font-family);
    font-weight:500;
    text-decoration:underline;
    text-transform:uppercase;
    cursor:pointer;
  }

@media (min-width:360px) {
  /* Branding */
  header.theme-header section.header-image {height:250px;}
  
  figure.branding img {
  height:70px;
  width:321px;
  }
  
  /* eCard Stuff */
  article .at.ngp-form .at-ecards {
    display:flex;
    flex-wrap:wrap;
    margin:0 -5px;
  }
  
  article .at.ngp-form .at-ecards .at-ecard {
    margin:5px;
    width:calc(50% - 10px) !important;
  }
  
  article .at.ngp-form .at-ecards .at-ecard .at-ecard-img {
    border:5px solid var(--main-rgb-biscuit);
    height:auto;
    overflow:auto;
  }
  
  article .at.ngp-form .at-ecards button.at-preview-ecard {margin:20px 5px 20px;}
}

@media (min-width:500px) {
  /* Form */
  article .at.ngp-form .FastAction,
  article .at.ngp-form ol.at-steps {margin:0;}
  
  article .at.ngp-form .fastAction {border-radius:4px;}
  
  article .at.ngp-form ol.at-steps {padding:0px;}
  
  article .at.ngp-form ol.at-steps li.at-step a,
  article .at.ngp-form ol.at-steps li.at-step b {
    grid-template-columns:auto 1fr;
    gap:8px;
    padding:0;
  }
  
  article .at.ngp-form ol.at-steps li.at-step a span.step-title {
    padding:0;
    text-align:left;
  }
  
  article .at.ngp-form ol.at-steps li.at-step:not(:first-child) a,
  article .at.ngp-form ol.at-steps li.at-step:not(:first-child) b {margin:0 auto;}
  
  article .at.ngp-form .at-form-submit .step-prevNext .btn-at {padding:16px 24px;}
  
  article .at.ngp-form fieldset.ContributionInformation label.label-amount.incrediblyLong,
  article .at.ngp-form fieldset.ContributionInformation label.label-amount.veryLong,
  article .at.ngp-form fieldset.ContributionInformation label.label-amount.tooLong {width:calc((100% / 3) - 20px) !important;}
  
  /* Form Steps */
  article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before,
  article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {border-width:24px 0 24px 12px;}
  
  article .at.ngp-form ol.at-steps li.at-step a,
  article .at.ngp-form ol.at-steps li.at-step b {
    gap:8px;
    grid-template-columns:1fr 24px auto 1fr;
    height:48px;
    padding:12px;
    }
  
  article .at.ngp-form ol.at-steps li.at-step a:before,
  article .at.ngp-form ol.at-steps li.at-step b:before {grid-column:2 / 3;}
  
  article .at.ngp-form ol.at-steps li.at-step a span.step-title {grid-column:3 / 4;}

  /* eCard Stuff */
  article .at.ngp-form .at-ecards .at-ecard {width:calc((100% / 3) - 10px) !important;}
  
  article .at.ngp-form .at-ecards button.at-preview-ecard {width:auto}
  
  /* EFT Section */
  article .at.ngp-form fieldset.PaymentInformation .at-eft-accepted-here > label {width:calc(50% - 20px);}
  
  article .at.ngp-form fieldset.PaymentInformation .at-fields:before,
  article .at.ngp-form fieldset.PaymentInformation .at-fields:after {font-size:16px;}
  
  article .at.ngp-form fieldset.PaymentInformation .at-fields:after {left:32px;}
}

@media (min-width:600px) {
  header.theme-header section.header-image {height:400px;}
  
  article .at.ngp-form fieldset.ContributionInformation .at-radios {grid-template-columns:1fr 1fr 1fr;}
  
  article .at.ngp-form fieldset.ContributionInformation label.label-amount.label-otheramount {grid-column: span 3;}
}

@media (max-width:800px) {
  header.theme-header.logo .button {display:none;}
  
  article .article-content .at-inner .logo-container,
  article .article-content .at-inner .inline-elements {display:none;}
  
/* Advocacy double load */
article .has-read-more .at.ngp-form header.HeaderHtml > span.show-full-body {
    font-family:var(--secondary-font-family);
    font-weight:500;
    text-decoration:underline;
    text-transform:uppercas;
  }
  
  .image-background footer.theme-footer .footer-container.expanded {border-top:1px solid var(--main-orange);}
}

@media (min-width:801px) {
  .has-main-image main > section.background-image {
    background-attachment:scroll;
    background-position:50% 33%;
    background-repeat:no-repeat;
    background-size:cover;
    min-height:100%;
    position:fixed;
    width:100%;
    z-index:-999;
  }
  
  header.theme-header figure.branding {justify-content:flex-start;}
  
  header.theme-header figure.branding a {padding:32px;}
  
  header.theme-header figure.branding img {
    height:56px;
    width:363px;
  }
  
  .background-blue.image-inline header.theme-header,
  .background-blue.image-none header.theme-header {border-bottom:1px solid #fff;}
  
  header.theme-header section.header-container {display:none;}
  
  body.image-header header.theme-header section.header-container {display:block}
  
  body.image-header header.theme-header section.header-container {
    background-position:50% 33%;
    border:0;
    height:500px;
  }
  
  main.theme-content figure.branding {
    /*! justify-content:flex-start; */
    /*! max-width: 680px; */
    /*! padding: 0; */
  }
  
  .no-main-image header.theme-header {border:0;}
  
  .no-main-image main > section.background-image {
    background-attachment:scroll;
    background-position:50% 33%;
    background-repeat:no-repeat;
    background-size:cover;
    position:fixed;
    min-height:100%;
    width:100%;
    z-index:-999;
  }
  
  main article {
    background:none;
    display:flex;
    justify-content:left;
    margin:0 auto;
    padding:0px;
    width:100%;
  }
  
  .image-background main article {
    padding-top:160px;
    padding-bottom:80px;
  }
  
  .background-grey:not(.image-background) main article {padding-bottom:0px;}
  
  main.form-left article {justify-content:flex-start;}
  
  main.form-right article {justify-content:flex-end;}
  
  body.image-header main article {
    margin-top:-200px;
    padding-top:0;
  }
  
  main article section.article-content {
    background:#fff;
    border-radius:0px;
    max-width: 50%;
    position:relative;
    width:100%;
  }
  
  body.background-biscuit main article section.article-content {background:var(--main-biscuit);  }
  
  main article.two-columns section.article-content {max-width:1160px;}
  
  main.form-left article section.article-content,
  main.form-right article section.article-content {width:450px;}
  
  main.form-center article.two-columns section.article-content {max-width:1160px;}
  
  .logo-inline main article section.article-content .branding {display:block;}
  
  article .at.ngp-form section.at-inner {padding-top:0;}
  
  article .at.ngp-form header.at-title {padding-top:0px;}
  
  :not(.image-background,
  .has-secondary-background).logo-above article .at.ngp-form header.at-title {display:none;}
  
  article .at.ngp-form figure.inline-image {
    display:block;
    line-height:0;
    margin:0;
    padding:20px;
    position:relative;
    width:100%;
  }
  
  article .at.ngp-form header.at-title + figure.inline-image {padding-top:0;}
  
  article .at.ngp-form figure.inline-image figcaption {
    font-size:.888889rem;
    font-weight:500;
    line-height:1.5em;
    padding:5px 0 0;
    text-align:right;
  }
  
  article .at.ngp-form figure.inline-image img {
    border-radius:12px;
    height:auto;
    width:100%;
  }
  
  article .article-content > .logo-container {
    display:block;
    max-width: 600px;
    margin: 0 auto;
  }
  
  .no-main-image article .at.ngp-form header.at-sr-only + header.HeaderHtml {padding-top:20px;}
  
  .image-none.logo-above .at.ngp-form section.at-inner {padding-top:20px;}
  
  article .at.ngp-form .FastAction .fastAction {padding:10px 5px;}
  
  article .at.ngp-form.multistep-layout header.HeaderHtml,
  article .at.ngp-form.multistep-layout form {
    float:none;
    width:unset;
  }
  
  article .at.ngp-form fieldset.AdvocacyFields .at-fields {margin:20px 0 10px;}
  
  footer.theme-footer .extended-footer-container {grid-template-columns:1fr;}
  
  footer.theme-footer h2.extended-footer-title {grid-column:span 1;}
  
  /* Form Steps */
  
  article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before,
  article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {border-width:36px 0 36px 12px;}
  
  article .at.ngp-form ol.at-steps li.at-step a,
  article .at.ngp-form ol.at-steps li.at-step b {
    gap:unset;
    grid-template-columns:auto;
    height:72px;
    padding:15px 12px 9px 12px;
  }
  
  article .at.ngp-form ol.at-steps li.at-step a:before,
  article .at.ngp-form ol.at-steps li.at-step b:before {grid-column:unset;}
  
  article .at.ngp-form ol.at-steps li.at-step a span.step-title {
    grid-column:unset;
    grid-row:2 / 3;
  }
}

@media (min-width:1000px) {
  article .at.oa-page,
  article .at.ngp-form {
  max-width:600px;
  width:100%;
  margin: 0 40px 0 auto;
}
 
  main article section.article-content {padding: 48px 40px 60px 40px;}
  
  .image-background main:not(.form-center) article section.article-content {width:640px;}
  
  article .at.ngp-form .at-row.Country.PostalCode.City.StateProvince label {
    flex:1 175px;
    min-width:175px;
  }
  
  article:not(.two-columns) .at.ngp-form fieldset.ContributionInformation .at-radios {grid-template-columns:1fr 1fr 1fr;}
  
  article .at.ngp-form .at-form-submit .step-prevNext .btn-at {padding:16px;}
  
  article.two-columns .at.ngp-form .content.thankYou {padding:10px;}
  
  /* Form Steps */
  
  article .at.ngp-form ol.at-steps li.at-step.active:not(:first-child):before,
  article .at.ngp-form ol.at-steps li.at-step.active:not(:last-child):after {border-width:24px 0 24px 12px;}
  
  article .at.ngp-form ol.at-steps li.at-step a,
  article .at.ngp-form ol.at-steps li.at-step b {
    gap:8px;
    grid-template-columns:1fr 24px auto 1fr;
    height:48px;
    padding:12px;
  }
  
  article .at.ngp-form ol.at-steps li.at-step a:before,
  article .at.ngp-form ol.at-steps li.at-step b:before {grid-column:2 / 3;}
  
  article .at.ngp-form ol.at-steps li.at-step a span.step-title {
    grid-column:3 / 4;
    grid-row:1 / 2;
  }
}

@media (min-width:1200px) {
  article .at.ngp-form fieldset.ContributionInformation .at-radios {grid-template-columns:1fr 1fr 1fr;}
}

@media (min-width:1360px) {
  article .at.ngp-form.multistep-layout {margin: 0 40px 0 auto;}
  
  article .article-content > .logo-container {margin: 0 40px 0 auto;}
}

/* Custom Buttons */

article .at.ngp-form .at-venmo-button-container,
article .at.ngp-form .at-paypal-button-container{
  width:100%;
}
```