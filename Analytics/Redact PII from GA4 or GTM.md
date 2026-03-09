Removing PII within GA4:

In the context of **Google Analytics 4 (GA4)** and the screen you are currently viewing, **parameter values** are the specific pieces of information attached to an event that provide extra context about a user's action.

### What are Parameter Values?

Think of an **Event** as the "what happened" (e.g., someone clicked a link) and a **Parameter** as the "details" of that action.

- **Parameter Name:** The category of information (e.g., `page_location`).

- **Parameter Value:** The actual data collected (e.g., `https://example.com/checkout?email=user@email.com`).

Common examples include:

- `page_title`: The value might be "Home Page" or "Shopping Cart."

- `link_url`: The value is the specific URL of the link that was clicked.

- `search_term`: The value is whatever the user typed into your site's search bar.

---

### Can the @ symbol be deleted?

**Yes**, you can use the tool you are looking at to delete values containing the `@` symbol. This is a common practice to remove **Personally Identifiable Information (PII)**—like email addresses—that may have been accidentally captured in your URLs.

According to the [Google Analytics Help Center](https://support.google.com/analytics/answer/9940393?hl=en_US&utm_id=ad), here is how the "Only delete parameter values that contain the following text" feature works for your case:

1. **The Trigger:** By entering `@` in the "Enter text to match with" box, you are telling Google to look at the parameters you selected (like `page_location` or `page_referrer`).

2. **The Action:** Google will identify any value within those parameters that contains an `@` symbol.

3. **The Result:** Those specific values will be scrubbed from your historical data for the date range you selected (`Feb 22, 2026` to `Mar 8, 2026`).

**Important Note:** This process is **permanent**. Once the deletion request is processed, that data cannot be recovered. It is highly recommended to double-check that the `@` symbol doesn't appear in legitimate, non-private data (like a specific CSS class name or a tracking ID) before finalizing the request.

Would you like me to explain how to verify if PII is currently being collected in your other reports before you run this deletion?

---

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