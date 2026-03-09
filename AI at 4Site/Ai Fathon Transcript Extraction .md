Asked DIA

> What would be the best way to automatically extract the transcripts from Fathom into a specified folder on my computer - is thier a script, ai, or integration I can use for this?

You’ve got a few good options here, depending on how “no-code” you want this to be and what format you want on your computer. Let me walk through the practical paths I’d consider in your shoes, then I’ll recommend one.

**Key idea: get transcripts out of Fathom automatically**

Fathom exposes transcripts via its API and via integrations / webhooks. That means you don’t need to manually download anything; you just need something in the middle to:

1. Listen for “new transcript” from Fathom
2. Grab the transcript text
3. Save it somewhere you can sync to your computer (Google Drive, Dropbox, local folder, etc.)

Then your desktop sync client (Google Drive for Desktop, OneDrive, Dropbox, etc.) can mirror that folder onto your machine.

So the real question becomes: what tool do you want to use for steps 1–3?

**Option 1: Zapier + Fathom “New Transcript” (least code)**

This is the most straightforward “click-configure” option right now.

From the Zapier integration page, Fathom exposes a **“New Transcript”** trigger that fires when a meeting transcript is ready. [​⁠http://zapier.com/apps/fathom/integrations/transcript-downloader](http://zapier.com/apps/fathom/integrations/transcript-downloader)

Here’s how I’d approach it:

1. In Zapier, create a new Zap.
2. Set **Trigger app** to Fathom, and choose the **“New Transcript”** trigger.
3. Connect your Fathom account using your Fathom API key (under Fathom Settings → API Access).
4. For the **Action**, choose where you want the file:
   - Google Drive: “Create File” in a specific folder (e.g., ‎⁠/Fathom Transcripts/⁠), using the meeting title as the filename and the transcript as the file content (plain text or Google Doc).
   - Dropbox / OneDrive: similar “create file” action.

As long as you have the corresponding sync client installed on your computer (for example, Google Drive for Desktop pointing at that folder), those transcript files will show up automatically in a specified folder on your machine.

Pros:
Very little technical setup, robust, easy to tweak (add date in filename, add metadata, etc.).
Cons:
Zapier pricing / task limits, and you are relying on a third-party SaaS.

This option also plays nicely with AI-in-the-middle if you want to transform the transcript before saving (e.g., an AI summary as the top section, raw transcript below) by inserting an “AI by Zapier” or OpenAI step before the “Create File” action.

**Option 2: [Make.com](http://Make.com) webhook + Fathom API (more control, still no-code-ish)**

The Substack tutorial you have open describes almost exactly what you want, just aimed at Notion. [​⁠https://aimaker.substack.com/p/ai-meeting-assistant-notes-fathom-notion-clickup-make-com-chatgpt-tutorial](https://aimaker.substack.com/p/ai-meeting-assistant-notes-fathom-notion-clickup-make-com-chatgpt-tutorial)

Fathom can send transcripts directly to a webhook in [Make.com](http://Make.com). From there you can:

1. Trigger: **Fathom → “Watch New Recording”** module in Make
   - Configure it to “Include transcript”.
2. Action: Write a file into a synced cloud folder:
   - Google Drive module → “Upload a file” or “Create a document from text”
   - Name the file ‎⁠{{Meeting Title}} – {{Date}}.txt⁠ or similar, and put the transcript in the body.

Again, your Google Drive / Dropbox sync client handles getting those onto your local machine.

Pros:
More flexible than Zapier, cheap/free at modest volume, good if you later want branching flows (send to Notion, task system, etc.).
Cons:
Slightly steeper learning curve than Zapier; more knobs and dials.

**Option 3: Use Fathom’s API directly and a local script (most control, most technical)**

If you prefer to avoid third-party automation tools, you can write a small script that runs on a schedule on your machine, uses your **Fathom API key** to fetch transcripts, and saves them directly to a local folder.

Conceptually:

1. Script calls Fathom API’s “list recordings” endpoint (with your API key).
2. For each recording that has a transcript and hasn’t been saved yet:
   - Call “get transcript” endpoint.
   - Save it as a ‎⁠.txt⁠ or ‎⁠.md⁠ file under ‎⁠\~/FathomTranscripts/⁠.
3. Mark it as “downloaded” locally (e.g., a small SQLite DB or a JSON file with IDs).

You could run this via:

- A Python script on a cron job (macOS/Linux) or Task Scheduler (Windows).
- Node.js script if you prefer JavaScript.

Pros:
No automation SaaS dependency, full control over file naming, structure, and privacy.
Cons:
You have to maintain the script and handle authentication / pagination, etc., yourself. Also requires Fathom API docs and a bit of dev time.

If you want, I can sketch a Python script skeleton that handles “fetch latest transcripts and save as files”, but I’d treat that as a second step after deciding that this is the direction you want.

**Option 4: n8n workflow to Google Docs (self-hosted or cloud)**

There is an existing n8n workflow specifically for **converting Fathom meeting transcripts to formatted Google Docs with AI summaries**. [​⁠https://n8n.io/workflows/9549-convert-fathom-meeting-transcripts-to-formatted-google-docs-with-ai-summaries/](https://n8n.io/workflows/9549-convert-fathom-meeting-transcripts-to-formatted-google-docs-with-ai-summaries/)

In practice that means:

1. n8n listens for new Fathom recordings / transcripts.
2. Uses AI to summarize and format.
3. Outputs a Google Doc in a chosen Drive folder.

If you like the idea of a slightly more “developer friendly” but still visual tool, and maybe self-hosting, this is a nice middle ground. Again, you would just point Google Drive’s sync folder at wherever those Docs are stored.

**So what’s “best” for your use case?**

Given how you work and the fact you’re already juggling a lot of tools, I’d recommend:

**Start with Zapier’s “New Transcript” trigger from Fathom and save to a synced cloud folder.**

That path gives you:

- Automatic capture from every Fathom call
- Files landing in a predictable folder on your machine
- Ability to later add AI transformation steps or routing into Notion / task tools without rewriting anything

If you’d like, the next thing I’d do is define a concrete structure, like:

- Folder: ‎⁠/Fathom Transcripts/Client/Org/⁠
- Filename pattern: ‎⁠YYYY-MM-DD – Client – Meeting Title.txt⁠
- File content: header with metadata, then transcript.

Then you can layer on search, summaries, or even a local knowledge base later.

> I'd actually like to move forward with option 3: Use Fathom’s API directly and a local script (most control, most technical) .
>
> I am pretty technical and think that I may be able to use Claude Cowork to do this, but what do you think about that idea? Is that possible?