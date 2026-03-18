---
pinned: false
Status: In Progress
external_files: codex
tags:
  - web dev
  - nerdy
Last Edited: 2025-11-19T17:27
Due Date: ''

---

SVG

```plaintext


<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M12 0C13.5923 0 14.3886 0.000173969 15.0569 0.0881696C19.6723 0.695853 23.3041 4.32761 23.9119 8.94309C23.9998 9.61147 24 10.4077 24 12C24 13.5923 23.9998 14.3886 23.9119 15.0569C23.3041 19.6723 19.6723 23.3041 15.0569 23.9119C14.3886 23.9998 13.5923 24 12 24C10.4077 24 9.61147 23.9998 8.94309 23.9119C4.32761 23.3041 0.695853 19.6723 0.0881696 15.0569C0.000173969 14.3886 0 13.5923 0 12C0 10.4077 0.000173969 9.61147 0.0881696 8.94309C0.695853 4.32761 4.32761 0.695853 8.94309 0.0881696C9.61147 0.000173969 10.4077 0 12 0ZM7.46206 8.56361L14.221 8.5692L6.85714 15.933L8.06696 17.1429L15.4309 9.77902V16.5435L17.1429 16.5379V6.85714H7.46206V8.56361Z" fill="#1F3245"></path>
        </svg>
```

# Markdown Notes for Callouts

Markdown itself doesn't define a standard "callout" (also called an info/warning note or admonition). Different Markdown renderers/extensions provide their own syntax. Here are the most common options and examples so you can pick the one that matches your renderer.

```plaintext
1. GitHub-style blockquote (works in any standard Markdown)

•	Use a blockquote with bold title to simulate a callout.
```

**Note:** This is a callout message.

It supports multiple paragraphs and lists.

```plaintext
2. Markdown with HTML (works where raw HTML is allowed)

•	Use an HTML &lt;div&gt; with classes for styling.
```

- &lt;div class="callout note"&gt;
- &lt;strong&gt;Note:&lt;/strong&gt; This is a callout message.
- &lt;/div&gt;
- 

```plaintext
•	You can style it with CSS in the containing page:
```

- &lt;style&gt;

- .callout.note { border-left: 4px solid #2b8aef; padding: 8px 12px; background:#f0f8ff; }

- &lt;/style&gt;

  3. Markdown with CommonMark/Admonition (used by many static site generators and docs tools)

  • Syntax (used by MkDocs Material, Sphinx with recommonmark or MyST, and some other tools):

- !!! note "Optional title"

- This is a callout message.

- !!! warning

- This is a warning callout.

  4. Markdown-it / VuePress / Docusaurus admonitions

  • Docusaurus and some Markdown-it plugins support the same triple-bang syntax:

- :::note

- **Note**

- This is a callout.

- :::

- Or the explicit admonition form:

- ::: warning

- **Warning**

- Content here.

- :::

  5. AsciiDoc-style admonition (if supported)

5. **[NOTE]**
6. **This is a callout.**

Which to use

```plaintext
•	If you're publishing on GitHub (README, issues, PRs), use the blockquote approach (#1).

•	If your documentation site uses MkDocs Material, Docusaurus, Sphinx with MyST, or similar, use the admonition/!!! or ::: syntax (#3/#4).

•	If you control the page HTML/CSS, use the &lt;div&gt; approach (#2) for full styling control.
```

If you tell me which Markdown renderer or platform you're using (GitHub, GitLab, MkDocs, Docusaurus, Obsidian, Notion, etc.), I can give the exact code and a styled example.

# :::note

Note

This is a callout.

---

## Read/Learn

- How to use Cursor: <https://cursor.com/en-US/docs>
- How to set up actions on my computer
- How to use Git propely
- How to code in WordPress
- UI/UX strategy & overall digital strategy

## Apps In Progress

- [Codex](https://chatgpt.com/codex)
- Client Dashboard

# **AI photo restoration tool:**

Kind of "free": Buy a GPU and DIY with FLUX.

---

API Demo

```python

import requests
import json

data = {
    'style': 'photo_mid',
    'scratch': '',
    'color': '',
    'input': 'YOUR_IMAGE_URL'
}

r = requests.post(
    url='https://jpghd.com/api/task/',
    headers={'X-API-KEY': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'},
    data=json.dumps(data)
)
print(r.json())

- data      is JSON format
- style     can by photo(Photo AI Enhance + Lossless Enlarge 4X), photo_mid(Photo AI Enhance + Lossless Enlarge 2X), photo_slim(Photo AI Enhance), art(Artwork Image AI Enhance + Lossless Enlarge 4X), art_mid(Artwork Image AI Enhance + Lossless Enlarge 2X), art_slim(Artwork Image AI Enhance)
- scratch   is Optional，set empty string will not repair scratch
- color     is Optional, set empty string will not colorize the photo
- livephoto is Optional, set empty string will not make magic photo
- return    status can be ok(means successed), conf_param_error(means conf parameter errors), exceed_limit(means api credits not enough)
```

# Read:

[Gitbook Agent - Possibilites!](https://gitbook.com/docs/gitbook-agent/what-is-gitbook-agent)