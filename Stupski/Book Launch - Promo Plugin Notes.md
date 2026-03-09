---
Client:
  - Stupski Foundation
Title: ' Video Lightbox Promo-Type - Scratch Notes - Working Doc'
Due Date: '2025-12-31'
Task Details: Finish QA
Link: https://stupski.org/wp-admin/post.php?post=6459&action=edit
Status:
  - In Progress
Last Edited: 2025-12-27T15:34
tags:
  - stupski
  - PromoPlugin
  - GlensBookLaunch

---

```javascript
<script src="/wp-content/uploads/stupski-control-book-pushdown/pushdown-countdown.js"></script>
```

```html
<template id="fs-pushdown-countdown">
  <div class="fs-promotion fs-promotion--pushdown-countdown">
    <div class="fs-promotion__inner">
      <div class="fs-promotion__inner__countdown" data-target-datetime="2026-03-10 00:00:01">
        <div class="fs-promotion__inner__countdown__element js-countdown-days"><div class="value" title="days"></div><div class="unit">DAY</div></div>
        <div class="fs-promotion__inner__countdown__element js-countdown-hours"><div class="value" title="hours"></div><div class="unit">HR</div></div>
        <div class="fs-promotion__inner__countdown__element js-countdown-minutes"><div class="value" title="minutes"></div><div class="unit">MIN</div></div>
        <div class="fs-promotion__inner__countdown__element js-countdown-seconds"><div class="value" title="seconds"></div><div class="unit">SEC</div></div>
      </div> <!-- /countdown -->
      <div class="fs-promotion__inner__copy">Ready to gain back <span class="highlight">control</span> ?</div>
      <div class="fs-promotion__inner__cta">
        <a
          href="https://www.amazon.com/Control-Glen-Galaich/dp/1394352425" 
          target="_blank" 
          class="fs-promotion__inner__cta__link"
        >Preorder CONTROL Now <img src="/wp-content/uploads/stupski-control-book-pushdown/control-book-icon.svg" /></a>
      </div>
    </div><!-- /inner -->
  </div><!-- /outer -->
</template>
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <link href="https://fonts.googleapis.com/css2?family=Chakra+Petch:wght@400;500;600;700&family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
    <!-- styles.css is injected by index.tsx -->
</head>
<body>
    <div id="app">
        <!-- Main Container -->
        <div class="main-container">
            <div class="banner">
                <!-- Background Gradient/Texture -->
                <div class="banner-bg-gradient"></div>
                
                <div class="banner-content">
                    <!-- Countdown Section -->
                    <div class="countdown-wrapper">
                        <!-- Days -->
                        <div class="time-block">
                            <div class="glass-panel"></div>
                            <div class="glass-sheen"></div>
                            <div class="time-content">
                                <span class="time-value" id="days">00</span>
                                <span class="time-label">Days</span>
                            </div>
                            <div class="bottom-highlight"></div>
                        </div>
                        <!-- Hours -->
                        <div class="time-block">
                            <div class="glass-panel"></div>
                            <div class="glass-sheen"></div>
                            <div class="time-content">
                                <span class="time-value" id="hours">00</span>
                                <span class="time-label">Hours</span>
                            </div>
                            <div class="bottom-highlight"></div>
                        </div>
                        <!-- Minutes -->
                        <div class="time-block">
                            <div class="glass-panel"></div>
                            <div class="glass-sheen"></div>
                            <div class="time-content">
                                <span class="time-value" id="minutes">00</span>
                                <span class="time-label">Min</span>
                            </div>
                            <div class="bottom-highlight"></div>
                        </div>
                        <!-- Seconds -->
                        <div class="time-block">
                            <div class="glass-panel"></div>
                            <div class="glass-sheen"></div>
                            <div class="time-content">
                                <span class="time-value" id="seconds">00</span>
                                <span class="time-label">Sec</span>
                            </div>
                            <div class="bottom-highlight"></div>
                        </div>
                    </div>

                    <!-- Main Text Section -->
                    <div class="text-wrapper">
                        <div class="text-content">
                    <span class="text-normal">Ready to gain back</span>       
                          
                          <span class="text-highlight">Control</span>
                            <span class="text-normal">?</span>
                        </div>
                    </div>

                    <!-- CTA Button Section -->
                    <div class="cta-wrapper">
                        <button class="cta-button">
                            <div class="btn-border"></div>
                            <div class="btn-inner-glow"></div>
                            <div class="btn-hover-fill"></div>
                            <span class="btn-text">Pre-purchase Book</span>
                        </button>
                    </div>
                </div>

                <!-- Mobile Header Text -->
                <div class="mobile-text">
                    Control Releases In
                </div>
            </div>
        </div>
    </div>
    <!-- script.js is injected by index.tsx -->
</body>
</html>
```

```css
@import "/wp-content/uploads/stupski-control-book-pushdown/pushdown-countdown.css";

/***  Colors & Font Family set here for ease of override  ***/
.fs-promotion.fs-promotion--pushdown-countdown {
  font-family: 'Poppins', sans-serif;
  background-color: rgba(12,32,51,1);
   color: #b6e97f;
}
.fs-promotion__inner__copy {
  color: inherit;
}
.fs-promotion__inner__cta__link {
    background-color: #b6e97f;
    color: #1f3245;
}
.fs-promotion__inner__cta__link:hover {
  color: #1f3245!important;
}
.fs-promotion__inner__countdown {
    border-color: inherit;
}
.fs-promotion__inner__countdown__element .value {
      color: #D1FAE5;
}
.fs-promotion__inner__countdown__element.unit {
    color: inherit;
}
```

```css
:root {
    /* Color Palette */
    --bg-page: #1f3245;
    --bg-gray: #0c2033; /* gray-900 equivalent */
    --cyber-dark: #131925;
    --cyber-panel: #b6e97f;
    --cyber-accent: #b6e97f;
    --text-highlight: #b6e97f;
    --text-dim: #b6e97f;
    --green-glow: #b6e97f;
    --glass-bg: rgba(182, 233, 127, 0.05);
    
    /* Fonts */
    --font-sans: 'apotek-variable', sans-serif;
    --font-tech: 'Chakra Petch', sans-serif;

    /* Shadows */
    --shadow-neon: 0 0 10px rgba(182, 233, 127, 0.2), inset 0 0 20px rgba(182, 233, 127, 0.05);
    --shadow-btn: 0 0 15px rgba(182, 233, 127, 0.3);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    /* Transparent background to allow placement over other content */
    background-color: transparent;
    font-family: var(--font-sans);
    margin: 0;
    padding: 0;
    width: 100%;
}

#app {
    width: 100%;
}

/* Main Container */
.main-container {
    width: 100%;
    /* Max-width removed to allow full screen span */
    max-width: 100%;
}

/* Banner Component */
.banner {
    position: relative;
    width: 100%;
    /* Adjusted heights for a bar look */
    height: 7rem;
    background-color: var(--cyber-dark);
    /* Removed border radius to be flush with edges */
    border-radius: 0;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
    overflow: hidden;
    display: flex;
    justify-content: center; /* Center the content wrapper */
    align-items: center;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    border-top: none; /* No top border needed if it's top of screen */
}

@media (min-width: 768px) {
    .banner {
        height: 8rem;
    }
}

/* Subtle Gradient Background */
.banner-bg-gradient {
    position: absolute;
    inset: 0;
    background: linear-gradient(to right, var(--cyber-dark), #1a2333, var(--cyber-dark));
    pointer-events: none;
    z-index: 0;
}

/* Content Layout */
.banner-content {
    position: relative;
    z-index: 10;
    width: 100%;
    /* Max width constrains the content while banner spans 100% */
    max-width: 1200px; 
    padding: 0 1.5rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;
}

@media (min-width: 768px) {
    .banner-content {
        flex-direction: row;
        gap: 0;
        padding: 0 2.5rem;
    }
}

/* Countdown Section */
.countdown-wrapper {
    flex-shrink: 0;
    display: flex;
    gap: 0.75rem;
}

@media (min-width: 768px) {
    .countdown-wrapper {
        gap: 1rem;
    }
}

.time-block {
    position: relative;
    width: 3.5rem; 
    height: 3.5rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

@media (min-width: 768px) {
    .time-block {
        width: 4.5rem;
        height: 4.5rem;
    }
}

/* Time Block Effects */
.glass-panel {
    position: absolute;
    inset: 0;
    background-color: var(--glass-bg);
    backdrop-filter: blur(2px);
    border-radius: 0.375rem; /* rounded-md */
    border: 1px solid rgba(182, 233, 127, 0.2);
    box-shadow: var(--shadow-neon);
    opacity: 0.8;
    transition: all 0.3s;
}

.time-block:hover .glass-panel {
    opacity: 1;
    border-color: rgba(182, 233, 127, 0.4);
}

.glass-sheen {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 50%;
    background: linear-gradient(to bottom, rgba(255, 255, 255, 0.05), transparent);
    border-top-left-radius: 0.375rem;
    border-top-right-radius: 0.375rem;
    pointer-events: none;
}

.bottom-highlight {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 1px;
    background: linear-gradient(to right, transparent, rgba(182, 233, 127, 0.3), transparent);
}

.time-content {
    position: relative;
    z-index: 10;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.time-value {
    font-family: var(--font-sans);
    font-weight: 700;
    font-size: 1.25rem; 
    color: #D1FAE5;
    text-shadow: 0 1px 2px rgba(0,0,0,0.1);
    letter-spacing: -0.05em;
    line-height: 1;
}

@media (min-width: 768px) {
    .time-value {
        font-size: 1.75rem;
    }
}

.time-label {
    font-family: var(--font-tech);
    font-size: 0.625rem; /* 10px */
    font-weight: 700;
    color: #b6e97f;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    opacity: 0.8;
    margin-top: 2px;
}

@media (min-width: 768px) {
    .time-label {
        font-size: 0.6875rem; /* 11px */
    }
}

/* Center Text */
.text-wrapper {
    display: none;
    flex-grow: 1;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0 1rem;
}

@media (min-width: 768px) {
    .text-wrapper {
        display: flex;
    }
}

.text-content {
    font-family: var(--font-sans);
    font-size: 1.5rem; /* 2xl */
    letter-spacing: 0.05em;
    color: #b6e97f;
    text-transform: uppercase;
    user-select: none;
}

@media (min-width: 1024px) {
    .text-content {
        font-size: 1.75rem;
    }
}

.text-highlight {
    font-weight: 800;
    color: var(--text-highlight);
    margin-right: 0.5rem;
    filter: drop-shadow(0 0 8px rgba(182, 233, 127, 0.4));
}

.text-normal {
    font-weight: 600;
    color: var(--text-dim);
}

/* CTA Button */
.cta-wrapper {
    flex-shrink: 0;
}

.cta-button {
    position: relative;
    padding: 0.6rem 1.75rem;
    background: transparent;
    border: none;
    border-radius: 9999px;
    overflow: hidden;
    cursor: pointer;
    transition: all 0.3s ease-out;
}

.cta-button:hover {
    box-shadow: var(--shadow-btn);
}

.btn-border {
    position: absolute;
    inset: 0;
    border-radius: 9999px;
    border: 1px solid var(--green-glow);
    opacity: 0.8;
    transition: opacity 0.3s;
}

.cta-button:hover .btn-border {
    opacity: 1;
}

.btn-inner-glow {
    position: absolute;
    inset: 0;
    border-radius: 9999px;
    background: linear-gradient(to bottom, rgba(182, 233, 127, 0.1), transparent);
    opacity: 0.5;
}

.btn-hover-fill {
    position: absolute;
    inset: 0;
    background-color: var(--green-glow);
    opacity: 0;
    transition: opacity 0.3s;
}

.cta-button:hover .btn-hover-fill {
    opacity: 0.1;
}

.btn-text {
    position: relative;
    z-index: 10;
    font-family: var(--font-sans);
    font-size: 1rem;
    font-weight: 500;
    color: #b6e97f;
    letter-spacing: 0.025em;
    transition: color 0.3s;
}

.cta-button:hover .btn-text {
    color: white;
}

/* Mobile Specific Text */
.mobile-text {
    position: absolute;
    top: 0.25rem;
    left: 0;
    width: 100%;
    text-align: center;
    font-size: 0.625rem; /* 10px */
    font-weight: 700;
    color: var(--cyber-accent);
    text-transform: uppercase;
    letter-spacing: 0.1em;
}

@media (min-width: 768px) {
    .mobile-text {
        display: none;
    }
}
```

Notes from Stef on requirements:

- [ ] QA today

**For development on Video 1 - Mike’s tasks would be:**

- Update the promo plugin styling to match the new “CONTROL” landing page design

  - Tayo wrote:

    > The current design draft is [here](https://www.figma.com/proto/zYcmbjxNLiA1AXuNtxr8z6/2025---Stupski-Foundation---Design-System?page-id=4201%3A9327&node-id=4273-432&starting-point-node-id=4273%3A432&t=b3ZWlv96Y4btRcHm-1). It isn’t finished yet, but it should be safe to use these styles for the lightbox. Attaching a screenshot of the current modal designs. What you would replicate is the close button, overlay, and call-to-action button style. I have a general working [example here](https://stupski.org/?page_id=6403&preview=true)as well if helpful, but it doesn’t show the updated styles. Here’s a [Devmode link](https://www.figma.com/design/zYcmbjxNLiA1AXuNtxr8z6/2025---Stupski-Foundation---Design-System?node-id=4492-1443&m=dev) as well to the Figma project.
    >
    > arrow.svg
    >
    > close.svg
    >
    > Screenshot_2025-12-15_at_3.54.23 PM.png
    >
    > Screenshot_2025-12-15_at_3.55.48 PM.png

  - Stef already created a promo using RAN’s video and vibe coded it to be responsive and updated the styling a bit - Mike can use the code from this working Promo:

    - [[4Site] Responsive Video Pop-up - For Mike to Use](https://stupski.org/wp-admin/post.php?post=6459&action=edit)

    - See promo in action here[ https://stupski.org/stef-test/](https://stupski.org/stef-test/)

- Once we have the video from Stupski, we can uploaded and update the code with the on-site URL.

- This is the most important video and the priority.

For development on Video 1 - Mike’s tasks would be:

Update the promo plugin styling to match the new “CONTROL” landing page design

Tayo wrote:

The current design draft is here. It isn’t finished yet, but it should be safe to use these styles for the lightbox. Attaching a screenshot of the current modal designs. What you would replicate is the close button, overlay, and call-to-action button style. I have a general working example hereas well if helpful, but it doesn’t show the updated styles. Here’s a Devmode link as well to the Figma project.

arrow.svg

close.svg

Screenshot_2025-12-15_at_3.54.23 PM.png

Screenshot_2025-12-15_at_3.55.48 PM.png

Stef already created a promo using RAN’s video and vibe coded it to be responsive and updated the styling a bit - Mike can use the code from this working Promo:

[4Site] Responsive Video Pop-up - For Mike to Use

See promo in action here <https://stupski.org/stef-test/>

Once we have the video from Stupski, we can uploaded and update the code with the on-site URL.

————-

**Old Scope - wait for updated information from Stef Jones**

1. Up to 9 hours estimated for initial development of the below requirements

2. Then, hand off to Stef in #1873 Strategy & QA during Glen's Book promo lightbox 1: Book Announcement and move to Waiting for Teammate to implement QA (there should be \~2 hours left on the task for any required improvements). Bugherd <https://www.bugherd.com/projects/488028/kanban>

3. Once improvements are made, then let Stef know so she can inform Claire (in this task)

Notes from Stef on requirements:

**For development on Video 1 - Mike’s tasks would be:**

- Update the promo plugin styling to match the new “CONTROL” landing page design

  - Tayo wrote:

    > The current design draft is [here](https://www.figma.com/proto/zYcmbjxNLiA1AXuNtxr8z6/2025---Stupski-Foundation---Design-System?page-id=4201%3A9327&node-id=4273-432&starting-point-node-id=4273%3A432&t=b3ZWlv96Y4btRcHm-1). It isn’t finished yet, but it should be safe to use these styles for the lightbox. Attaching a screenshot of the current modal designs. What you would replicate is the close button, overlay, and call-to-action button style. I have a general working [example here](https://stupski.org/?page_id=6403&preview=true)as well if helpful, but it doesn’t show the updated styles. Here’s a [Devmode link](https://www.figma.com/design/zYcmbjxNLiA1AXuNtxr8z6/2025---Stupski-Foundation---Design-System?node-id=4492-1443&m=dev) as well to the Figma project.
    >
    > arrow.svg
    >
    > close.svg
    >
    > Screenshot_2025-12-15_at_3.54.23 PM.png
    >
    > Screenshot_2025-12-15_at_3.55.48 PM.png

  - Stef already created a promo using RAN’s video and vibe coded it to be responsive and updated the styling a bit - Mike can use the code from this working Promo:

    - [[4Site] Responsive Video Pop-up - For Mike to Use](https://stupski.org/wp-admin/post.php?post=6459&action=edit)

    - See promo in action here[ https://stupski.org/stef-test/](https://stupski.org/stef-test/)

- Once we have the video from Stupski, we can uploaded and update the code with the on-site URL.

- This is the most important video and the priority.

#### 

[*SOW*](https://docs.google.com/document/d/1_RcWEm5C7SHUrgpvcIJhm0ClT-hz7Ve1W2CYycKYA0Q/edit?tab=t.0) (detailed copied below too)

This video light box will be a direct announcement from Glen, recorded and provided by a third-party vendor for 4Site for upload and use. Using the current 4Site Promo Plugin we will be creating this new feature light box which will be designed reflect the branding of “*Control”* and easily communicate with visitors.

**Functionality & Features**

- Video provided by the Stupski team

- Autoplay enabled on load, muted by default with optional audio toggle

- Support for both embedded and self-hosted video files

- Floating CTA button placed beneath the video (design link:[ example](https://cln.sh/Lg0J4J86))

  - CTA URL, copy, and color editable within the plugin editor

  - Option to hide the CTA when not needed

- Video-swap logic to support different video files for desktop (16:9) and mobile (9:16), pending budget

- Branded "close" (X) icon in upper right corner (color editable)

- Dimmed background overlay (color editable) to enhance focus

- Smooth open/close animations

- Easy admin experience to swap out or update video content

- Ideally a way to track video plays, views, and CTA clicks - however, not sure how much is possible without hosting the video on YouTube