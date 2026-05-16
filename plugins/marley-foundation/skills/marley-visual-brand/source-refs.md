# Source references — marley-visual-brand

Distilled from `visual brand/Brand Assets/`:

- `Marley Colors/Marley Medical_Brand Colors_RGB.cclibs` — Adobe Creative Cloud library file (zip-structured DCX). Unzipped and parsed the `manifest` JSON to extract eight RGB-mode color elements with their hex names and RGB values. Source for: all RGB hex values in [[colors]].
- `Marley Colors/Marley Medical_Brand Colors_CMYK.cclibs` — same format. Source for: all CMYK values in [[colors]].
- `Marley Logos/Digital/SVG/Wordmark/*.svg` (6 files) — copied to `assets/logos/`. Confirms canonical six color treatments.
- `Marley Logos/Digital/SVG/Monogram/*.svg` (6 files) — copied to `assets/logos/`.
- `Marley Logos/Digital/SVG/Icons/<Color>/*.svg` (30 files: 6 colors × 5 icons) — NOT copied into plugin (too redundant); referenced from full library path.
- `Marley Logos/Animated/MarleyMed_Animated-Logo_*.gif` — animated logo variants noted in [[logo-usage]].
- `Marley Logos/Print/` — CMYK print variants in `.ai` format; noted, not copied.
- `Marley Iconography/SVG Exports/*.svg` (13 files: Apple, Bandage, Blood droplet, blood pressure, cross, excercise, heart, needle, pill, scale, sleep, stethoscope, stress, tablet — note: `excercise.svg` is misspelled in source) — copied to `assets/icons/`. Source for icon list in [[image-style]].
- `Marley Iconography/Marley_Icons_Master.ai` — Illustrator master file; not copied (source file).
- `Marley Photography/Headshots/` — 13 BW headshots in both Print (jpg) and Social Media (jpeg) variants. Style noted in [[image-style]]; files not copied.
- `Marley Photography/Marketing photos/` — 7 marketing photos. Three (`Marley_Studio_1.jpg`, `Marley_Studio_Instruments.jpg`, `Marley_Studio_Pills_Hands.jpg`) copied to `assets/photography/` as representative samples.
- `Marley Patterns/Marley_Pattern Template.ai` — pattern template; noted in [[image-style]], not copied.
- `Marley Typography/Primary Fonts/Reckless/` — full Reckless font family with licenses (Desktop + Web). Source for [[typography]].
- `Marley Typography/Primary Fonts/Greycliff_Adobe Fonts.txt` — note about Greycliff being licensed via Adobe Fonts. Source for [[typography]].
- `Marley Typography/Backup Fonts/Newsreader/`, `Backup Fonts/Poppins/` — backup font files noted in [[typography]].
- `Marley_Presentation_MasterTemplate.pptx` — PowerPoint master template. Referenced as a structural source for `payer-pitch-deck/templates/`, `product-scoping-deck/templates/`, and `fundraise-pitch-deck/templates/`. **Layout vocabulary in `layouts.md` was extracted from this file on 2026-05-16 via .pptx-as-zip XML inspection.** The 13 raw PPT layout names (CUSTOM, TITLE, TITLE_1, TITLE_3, TITLE_1_2, TITLE_AND_BODY, TITLE_ONLY, SECTION_TITLE_AND_DESCRIPTION + 4 variants, BLANK) were collapsed to 7 conceptual layout types (TITLE_FAMILY, TITLE_AND_BODY, TITLE_1_2, SECTION_DIVIDER, HERO_STATS, CUSTOM, BLANK) for usability — the raw layout names remain addressable as sub-variants in `layouts.md`.

- `~/epch-claude/payer pitch decks/` — all 5 source payer-deck PDFs. **Composition-pattern vocabulary in `slide-patterns.md` was extracted from these on 2026-05-16 by walking each deck slide-by-slide and identifying recurring visual patterns above the layout level and below the asset level.** Source decks:
  - `Marley Medical - BCBS FL Deck - March 6 2024.pdf` (canonical reference, ~26 slides)
  - `Marley Medical - OSF - March 7 2024.pdf` (health-system-customized, adds ~6 patterns)
  - `Marley Medical Payer Deck - Feb 13 2024.pdf` (generic Feb)
  - `Copy of Marley Medical Payer Deck - Jan 10 2024.pdf` (generic Jan — the first deck of the matured 2024 arc)
  - `Marley Medical - UHC Accelerator - Company Comments - May 2023.pdf` (pre-current-arc, used for evolution analysis only)
  The pattern set is **15 most-used patterns** (appearing in 3+ decks) + ~7 customer-specific patterns (1–2 decks; used when audience calls for them) + ~6 dropped patterns (May 2023 only, replaced in Jan 2024 redesign).

## What's NOT in source

- No formal brand book PDF spelling out color usage rules, clear-space rules, type scale, or photography direction. The rules in [[colors]] / [[logo-usage]] / [[typography]] / [[image-style]] are extracted from observed practice + standard brand-system convention, not from a written brand book.
- Color names ("Marley Purple", "Marley Red", etc.) are derived from logo asset filenames — the Adobe library identifies colors only by hex.
- **Pattern guidance is thin** — the `.ai` pattern template exists in `Brand Assets/Marley Patterns/` but no exported PNG/SVG patterns. `image-style.md` notes pattern use in general terms but doesn't specify named pattern assets. Punted to a future iteration if/when pattern PNGs get exported.
- **Semantic icon and photo mappings in `image-style.md`** are extrapolated from how Marley actually uses these assets in source decks plus standard brand-system convention. Not from an explicit brand-agency mapping document.
- **Pattern names in `slide-patterns.md`** are coined for this skill (Marley uses these patterns consistently but has no formal pattern naming convention). Composition rules per pattern (element counts, surface tendencies, icon roles) are extracted from observed repetition across the 5 source decks, not from a written design system.

## Confidentiality

No confidential material in this category. Type licenses contain invoice IDs and the licensee organization — not copied into plugin.
