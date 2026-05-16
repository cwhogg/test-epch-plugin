# Marley Slide Layouts

Marley's master PowerPoint template (`~/epch-claude/visual brand/Marley_Presentation_MasterTemplate.pptx`) contains **13 named slide layouts**. They collapse into **7 conceptual layout types** that compose deck visuals. Each generated deck slide should explicitly name its layout from this vocabulary.

The 13 raw PPT layout names are preserved as sub-variants so PowerPoint users can map directly to the master's Slide Layout panel.

---

## 1. TITLE_FAMILY — cover / section title

**PPT variants:** `TITLE`, `TITLE_1`, `TITLE_3`, `TITLE_ONLY` (differences are placement of subtitle and date block — minor)

**Description:** large title at slide center, optional subtitle below, optional date and "Prepared for [audience]" line.

**Use for:**
- Cover slide (Slide 1 of every deck)
- Internal section dividers when minimal info needs to surface ("Appendix", "Thank You", section names)
- Closing slide

**Surface (palette):** Marley Purple (`#5A38B2`) as primary surface with white reverse type for high-impact cover; or Cream (`#FDF7EF`) with Purple type for quieter internal section titles.

**Asset pairing:**
- Wordmark logo (white or purple, depending on surface)
- No photo, no icon
- Date and audience-name in Greycliff Regular small caption type

---

## 2. TITLE_AND_BODY — standard content

**PPT variant:** `TITLE_AND_BODY` (slideLayout6)

**Description:** slide title at top (Reckless Medium), body content area below (Greycliff for text, or mixed media). The workhorse layout — most narrative slides use this.

**Use for:**
- Single-point content slides where the title states the point and the body unpacks it
- Bulleted explanations
- Single-table slides
- Slides with one chart + brief annotation

**Surface (palette):** Cream (`#FDF7EF`) is the default. Switch to Sky (`#C9E5FC`) for data/clinical slides. Peach (`#FFDFD6`) for empathetic/patient-story slides. Avoid all-purple for body slides — purple should accent, not dominate.

**Asset pairing:**
- Optional Marley iconography SVG locked top-left or top-right of slide title (chosen by topic — see `image-style.md` semantic mapping)
- No hero photo (use BLANK for that)
- Optional small monogram bottom-right as a brand sign-off (subtle)

---

## 3. TITLE_1_2 — two-panel

**PPT variant:** `TITLE_1_2` (slideLayout5)

**Description:** title at top + two equal columns of content below. The single most under-used layout in current generated decks — high-impact for comparisons.

**Use for:**
- Comparison slides (before/after, option A vs. option B, current state vs. new state)
- Pivot slides (e.g. Slide 16 "Marley meets payer needs": left column = what Marley is, right column = what we solve)
- Pairing related concepts (clinical evidence + economic evidence; what we ask + what you get)
- Per-cohort breakouts (Stage 2 entry / Stage 3 entry results)

**Surface (palette):** paired surfaces give this layout punch. Recommended:
- Peach left / Sky right — warm + cool pairing (empathy + clinical)
- Cream left / Sky right — neutral + data
- Cream left / Peach right — neutral + warm
- Avoid same-color both panels — defeats the purpose

**Asset pairing:**
- Optional small icon per column (different icons signal different concepts)
- Typography: column headers in Reckless Medium, body in Greycliff
- No hero photo — this is a text/data layout

---

## 4. SECTION_DIVIDER — chapter break

**PPT variants:** `SECTION_TITLE_AND_DESCRIPTION`, `SECTION_TITLE_AND_DESCRIPTION_1`, `SECTION_TITLE_AND_DESCRIPTION_1_1`, `SECTION_TITLE_AND_DESCRIPTION_1_2`, `SECTION_TITLE_AND_DESCRIPTION_1_2_1` (variants differ in media-slot placement and accent-strip layout — pick by visual context)

**Description:** full-bleed section opener with a large section title, an optional descriptive subline, and an optional image or accent-color band. Used to break the deck rhythm.

**Use for:**
- Transitions between acts (Act 1 → Act 2 in a payer deck, e.g. "How Marley Works with Payers")
- Chapter breaks inside dense sections ("Clinical Data Deep Dive")
- Slide 16 in payer deck — the pivot from "what Marley is" to "what Marley does for payers"

**Surface (palette):** rotate to break monotony. Pick a different surface than the preceding 3–4 slides:
- Full Marley Purple (white type) for high-impact transitions
- Full Marley Red (#FF4E1E, with white type) for energy / urgency transitions (use sparingly)
- Full Peach for empathetic/patient-story transitions
- Full Sky for clinical/data transitions

**Asset pairing:**
- Large brand photo from `Marley_Studio_*.jpg` set fills half/full bleed (the `_1_2` variants are media-led; use these for photo-driven dividers)
- Or large iconography SVG as visual anchor (e.g. `Marley_stethoscope.svg` enlarged on a clinical section divider)
- No body text beyond the section description

---

## 5. HERO_STATS — multi-stat grid

**Not a unique PPT layout name** — typically built atop `TITLE_AND_BODY` or `TITLE_1_2` with custom internal structure. Worth naming as a concept because it appears repeatedly in Marley decks and has distinctive visual rules.

**Description:** title at top + 4–6 large hero statistics arranged in a grid (2×2, 2×3, or 3×2). Each stat is a giant number + small caption + small source line. The statistic is the visual lead, not the surrounding text.

**Use for:**
- Slide 4 in payer deck (60+% uncontrolled / 2/3 hospitalizations avoidable / <7% optimal / 26+ days to provider)
- Engagement metrics slide (78% active / 75% retention / NPS 86 / 5 device readings)
- Clinical results slide (70% at goal / 14.8 mmHg reduction / 20% less CV risk / 27% less stroke risk)

**Surface (palette):** Cream or Sky. Statistic numbers in Marley Purple (`#5A38B2`) or Dark Purple (`#472B8C`); captions and source lines in dark gray. Red (`#FF4E1E`) can highlight one specific stat for emphasis (use only when one stat genuinely outranks the others).

**Asset pairing:**
- Statistic numbers in Reckless Medium 60–84pt (the typography hierarchy is the visual)
- Captions in Greycliff SemiBold 12–14pt
- Source citations in Greycliff Regular 9–10pt below the grid
- No icons inside the stat cells (clutter)
- No photos

---

## 6. CUSTOM — flexible canvas

**PPT variant:** `CUSTOM` (slideLayout1)

**Description:** fully editable canvas with no enforced placeholder structure. Build per-slide.

**Use for:**
- Org charts and team diagrams
- Complex flowcharts (patient journey, GTM strategy diagram)
- Signature patient case slides (annotated timeline showing intervention sequence)
- Multi-component slides that don't fit a standard layout

**Surface (palette):** match to slide purpose. Cream is the safe default. Sky for data-flow diagrams. Peach for human-story custom layouts.

**Asset pairing:** open. Pull from icons, photos, logos as the slide requires. Document the specific assets used so the layout can be reproduced.

---

## 7. BLANK — full freedom

**PPT variant:** `BLANK` (slideLayout13)

**Description:** entirely empty canvas. Maximum flexibility — and maximum responsibility for visual hierarchy.

**Use for:**
- Hero photography slides (image fills entire slide as background)
- "Large headline + big image" moments (slide template includes one of these in the master)
- Patient-quote slides with photo background
- Closing impact moments

**Surface (palette):** typically the image IS the surface. If text overlays the image, use white reverse type with sufficient contrast.

**Asset pairing:**
- Hero photo strongly recommended — from `Marley_Studio_1.jpg`, `Marley_Studio_2.jpg`, `Marley_Studio_3.jpg`, `Marley_Studio_Blood Samples.jpg`, `Marley_Studio_Instruments.jpg`, `Marley_Studio_Pills_Hands.jpg`, or `Marley_Nurse_bruno-rodrigues_unsplash.jpg`
- Or large iconography SVG at 60–80% slide width
- Headline text in Reckless Medium, white reverse on dark image areas
- No bulleted body text — if the slide needs bullets, use TITLE_AND_BODY instead

---

## Choosing layouts — quick decision tree

| If the slide is… | Use… |
|---|---|
| Cover / section title / closing | TITLE_FAMILY |
| Single point + body | TITLE_AND_BODY |
| Two paired concepts or columns | TITLE_1_2 |
| Act/chapter transition | SECTION_DIVIDER |
| Multiple statistics in a grid | HERO_STATS (built atop TITLE_AND_BODY or TITLE_1_2) |
| Org chart / patient journey / non-standard structure | CUSTOM |
| Hero photo / impact image / large headline | BLANK |

## Deck-level layout diversity rule

A well-composed Marley deck uses **at least 4 distinct layout types** across its slides. Decks where >70% of slides share one layout (typically TITLE_AND_BODY) read as monotonous and miss the master template's visual range.

For reference, the 2024 BCBS-FL payer deck uses:
- TITLE_FAMILY (2 slides: cover + Thank You)
- TITLE_AND_BODY (~12 slides)
- TITLE_1_2 (~4 slides: payer-needs pivot, contracting structures comparison)
- SECTION_DIVIDER (3 slides: Topics for Discussion + the 2 act-divider moments)
- HERO_STATS (3 slides: problem stats, engagement metrics, clinical results)
- CUSTOM (3 slides: patient journey, patient case example, contracting structure visualizations)
- BLANK (1 slide: patient-experience photo lead-in, if used)

= 7 distinct layouts across 28 slides. That's the bar.

---

## See also

- [[colors]] — palette details and per-context color guidance
- [[typography]] — Reckless / Greycliff scale referenced throughout this file
- [[logo-usage]] — when to use wordmark vs. monogram on each layout type
- [[image-style]] — icon and photo semantic mapping (what each asset signals)
- [[source-refs]] — how this file was extracted from the .pptx master
