# Marley Image Style

From `visual brand/Brand Assets/Marley Photography/` and `Marley Iconography/`.

The Marley visual style has three image categories: **iconography**, **photography**, and **patterns**. Each has its own rules.

---

## Iconography

Marley has a custom icon set of **13 hand-drawn icons** representing the clinical / wellness world Marley operates in. Each icon has a **semantic mapping to slide types** — reference icons by their canonical SVG filename when describing slide assets:

| Icon | SVG filename | Use for slide types involving… |
|---|---|---|
| Apple | `Marley_Apple.svg` | Nutrition, diet, lifestyle, healthy eating |
| Bandage | `Marley_Bandage.svg` | Injury, acute care, recovery, wound-care |
| Blood droplet | `Marley_Blood_droplet.svg` | Labs, blood work, blood draws, sample collection |
| Blood pressure | `Marley_blood_pressure.svg` | **BP monitoring, hypertension management, RPM device, BP outcomes** (primary clinical icon for Marley) |
| Cross | `Marley_cross.svg` | General medical / clinical / hospital references |
| Exercise | `Marley_excercise.svg` *(note: misspelled in source)* | Physical activity, lifestyle change, behavioral intervention |
| Heart | `Marley_heart.svg` | **Cardiovascular outcomes, CV events, stroke/CHF risk-reduction stats** |
| Needle | `Marley_needle.svg` | Injectables, vaccines, blood draws (clinical-procedure slides) |
| Pill | `Marley_pill.svg` | **Medication management, polypharmacy, adherence, mail-order Rx** |
| Scale | `Marley_scale.svg` | Weight, obesity management, weight-meds slides |
| Sleep | `Marley_sleep.svg` | Sleep, stress, behavioral health |
| Stethoscope | `Marley_stethoscope.svg` | **Clinical credibility, care-team slides, data-driven care model, multi-disciplinary team** |
| Stress | `Marley_stress.svg` | Mental health, anxiety, stress's effect on BP |
| Tablet | `Marley_tablet.svg` | Medication (paired with pill), digital tablet/device |

**The 4 highest-frequency icons** for Marley payer/fundraise decks are bolded — they should appear most often:
- `Marley_blood_pressure.svg` — anchors any BP/RPM/clinical-monitoring slide
- `Marley_heart.svg` — CV outcomes, risk-reduction
- `Marley_pill.svg` — medication-management thesis
- `Marley_stethoscope.svg` — care team, clinical credibility

Style:
- **Line-based, hand-drawn feel.** Not flat / geometric — these have weight and gesture.
- **Single-color.** Each icon is rendered in a single brand color (purple, red, peach, sky, black, or white). No gradients, no multi-color icons.
- **Generous negative space.** The icons read clearly at small sizes.

Use icons:
- To label a content category (clinical content → stethoscope; medication content → pill or tablet)
- To accent a deck slide section opener
- To create visual rhythm in long-form content
- Locked with the wordmark to make an icon-logo
- **Always name the SVG filename** when specifying an icon in a slide — e.g. "locked top-left with `Marley_stethoscope.svg` (purple variant)", not "with a clinical icon"

Files: `assets/icons/Marley_<Name>.svg` (14 files copied to plugin — 13 icons + a `blood_pressure` variant).

Don't:
- Mix Marley icons with stock icons from other libraries in the same surface
- Re-color icons outside the brand palette
- Use the icons at sizes where line weight becomes uneven
- Refer to icons generically ("an icon", "a heart icon") — always name the file

---

## Photography

Marley's photography splits into two registers, both extracted from `visual brand/Brand Assets/Marley Photography/`:

### Headshots — black and white
**13 professional headshots** of the team, all shot in **black-and-white** with consistent lighting (`Marley Photography/Headshots/Print/` and `…/Social Media/`).

Style cues:
- B&W only — never color headshots for brand use
- Soft, even lighting — no high-contrast or dramatic shadows
- Warm but professional — eye contact, slight smile, no fake stock-photo poses
- Plain background — no busy environments

Use:
- Team pages
- About-us slides in decks
- Author bylines

### Marketing photos — warm studio

**7 studio marketing photos** with a consistent palette and styling (`Marley Photography/Marketing photos/`). Each has a **semantic mapping** — reference by filename when specifying slide hero imagery:

| Photo | Filename | Use for slide types involving… |
|---|---|---|
| Studio composition (general) | `Marley_Studio_1.jpg` | Cover slides, generic hero moments, opening section dividers |
| Studio composition (warm) | `Marley_Studio_2.jpg` | Empathetic moments, patient-experience slides, peach-toned sections |
| Studio composition (clean) | `Marley_Studio_3.jpg` | Clinical credibility slides, professional / cool sections |
| Blood samples close-up | `Marley_Studio_Blood Samples.jpg` | Lab/diagnostic slides, clinical-evidence sections, RPM data discussion |
| Instruments arrangement | `Marley_Studio_Instruments.jpg` | Clinical tooling, multi-disciplinary care team slides, what-we-do composition slides |
| Pills + hands close-up | `Marley_Studio_Pills_Hands.jpg` | **Medication management, mail-order Rx, polypharmacy, adherence slides — the primary "what Marley does" hero photo** |
| Nurse photo (Unsplash) | `Marley_Nurse_bruno-rodrigues_unsplash.jpg` | Care-team slides, "your team of experts" sections, human-led moments |

Style cues:
- **Warm, natural light** — never harsh studio strobes
- **Tight crops** on objects (pills, instruments, blood samples) with hands present for human warmth
- **Cream / peach / sky background tones** — explicitly on-palette
- **Color photography** for marketing (distinct from B&W headshots)
- **Human presence implied** — hands, partial figures — never sterile object-only shots

Use:
- Hero images on marketing pages
- Section openers in payer decks (clinical credibility)
- Patient-experience storytelling
- Social media campaigns

A curated subset (3 marketing photos) is copied into `assets/photography/`. The full set is at `visual brand/Brand Assets/Marley Photography/Marketing photos/`.

Don't:
- Use stock photography that doesn't match this palette and lighting style
- Mix the B&W headshot register with the color marketing register in the same surface
- Use cold, blue-cast clinical photography — Marley's photography is warm
- Refer to photos generically ("a hero photo", "a clinical photo") — always name the file

---

## Patterns

A pattern template exists at `visual brand/Brand Assets/Marley Patterns/Marley_Pattern Template.ai`. The source library does not include exported pattern PNGs, so concrete pattern guidance is limited.

When using patterns:
- Use the pattern template as the source of truth
- Keep patterns to subtle background-surface use; never let pattern dominate
- Stay in the brand palette

---

## See also

- [[colors]] — palette that constrains all imagery
- [[logo-usage]] — logo treatments on photography
- `assets/icons/` — 14 icon SVGs copied into the plugin
- `assets/photography/` — 3 marketing photo samples copied into the plugin
- Full asset library: `~/epch-claude/visual brand/Brand Assets/`
- [[source-refs]] — extraction notes
