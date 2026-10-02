# Pragma Blog Production Context — Current Standard

This file is the working production brief for the remaining Pragma blogs. It records the decisions implemented in `Blog 7.md` through `Blog 10.md`, alongside the deeper format study in `Blog Writing Blueprint.md`. Follow this file when drafting, revising, or generating assets; do not revert to a generic SEO-blog structure.

## Scope and sources of truth

- The six original sample blogs established the long-form structure, editorial visual system, CTA placement, FAQ treatment, and Markdown export style.
- `10 Topics& Keywords.md` supplies the planned topic, primary keyword, secondary keywords, product alignment, and commercial angle.
- `Keyword Dump - Anmol (Edit).xlsx` is the keyword source. Use relevant terms naturally; never force keyword repetition.
- `Site Product Pages - Content (Edit 1).pdf` is the primary source for Pragma product capabilities, data points, and product-specific proof. Use it especially in the TL;DR and Pragma product sections.
- Pragma’s applicable live product page may be used for additional approved product metrics. Attribute vendor-reported metrics as vendor-reported; do not turn them into universal benchmarks.
- Blogs 7–10 are the current live implementation examples. Preserve their improvements: product-grounded TL;DR facts, captions, external H2 links, PRAGMA-branded visuals, and matching FAQ schema.
- `Pragma Visual Reference Guide.md` is the detailed style audit of the available light and dark image references. Use it with this document whenever an image set is planned.

## Article structure and Markdown rules

- Target roughly 2,700–3,100 words, normally with seven visuals.
- Begin with the hero inside the H1: `# ![][image1]Full title`.
- Follow the H1 with two or three short opening paragraphs, one italic scope statement, then `![][image2]`, then a horizontal rule before the first H2.
- Use one physical Markdown line per prose paragraph and a blank line around headings, paragraphs, images, rules, lists, and code fences. Do not hard-wrap prose.
- Use an outcome-led H2 sequence: define the business problem, gather/segment evidence, build the operating framework, measure the trade-off, test/operationalise, explain the relevant Pragma product, then conclude.
- Use one H1 only. The main body normally contains 5–7 H2s and 10–15 H3s; exclude FAQs, TL;DR, FAQ schema, and Sources from those counts.
- H3 is the main subheading level. Use H4 only for a genuine condition, exception, calculation, threshold, or control; use H5 only for a brief, specific subdivision of an H4. Never use H6 or add lower-level headings merely to meet a count.
- Maintain the complete hierarchy: H1 → H2 → H3 → H4 → H5. Do not skip levels. H2 and H3 sections carry the substantive explanation; each H4 must be narrower and shorter than its parent H3, and each H5 must be narrower and shorter than its H4.
- Every H2 needs meaningful framing body copy before its first H3. Every H3 that contains H4s likewise needs a shared introduction before those children. Never stack headings without explanatory text between them.
- Read headings alone as a final outline: every child must clearly belong to its parent, and heading language must remain descriptive and consistent with the source article.
- Keep paragraphs practical and compact (usually about 25–65 words). Use bullets for signals, states, KPIs, and exclusions; use numbered lists only for an actual sequence.
- Put the visible FAQ section after the conclusion and CTA. Use six or seven high-intent questions and answers.
- Place `## **TL;DR**` after the visible FAQs, followed by `## **FAQ JSON-LD Schema**`, then `## Sources & Further Reading`. The JSON-LD questions and answers must faithfully match the visible FAQs in the same order.
- End with local image-reference definitions only, e.g. `[image3]: <Blog N-images/image3.png>`. Do not embed base64 assets in the blog.

## Heading and linking requirement

Every `##` section must contain one useful external research link and, where a relevant Pragma article exists, one natural internal link. The external reading link goes immediately below the H2 (after the blank line) as a useful resource sentence—not as a link dump. The internal link belongs in the body where it helps the reader continue the journey.

- Prefer official or primary sources: product documentation, government material, standards bodies, or the original platform documentation.
- Use the source only when it genuinely supports that section. Common approved examples in the current articles include Shopify help, India’s Department of Consumer Affairs, NIST AI RMF, Twilio Verify, Optimizely, Qualtrics, and Google’s FAQPage documentation.
- Do not force an internal link where there is no genuinely relevant article. Use a helpful Pragma blog/resource link rather than a homepage link.
- **Pragma product section exception:** the `How Pragma…` H2 must not contain any Pragma blog/internal article link. It may link only to the relevant product page (for example, RMS or RTO Suite), plus the required external research source.
- The external research links used in the article—including competitor links where used for research—must be collected in one `## Sources & Further Reading` section for that individual blog. Keep this section concise and do not cite a competitor as validation of a Pragma claim.

## Writing, evidence, and product-claim rules

- Lead with a concrete Indian D2C/e-commerce operating tension. Explain the decision boundary early; avoid promises that imply one universal answer.
- Define acronyms at first use, then stay consistent: Return to Origin (RTO), Cash on Delivery (COD), Average Order Value (AOV), Net Promoter Score (NPS), and so on.
- Treat a score as a decision aid, not a customer verdict. Favour the least-friction action: allow, correct, verify, offer an alternative, then restrict only when justified.
- Distinguish operational facts, illustrative figures, and vendor-reported outcomes. Label illustrative calculations clearly. A vendor-reported range is not a benchmark that applies to every merchant.
- Never claim results, customer stories, integrations, compliance, or product behaviour that cannot be supported by the supplied product pages.
- Use relevant keywords in the title, introduction, selected headings, body copy, FAQ questions, and TL;DR only when they sound natural. Do not add a keyword-stuffing section.

### Documented Pragma RMS facts available for relevant blogs

- Granular return eligibility and windows by SKU, category, and seasonal sale.
- Refund destinations including source, UPI, wallets, credits, and gift cards.
- Advanced exchanges covering SKU swaps, value variance, and style or size changes.
- Reverse AWB generation, retry/cancellation/regeneration flows, and multi-item clubbing.
- Nested return reason codes, reason-based media uploads for QC, and two-way OMS pass/fail updates.
- PIN-code-based courier allocation and routing to the nearest, source, or custom warehouse.

### Documented Pragma RTO Suite facts available for relevant blogs

- Pre-dispatch device and behavioural fingerprinting, address and PIN-code correction, and instant phone verification through OTP-less or Truecaller flows.
- Context-aware COD controls by order value, region, and user history, with dynamic rules for sales, festivals, and traffic surges.
- COD-to-prepaid workflows, payment fallback, and nudges through WhatsApp, SMS, or email; risk rules can be A/B tested.
- Automated NDR workflows, including confirmation/re-slotting through WhatsApp and SKU-, location-, sale-, or customer-specific reattempts.
- The product material reports a 25–35% COD-to-prepaid conversion range for its strategy. Attribute it as vendor-reported and never present it as a universal outcome.

### Documented 1Checkout facts available for relevant blogs

- Address intelligence supports history-based address suggestions, invalid/gibberish correction, and instant PIN-code validation; it can also map shipping cost by payment type and courier.
- Checkout supports UPI, cards, wallets, BNPL, prepaid nudges, and fallback/cascading payment routing; use only the payment methods relevant to the article.
- Funnel drop-off and gateway success/failure are available as real-time optimisation inputs, and checkout variations can be A/B tested.
- The product material claims checkout in under five seconds, auto-login for 65%+ of returning users, and instant address auto-fill for 8/10 shoppers. It also reports 15%+ more conversions and 30% fewer abandons. These are vendor-reported product claims, not universal benchmarks.

### Documented WhatsApp Business Suite facts available for relevant blogs

- Campaigns can be broadcast or segmented by PIN code, SKU, and lifecycle; journeys can be triggered in real time by orders, deliveries, and returns.
- The suite supports Click-to-WhatsApp ads, cart-recovery nudges, prepaid-first offers, address verification, and operations-aware suppression for customers in return/refund flows.
- Customers can browse, order, pay, and track in WhatsApp; catalogues can stay synced with SKUs, variants, prices, and collections. UPI/card payments and fallback links for failed gateways are listed.
- The product material reports 11× ROAS, 99%+ open rates, 15%+ more conversions, 40% cost savings, 75%+ automation of routine queries, and 13× faster agent resolutions. Each is a vendor-reported product claim and must be labelled accordingly.

### Documented ShipAxis facts available for relevant blogs

- Courier allocation can use PIN code, SKU, weight, payment mode, and historic performance; it can dynamically re-route for sales, surges, or courier outages.
- The delivery engine lists PIN-code-level TAT prediction, courier delay/NDR/RTO benchmarks, SLA-breach escalation, and live ETA recalibration.
- The product content lists risk-aware courier allocation, NDR-triggered confirmation/re-attempt/re-routing, multi-warehouse selection by proximity/stock/SLA, and cost/margin intelligence such as weight-discrepancy audits and invoice reconciliation.
- Native connections to 65+ Indian couriers, daily adaptive courier scoring, and models trained on millions of shipments are documented. The stated 18–25% lower shipping costs is a vendor-reported result, not a universal benchmark.

### Documented Pragma Omnichannel CRM facts available for relevant blogs

- Unified profiles can merge orders, returns, tickets, and campaigns, with identity stitching across channels, devices, and aliases plus real-time updates.
- CRM/JMS capabilities include lifecycle journeys triggered by carts, tickets, deliveries, and refunds; CTWA attribution from ad to chat to purchase; and suppression of promotions during return/refund flows.
- Conversation analytics lists FRT, AHT, CSAT, SLA, quality, and sentiment; support and commerce workflows include in-chat payments, fallback orchestration, and OMS/WMS synchronisation.
- The product content says it powers 1,500+ D2C brands and lists 10× faster resolution through the AI Copilot. Treat both as vendor-reported product claims.

### Product/topic routing for the remaining planned blogs

| Planned topic | Product evidence to prioritise | Required visual identity |
| --- | --- | --- |
| Progressive Address Capture to Improve Delivery Accuracy | 1Checkout address intelligence, checkout funnel data, and A/B testing | PRODUCT_1CHECKOUT / dark |
| Modelling Delivery Promise at Cart Stage in India | 1Checkout address intelligence and checkout context; do not claim ETA capabilities not documented for 1Checkout | PRODUCT_1CHECKOUT / dark |
| Message Timing Experiments to Improve COD Acceptance | WhatsApp segments, real-time triggers, COD/prepaid and cart-recovery flows | PRODUCT_PRAGMA / light |
| Broadcast Throttling to Prevent WhatsApp Account Blocks | WhatsApp segmentation, lifecycle journeys, and official Meta/WhatsApp policy sources | PRODUCT_PRAGMA / light |
| Reverse Routing Optimisation for Faster Returns | ShipAxis allocation/SLA/warehouse intelligence, plus RMS reverse-return facts where relevant | PRODUCT_PRAGMA / light |
| Predicting Repeat Purchase Probability Using CRM Data | Unified profile, lifecycle triggers, attribution, and conversation/customer context | PRODUCT_PRAGMA / light |

## Required TL;DR format

The TL;DR is not a generic recap. It must carry the most important verified product facts that are relevant to the article.

```md
## **TL;DR**

For [contextual external resource], see [source](https://example.com/).

[One concise recap of the operating decision and outcome.]

**Documented [RMS / RTO Suite] facts:** [Relevant, source-supported capabilities and any clearly labelled vendor-reported outcome.]

### **Key Takeaways**

• **Action-led label:** evidence-led takeaway.
• **Action-led label:** evidence-led takeaway.
• **Action-led label:** evidence-led takeaway.
• **Action-led label:** evidence-led takeaway.
• **Action-led label:** evidence-led takeaway.

### **How Pragma [Product] Supports [Outcome]**

[Two concise, product-grounded paragraphs.]

**Verified product proof point only**

[Explore Product](https://www.bepragma.ai/)
```

Keep exactly five takeaway bullets. The product subsection must stay useful and specific, not become a sales-page rewrite.

## Sources & Further Reading format

Create one source list for each blog, after FAQ JSON-LD and before image-reference definitions. This is the single research record for the article.

```md
## Sources & Further Reading

- [Official source or standard](https://example.com/) — used for [specific claim or framework].
- [Platform documentation](https://example.com/) — used for [specific workflow context].
- [Competitor resource, if used](https://example.com/) — used only as market/context research, not as proof of Pragma capability.
```

- Include every external research source used in the article, including competitor links.
- Use direct, stable URLs and identify why each source was used.
- Do not use this section as a generic resource dump, and do not make unsupported claims by association with a linked source.

## Visual system and image handling

Read `message (2).txt` and inspect the relevant extracted references before creating a new image set. There are two separate product identities—not one theme with inverted colours. Never mix their palettes, motifs, typography, compositions, or branding unless a cross-product visual is explicitly requested.

- **PRODUCT_PRAGMA / light system:** use the relevant references from `Light Images/`. This is Pragma’s light, muted-colour visual family. Current RMS and RTO Suite blog visuals follow this identity: explanatory flat/vector diagrams, rounded cards, thin line icons, short labels, and decision-oriented flows, matrices, scorecards, or comparisons.
- **PRODUCT_1CHECKOUT / dark system:** use the relevant references from `Dark Images/`. This is the distinct 1Checkout visual family with its own dark palette and product-specific treatment. Do not reuse the light Pragma palette, logo treatment, or compositional conventions here.
- For light Pragma visuals, use a white or very pale-blue canvas; navy type and line work; bright-blue primary accents/arrows; pale-blue cards; restrained yellow highlights; and coral/red only for loss, risk, or failure. This description does not authorise those colours for 1Checkout.
- Keep image text concise and legible. Never place essential paragraphs, citations, exact long copy, or invented UI labels inside an AI-generated image; reserve a text-safe zone if typesetting will be added later.
- Do not ask an image-generation model to recreate, approximate, or distort either product logo. For every new Pragma blog image, add the official `P R A G M A.` wordmark as a post-generation overlay at the lower-right, matching the existing Blog 7–10 dark-navy treatment and clear space. Existing images have already been updated with that wordmark.
- For 1Checkout, use only an official 1Checkout asset and its own approved lockup after generation; never substitute the Pragma wordmark.
- Images should clarify the argument rather than duplicate whole paragraphs.
- Use local numbered folders such as `Blog 11-images/` and name assets `image1.png` through `image7.png`.
- Retain all seven image roles unless the topic truly needs fewer:
  1. hero inside H1;
  2. opening journey/contrast after the italic scope statement;
  3. early diagnostic matrix, checklist, or example;
  4. core framework, calculation, or policy comparison;
  5. recovery/measurement/failure-state explanation;
  6. pilot, rollout, or operating scorecard;
  7. linked closing CTA before FAQs.
- Put every body image on its own line with blank lines around it.
- Add an italic caption directly below **every** displayed image, including the hero and linked CTA image, in this exact pattern: `*Alt text: Clear, specific description of the visual and its decision context.*`
- The caption must describe what is actually visible and explain the context. Do not use vague text such as “Pragma illustration.”
- Design for mobile and thumbnail resilience: keep the focal point in a crop-safe central area, use clear contrast, and do not make meaning depend on tiny details, subtle colour differences, or colour alone. Heroes should be at least 1,200 px wide and survive a 16:9 crop.
- Never fabricate data, statistics, product capabilities, interfaces, or factual relationships in an image. Supply verified facts and minimum required labels in the image brief.

### Image brief preflight

Before any new image is generated, state the product (`PRODUCT_PRAGMA` or `PRODUCT_1CHECKOUT`), selected reference family, visual purpose, subject, focal point, key elements and their relationship/sequence, aspect ratio, text-safe zone, logo-safe zone, verified factual constraints, and elements to exclude. Attach or inspect only references belonging to the selected product. Keep the composition balanced even if text and the official logo are added later.

## CTA, FAQs, and quality checks

- The conclusion is followed by the linked CTA image: `[![][image7]](https://www.bepragma.ai/#wf-form-bepragma_form)`, then its alt-text caption, then a horizontal rule, then FAQs.
- Use the relevant product page in the TL;DR CTA: RMS `https://bepragma.ai/product/rms`; RTO Suite `https://www.bepragma.ai/product/rto`.
- Before delivery, confirm:
  - main-body headings meet the 5–7 H2 and 10–15 H3 targets, with a valid hierarchy and meaningful introduction text before child headings;
  - every H2 has an external contextual link and a natural internal link where relevant, while the Pragma product section uses the product link only (no internal blog link);
  - every visible image has an adjacent italic `Alt text:` caption;
  - each visual uses either the approved light PRODUCT_PRAGMA family or the approved dark PRODUCT_1CHECKOUT family, never a hybrid;
  - every Pragma image has the official lower-right PRAGMA wordmark post-production overlay;
  - image references resolve to local assets;
  - FAQ JSON-LD parses and mirrors the visible FAQs;
  - all product facts appear in the supplied product content or an approved live Pragma product page;
  - the TL;DR includes relevant documented product facts and exactly five takeaways;
  - the article has one complete `Sources & Further Reading` list, including any competitor research link;
  - no universal or unsupported performance claim has slipped in.

## Current implementation reference

- `Blog 7.md` — Refund Timing Impact: Instant vs Delayed Refunds for Cash Flow and NPS (RMS).
- `Blog 8.md` — Tiered Return Windows: Build Category and AOV Rules That Protect Recovery Value (RMS).
- `Blog 9.md` — RTO Risk Scoring at Order Confirmation Stage: Build Decisions Before Dispatch (RTO Suite).
- `Blog 10.md` — Reducing RTO Without Lowering COD Conversions: A Customer-Preserving Framework (RTO Suite).

Treat these four as the live formatting and quality reference, with this document supplying the non-negotiable rules to carry forward.
