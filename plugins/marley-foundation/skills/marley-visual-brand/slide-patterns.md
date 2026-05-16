# Marley Slide Composition Patterns

Distilled from all 5 source payer decks (BCBS FL March 2024, OSF March 2024, Feb 13 generic, Jan 10 generic, UHC Accelerator May 2023). Patterns are reusable across deck types — payer, fundraise, product-scoping — even though the extraction source was the payer-deck library.

This vocabulary sits **between** [[layouts]] (the PowerPoint structural skeleton) and [[image-style]] (the brand-asset filenames). A slide spec should name:

1. **Layout** (one of 7 from `layouts.md`) — the structural skeleton
2. **Pattern** (one of ~15 from this file) — the composition treatment
3. **Surface color** (from `colors.md`) — the palette assignment
4. **Brand assets** (icon SVG / photo JPG / logo lockup from `image-style.md`) — the named visual elements

Patterns capture the *visual templates that recur across slides*. They're how Marley's payer decks read as a coherent visual system rather than a sequence of unrelated slides.

---

## Most-used patterns (use these often)

Ordered roughly by frequency across the 5 source decks.

### `horizontal-process-flow`
**14 occurrences across all 5 decks** — the single most-used pattern.

3–6 boxes or circles laid out left-to-right, connected by arrows, thin lines, or arrow-tails. Three sub-variants by content:

- **Narrative-box variant** — 4 rounded Peach cards with arrow-tail connectors between (e.g. Access → Engagement → Outcomes → ROI). Used for high-level sales narrative.
- **Patient-journey variant** — 5–6 thin-connector steps with a row of 4 real photo/screenshot tiles below the step row. Used for "what the patient experiences."
- **Claim-circle variant** — small Sky circles on a thin Purple line, terminal Peach summary box on far right. Used for contracting-structure timelines (each of the 3 contracting-structure slides).

**Surface:** Peach when sales-narrative; white when timeline/technical.
**Icons:** small per-step icons above each step (e.g. `Marley_blood_pressure.svg` above "continuous monitoring"; `Marley_pill.svg` above "ship kit"). Marley logo never appears as a step — Marley is implicit.
**Host layout:** `TITLE_AND_BODY` or `CUSTOM`.
**Source:** BCBS slides 11, 20, 22, 25–27; OSF 7, 11; Feb 11; Jan 10, 18; UHC 6.

### `2-column-pivot`
**8 occurrences across 4 decks.**

Paired left/right columns where the left and right halves carry parallel but contrasting content. The canonical use is **the Act 1 → Act 2 pivot slide** ("our design choices" left / "your challenges" right) — this is the visual fulcrum of the entire payer deck.

Sub-variants:
- text-left / diagram-right (positioning slide)
- bulleted-checklist-left / callout-cards-right (payer-needs)
- long-quote-left / testimonials-and-stat-right (NPS slide)

**Surface:** Peach left / Sky right is the canonical pivot treatment. Never Purple full-bleed (this is a content slide, not a brand slide).
**Icons:** one per column, anchored top-corner.
**Host layout:** `TITLE_1_2`.
**Source:** BCBS 6, 16; OSF 6, 18; Feb 6, 9; Jan 3, 11.

### `positioning-diagram`
**8 occurrences across 4 decks.**

Marley placed inside a vertical stacked-band diagram between existing categories. Composition rules that hold consistently:

- **Always 3–4 horizontal bands**, never side-by-side columns
- **Marley middle band always elevated** — white border, white surface, or the orange m-diamond logo (visual "lift")
- **Top band Specialists** (Orange/Red); **bottom band PCPs** (Sky); **middle-extra band Care Managers** (light Peach/pink)
- **Right-side arrow labels** when framing the payment-model gap ("Paid for procedures / Paid for outcomes / Paid for time-based visits"); omit arrow labels when framing the clinical-category gap

Used to frame both *the clinical category gap* (Marley is not a PCP, not a specialist) and *the payment-model gap* (Marley wants to be paid for outcomes).

**Surface:** Cream typically; the bands themselves carry the color.
**Host layout:** `CUSTOM`.
**Source:** BCBS 6, 9; OSF 6, 29, 32; Jan 3, 6; Feb 6, 9.

### `3-column-option-compare`
**7 occurrences across 4 decks.**

Three equal-weight columns comparing options on the same dimensions. Two presentations:
- **Numbered (01/02/03)** when the options are sequential or labeled by index
- **Feature-name-labeled** when the options have distinct names (FFS+QB / Capitation / Milestones)

Used for the 3 contracting structures and the 3 ways patients come to Marley.

**Surface:** Purple-header + white body when comparing complex options that need explanation. All-Peach cards when the options are simpler.
**Icons:** one per column, semantically distinct (e.g. `Marley_pill.svg` for FFS, `Marley_scale.svg` for capitation, `Marley_heart.svg` for milestones).
**Host layout:** `TITLE_1_2` (3-column variant) or `CUSTOM`.
**Source:** BCBS 10, 24; OSF 10, 30; Feb 10, 24; UHC 10.

### `paper-thumbnails`
**8 occurrences across 4 decks.**

1–3 journal article or press-piece thumbnails used as background credibility props. Always slightly rotated and angled (~5–10°), giving a "stack of papers" feel rather than a clean grid. Three contexts:
- Alone — single citation supporting a clinical claim (e.g. Lancet meta-analysis for downstream-risk reduction)
- With a stat-strip — Propeller comparable evidence (57% / 33% reduction stats)
- With logos — team credibility slide

**Surface:** typically Cream; the papers carry their own color.
**Host layout:** `TITLE_AND_BODY` or `CUSTOM`.
**Source:** BCBS 5, 13, 17; OSF 5, 13, 21, appendix; Feb 5, 13; UHC 7, 8.

### `logos-row`
**7 occurrences across 4 decks.**

Row of partner/customer/payer logos as credibility signal. Three modes:
- **Investor row** — 3 logos in a single horizontal line (a16z / CRV / Rock Health), always at bottom of the team slide. Appears in every deck.
- **Payer-portfolio grid** — 3×3 grid of 8–10 payer logos (BCBSIL, BCBSMN, BCBSMI, UHC, CMS, Aetna, Humana, Priority Health, Cigna). Used in the *generic* decks (Jan, OSF) but **not** in customer-specific BCBS or Feb decks — multi-payer logos would be awkward when pitching one BCBS plan.
- **Press-article credibility** — 3 article cards with circular Sky-blob backgrounds.

**Surface:** Cream typically.
**Host layout:** `TITLE_AND_BODY`.
**Source:** BCBS 17; OSF 16, 21; Feb 17; Jan 20; UHC 12.

### `hero-photo-with-overlay`
**6 occurrences across all 5 decks** — the canonical Welcome-slide treatment.

Full-bleed photo on the right ~40% of the slide; Purple surface on the left ~60%. Italic-serif "Welcome to" + bold sans "Marley Medical" headline; 2–3 short paragraphs below. The 3-women-laughing photo is the standard hero. OSF adds a second hero-photo slide using a single-elder-woman portrait.

**Surface:** Purple left, image-as-surface right.
**Photo:** typically a hero studio shot — never a stock photo.
**Logo:** small Monogram White or small Wordmark White, bottom-right or top-left.
**Host layout:** `BLANK` with structured overlay, or `TITLE_1_2`.
**Source:** every deck's slide 2 or 3.

### `headline-only-section-divider`
**6 occurrences across 3 decks.**

Two presentations:
- **Mid-deck navigation** — Purple/Peach split with section title in Reckless Medium and m-diamond on the Purple side
- **Closing** — full-bleed Peach "Thank You!" with orange m-logo center

Used between Acts (Act 1 → Act 2 transition) and at the close.

**Surface:** Purple or Peach full-bleed.
**Host layout:** `SECTION_DIVIDER`.
**Source:** BCBS 18, 28; OSF 23, 27; Feb 18, 22.

### `multi-chart-grid + stat-strip`
**5 occurrences across all 5 decks** — the canonical clinical-results slide.

Two-tier composition that's instantly recognizable across the deck library:
- **Top tier:** Peach card containing 3 visualizations — Goal Attainment area chart (left), Reduction-by-Initial-Stage grouped bar chart (middle), BP Results data table (right)
- **Bottom tier:** 2 Sky stat cards on the left (70% at goal / 14.8 mmHg average reduction) + a Purple arrow connector + 3 Sky risk-reduction stats on the right (20% CV / 27% stroke / 28% CHF)

Always has Lancet citation in the footer (Ettehad 2015 meta-analysis for the downstream-risk stats).

**Surface:** Peach card on Cream background, with Sky inset cards.
**Host layout:** `CUSTOM`.
**Source:** every deck.

### `n-box-equal-grid` — `4-box` variant
**5 occurrences across 4 decks.**

4 equal-weight category boxes in a 2×2 grid. Each box has a Purple header bar + white body with bullets or short caption. Used for selection criteria (4 patient-selection rules) and value-prop summary (Access / Engagement / Outcomes / ROI).

**Surface:** Cream or Sky background; cards carry Purple+white.
**Icons:** one per box (semantically distinct).
**Host layout:** `HERO_STATS` (when boxes are stat-flavored) or `CUSTOM`.
**Source:** BCBS 21, 23; OSF 18, 20; Feb 21; Jan 18, 19.

### `n-box-equal-grid` — `6-box` variant
**4 occurrences across 4 decks.**

6 equal-weight category boxes in a 3×2 grid. All-Peach cards with orange titles, body in Greycliff Regular. Used for payer-fit summary (Broad population / Guideline-based / Highly scalable / Easy contracting / Value-based / Path to geo expansion).

**Surface:** Cream background; all cards Peach.
**Icons:** one per box (optional but consistent if used).
**Host layout:** `HERO_STATS` or `CUSTOM`.
**Source:** BCBS 19; OSF 18; Feb 19; Jan 19.

### `hero-stat-grid`
**4 occurrences across 4 decks** — the canonical problem-framing slide.

6 stats (3×2) or 8 stats (4×2) in big-number cards. Purple rounded cards on white surface in the 2024 decks; UHC May 2023 used Peach cards on Peach surface (older treatment). Tiny gray source-citation footer always present.

**Position in deck:** always position 4, immediately after Welcome — never mid-deck.
**Surface:** White or Sky with Purple cards.
**Icons:** none — the numbers are the visual.
**Host layout:** `HERO_STATS`.
**Source:** BCBS 4; OSF 4; Feb 4; UHC 2.

### `stat-stack`
**4 occurrences across 4 decks** — the canonical engagement-KPIs slide.

6 stats in a 2×3 grid (78% active / <1 wk access / 75% retention / 5 readings/wk / 2.5 msg/wk / 86 NPS). Always Purple rounded cards on white surface. Big number on top, small caption in white text below. **No icons** — this is the key visual distinction from `hero-stat-grid`, which also has no icons but uses 8 stats and sits in a different deck position. Jan 10 uses a 4-stat 2×2 variant.

**Surface:** White or Sky background; cards Purple.
**Host layout:** `HERO_STATS`.
**Source:** BCBS 12; OSF 12; Feb 12; Jan 12.

### `annotated-timeline`
**4 occurrences across 4 decks** — the canonical patient-case slide.

Single-patient BP trajectory. Composition rules that hold consistently:
- **8–9 dots** connected on a horizontal line — never fewer, never more
- **Y-axis:** 4 colored stage zones as horizontal background bands — Crisis (Red), Stage 2 (Orange), Stage 1 (Yellow), At goal (Green)
- **Dot colors** match the zone they fall in
- **3 intervention labels** below the line in equal-width spans (e.g. "Med change (MD)", "Lifestyle change (health coach)", "Med change (pharmacist)")
- **Explanatory paragraph in upper-right margin**, always starts "Within 23 days…"

**Surface:** Cream.
**Icons:** small per-intervention markers on the timeline (e.g. `Marley_pill.svg` for med changes, `Marley_exercise.svg` for lifestyle change).
**Host layout:** `CUSTOM`.
**Source:** BCBS 14; OSF 14; Feb 14; Jan 15.

### `radial-team-diagram`
**4 occurrences across 4 decks** — the canonical multidisciplinary-care-team slide.

Marley orange-m-diamond at center, with **6 satellite role labels** radiating around it: Pharmacist, Internal Medicine Physician, Cardiologist, Endocrinologist, Dietitian, Health Coach. Bounded by an Orange rounded rectangle.

Per-role icons:
- Pharmacist → `Marley_pill.svg`
- Internal Medicine Physician → `Marley_cross.svg`
- Cardiologist → `Marley_heart.svg`
- Endocrinologist → `Marley_needle.svg` (or `Marley_blood_droplet.svg`)
- Dietitian → `Marley_apple.svg`
- Health Coach → `Marley_blood_pressure.svg`

OSF variant swaps the center logo for an embedded photo of an MD.

**Surface:** Cream typically.
**Host layout:** `CUSTOM`.
**Source:** BCBS 7; OSF 9; Feb 7; Jan 9.

---

## Customer-specific patterns (use when audience calls for them)

These appear in only 1–2 decks but are useful when the audience or context calls for them. Don't default to them — invoke deliberately.

### `geographic-map`
US map with target states highlighted Purple, expansion-target states Orange, de-emphasized states de-saturated. Used when the audience cares about regional expansion (OSF — Midwest health system; UHC — multi-state payer).
**Source:** OSF 20, 43; UHC 13. **Not in BCBS or Feb generic decks.**

### `gantt-chart` — B2B contracting pipeline
Payer logos on Y axis, contracting stages on X axis (Contracted FFS / Claims Filed / Targets ID'd / Initial Conversations / Pitch Stage / Contract / Implementation). M-diamond markers at each payer's current stage. Unique to health-system audiences who care about payer-contracting transparency.
**Source:** OSF 19 only.

### `diagram-with-arrows` — FFS → VBC contract upgrade
Purple "FFS Foundation" pedestal at the bottom with 4 diagonal arrows shooting up-right to PPPM / gross-margin pill cards. Shows how each contract type upgrades the economics. Used to lay out the contract-upgrade economics narrative.
**Source:** OSF 17 only.

### `2-column-photo-overlay` — illustrative patient photo
Older man with BP cuff sitting at a brick-walled cafe, paired with bulleted text. Used to humanize the polychronic patient. Mostly demoted to appendix in the matured decks; only present in OSF appendix and Jan 10.
**Source:** OSF appendix; Jan 4.

### `logos-grid` — payer portfolio
3×3 grid of 8–10 payer logos (BCBSIL, BCBSMN, BCBSMI, UHC, CMS, Aetna, Humana, Priority Health, Cigna). Use only in generic / non-payer-specific decks. **Don't use in customer-specific BCBS or Anthem decks** — naming competitors directly to the audience is awkward.
**Source:** OSF 16; Jan 20.

### `metric-over-time-chart`
Single metric on Y axis, time on X axis (patient-growth bar chart or retention area chart). Used when one metric over time is the story. Rarer than expected — usually subsumed inside `multi-chart-grid + stat-strip`.
**Source:** OSF 8; Jan 13.

### `two-stat-emphasis` — huge single number
One or two giant numbers taking the whole slide (e.g. "26.7 hours per day"). Often paired with a small chart or paper thumbnail below as substantiation.
**Source:** BCBS 5; Feb 5; UHC 5.

### `bulleted-toc`
Topics-for-Discussion slide — 3-item bulleted list with m-icon markers on Peach surface, paired with giant m-diamond on Purple right side. Use on longer / more formal customer decks. Skip on lean decks.
**Source:** BCBS 2; Feb 2.

---

## Dropped patterns (don't use)

These appeared in May 2023 or earlier and were dropped in the Jan 2024 redesign. Don't reach for these.

- **`checklist-vs-status-table`** (UHC May 2023) — "Components of a successful system" 6 rows × 2 columns (checkmark or empty circle). Read as too critical-of-status-quo.
- **`tabbed-card`** (UHC May 2023) — tabbed selector across 4 diseases above a single content card. Too interactive-fiddly for a static PDF.
- **`9-icon services grid`** (UHC May 2023) — 9 icons in a 3×3 grid covering services. Too dense; replaced by the cleaner `radial-team-diagram`.
- **`distribution-bar-breakdown` / ROI waterfall** (Jan 10 only) — Uncontrolled Patient $20,547 → reductions → Controlled Patient $14,981. Replaced by the simpler `horizontal-process-flow` (Access/Engagement/Outcomes/ROI).
- **`8-box n-grid` (4×2)** (UHC May 2023) — too many boxes to read at a glance. Collapsed to the cleaner 6-box.
- **`radial-ecosystem-diagram`** (Jan 10 only) — variant of radial-team where satellites are service categories (Primary care, Labs, Urgent care, etc.) rather than internal roles. Dropped in favor of the consistent team-roles radial.

---

## Evolution notes

**May 2023 → Jan 2024 (the biggest leap).** Deck length roughly doubled. Surface palette shifted from Peach-dominant (warmer, more startup-y) to Purple-dominant (more institutional). Hero stats moved from Peach cards to Purple cards on white — more authoritative. Several experimental patterns dropped (`checklist-vs-status-table`, `tabbed-card`, `9-icon services grid`). The `annotated-timeline` and `stat-stack` patterns first appeared in Jan and stuck. The `2-column-photo` (older man with BP cuff) started getting demoted to appendix.

**Jan 2024 → Feb 2024.** Refinement, not reinvention. The 6-box payer-fit grid and the Access/Engagement/Outcomes/ROI horizontal-process-flow appeared. The `multi-chart-grid + stat-strip` clinical results slide became more polished. The `radial-team-diagram` stabilized on roles (not services).

**Feb 2024 → March 2024 (customer-specific decks).** The Feb deck became the template. BCBS FL March is essentially the Feb deck with date / customer swap and emphasis tweaks ("active provider agreements with BCBS in several states"). OSF March is the same template plus ~6 patterns added for the health-system audience (`gantt-chart`, B2C2B `horizontal-process-flow` with embedded screenshots, FFS→VBC `diagram-with-arrows`, `geographic-map` with target states, top-of-license stacked bars, partnership-terms data table).

**Net trajectory:** ~15 stable patterns by Feb 2024. Per-customer variation happens through pattern *selection* (which subset of the 15) and *content* (data, logos, language), **not** through new pattern invention. The exception is OSF, which adds several health-system-specific patterns.

---

## Pattern → host layout

| Pattern | Host layout |
|---|---|
| `hero-photo-with-overlay` | `BLANK` with overlay, or `TITLE_1_2` |
| `hero-stat-grid` | `HERO_STATS` |
| `two-stat-emphasis` | `TITLE_AND_BODY` with hero number |
| `positioning-diagram` | `CUSTOM` |
| `radial-team-diagram` | `CUSTOM` |
| `2-column-pivot` | `TITLE_1_2` |
| `3-column-option-compare` | `TITLE_1_2` (3-column) or `CUSTOM` |
| `horizontal-process-flow` | `TITLE_AND_BODY` or `CUSTOM` |
| `stat-stack` | `HERO_STATS` |
| `annotated-timeline` | `CUSTOM` |
| `multi-chart-grid + stat-strip` | `CUSTOM` |
| `n-box-equal-grid` (4-box, 6-box) | `HERO_STATS` or `CUSTOM` |
| `logos-row` / `logos-grid` | `TITLE_AND_BODY` |
| `paper-thumbnails` | `TITLE_AND_BODY` or `CUSTOM` |
| `headline-only-section-divider` | `SECTION_DIVIDER` |
| `geographic-map` | `TITLE_AND_BODY` or `CUSTOM` |
| `gantt-chart` | `TITLE_AND_BODY` |
| `bulleted-toc` | `TITLE_AND_BODY` or `TITLE_1_2` |

---

## Pattern → surface tendencies

| Pattern | Canonical surface |
|---|---|
| `hero-photo-with-overlay` | Purple left + image right (Welcome slide) |
| `hero-stat-grid` (problem-framing) | White or Sky with Purple cards |
| `stat-stack` (engagement KPIs) | White with Purple cards |
| `positioning-diagram` | Cream (bands carry color) |
| `2-column-pivot` | Peach left / Sky right (canonical pivot) |
| `3-column-option-compare` | Peach / Cream / Sky (signaling progression) |
| `horizontal-process-flow` (narrative) | Peach boxes |
| `horizontal-process-flow` (timeline) | White |
| `radial-team-diagram` | Cream |
| `annotated-timeline` | Cream (zones colored) |
| `multi-chart-grid + stat-strip` | Cream with Peach + Sky cards |
| `n-box-equal-grid` (4-box) | Cream or Sky |
| `n-box-equal-grid` (6-box, payer-fit) | Cream with all-Peach cards |
| `logos-row` / `logos-grid` | Cream |
| `paper-thumbnails` | Cream (papers carry color) |
| `headline-only-section-divider` | Purple full-bleed (mid-deck) or Peach (closing) |

---

## How to use this file

When drafting a slide:

1. **Identify the slide's communicative job** — is it problem-framing? Positioning? Outcomes? Contracting? Transition?
2. **Pick a pattern that fits the job** — see the most-used patterns above; reach for customer-specific ones only when audience justifies it.
3. **Apply the composition rules** — element count, asset role, surface, icon set are constrained per pattern.
4. **Name the pattern in the slide's Visual spec** alongside the layout, surface, icon, and photo lines.

Don't invent new patterns when an existing one fits — Marley's visual coherence comes from the small fixed vocabulary repeated across decks.

---

## See also

- [[layouts]] — the 7 PowerPoint layouts patterns are hosted in
- [[colors]] — surface palette and deck-level distribution rules
- [[image-style]] — semantic icon and photo mapping (which assets fit which patterns)
- [[typography]] — type roles inside patterns (Reckless for headlines, Greycliff for body)
- [[source-refs]] — extraction notes
- `../payer-pitch-deck/narrative-arc.md` — every slide annotated with pattern + layout + surface + assets
- `../payer-pitch-deck/examples/bcbs-fl-march-2024-slide-by-slide.md` — canonical reference deck
