Absolutely. Here’s the “more Stef-authored” Reading Room Content Plan draft, restructured to match the 4Site Website Redesign Content Plan template you attached, and with the key Phase 1 framing, layering rules, taxonomy discipline, and intake and kickoff decisions woven into the right places so it reads like an intentional blueprint (not meeting notes).

---

## Intelligent tools to power engagement

## The Gambrell Foundation

## Reading Room Phase 1 Content Plan

### Quick Links

Content Plan, Production Task: [LINK]
Reading Room Phase 1 Scope of Work (Approved): [LINK]
Kickoff Notes and Recording: [LINK]
Reading Room Intake Questionnaire: [LINK]
Reading Room Book List + Content Tracker: [LINK]
Reading Room Sitemap / IA: [LINK]
Figma, Reading Room Mockups: [LINK]

---

## Table of Contents

Reading Room (Landing Page)
Reading Room, Constellation View
Reading Room, List View
Book Detail Overlay (Modal)
Book Page Template (Book Post)
Good Life Bingo (Prototype Page or Modal)
QR Friendly Access Pattern (Good Life Bingo)
Post Types
Site Navigation Placement
Footer Placement
Mockups
Development Notes
Additional Information and Features
Dynamic Content Functionality
Taxonomies and Terms
Content Governance and Editorial Rules
Appendix A: Book Content Template
Appendix B: Phase 1 Content Readiness Tracker

---

## Post Types

Book (Custom Post Type)
This is the core content unit of the Reading Room. It must be structured to scale cleanly from the initial 20–25 books to hundreds over time without forcing a redesign of fields, templates, or tagging.

Reading Room (Hub Page)
The unified landing environment that holds the constellation and list experiences, plus the curated modules that set context and invite exploration.

Good Life Bingo (Page or Modal Prototype)
A lightweight, on-brand prototype that connects Reading Room themes to real world actions, designed to work well for events and QR access.

Future Phase Considerations (not required for Phase 1)
Book Club Hub, Saved List functionality, additional media types beyond books. These can be planned for structurally now, but should not be treated as required Phase 1 content.

---

## Site Navigation

Recommended placement is a top level “Reading Room” entry, labeled plainly. The goal is discovery and return visits, not burying the experience under an abstract label. This also helps ensure the Reading Room is understood as distinct from News or Insights content.

Open discussion
Confirm where Reading Room sits relative to other Gambrell site sections, and confirm label preference.

---

## Footer

The Reading Room should be represented in the footer as an evergreen destination. Good Life Bingo can be included if Gambrell wants it to remain accessible outside event use, otherwise it can remain discoverable through the Reading Room experience and QR entry.

---

## Mockups

Phase 1 mockups to be created in desktop and mobile layouts, aligned to the approved SOW.

Reading Room landing experience (includes constellation and list browsing patterns)
Book detail overlay (modal)
Book page template
Good Life Bingo prototype

---

## Development Notes

The content plan is intentionally written to support Phase 2 development estimation. Wherever a section introduces dynamic behavior, filters, relationships, or overlays, it includes the content rules needed to scope the build accurately.

Core principle we are protecting
Books lead, interface recedes. The experience should reward curiosity, avoid gatekeeping, and never feel like homework. That principle affects content length, overlay density, taxonomy discipline, and the tone of commentary.

---

# Website Pages

## Reading Room (Landing Page)

### Page Details

Post Type: Hub Page
Proposed URL: /reading-room/
Primary audience: People who want to understand what Gambrell is reading and why, including Sally’s personal and professional network, peer foundations, nonprofit leaders, and curious visitors.

### Page Goal

The goal of the Reading Room landing page is to orient visitors quickly, invite exploration, and make it easy to browse without friction. This page needs to answer the most common entry question, “What is Gambrell reading?”, while also quietly communicating what makes Gambrell distinct: curiosity, rigor, and a human centered point of view.

This page should increase time on site by encouraging visitors to click through multiple books. A realistic success signal is that visitors explore at least 3–4 books in a session. When appropriate, the experience can offer low pressure pathways to stay connected, such as Book Club or a newsletter, without creating a contact funnel that invites unsolicited proposals.

### Section: Hero / Intro

Static evergreen content.

Why this matters
The hero is not a marketing banner. It is the on ramp that teaches visitors what they are looking at and how to explore it.

Content
Headline and short intro paragraph that frames the Reading Room as an invitation to learn with Gambrell, and explains that the experience is organized by themes and connections.
Optional “How to explore” line that sets expectations for Constellation View and List View.

Notes from meeting
We want curiosity and return visits, not a one and done experience. We also want to avoid language that encourages cold outreach about funding since Gambrell does not accept unsolicited proposals.

### Section: Essentials (Module)

Dynamic curated content.

Why this matters
Essentials are the anchor and the fastest way to communicate what this collection is fundamentally about. Essentials should feel intentional, not algorithmic.

Content
Short framing sentence defining what “Essentials” means at Gambrell.
Curated display of Essentials books.

Functionality notes
Essentials should be editorially controlled, not auto generated by date.

### Section: Staff Recommendations (Module)

Dynamic curated content.

Why this matters
Staff recommendations can add warmth and personality, but we should be thoughtful about whether the label is doing real work. If everything is recommended, we may want to instead use a “favorites” style badge or occasional spotlight, rather than treating this as a permanent category.

Content
If used, a curated selection of books plus simple attribution rules.

Open discussion
Confirm whether Gambrell wants staff recommendations as a visible module, or whether it is better framed as occasional spotlights.

### Section: Thematic Clusters Preview (Module)

Dynamic taxonomy driven content.

Why this matters
The clusters are what make the Reading Room legible. Without clear themes, the constellation becomes a beautiful but confusing map.

Content
Theme names and short descriptions, written consistently.
A short line that reinforces that themes are lenses, not rigid categories.

Notes from intake
Filtering should remain disciplined. The target is roughly 10 filter options to keep List View usable and to prevent taxonomy sprawl.

### Section: Constellation View Entry

Primary interaction entry.

Content
Minimal supporting copy that invites exploration and reinforces that clicking around is expected.

### Section: List View Entry

Accessibility and mobile first browsing entry.

Why this matters
List View is not a secondary experience. It is the primary experience for many visitors, especially on mobile and for accessibility.

Content
Short line that frames List View as a clean browsing alternative, with search and filtering.

### Open Question(s) and Notes

Hero direction, text only versus visual.
Where Book Club or newsletter CTA should appear, and how we phrase it so it feels welcoming but not like an invitation to pitch funding.

### Development and Design Considerations

Landing page should be modular so Gambrell can evolve emphasis without rebuilding templates.
Curated modules should remain curated. Taxonomy driven modules should remain rules based.

---

## Reading Room, Constellation View

### Page Details

Type: Primary interactive experience, accessed via toggle or dedicated view within /reading-room/
Primary audience: Desktop users and exploratory browsers.

### Page Goal

The goal of Constellation View is to make relationships visible. Visitors should be able to scan, hover, click, and understand that books connect to themes and ideas that connect to how Gambrell shows up in the world. This view should encourage playful exploration and clicking around.

### Section: Constellation Layout and Cluster Labels

Why this matters
If the constellation is purely visual without legible cluster framing, visitors will not know what they are looking at. We want wonder, not confusion.

Content requirements
Books must have a primary thematic cluster assignment.
Cluster labels and descriptions must be clear enough to orient first time visitors.
Essentials must be visually distinct and centrally positioned.

Notes from intake
Inspiration included Connected Papers as a reference for relational exploration. The Reading Room should take inspiration without inheriting complexity that makes the interface feel academic or intimidating.

### Section: Interaction Pattern and Content Density

Why this matters
We discussed layered interaction in kickoff for a reason. If everything appears at once, the experience becomes heavy. If nothing appears until deep clicks, the experience feels empty.

Layering rule
Hover or focus should reveal identity level information, like title and author, with clear accessibility support.
Click or tap should open the Book Detail overlay.
The overlay should offer a clear path to the full Book page.

### Open Question(s) and Notes

How much information is visible at rest versus on hover or focus.
Whether book covers appear as part of the constellation nodes, or primarily inside the overlay for performance and clarity.

### Development and Design Considerations

Accessibility needs to be designed in, including keyboard navigation, focus states, and non color dependent cues for relationships.
Performance matters, especially if we are rendering many elements at once.

---

## Reading Room, List View

### Page Details

Type: View toggle within /reading-room/ or dedicated route
Primary audience: Mobile users, accessibility first users, and visitors who want search and scanning.

### Page Goal

The goal of List View is clarity. It should make it easy to search, filter, and browse without interpreting the constellation. List View should still feel curated and on brand, but it must prioritize usability.

### Section: List Intro

Optional static copy that explains this view in one sentence.

### Section: Search and Filtering

Dynamic functionality.

Why this matters
Filters are only helpful if they are disciplined. Too many tags becomes noise, and noise reduces exploration.

Content requirements
Search across title, author, synopsis, and commentary.
Filters driven by primary thematic clusters, with a limited set of optional secondary tags.

Notes from intake
Target is a small number of filters, roughly 10, including high value distinctions like fiction versus nonfiction if that is meaningful to Gambrell’s collection.

### Section: Book Listing Cards

Dynamic listing.

Content requirements
Title and author.
Primary thematic cluster label.
Optional short synopsis preview for scanability.
Cover image can be used if it supports browsing without slowing the experience.

Open discussion
Whether the listing preview should show synopsis only, or synopsis plus a short commentary excerpt. My recommendation is synopsis for scanability, and save the Gambrell commentary for overlay and the full Book page to keep browsing fast.

### Development and Design Considerations

Filtering should remain fast and predictable.
List View needs to feel complete without requiring the constellation.

---

## Book Detail Overlay (Modal)

### Component Details

Type: Overlay launched from Constellation View and optionally from List View
Goal: Provide quick view context and a clean path to the full Book page.

### Component Goal

The overlay should help a visitor decide, “Do I want to read more about this book?” without turning into a full page. This is where we balance context with speed.

### Content Requirements

Cover image
Title and author
Thematic tags, including the primary cluster and a small set of secondary tags if used
Optional related books, only if it stays clean and meaningful
CTA to Learn More, which routes to the full Book page
Optional link to purchase, if Gambrell wants that as a consistent CTA

Notes from kickoff
We discussed “Recommended By” in the overlay and also noted the potential for it to create unnecessary tension or distract from the experience. The safest content plan is to support attribution structurally, but keep it off the overlay by default, and only display it if Gambrell explicitly decides it improves browsing.

Content integrity note
The overlay is not the place for long excerpts. If we include any copy beyond metadata, it should be a single sentence that stands on its own.

### Development and Design Considerations

The overlay must remain scannable.
Accessibility requirements include focus trapping, clear close behavior, and keyboard support.

---

## Book Page Template (Book Post)

### Page Details

Post Type: Book
Proposed URL: /reading-room/book/{slug}/
Primary audience: Visitors who want depth, and visitors arriving from search or external links.

### Page Goal

The Book page is where Gambrell’s voice matters most. It should provide a clean structure for synopsis and Gambrell commentary, support connections to themes and related books, and keep visitors exploring. This page also needs to protect Gambrell from content risk. We will not rely on third party synopsis scraping or long excerpts that could raise copyright issues. If we reference patterns from places like Goodreads or Amazon, it is for structure inspiration only, not for copying content.

### Section: Header

Title and author, plus cover image placement as determined by design.

### Section: Short Synopsis (Required)

This should be concise and factual. It explains what the book is.

### Section: Gambrell Commentary, “Why it matters” (Required)

This is the value of the Reading Room. It explains why Gambrell cares.

Why this matters
In kickoff, we explicitly called out that Gambrell commentary is essential. It keeps this from being a catalog, and it helps ensure the page is clearly transformative and not simply republishing book descriptions.

Guidance
Keep it short, warm, and specific. It should feel like a thoughtful recommendation, not an academic review.

### Section: Tags and Metadata

Primary thematic cluster displayed clearly. Secondary tags displayed only when used and limited.

### Section: Recommended By or Favorite Badge (Conditional)

If Gambrell wants attribution, the Book page is the best place for it. This keeps the overlay clean while still allowing the human layer.

### Section: Related Books (Optional)

Only include when relationships are meaningful. “More like this” should not feel random.

### Section: Related Gambrell Connections (Optional)

If relevant, link to related Gambrell programs, partners, or content. This supports the broader goal of showing how ideas connect to real world outcomes, but we should be intentional. We do not want this to become a pathway for unsolicited proposals.

### Section: External Links (Optional)

Optional purchase link and optional supporting links, used intentionally.

### Open Question(s) and Notes

Whether to include a “save this book” concept in Phase 2, similar to a saved list pattern, which could let visitors email themselves a list of books. This was discussed as a potential high value action, but it is not required for Phase 1.

### Development and Design Considerations

Only completed fields should display. Required fields must be enforced as part of editorial governance.
We should define character guidance so synopsis and commentary remain consistent and usable across views.

---

## Good Life Bingo (Prototype Page or Modal)

### Page Details

Post Type: Page or modal experience
Proposed URL: /good-life-bingo/ or nested under Reading Room, depending on IA decision
Primary audience: Event participants and visitors who want a playful, practical entry point.

### Page Goal

Good Life Bingo should feel inviting and shareable. It is a lightweight activation that helps visitors connect Reading Room themes to real world actions. Phase 1 is a prototype, so the goal is to establish the framework, tone, and visual system, not a full interactive game.

### Section: Bingo Grid

Content requirements
One complete 5x5 set of prompts.
Prompts should be action oriented, short enough for the square design constraints, and aligned to the Reading Room themes without feeling literal or preachy.

### Section: Framing Copy

Short intro that explains how to use the card, and why it exists. This should feel playful and welcoming, not like an instruction manual.

### Notes from intake

This needs to work well for QR based event entry. It should load quickly, be readable on mobile, and not require a complex navigation journey.

### Development and Design Considerations

Phase 1 is visual prototype only. Interactivity is a future phase option.
We should still write prompts in a way that supports future multiple boards or themed rotations.

---

## QR Friendly Access Pattern (Good Life Bingo)

### Component Details

Type: Short path entry to Bingo experience
Goal: Make event access frictionless.

### Development and Design Considerations

Mobile first, fast load, clear orientation.
If this is separate from the Reading Room navigation, we should still provide a simple path back to the Reading Room for visitors who want more.

---

# Additional Information and Features

## Dynamic Content Functionality

Curated dynamic
Essentials and any Staff Recommendations should be curated to remain intentional.

Rules based dynamic
List filtering and any related book logic can be taxonomy driven, but we need guardrails so it stays meaningful.

Character guidance
This is a content plan, but it also protects the UX. Short synopsis and brief commentary must remain brief so they work across List View, overlay, and full page.

## Taxonomies and Terms

Primary Thematic Clusters, required, one per book. This drives constellation placement and prevents books from living everywhere.
Secondary Tags, optional, limited. This supports filtering without noise.
Essentials flag or taxonomy term for center cluster membership.
Optional attribution fields, such as Recommended By or Favorite badge, supported structurally with conservative display rules.
Authors can be handled as a structured field, with search support in List View, rather than a dedicated filter unless needed.

Notes from intake
Events and Expeditions were discussed as possible metadata, but not a priority taxonomy driver for the initial version. If we include them, they should be treated as deeper layer metadata, not as top level filters.

## Content Governance and Editorial Rules

Definition of done for a Book
Cover image is final.
Synopsis is final.
Gambrell commentary is final.
Primary thematic cluster is assigned.
If these are complete, design and development can proceed confidently. Optional fields enhance, but they do not block Phase 1 planning.

Copyright and content integrity
Synopsis should be original, short, and factual.
Commentary must be original and clearly Gambrell’s perspective.
We should avoid pulling book descriptions from third party sources. Even when we reference external sites structurally, the content itself should be authored by Gambrell.

Audience and CTA discipline
Primary actions we want include adding books to a personal TBR, buying a book, and joining Book Club or a newsletter when appropriate.
We should avoid CTAs that encourage “contact us about funding,” since Gambrell does not accept unsolicited proposals.

---

# Appendix A: Book Content Template

- Book Title:

- Author:

- Edition or Year (optional):

- Cover Image: link or file, note if crop needed

- Primary Thematic Cluster (required):

- Secondary Tags (optional, limited):

- Essentials: yes or no

- Staff Recommendation or Favorite Badge (optional):

- Short Synopsis (required):

- Gambrell Commentary, Why it matters (required):

- Overlay Snippet (optional, single sentence):

- Related Books (optional, up to 3):

- Related Gambrell Connections (optional):

- External Links, including purchase link (optional):

- Notes or open questions (internal):

---

# Appendix B: Phase 1 Content Readiness Tracker

| Book Title | Author | Essentials | Primary Cluster | Secondary Tags | Cover Status | Synopsis Status | Commentary Status | Attribution | Related Books | Gambrell Connections | QA Status | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Book 01] | [Author] | Yes or No | [Cluster] | [Tags] | Not started, In progress, Final | Not started, In progress, Final | Not started, In progress, Final | [Optional] | Not started or Added | Not started or Added | Not reviewed, Needs edits, Approved | [Notes] |

---

If you want, I can also convert this into the same “PDF-ready” layout style as the website redesign content plan you shared, with the same visual cadence and spacing so it is ready to send to Gambrell as a formal deliverable. Let me know your thoughts and how you’d like to proceed!