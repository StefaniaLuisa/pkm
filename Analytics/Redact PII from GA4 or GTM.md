Update to ensure settings and GA4 are setup to not track PII

Then in GTM 

```javascript
{{CJS - Cleaned Page URL}}

function() {
  var sensitiveParams = ['token', 'email', 'EMAIL'];
  try {
    var urlObj = new URL(window.location.href);
    urlObj.searchParams.forEach(function(value, key) {
      sensitiveParams.forEach(function(param) {
        if (key.toLowerCase() === param.toLowerCase()) {
          urlObj.searchParams.set(key, '[REDACTED]');
        }
      });
    });
    return urlObj.href;
  } catch(e) {
    return window.location.href;
  }
}
```