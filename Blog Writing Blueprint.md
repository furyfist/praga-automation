# Pragma Blog Production Blueprint

## Purpose and evidence base

This is the house format for the ten planned topics in `10 Topics& Keywords.md`. It is based on a close structural and visual audit of `Blog 1.md` through `Blog 6.md`, not on a generic SEO template.

The samples are long-form operational explainers. They make one commercial decision legible, define the evidence needed to make it, show a framework or worked example, explain how to test it, then position the relevant Pragma product as an enabler rather than the proof of the argument.

Treat the rules marked **required** as the default production standard. The samples have small inconsistencies (for example, Blog 5 has five graphics, while most have seven), so do not copy accidental omissions such as an unlabelled schema block or an empty `##` heading from a single file.

## The measurable sample pattern

| Sample | Words | H1 / H2 / H3 / H4 / H5 / H6 | Direct image slots |
| --- | ---: | --- | ---: |
| Blog 1 | 3,010 | 1 / 9 / 24 / 7 / 1 / 0 | 7 |
| Blog 2 | 2,932 | 1 / 9 / 22 / 5 / 2 / 0 | 7 |
| Blog 3 | 3,045 | 1 / 8 / 19 / 8 / 0 / 0 | 7 |
| Blog 4 | 3,006 | 1 / 8 / 23 / 9 / 3 / 0 | 7 |
| Blog 5 | 2,586 | 1 / 8 / 19 / 2 / 0 / 0 | 5 |
| Blog 6 | 2,687 | 1 / 11 / 20 / 12 / 3 / 0 | 7 |
| **Working target** | **2,700–3,100** | **1 / 9–10 / 20–24 / 5–10 / 0–3 / 0** | **7** |

The hierarchy is intentionally dense but never arbitrary. Across the six samples:

- Every H1 is followed by an H2; do not skip directly from the title to an H3.
- H2s most often open into H3s. A second H2 follows only when the previous major section is complete.
- H3 is the workhorse level: it either contains one tight explanatory block or introduces a small H4 cluster.
- Use H4 for a decision rule, calculation, exception, numbered item, or important control that genuinely needs its own explanation.
- Use H5 sparingly for a caveat, test, or proof point nested inside an H4. Do not use H6.

The observed immediate successors reinforce this: H1 → H2 in all six articles; H2 → H3 is the dominant move (40 occurrences); H3 most often moves to an H3 sibling or back to an H2, and only sometimes opens an H4. This means the structure should read as a sequence of tight, parallel subtopics—not a deeply nested document outline.

### Line and spacing discipline

Each visible paragraph should be one physical Markdown line, followed by one blank line. Do not wrap prose manually at 80 characters. This is how the source exports are formatted.

Use this exact opening rhythm:

```md
# ![][image1]Article title in title case

Opening paragraph: a concrete commercial situation or failure mode.

Second paragraph: the hidden trade-off, cost, or risk.

*“Article Title” explains what the reader will measure, decide, or change.*

![][image2]

---

## First major question or decision
```

There are normally five to seven non-blank lines between H1 and the first H2: two or three short opening paragraphs, one italicised scope statement, image 2, and a rule. The title itself contains image 1. Keep one blank line around every heading, image, rule, list, and code fence.

For the body, the samples have a median of two non-blank lines between any heading and the next heading. In practice, that means:

- H2: one or two lead paragraphs before the first H3; occasionally a short list or image supports the lead.
- H3: usually one or two paragraphs, then either the next sibling or an H4 that breaks out a specific control.
- H4: one or two paragraphs, a compact list, formula, or visual; then move on.
- H5: one compact clarification only. It should never become a long section.

Longer stretches are allowed only for a genuinely useful worked example, checklist, formula, or numbered framework. Do not create a heading solely to force a word count.

## Required document skeleton

Use this sequence for every new article unless the topic makes a named section irrelevant. Keep the FAQ, TL;DR, product CTA, and schema as separate end sections.

````md
# ![][image1]Primary-keyword title: concrete commercial outcome

[2–3 short opening paragraphs]

*“Full title” explains [the decision, framework, or measurement outcome].*

![][image2]

---

## What the topic means / the hidden commercial problem

### Define the unit of analysis, journey, or decision

### Explain why a simple metric or default rule is misleading

## Find the evidence before changing the process

### Segment the relevant cohort or workflow

#### Define the calculation, evidence boundary, or exception

### Identify the costly failure mode

![][image3]

## Build the operating framework

### Present the decision ladder, policy, or model

#### Explain each intervention, threshold, or rule

![][image4]

### Add a worked example, comparison, or guardrail

![][image5]

## Test and operationalise the change

### Define baseline, control, success metrics, and rollback signal

### Explain ownership, monitoring, and exceptions

![][image6]

## How Pragma [product] supports [the outcome]

### Capability one, stated precisely

### Capability two, stated precisely

## To Wrap It Up: [action-oriented conclusion]

[1–2 conclusion paragraphs]

**Methodology note:** [only if illustrative numbers, external evidence limits, or an anonymous case need disclosure.]

[![][image7]](https://www.bepragma.ai/#wf-form-bepragma_form)

---

## FAQs (Frequently Asked Questions On [full article title])

### 1\. [Question]

[2–4 sentence answer]

[Repeat for 6–7 questions.]

---

## **TL;DR**

[One concise recap paragraph.]

### **Key Takeaways**

• **Action:** short evidence-led takeaway.  
• **Action:** short evidence-led takeaway.  
• **Action:** short evidence-led takeaway.  
• **Action:** short evidence-led takeaway.  
• **Action:** short evidence-led takeaway.

### **How Pragma [product] Supports [outcome]**

[Two short product paragraphs.] 

**Verified product proof point only**

[Explore Product](https://www.bepragma.ai/)

---

## **FAQ JSON-LD Schema**

```json
{ ...the same six or seven visible FAQs, in the same order... }
```

[image1]: <Blog N-images/image1.png>
...
[image7]: <Blog N-images/image7.png>
````

### Non-negotiable ending rules

1. The visible FAQ questions and the JSON-LD `name` values must match exactly. The visible answer and JSON-LD `text` must also match in substance.
2. Use six or seven FAQs, not filler questions. Each should answer a high-intent operational query that has not already been answered in exactly the same wording.
3. Keep the TL;DR after visible FAQs and before schema. It contains one recap paragraph and exactly five takeaway bullets in the samples.
4. The second product block is a concise CTA, not a second sales page. Use two paragraphs, one verified numeric or qualitative proof line, then one linked action.
5. End with image reference definitions. Use local paths such as `<Blog N-images/image4.png>`; never embed base64 in the Markdown.

## Writing and information-design rules

### Argument and voice

- Begin with a specific operational tension: lower refunds can harm trust; lower RTO can block good COD customers; the cheapest courier can cost more; a fast reply can still fail to solve the issue.
- Answer the title’s question early, then qualify it with the decision boundary. The samples avoid a universal promise where no reliable benchmark exists.
- Use clear Indian D2C/e-commerce context when relevant: COD, RTO, PIN code, UPI, affordable Android devices, NDR, reverse pickup, and payment-provider handoffs.
- Define specialised terms on first use. Then use the short form consistently: Return to Origin (RTO), Cash on Delivery (COD), Average Order Value (AOV), service-level agreement (SLA), and so on.
- Prefer practical verbs: segment, compare, validate, verify, model, test, monitor, scale, restrict, recover, reconcile.
- Be evidence-led and precise. Distinguish merchant-controlled delays from provider, carrier, telecom, or customer-action delays.
- Do not claim an invented universal benchmark, customer result, integration, percentage, or product capability. Mark worked figures as **illustrative** and add a methodology note when readers could mistake them for results.

### Paragraphs, lists, calculations, and links

- Keep prose paragraphs to roughly 25–65 words. A section normally has 1–3 paragraphs before it needs a list, visual, deeper heading, or transition.
- Use bullets for inputs, signals, exclusions, states, or KPIs. Use numbered lists only for chronological paths, prescribed sequences, or audit steps.
- Use bold only for consequential labels, metric names, thresholds, and carefully verified claims. Do not bold whole paragraphs.
- Use italics for the opening scope statement, an occasional methodology caveat, or a product name in a sentence. Do not italicise body prose for emphasis.
- Link Pragma’s relevant internal resource naturally inside a sentence when it adds a next step. Do not make a link dump. Use official or primary sources for external standards.
- Write formulas in plain Markdown lines; escape `=` as `\=` only when matching the sample export style. Explain every input immediately after the formula.
- Put dense comparison tables, matrices, scorecards, and flow diagrams in images rather than Markdown pipe tables. The samples’ data-heavy tables are visual assets, which keeps the article scannable and keeps the visual language consistent.

### Heading style

- H1 starts with the primary keyword or a recognisable variant and states the commercial question or outcome.
- H2s are outcome-led: `How to…`, `Why…`, `Build…`, `Calculate…`, `Test…`, `How Pragma…`, `To Wrap It Up…`.
- H3s name the discrete decision, cohort, system, calculation, or action.
- H4s sharpen a condition: `Use … when`, `Why … matters`, `Set … separately`, `Avoid …`.
- Use title case for core section titles, but use natural sentence case where it reads better as a real question. Preserve proper product spelling: `1Checkout`, `ShipAxis`, `WhatsApp Business Suite`, `Pragma RMS`, `Pragma RTO Suite`, and `Pragma Omnichannel CRM`.

## Visual system and image-placement rules

All 40 source graphics were reviewed visually. They are editorial diagrams, not decoration. Build a visual only when it clarifies a process, comparison, decision, state transition, or worked example that would be slow to parse in prose.

### Shared visual language

- White or very pale-blue canvas; navy headings and line work; bright blue arrows and primary accents; pale blue cards; yellow highlight behind the key phrase; coral/red only for loss, risk, failed state, or manual review.
- Clean flat/vector illustrations, rounded cards, thin outline icons, and short high-contrast labels. No photorealistic stock imagery.
- Most assets are 602 px wide. Use a wide hero or diagram (roughly 602×301–451); use a taller process flow or scorecard only when the content requires it.
- Put the `PRAGMA.` wordmark subtly at the lower-right. Product-specific creative can use the relevant product lockup (for example `1Checkout by PRAGMA`).
- Tables inside images use pale-blue headers, navy type, restrained grid lines, and only the information needed to make the decision.

### The seven image roles

| Slot | Placement | Required job | Source examples |
| --- | --- | --- | --- |
| `image1` | Inside the H1 | Hero: frame the central commercial tension in one phrase plus a simple process illustration. | `Same SKU. Why a Bigger Loss?`; `Are We Blocking Good Orders?`; `How WhatsApp Commerce Works`. |
| `image2` | After italic opening scope, before first rule | Orienting journey or contrast: show the before/after, major systems, or high-level flow. | Return during peak vs delayed return; one conversation’s eight systems; cheaper vs higher-rate courier path. |
| `image3` | Early body, after the first diagnostic/framework explanation | Decision table, checklist, or concrete in-context example. | SKU resolution matrix; mobile timing map; COD intervention matrix; WhatsApp product-selection screen. |
| `image4` | At the central framework/calculation section | Worked economics, policy comparison, scorecard, or key model. | Illustrative SKU economics; LCP/INP/CLS thresholds; delivery-contribution comparison; QA criteria. |
| `image5` | After the core model or failure-state section | Flow, recovery matrix, or measurement standard. | Return signals to action; wait-state diagnostic; payment/order failure recovery; refund conversation audit. |
| `image6` | Near testing/operationalisation or immediately before product section | Pilot scorecard, rollout metric set, allocation flow, or specific product proof visual. | Return pilot scorecard; RTO test metrics; courier-assignment flow; CRM social proof. |
| `image7` | After conclusion/methodology note and before FAQs | Linked closing CTA asset. In several exports it renders as an almost blank transparent/white field; retain the linked slot unless a supplied CTA asset replaces it. | Present in Blogs 1–4 and 6. |

Blog 5 proves that five images can work for a narrower economics article, but seven is the new default. Do not add empty visuals simply to hit seven; each must have a distinct explanatory role.

### Image-adjacent formatting

- Put the image on its own line with a blank line above and below.
- A visual can appear immediately after a section heading only when the heading itself introduces it (as in the ShipAxis product H2). Otherwise give readers one short orienting paragraph first.
- Never put a raw image URL in body text. Use `![][imageN]`, then put all reference definitions at the end.
- Do not repeat the full diagram text in the paragraph below it. Introduce what the reader should compare, then interpret the implication after the visual.

## Ten production briefs

The exact headings may be polished while drafting, but each article must preserve its primary keyword, commercial question, evidence boundary, product alignment, and visual plan below.

### 1. RMS — Instant vs Delayed Refunds: Impact on Cashflow and NPS

**Primary keyword:** `refund timing impact`  
**Secondary keywords:** `NPS ecommerce`, `customer satisfaction refunds`, `working capital`

**Core argument:** Instant refunds reduce waiting and may protect trust, but they release cash and can create loss exposure before pickup, receipt, QC, or fraud checks. Delayed refunds can protect recovery value but can damage NPS when the trigger is opaque or disproportionate. The policy should match refund timing to evidence, recovery risk, customer context, and promised service level.

**H2 sequence:** What instant and delayed refunds actually mean → Identify the cashflow and customer-experience exposure → Build a trigger ladder by product, evidence, and customer risk → Model the working-capital and NPS trade-off → Pilot timing changes with a control → How Pragma RMS supports configurable triggers → Wrap-up.

**Must cover:** approval, pickup scan, carrier scan, receipt, and QC as distinct trigger points; cash released; reverse-pickup completion; refunds issued but returns not received; complaints and repeat purchase; clear customer communication; a no-surprises policy disclosure.

**Seven visuals:** hero `Fast Refund or Safe Refund?`; customer-facing timing journey; trigger-decision matrix; illustrative cashflow comparison; evidence-to-refund flow; pilot metric scorecard; RMS CTA.

### 2. RMS — Building Tiered Return Windows by Category and AOV

**Primary keyword:** `tiered return windows`  
**Secondary keywords:** `AOV return strategy`, `high-value returns policy`, `category-based rules`

**Core argument:** One universal return window treats products with very different recovery curves as identical. A tiered policy can protect recovery and margin when it is based on category, seasonality, resale horizon, AOV, condition sensitivity, and operational feasibility—and when it remains transparent to the shopper.

**H2 sequence:** Why a universal window fails → Segment categories by recovery economics and AOV → Build window tiers and exceptions → Calculate the cost of delay versus customer friction → Test category rules and customer comprehension → How Pragma RMS supports eligibility/window configuration → Wrap-up.

**Must cover:** category versus AOV as complementary, not interchangeable, inputs; fashion/seasonal, hygiene-sensitive, serialised/high-value, and clearance examples; policy display at PDP and order stage; exchange availability; late-return exception handling; guardrails for inconsistent treatment.

**Seven visuals:** hero `One Return Window, Unequal Loss?`; recovery clock by category; category/AOV tier table; seasonal-resale worked example; decision tree for exceptions; pilot outcomes/complaints scorecard; RMS CTA.

### 3. RTO Suite — RTO Risk Scoring at Order Confirmation Stage

**Primary keyword:** `RTO risk scoring`  
**Secondary keywords:** `order confirmation analytics`, `checkout signals`, `COD validation`

**Core argument:** A score at confirmation is useful only when it selects a proportionate next action. It should separate known loss evidence from incomplete but repairable data, use observable signals, and be judged by delivered orders and contribution—not RTO rate alone.

**H2 sequence:** What a confirmation-stage RTO score should decide → Gather and segment customer/order/address evidence → Separate score bands from intervention actions → Define signals and decision ownership → Measure false positives and delivered-order economics → Test thresholds before rollout → How Pragma RTO Suite supports scoring and verification → Wrap-up.

**Must cover:** prior successful deliveries and confirmed RTOs, address completeness, PIN-code serviceability, order value, product/category, channel, and explainability; allow, validate, verify, prepaid nudge, restrict; a manual override path; reason codes; no black-box or discriminatory claims.

**Seven visuals:** hero `Which COD Orders Need a Second Check?`; inputs-to-score journey; risk-band/action table; confirmation-stage decision ladder; false-positive versus prevented-RTO comparison; threshold-test scorecard; RTO Suite CTA.

### 4. RTO Suite — Reducing RTO Without Lowering COD Conversions

**Primary keyword:** `reduce RTO without harming conversion`  
**Secondary keywords:** `COD optimisation India`, `payment mix strategy`

**Core argument:** This is a companion to Blog 3, but it must focus on preserving COD access and choosing low-friction interventions before restriction. A lower reported RTO rate is not success if profitable customers abandon checkout or move to an unaffordable payment route.

**H2 sequence:** Why blanket COD removal is a false win → Find cohorts with preventable RTO → Build a least-friction COD intervention ladder → Compare COD, prepaid incentive, verification, and restriction economics → Test payment-mix shifts and customer guardrails → How Pragma RTO Suite supports interventions/NDR recovery → Wrap-up.

**Must cover:** checkout conversion, COD share, prepaid migration, delivered-order conversion, contribution per eligible checkout, discounts/payment fees, complaints, and false-positive proxy; distinguish a helpful prepaid offer from hiding COD; consider post-dispatch NDR as a separate recovery layer.

**Seven visuals:** hero `Lower RTO. Keep Good COD Orders.`; COD journey with drop-off risks; intervention comparison table; illustrative payment-mix/contribution comparison; friction ladder; controlled-rollout metric panel; RTO Suite CTA.

### 5. 1Checkout — Progressive Address Capture to Improve Delivery Accuracy

**Primary keyword:** `progressive address capture`  
**Secondary keywords:** `delivery accuracy`, `address validation India`, `form UX`

**Core argument:** Asking for every field immediately can create form friction, while accepting incomplete data creates serviceability, delivery, and RTO problems. Progressive capture should collect only what is useful at each stage, validate it in context, and make the completion of a usable address visible to the shopper.

**H2 sequence:** What progressive address capture means → Identify address defects and their operational cost → Design the staged collection/validation sequence → Handle Indian address and PIN-code realities → Measure completion, correction, and delivery outcomes → Test the form without masking errors → How 1Checkout supports prefill and address correction → Wrap-up.

**Must cover:** phone-based recognition only where consent/availability allows; PIN code first or early serviceability checks; locality, house number, landmark, and address-type validation; editability; stored-address confidence; first-time versus returning shopper; invalid/ambiguous address fallback; do not claim that any single field guarantees delivery.

**Seven visuals:** hero `Less Typing, Fewer Bad Addresses`; staged address journey; field-by-field purpose matrix; address-validation decision flow; before/after completion and correction example; form test scorecard; 1Checkout CTA.

### 6. 1Checkout — Modelling Delivery Promise at Cart Stage in India

**Primary keyword:** `delivery promise modelling`  
**Secondary keywords:** `cart stage logistics`, `ETA accuracy`, `shipping logic`

**Core argument:** A cart-stage delivery promise is a probabilistic operational commitment, not a marketing label. It needs a defined cutoff, inventory/warehouse readiness, serviceability, carrier/lane evidence, payment method, and exception logic. Accuracy matters more than showing an aggressively early date.

**H2 sequence:** What a cart-stage promise must represent → List the data and ownership boundaries → Build ETA logic from readiness, location, lane, and cutoff → Handle uncertainty and promise ranges → Measure promise accuracy and conversion impact → Test a more precise promise versus a generic promise → How 1Checkout supports checkout-level collection/handoff → Wrap-up.

**Must cover:** destination PIN code, fulfilment node, stock availability, order time, weekends/holidays, carrier SLA, payment/COD readiness, and unserviceable locations; `dispatch ETA` versus `delivery ETA`; exact date versus range; missed-promise rate, delivery time, cart conversion, and support contacts.

**Seven visuals:** hero `Can the Cart Keep Its Delivery Promise?`; order-to-door input map; ETA calculation stack; precise-date/range/unknown decision table; illustrative promise-versus-actual cohort chart; experiment scorecard; 1Checkout CTA.

### 7. WhatsApp Business Suite — Message Timing Experiments to Improve COD Acceptance

**Primary keyword:** `WhatsApp timing optimisation`  
**Secondary keywords:** `COD acceptance rate`, `messaging A/B testing`, `behavioural nudges`

**Core argument:** Timing affects whether a confirmation message is seen, trusted, and acted on, but a message experiment must not confuse a send-time effect with audience quality, template wording, delivery failures, or opt-in differences. Optimise confirmed delivery and acceptance with frequency and customer-experience guardrails.

**H2 sequence:** Define COD acceptance and the timing hypothesis → Map the post-order customer journey → Design clean message-time experiments → Separate time, template, and audience effects → Measure acceptance, delivered orders, opt-outs, and complaints → Operationalise winning timings by cohort → How WhatsApp Business Suite supports triggered messaging → Wrap-up.

**Must cover:** valid opt-in and platform/template compliance; placed order versus dispatched order; send, delivered, read, click, confirmation, and final delivery timestamps; holdouts; local time; customer fatigue; no unsupported claims about WhatsApp rules or open rates.

**Seven visuals:** hero `When Should a COD Buyer Hear From You?`; order-to-confirmation timeline; experiment-cell matrix; timing versus acceptance illustrative chart; message-state/retry flow; rollout guardrail scorecard; WhatsApp Suite CTA.

### 8. WhatsApp Business Suite — Broadcast Throttling to Prevent WhatsApp Account Blocks

**Primary keyword:** `WhatsApp broadcast limits`  
**Secondary keywords:** `throttling strategy`, `bulk messaging compliance`, `spam prevention`

**Core argument:** Throttling is not merely a volume cap. It is a controlled send strategy that respects opt-in, template approval, engagement/reaction signals, audience recency, error response, and account health. The article must avoid inventing a universal numerical limit; official platform policies and account conditions change.

**H2 sequence:** Why high-volume sending becomes an account-health problem → Define the compliance and delivery boundaries → Build a throttling policy by audience and risk → Queue, pace, pause, and recover sends → Monitor quality signals and failure states → Test throughput changes safely → How WhatsApp Business Suite supports segmentation and automation → Wrap-up.

**Must cover:** explicit opt-in, template use, suppression lists, frequency caps, message relevance, opt-outs, failed sends, quality feedback, retry policy, queue ownership, audit trail, and incident response. Use official Meta/WhatsApp sources for any platform-specific rule.

**Seven visuals:** hero `More Sends, or More Risk?`; safe-send lifecycle; audience/recency throttle matrix; queue-and-pause flow; health-signal dashboard/table; controlled-volume test plan; WhatsApp Suite CTA.

### 9. ShipAxis — Reverse Routing Optimisation for Faster Returns

**Primary keyword:** `reverse logistics routing`  
**Secondary keywords:** `return shipping optimisation India`

**Core argument:** The nearest pickup or return destination is not always the best one. Reverse routing should optimise for the next usable state of the item—resale, refurbishment, QC, vendor return, disposal, or exchange inventory—while balancing pickup speed, reverse cost, processing capacity, and recovery value.

**H2 sequence:** Why reverse routing is more than pickup assignment → Map return disposition and network inputs → Build routing rules by SKU, condition, capacity, and recovery → Compare cost/speed/recovery trade-offs → Measure pickup-to-disposition and resale outcomes → Pilot node/courier changes → How ShipAxis supports routing intelligence → Wrap-up.

**Must cover:** customer pickup location, return reason, SKU/category, expected condition, destination capacity, warehouse/QC capability, courier reverse coverage, consolidation, seasonal demand, and turnaround time; distinguish pickup speed from time to saleable inventory; protect against cross-country shipping for low-recovery items.

**Seven visuals:** hero `Where Should This Return Go Next?`; reverse network journey; disposition-routing matrix; two-node economics comparison; pickup-to-resale flow; pilot KPI scorecard; ShipAxis CTA.

### 10. CRM — Predicting Repeat Purchase Probability Using CRM Data

**Primary keyword:** `repeat purchase prediction model`  
**Secondary keywords:** `retention analytics`, `behavioural scoring`

**Core argument:** A repeat-purchase score should prioritise relevant retention action, not label customers as intrinsically valuable. The model must use a clear outcome window, leakage-safe features, calibration, and measured incremental lift. It should never use sensitive or inappropriate attributes without a lawful, fair basis.

**H2 sequence:** Define repeat probability and the decision it supports → Choose the outcome window and CRM evidence → Build interpretable customer segments/scores → Turn a score into a proportionate campaign or service action → Validate calibration and incremental lift → Monitor drift, fatigue, and privacy → How Pragma CRM unifies the required context → Wrap-up.

**Must cover:** recency, frequency, monetary value, category affinity, delivery/return experience, campaign engagement, support interactions, and consent status; outcome window; training versus holdout periods; precision/calibration/lift; control group; unsubscribe/frequency guardrails; data minimisation and human review for sensitive action.

**Seven visuals:** hero `Who Is Likely to Buy Again?`; customer-data-to-action journey; feature/eligibility matrix; score-band treatment table; calibration versus campaign-lift example; monitoring/drift scorecard; CRM CTA.

## Pre-publication checklist

- [ ] Article is 2,700–3,100 words before JSON-LD and image reference definitions.
- [ ] There is one H1, 9–10 H2s, 20–24 H3s, 5–10 purposeful H4s, at most three H5s, and no H6.
- [ ] Opening uses the H1 → short context → italic scope statement → image 2 → `---` pattern.
- [ ] Every major claim has an evidence boundary; all illustrative numbers are labelled.
- [ ] The relevant Pragma product appears after the reader already understands the operational framework.
- [ ] There are six or seven visible FAQs, and JSON-LD exactly mirrors them.
- [ ] TL;DR has one recap paragraph and five takeaway bullets.
- [ ] Seven visuals have seven different explanatory jobs; local image links resolve.
- [ ] Every image uses the established Pragma visual language and is placed beside the section it explains.
- [ ] Product proof points, integrations, compliance claims, external standards, and outbound links are verified before publication.
