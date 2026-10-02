# Pragma Visual Reference Guide

This guide is a visual audit of the locally available reference sets: `Light Images/`, `Dark Images/`, the original Blog 1–6 graphics, and the current Blog 7–10 graphics. It operationalises the requirements in `message (2).txt` for future blog-image briefs. It is a style guide, not a source of product facts or data.

## Asset and product routing

| Asset set | Product assignment | Confidence | Visual evidence |
| --- | --- | ---: | --- |
| `Light Images/image1.png`–`image9.png` | PRODUCT_PRAGMA | High | White/pale backgrounds, muted blue/yellow cards, and lower-right `PRAGMA.` signature. |
| `Dark Images/image1.png`–`image7.png` | PRODUCT_1CHECKOUT | High | Charcoal backgrounds, electric-blue UI highlights, and `1Checkout by PRAGMA` lockup. |
| Blog 1, 3–6 graphics | PRODUCT_PRAGMA | High | Light editorial diagrams with the Pragma lower-right signature and supporting product themes. |
| Blog 2 graphics | PRODUCT_1CHECKOUT | High | Dark checkout-performance graphics and 1Checkout lockup. |
| Blog 7–10 graphics | PRODUCT_PRAGMA | High | Light D2C operational diagrams with the current lower-right Pragma wordmark. |

The two product identities are separate. They are not light and dark variants of the same system. Never carry a colour, logo lockup, motif, or compositional convention from one product into the other without explicit approval.

## Family A — Light operational explainer

**Product:** PRODUCT_PRAGMA  
**Reference members:** `Light Images/image1.png`–`image9.png`; Blog 1, 3–6 graphics; Blog 7–10 graphics.  
**Confidence:** High. The shared product signature, white/pale-blue canvas, clean operational diagrams, and blue/yellow accent hierarchy recur across the set.

### Defining characteristics

- Predominantly wide, landscape cards with generous white space and a simple left-to-right or centre-out reading path.
- A short, bold, dark-navy headline sits at the top or upper-left. Use sentence fragments or a question, not a paragraph.
- Flat/vector illustration with rounded cards, uniform thin outlines, simple line icons, dotted/curved connectors, and restrained isometric depth when a process needs it.
- Near-white or pale-blue canvas; dark-navy text/lines; saturated blue for action/flow; pale blue for containers; yellow for a key highlight; coral/red for a failure, risk, or negative state only.
- Common motifs: parcel, phone, shield, check, delivery truck, warehouse, customer, route pin, calendar, dashboard, card matrix, arrows, and process nodes.
- Suitable for a hero, workflow, decision ladder, evidence matrix, scorecard, or illustrative comparison. Use one clear job per image.

### Stable style prompt

`PRODUCT_PRAGMA light operational explainer; clean editorial flat-vector diagram on a near-white or pale-blue canvas; dark-navy typography and thin outline icons; bright-blue connectors and active states; pale-blue rounded cards; restrained yellow highlights and coral only for risk or failure; generous margins, simple left-to-right or centre-out visual flow, calm Indian D2C operations context, mobile-legible hierarchy, no stock photography, no 3D render, no invented brand elements.`

### Text, logo, and crop policy

- Reserve an upper-left or upper-centre text-safe zone for a short headline that can be typeset after generation. Keep any generated text to the absolute minimum needed to understand a simple diagram.
- Reserve the lower-right corner with clear space for the official Pragma wordmark. Add `logo.png` or an approved dark-navy wordmark treatment after generation; do not ask the image model to draw it.
- Keep the focal flow in the centre 70% of the canvas. This protects a 16:9 crop and keeps the image useful at mobile width.
- Produce heroes at least 1,200 px wide. In-body diagrams may be denser but cannot depend on tiny labels or colour alone.

### Best and poor uses

- Best: return/refund flows, RTO action ladders, logistics decisions, customer-support workflows, operational metrics, comparisons, and rollout scorecards.
- Avoid: photorealistic lifestyle scenes, dense unverified data charts, pixel-perfect product UI, or a dark 1Checkout-style payment experiment graphic.

## Family B — Dark checkout intelligence card

**Product:** PRODUCT_1CHECKOUT  
**Reference members:** `Dark Images/image1.png`–`image7.png`; Blog 2 graphics.  
**Confidence:** High. The same charcoal/black field, white line work, blue highlight treatment, and `1Checkout by PRAGMA` lockup are consistent across the set.

### Defining characteristics

- Wide, dark charcoal or black canvas with a high-contrast white headline, usually aligned left or upper-left.
- Electric/medium blue acts as the active state or typographic highlight. Use quiet blue-grey panels and fine white/grey outlines for cards and UI metaphors.
- Vector line-art, card grids, controlled infographic modules, large outline arrows, device outlines, simple icons, and sparse blue glows. It is more technical and conversion-oriented than the light system.
- Common motifs: checkout/payment cards, phone, cart, shield, transaction route, experiment arrows, funnel/pyramid, user-intent states, and comparison panels.
- Suitable for 1Checkout heroes, checkout-performance comparisons, address/form logic, payment fallback, A/B experiments, and conversion frameworks.

### Stable style prompt

`PRODUCT_1CHECKOUT dark checkout-intelligence graphic; charcoal-black landscape canvas; crisp white sans-serif display hierarchy; electric-blue emphasis, blue-grey information panels, thin white/grey outline icons and cards; sparse controlled glow, high contrast, precise conversion and payment-system metaphor, ample negative space, mobile-legible, no pale Pragma canvas, no yellow/coral operational palette, no stock photography, no fabricated interface or logo.`

### Text, logo, and crop policy

- Reserve upper-left space for a short white headline with a blue highlighted phrase; typeset it after generation when accuracy matters.
- Reserve a small lower-right logo-safe area. Add the supplied `1checkout-by-pragma.svg` post-generation; never replace it with `PRAGMA.` or ask the image model to imitate it.
- Keep cards and decision paths inside the central crop-safe area. Dark graphics must retain clear white/blue contrast in a small social thumbnail.
- Avoid paragraphs, fine-print statistics, or dense labels. If verified figures are necessary, add them in a design pass with a source note in adjacent article copy.

### Best and poor uses

- Best: progressive address capture, cart-stage delivery-promise logic, checkout friction, payment fallback, prepaid nudges, trust/risk controls, and experiment frameworks.
- Avoid: light operational return/warehouse diagrams, yellow striped checklists, human/parcel isometric scenes from the light system, or generic dark “cybersecurity” imagery.

## Universal factual and accessibility constraints

- Use only product capabilities, metrics, and data points verified in `Site Product Pages - Content (Edit 1).pdf` or an approved live Pragma product page. Mark product-reported outcomes in surrounding copy as vendor-reported.
- Do not invent a statistic, chart proportion, product UI, technical process, map, third-party logo, or factual relationship.
- An image should communicate one decision or relationship even when its text is not read. Use nearby article prose and the mandatory `*Alt text: …*` caption to provide the full explanation.
- Do not rely on colour alone. Use icon, placement, label, or connector differences for success/failure and comparison states.
- Avoid tiny details, low contrast, visual clutter, random lettering, misspelled labels, distorted people/hands, heavy gradients, incompatible shadows, texture noise, generic stock-image aesthetics, and watermarks.

## Image brief template

Use this before image generation:

```md
Product: PRODUCT_PRAGMA | PRODUCT_1CHECKOUT
Reference family: Light operational explainer | Dark checkout intelligence card
Visual purpose: [hero / workflow / comparison / decision ladder / scorecard]
Subject: [one operational decision]
Key elements: [3–6 verified objects or states]
Relationship or sequence: [left-to-right flow, comparison, or centre-out decision]
Focal point: [the one action, trade-off, or outcome]
Aspect ratio and target width: [e.g. 16:9, at least 1,200 px]
Text-safe zone: [position; post-typeset headline/labels]
Logo-safe zone: [lower-right; official asset added after generation]
Factual constraints: [approved product facts, any labelled illustrative values]
Elements to exclude: [product-family conflicts, unverified UI/data, long text]
```

## Final visual QA

- Product identity and reference family are explicit and correct.
- The image explains a specific section; it is not decorative filler.
- The intended product’s official logo is overlaid post-generation in its reserved safe area.
- The appropriate caption appears immediately below the image in the blog Markdown.
- The visual remains understandable at mobile width and supports a 16:9 crop.
- No unverified claim, data visualisation, product interface, or third-party branding has been invented.
