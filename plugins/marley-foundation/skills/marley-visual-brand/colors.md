# Marley Medical Color Palette

Extracted from the official Adobe Creative Cloud library files (`Marley Medical_Brand Colors_RGB.cclibs` and `_CMYK.cclibs`) in `visual brand/Brand Assets/Marley Colors/`.

The palette has six named brand colors plus tints. Logo asset filenames confirm the canonical six color names: **Purple, Red, Peach, Sky, Black, White**.

---

## Primary brand colors (digital / RGB)

| Color name | Hex (RGB) | RGB | When to use |
|---|---|---|---|
| **Marley Purple** | `#5A38B2` | rgb(90, 56, 178) | Primary brand color. Headers, primary CTAs, brand surfaces. The Marley logo's signature color. |
| **Marley Dark Purple** | `#472B8C` | rgb(71, 43, 140) | Hover states for purple CTAs, darker accents, deep brand surfaces, on-image text. |
| **Marley Red** | `#FF4E1E` | rgb(255, 78, 30) | Secondary brand color. Accents, urgent/attention-grabbing CTAs, emotional/energetic moments. Use sparingly — it pulls the eye fast. |
| **Marley Peach** | `#FFDFD6` | rgb(255, 223, 214) | Warm background surfaces, soft accents, empathetic content (patient stories, care-team imagery). |
| **Marley Sky** | `#C9E5FC` | rgb(201, 229, 252) | Cool background surfaces, soft accents, content-card backgrounds, data-vis backgrounds. |
| **Marley Cream** | `#FDF7EF` | rgb(253, 247, 239) | Off-white page background. Warmer than pure white. Default body background in long-form content. |

## Tints / supporting

| Color name | Hex | When to use |
|---|---|---|
| **Peach Light** | `#FFF5F5` | Tint of peach — even softer; very-light section backgrounds. |
| **Sky Light** | `#EDF7FF` | Tint of sky — even softer; very-light section backgrounds. |

## Print (CMYK) equivalents

The CMYK library is the print version of the same palette. Hex equivalents shift slightly because the CMYK gamut is smaller than RGB.

| Color | CMYK hex (approx) | CMYK values |
|---|---|---|
| Purple | `#5C469C` | C77 M86 Y0 K0 |
| Dark Purple | `#4C4183` | C84 M87 Y17 K5 |
| Red | `#F15629` | C0 M82 Y95 K0 |
| Peach | `#FCDBD6` | C0 M16 Y10 K0 |
| Sky | `#B3DEF2` | C25 M0 Y0 K3 |
| Sky Light | `#E7F6FD` | C8 M0 Y0 K0 |
| Peach Light | `#FEECEC` | C0 M8 Y3 K0 |
| Cream | `#FFF8EF` | C0 M2 Y5 K0 |

For digital work always use the RGB hex. For print files use CMYK from the `.cclibs` library directly.

---

## When to use which color — the practical rules

- **Purple = brand.** If the surface needs to read "Marley," it gets purple. Logo lockup, headers, primary CTA buttons.
- **Red = energy / accent.** Use when copy needs urgency, attention, or emotional punch. Used sparingly — it should pop, not dominate. Marley uses red in animated logo treatments and in moments of high contrast.
- **Peach + Sky = warmth + calm.** These are the supporting surfaces. Peach in empathetic / human contexts. Sky in informational / clinical / data contexts.
- **Cream = the default canvas.** Never pure white for long-form. Cream is warmer and more on-brand.
- **Black + white** exist for accessibility and for monochrome logo treatments — not as brand surfaces.

## Pairings that work

- Purple + cream — the canonical Marley deck slide.
- Purple + peach — warmth + brand.
- Purple + sky — calm + brand.
- Red + cream — energy + brand-quiet.
- Purple + red — high-contrast, use only when both colors are doing distinct work.

## Pairings to avoid

- Red on peach — they fight; the warm cast on both makes red read muddy.
- Red on sky — color-clash.
- Purple on dark surfaces other than cream — low contrast.

---

## Deck-level palette diversity

A common failure mode is decks that use one surface color throughout (almost always cream-on-purple). The master PowerPoint template ranges across the palette deliberately — generated decks should too. A well-composed Marley deck distributes across surfaces approximately like this:

| Surface | Target % of slides | Slide types that fit |
|---|---|---|
| **Cream** (`#FDF7EF`) | ~40% | Default canvas. Most TITLE_AND_BODY narrative slides, headers, table-heavy slides. |
| **Peach** (`#FFDFD6`) | ~25% | Empathetic, human-story, patient-narrative slides. Care-team slides. Quote slides. |
| **Sky** (`#C9E5FC`) | ~25% | Clinical, data-evidence, outcomes, technical slides. HERO_STATS for clinical metrics. |
| **Red accent** (`#FF4E1E`) | ~10% | High-stakes moments: section dividers, "the ask" slides, urgency/CTA slides. Rarely a full background — usually accent strips, callouts, single-stat highlights. |
| **Purple full-bleed** (`#5A38B2`) | rare | Cover slide, occasional high-impact SECTION_DIVIDER. White reverse type. Not a body-content surface. |

**Diversity rule:** if >70% of a deck's slides use a single surface color, the deck is too uniform. Mix it up. The most common failure is "everything is Cream" — break this by routing patient-story slides to Peach, data slides to Sky, and at least one SECTION_DIVIDER to Purple full-bleed or Red.

This is a chris-critic check on every deck draft (see the `Visual specificity` diagnostic in the critic).

## When to use which color — slide-type quick reference

| Slide type | Surface | Accent / type |
|---|---|---|
| Cover / TITLE_FAMILY | Purple full-bleed OR Cream | White reverse / Purple type |
| Standard narrative (TITLE_AND_BODY) | Cream | Purple type, accent icon in Sky or Peach |
| Patient story / care-team / empathetic | Peach | Purple type, optional warm photo |
| Data / clinical / outcomes (HERO_STATS, TITLE_AND_BODY) | Sky | Purple type, Red accent on one hero stat |
| 2-panel pivot (TITLE_1_2) | Peach left / Sky right (or Cream/Sky) | Purple type, paired icons |
| Act transition (SECTION_DIVIDER) | Rotate — Purple full-bleed, Red, Peach, or Sky | White reverse on dark surfaces; Purple on light |
| The ask / high-stakes call | Red accent or Purple full-bleed | White reverse |
| Hero photo (BLANK) | Image is surface | White reverse type if needed |

---

## See also

- `assets/logos/` — wordmark + monogram SVGs in all six color treatments.
- [[typography]] — how type pairs with these colors.
- [[logo-usage]] — color choices specifically for logo lockups.
- [[source-refs]] — where this was extracted from.
