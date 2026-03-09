# PaintCare Site Locator - Content Plan

[Current Site Locator tool](https://www.paintcare.org/drop-off-sites/)

[Similar recycling locator for inspiration](https://www.productcare.org/recycling-locator/)

## Key Requirements of Project

- **Mobile experience**
  - Mobile to be designed first - then inform desktop
  - [Mobile Example - Sebrinia this design kinda somewhat reminded me of your wireframes - just figured I would share](https://cln.sh/Fh60j8wZ)
- **Improved Map Key/legend**
  - Needs to be seen sooner - above map - side of map?
  - Rework entirely, icons and how the map is described
- **Improved Search and filtering**
  - Have some ideas - and room for improvement/expansion
- **Improved/New map iconography**
  - They are not married to any of the current colors used at all nor the style
- **More Icons for Scalability**
  - Paint Bucket Icon
  - Aerosol Icon
- **Better use of space.**
  - The iframe is what is causing the black outline especially visible on Mobile
- **Spanish Translation**
  - Use of [Weglot Translation Plugin](https://www.weglot.com/) - which currently does not translate the front-end UI copy because everything within the current locator is passing to the WP site via a third party database
  - Current site does not translate key UI copy of the form - use Weglot to translate these front-end elements (submit, information etc.)
- **Better sync.** The FileMaker sync has broken down multiple times recently; let’s ensure the Wordpress plugin has a strong sync with the database and that users are trained in updating it to ensure a seamless sync.
- **Plugin Editing and ease of use:**
  - Ability to edit site all site
  - Ability to toggle visibility on/off fields
  - No need to reach out to a dev to make updates to the content that is available

#### Risk Areas for Scope Creep

- Any new filters are beyond scope
  - Scoped to keep the current filters as-is
  - If new filters are essential we should notify Paintcare and request additional budget
- FileMaker Sync Automation Exploration
  - Discovery around the idea of pulling data live from the web or using APIs to automate facility data updates was discussed as potential future enhancement, not scoped in current work.
- Map Base Redesign
  - Change of map base (e.g., Google Maps) is noted as possible but separate scope if design change is needed.
  - Could be a future enhancement
- Reuse & HHW Filter Rework
  - Whether to include HHW and Reuse as filters, these are still in flux and might require scope confirmation.
- API & Credential Work With DB Services
  - Coordination with third parties (DB Services, Incatech), if it involves out-of-scope effort by those vendors, that would need planning.

## Map Functionality

- Design wise and functionality we can keep as-is, if there is room to refine and we have the time we can think about different
- On state pages, the map should default to that state
- On national locator pages, show all states by default
- Similar map interaction as current but smoother state navigation
- Current mapping base (topographic-leaning) is acceptable
- Only switch to Google Maps unless there’s a *major technical benefit/time saving*

###### Non-PaintCare States - Out of Scope

- Do *not* actively show results from neighboring state if user is outside PaintCare state
  - Could we get away with “Find my closest location”
- Keep a label/indicator for non-PaintCare states
  - How can we elegantly solve this?

###### Notes from Meeting:

I**\~1:12–1:18 — Usability Issues With the Current Label**

- While navigating the map live, the group observes:

  - The label is **hard to notice**.
  - It is **not intuitive** how or when it appears.
  - The interaction for switching states is confusing.

- Someone notes that:

  - The label is **very small**.
  - Users may not understand why the label appears or what it means.

- There is agreement that **the label could be clearer and easier to understand**.

---

### **\~1:18–1:25 — Meaning and Messaging of Non-PaintCare States**

- The group discusses that the label:
  - Does **not explain why** the state is non-PaintCare.
  - Can be confusing because **locations are still shown** even though the state is not part of the program.
- It’s stated that the intent is to communicate:
  - This is **not an official PaintCare state**.
  - Information is shown as a courtesy.
  - Users should not assume they do not need the PaintCare program.

### **Navigation Between States**

- Concerns are raised about how **state borders work on the map**:
  - Current behavior requires users to actively cross borders.
    This interaction feels unintuitive.
- A suggestion is raised that users may expect to see:
  - The **closest location**, even if it is in another state.
- This leads into a clarification about program rules.

---

### **\~1:35–1:45 — Program Rules About Crossing State Lines**

- It is stated clearly that:

  - Users are **supposed to stay within their own state**.
  - The PaintCare fee is paid in the state where paint is purchased.

- However:

  - Enforcement is **not strict** in practice.
  - Cross-border drop-offs do happen, especially in areas like DC.

- Despite this:

  - The program does **not want to actively encourage** users to cross state lines.

### **\~1:45–1:55 — Design Implications for Non-PaintCare States**

- Stef asks whether, for a non-PaintCare state:
  - Users should be able to request “closest locations” even if those are in other states.
- The response:
  - The team prefers **not to explicitly offer or promote cross-border options**.
  - Passive exploration is acceptable.
  - The UI should **not push users toward another state**.
- It’s noted that:
  - This constraint is driven largely by **state politics and internal stakeholders**.

### **\~1:55–2:00 — Desired Outcome**

- Agreement that:

  - The non-PaintCare messaging should be **more intuitive**.
  - It should explain the situation more clearly without taking up excessive space.
  - A different presentation (label, popover, or messaging style) is preferred over the current implementation.

---

# Desktop Requirements

Some initial layout thoughts on how we can give this map an update:

- <https://cln.sh/Zk0NwqVW>
- <https://cln.sh/4jYqqTLZ> - When I saw these, it kind of stopped me in my tracks - could we use a sidebar with icons to assist with some of the search requirements/needs?
- <https://cln.sh/LzgJbLQJ> - Similar concept but accordion side-bars/listing area

## Legend

- Legend should be visible upfront (possibly above the map)
- Provide explanatory text for acronyms - tooltip (`Household Hazardous Waste`)
- Icons/legend should be intuitive and scalable

## Listing card Requirements

Data will be synced from FileMaker- but they would also like more flexibility to edit the copy themselves.

Main visible items before “more info” should include:

- Location Name
  - Address
  - Phone
  - Quantity limit (“limit up to X gallons” style copy)
  - Accepted products -
    - *show icons of what is accepted - I like [the tooltip they did here](https://cln.sh/29hVcPGt) so it is absolutely clear what the icons are*
      - *Paint bucket*
      - *Aerosol Can*
        - *Aerosol Can with an x to make sure that is clear?*
- Additional details go behind “More info” or overlay

**More information:**

- Address
- Website
- Hours
- Who Can Use This Program
  - *- I’d like to think of a better field name - something like:*
  - *Who Can Use These Drop-Off Locations*
  - *Program Eligibility*
- Further Information:
  - *This site does not accept aerosols (spray paint or other spray products), containers without original labels, or containers that are leaking or empty.*
  - Reuse Program
  - Household Hazardous Waste
    - *Could have these present at all times but greyed out when not a part of the program, then Paintcare can toggle in the backend which Programs are related and link out to them for more information.*
    - *- Maybe a tool tip when hovered to provide what ReUse Program is*
      - *“This site gives away for free -- or sells at a nominal cost -- some of the unused paint and other products that are dropped off by others. Please contact site for details.”*

## Search Filter

- **Search Bar Field**
- **Drop-down Selector Fields**
- **Products:**
  - **Reuse Program**
    - *We should add a tool-tip or someway to provide more information on what this is*
  - **Household Hazardous Waste (HHW)**
    - Same - tool tip if possible

**These are future options - they are beyond current scope:**

- Filter By:
  - Products
    - Bucket of Paint
    - Areosaul Can
      - Depending on design could the icons assist with search in some way
  - Quantity/Limit
    - Quantity filter should *highlight* instead of *exclude* results
- *Expandable Selectors? Sidebar?*
  - [*https://cln.sh/dSGFm2Qs*](https://cln.sh/dSGFm2Qs)
  - [*https://cln.sh/nYR03hg6*](https://cln.sh/nYR03hg6)