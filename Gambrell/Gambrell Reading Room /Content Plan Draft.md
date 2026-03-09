Below is a draft Content Plan document in your voice, built directly off the approved Phase 1 SOW as the spine, with the key Kickoff and Intake context woven in so it reads like a clean blueprint (not a transcript). You can paste this into a Google Doc as-is, or keep it in Markdown for internal use.

---

# Gambrell Reading Room Phase 1 Content Plan

Prepared by 4Site Studios
Owner: Stef Jones
Version: Draft for internal review + Gambrell alignment

## Overview

Phase 1 is designed to end with approved designs and a detailed technical plan and estimate to guide Phase 2 development. The content plan is the foundation for both. It defines what content we need at launch, how that content is structured, how it appears across the Reading Room experience, and how Gambrell can keep the system sustainable as it grows beyond Phase 1.

The Reading Room is intended to be an interactive, narrative-driven experience that shows how ideas, books, and curiosity shape Gambrell’s worldview, grantmaking, and programming. The centerpiece is the constellation-style interface with Essentials anchored at the center and thematic clusters radiating outward, supported by a List View for accessibility and mobile browsing. This content plan aligns with that concept by defining a clear content model, taxonomy framework, and practical authoring rules so the experience feels cohesive, warm, and intellectually rigorous.

This content plan covers two Phase 1 scope areas together: the Reading Room and the Good Life Bingo prototype.

## What Phase 1 needs to launch truthfully

Phase 1 is design and planning only, but we still need “real” content to design against. The goal is to avoid designing an experience that only works with placeholder text, or building a structure that becomes difficult to scale when Gambrell adds more books later.

For Phase 1, we will plan and design around a launch set of approximately 20–25 books, including an “Essentials” subset. We will also plan for Staff Recommendations and an initial set of curated highlights for the “Gambrell Galaxy” contributions area. This is enough content to validate the constellation experience, test clustering logic, and confirm the Book Detail overlay and full Book page patterns. It also gives us the inputs required to produce an accurate Phase 2 development estimate.

Separately, Phase 1 includes a visual, on-brand Good Life Bingo prototype, using a 5x5 prompt grid and a QR-friendly access pattern for events.

## Content model: what a “Book” is in the Reading Room

The Book content model needs to support both the immediate Phase 1 experience and Gambrell’s longer-term goal of scaling to hundreds of books. The model below is intentionally structured so content is reusable across multiple views without requiring manual duplication.

### Required fields (must be completed to publish)

A book is “launch-ready” when every required field is complete and reviewed.

Cover image
This should be clean, high-quality, and consistent in aspect ratio across books. We will confirm target cropping guidance during design.

Title and author
These are treated as the book’s identity fields and are always displayed wherever the book appears.

Short synopsis
This is a brief description of the book itself. It should be concise and factual in tone, not a long excerpt. The synopsis supports scanning and comprehension, especially in List View and on the full Book page.

Brief Gambrell commentary (“why it matters”)
This is the heart of the Reading Room. It is Gambrell’s framing for why the book matters in relation to Gambrell’s worldview, programming, and curiosity. It should read as warm, human, and thoughtful, without becoming academic or overly long.

Tagging and metadata
Every book must be tagged so it can be meaningfully clustered and discovered. Tagging rules are defined in the taxonomy section below.

### Optional fields (display only when populated)

These fields deepen context but are not required for Phase 1.

Related books
Used to show meaningful connections and keep visitors exploring.

Related Gambrell programs or content
Used when a clear connection exists to a grant area, convening, expedition, or other Gambrell initiative.

Optional video
Used selectively. Not every book needs this.

Optional resource or purchase links
If included, these should be intentional and simple. The Kickoff conversation included the idea of linking out to a publisher page as an option, not a requirement.

Recommended By / staff attribution
This needs to be handled carefully. The SOW includes “Recommended By” as a category, and the overlay concept includes it as a potential element. In kickoff, we also discussed keeping the overlay light and not overloading it with metadata. The content plan approach is to support this field structurally, but to be intentional about where it appears. My recommendation is that “Recommended By” lives on the full Book page by default, and only appears in the overlay if Gambrell believes it adds immediate value to browsing.

##  Views

A recurring theme in kickoff was making sure the experience stays exploratory and intuitive without overwhelming visitors. The best way to achieve that is to explicitly define content layers across the Reading Room.

### Layer A: Constellation browsing

The constellation is visual-first. At this layer, we want visitors to scan, hover, and click with very low friction. Content should be minimal and identity-driven.

At minimum, we assume title and author are accessible in this view via hover or focus behavior, with the book cover used sparingly depending on design and performance decisions.

### Layer B: Book Detail overlay

The overlay is the “quick view.” It should help a visitor decide whether to open the full Book page. The SOW defines the overlay elements as cover image, title and author, thematic tags, related books, and a Learn More link, and it also lists “Recommended By” as a potential field.

The content plan assumption is that the overlay remains lightweight and scannable. Thematic tags belong here because they reinforce clustering logic and help the visitor understand why the book is placed where it is. Related books can work here if the UI remains clean and doesn’t become crowded.

For “Recommended By,” the plan is to support it, but treat it as optional at this layer, to avoid cluttering the browsing experience.

### Layer C: Full Book page

The full Book page is where deeper reading happens. This is where the synopsis and Gambrell commentary live in a clear, standardized layout. This is also the best home for Recommended By attribution, deeper metadata, optional video, optional links, and related Gambrell connections.

This layered approach supports two key goals discussed in kickoff: visitors clicking around and staying engaged, and visitors adding books to their own “to be read” list, without forcing heavy reading at every interaction.

## Taxonomy framework and tagging rules

Phase 1 includes defining a taxonomy framework that supports thematic organization and future growth. This is essential because the constellation experience only works if clustering and tagging are consistent.

The SOW calls out support for thematic clusters, Essentials, Staff Recommendations, and categories such as Authors, Events, Expeditions, Recommended By, and Related Content.

### Taxonomy types we will define in Phase 1

Thematic clusters
These are the primary drivers of the constellation structure. They represent the conceptual “zones” in the Reading Room.

Essentials
A designated subset of books anchored at the center of the constellation.

Staff Recommendations
A way to surface human curation beyond Essentials.

Authors
A structured taxonomy for browsing and future expansion.

Events, expeditions, related content
These support Gambrell-specific connections and future storytelling.

Recommended By
A structured field or taxonomy that supports attribution without being required to display everywhere.

### Tagging rules that keep the system clean

To keep the experience understandable, every book should have a single primary thematic cluster assignment that determines its constellation placement. Books can have secondary tags, but the primary cluster should be the anchor. This prevents books from feeling “everywhere” and makes the visualization coherent.

We will also set a practical cap on how many secondary tags are encouraged, so metadata remains useful rather than noisy. This cap can be confirmed once we see the real Phase 1 book set and how naturally the themes emerge.

We will refine final taxonomy labels collaboratively with Gambrell during Phase 1, with the explicit goal that the taxonomy works for Phase 1 and remains scalable for long-term growth.

## Reading Room landing page content modules

The Reading Room landing environment is the unified place where all components come together. The SOW defines the page as including a hero section (layout TBD with Gambrell), Essentials grouping, Staff Recommendations, thematic clusters, a Gambrell Galaxy contributions area (initial curated highlights), the Constellation View as the primary interactive experience, and the List View as an accessible alternative.

From a content planning standpoint, each module needs a clear content input and a clear owner.

Hero section
We will define the message, length, and tone once we decide whether the hero is primarily text-led or visual-led. The content goal here is simple: orient visitors quickly, set expectations for how to explore, and reinforce the “ideas shape outcomes” story without sounding like an academic archive.

Essentials grouping
This requires final selection of Essentials, plus a short framing message that explains what “Essentials” means in the context of Gambrell.

Staff Recommendations
This requires a defined set of recommended books plus a consistent way of framing why they were recommended. We will decide whether this is best represented through a short “recommended by” label, a consistent micro-note, or something that lives on the full Book page.

Thematic clusters
This requires final theme labels and a short description for each theme so clusters feel legible and intentional.

Gambrell Galaxy contributions
For Phase 1, this is “initial curated highlights.” Content needs include the items selected, how they are described, and what relationship they have to the Reading Room themes.

Constellation View and List View
Both views rely on the same underlying content model. The content plan role here is defining what appears in each view and confirming that the required fields support both experiences without compromise.

## Good Life Bingo prototype content plan

Phase 1 includes a Good Life Bingo prototype that connects Reading Room themes to real-world personal actions. Phase 1 is conceptual and visual, with potential interactivity in future phases.

The content we need for Phase 1 is straightforward but should be authored with consistency.

We need one complete 5x5 card of prompts. Prompts should be action-oriented, short enough to fit within the square design constraints, and aligned to Reading Room themes without feeling overly literal. We also want to avoid prompts that feel prescriptive or moralizing. The tone should feel inviting, playful, and thoughtful.

We will also define basic formatting rules so future Bingo boards can be authored quickly without redesigning the system.

## Content workflow, governance, and definition of done

The Reading Room will only succeed long-term if Gambrell can add and maintain content without friction. This section defines how we keep quality high and the system easy to operate.

Source of truth
We will identify where the canonical content lives during Phase 1 authoring (for example, a shared doc or sheet), and how it maps to the future site content entry process.

Drafting and review
We will identify who drafts synopses and who drafts the Gambrell commentary. Commentary likely requires the most care, because it carries voice and interpretation.

Definition of done for a book
A book is complete when required fields are populated, tagging rules are followed, and the commentary has been reviewed for clarity, tone, and consistency. Optional fields are only added when they materially improve the book’s usefulness.

Consistency guidance for commentary
Commentary should remain brief and human. The goal is to help a visitor understand why Gambrell cares about this book and what it connects to. It should not read like a grant description or an academic review.

## Phase 1 content readiness tracker

To keep Phase 1 efficient, we will maintain a simple tracker for the initial 20–25 books. This tracker will prevent churn and will make design review smoother because we can clearly see what content is “real” versus still in progress.

At minimum, each book row should track: cover image status, synopsis status, commentary status, primary theme assignment, secondary tags, and whether it is marked as an Essential. If Gambrell wants Staff Recommendations attributed, we will track that field as well.

## Open decisions we will finalize during Phase 1

The content plan intentionally captures a few decisions that are best finalized once we see the Phase 1 book set and design directions coming together.

Hero content direction
We will align on the role of the hero and the right balance of text versus visual.

Recommended By display rules
We will confirm whether “Recommended By” appears in the Book Detail overlay or is reserved for the full Book page by default.

Final taxonomy labels and cluster descriptions
We will lock taxonomy once we see the Phase 1 book set mapped to themes and can sanity-check that the clusters feel both intuitive and scalable.

---