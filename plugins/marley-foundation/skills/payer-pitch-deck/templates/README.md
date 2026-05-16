# Payer deck templates

The canonical visual template lives in source at:
`~/epch-claude/visual brand/Marley_Presentation_MasterTemplate.pptx`

This is a PowerPoint master template that contains Marley's brand-formatted slide layouts (title, section, content, data, etc.). Use it as the starting point for any payer-facing deck.

## Workflow

1. Open `Marley_Presentation_MasterTemplate.pptx` in PowerPoint or Keynote.
2. Save a copy named for the specific deck: `Marley Medical - <Payer> Deck - <Date>.pptx`.
3. Build the deck following the canonical 3-act narrative arc in `../narrative-arc.md`.
4. Customize for the specific payer (see "Payer-specific customization" in narrative-arc.md).
5. Apply visual brand rules from `../../marley-visual-brand/` — colors, typography, logo placement.
6. When building in PowerPoint, choose the named layout from the master's Slide Layout panel that matches what `../narrative-arc.md` specifies for each slide — the names in narrative-arc.md (e.g. `TITLE_1_2`, `BLANK`, `HERO_STATS`) map directly to the master's layout panel via `../../marley-visual-brand/layouts.md`.

## What this folder does NOT contain

The actual `.pptx` is not duplicated into the plugin. The source-of-truth template lives in `visual brand/`. This folder is a pointer; treat the source path as canonical.

If a separate payer-deck-specific master ever gets produced (e.g. a payer-optimized layout set), drop it here.
