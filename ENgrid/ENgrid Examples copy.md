#4site/ENgrid #examples 

**Agenda: Design & Platform Examples Review**

Walk through concrete examples of how 4Site approaches **Engaging Networks forms**, **embedded experiences**, and **Marketing Tools email templates**, with a focus on conversion, flexibility, and long-term maintainability. These examples are meant to spark discussion about what patterns may be most effective for CLF’s goals.

- 4Site Reference Work

  - **Portfolio (visual grounding):**
    <https://www.4sitestudios.com/portfolio/>

- Single-Step Donation Layout Patterns

  - **Left-side column layout**
    Rainforest Action Network (RAN)
    <https://www.ran.org/donate/>

  - **Right-side column layout**
    Food & Water Watch (FWW)
    <https://www.foodandwaterwatch.org/donate/>

  - **Floating column layout**
    Amnesty International USA (AIUSA)
    <https://www.amnestyusa.org/donate/>

- Thank-You & Tribute / eCard Flows

  - **WWF Thank-You Gift (post-donation experience)**
    <https://support.worldwildlife.org/site/SPageServer?pagename=main_donation>

  - *(Note: confirm whether this is driven from an eCard template)*

  - **WWF Tribute eCard**
    <https://support.worldwildlife.org/site/SPageServer?pagename=donate_ecard>

  - **The Nature Conservancy (TNC) Tribute eCard**
    <https://preserve.nature.org/page/80429/donate/1>

- Single-Step Email-to-Target (Low-Friction Actions)

  - Example reference (generic ENgrid pattern):
    <https://act.everytown.org/signup/act/>

- Multi-Step Experiences

  - **Environmental Texas Two-Step Reference Page**
    <https://environmenttexas.org/action/tell-legislators-protect-clean-energy/>

- Embedded ENgrid Forms (Native Page Experience)

  - Embedded forms are styled to visually disappear into the page so they feel native rather than like a standalone form.

  - **Amnesty Urgent Action (Embedded Form Example)**
    <https://www.amnestyusa.org/urgent-actions/urgent-action-jury-voted-for-life-execution-scheduled/#take-actions>

  - **Supporting Outline / Technical Notes**
    <https://cln.sh/PMY3T0g9>

- Conversion-Focused Form Optimization Example

  - **PETA Donation Form (Monthly Giving Emphasis)**
    This redesign focused specifically on drawing more users into monthly giving, without changing any other page elements.

  - Demo link:
    <https://support.peta.org/page/70505/donate/1?mode=DEMO>

- Marketing Tools: Email Template Architecture

  - Email Template Strategy (MJML → HTML → EN Marketing Tools)

  - **Field Configuration Reference**
    <https://cln.sh/jY34ByBj>

  - **Developer Experience Reference**
    <https://cln.sh/4GWCrvZY>

  - **Content Admin Experience Reference**
    <https://cln.sh/NjD0TYrP>

  - **Litmus Proof Example (SPCAI)**
    <https://litmus.com/pub/proofs/WyFFUmtDUmNsY1QI>

  - **Internal Reference Document**
    <https://docs.google.com/document/d/1e4Y1-A3ucVTR-VwmT9v0b5ObCsmMtMwl9Py0FGomCKs/edit?usp=sharing>

Internal Dump of examples to clean up and provide:

<https://www.4sitestudios.com/portfolio/>

1. [**ENgrid Framework:**](https://engrid.4sitestudios.com/)

   1. Single Step (One-Column)

      1. [RAN - Left-Side](https://act.ran.org/page/90802/donate/1) Column

      2. [FWW - Right Side Column](https://give.foodandwaterwatch.org/page/81437/donate/1)

      3. [AIUSA - Floating Column](https://donate.amnestyusa.org/page/92978/donate/1?supporter.appealCode=W26XXWDEVR0HP&en_og_source=W26XXWDEVR0HP&ea.tracking.id=W26XXWDEVR0HP&_gl=1*zktohp*_gcl_au*NDUzNDg3MTQzLjE3NjM0MTI1NjY.*_ga*MTE4NTU3Njc5MS4xNzYzNDEyNTY2*_ga_3XY9JBWKR7*czE3Njg5NjIwOTEkbzExJGcxJHQxNzY4OTYyMDkzJGo1OCRsMCRoMA..)

      4. [WWF - Thank You gift](https://protect.worldwildlife.org/page/92201/donate/1) - Ask Bryan, is this created from a eCard template?

      5. WWF [eCard as Tribute](https://protect.worldwildlife.org/page/52883/donate/1?en_og_source=Web_Donation&ea.tracking.id=Web_Topnav&supporter.appealCode=AWE2604OQ18336A06078RX&_gl=1*1kjqtki*_gcl_au*MTI5ODA1NDE4Ny4xNzY2NDU0OTcx*_ga*NDM3ODkzMzY5LjE3NjY0NTQ5NzA.*_ga_FK6M9RK84Z*czE3Njg5NjIxNjgkbzQkZzEkdDE3Njg5NjI4NDMkajQyJGwwJGg5MTk0MjM2NDM.)

      6. [TNC - eCard](https://preserve.nature.org/page/146226/donate/1?mode=DEMO)

      7. [Single-step Email to Target ](https://act.oceana.org/page/170852/action/1?mode=DEMO)

   2. Multistep

      1. [ETT Two-step Reference Page](https://act.oceana.org/page/167959/action/1?mode=DEMO)

2. Embedded ENgrid Forms:

   1. Visually they disappear and just look like a native part of the page

      - Example: <https://www.amnestyusa.org/urgent-actions/urgent-action-jury-voted-for-life-execution-scheduled/#take-actions>

      - Outline: <https://cln.sh/PMY3T0g9>

   PETA wanted us to redesign the giving frequency selection to try and visually/emotionally draw more visitors into the monthly giving option.

   <https://support.peta.org/page/70505/donate/1?mode=DEMO>

   We weren’t allowed to change anything else so we made it in a way that it can be deployed onto their existing pages

   1. 

   Marketing Tools :

3. -- 4Site convincing NWF around the idea of using MJML &gt; HTML &gt; EN Marketing Tools Email Template
   -- 4Site's first large end-to-end development for marketing tools, had to do some trailblazing/discovery scoping
   ---- Code Architecture: Figure out what would be managed in code, versus in the Marketing Tools editor
   ------ Field Configuration: <https://cln.sh/jY34ByBj>
   ------ Developer Experience: <https://cln.sh/4GWCrvZY>
   ------ Content Admin Experience: <https://cln.sh/NjD0TYrP> 
   Litmus example from SPCAI - <https://litmus.com/pub/proofs/WyFFUmtDUmNsY1QI>

Why oh why did I not look at this first:

<https://docs.google.com/document/d/1e4Y1-A3ucVTR-VwmT9v0b5ObCsmMtMwl9Py0FGomCKs/edit?usp=sharing>