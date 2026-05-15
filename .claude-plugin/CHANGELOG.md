# Changelog — marley-foundation

## v0.1.0 — Initial scaffold

**Foundation skills**
- `marley-principles` — 12 operating principles + decision frameworks, distilled from the June 2020 founding concept doc and the May 2021 Series Seed narrative.
- `marley-voice` — five personality descriptors, voice patterns, banned-phrases and preferred-phrases lists, three exemplar files (brand headlines, elevator pitches, investor-update voice sample). Distilled from the HUb personality deliverable + Brand Voice Marketing Prompt.
- `marley-visual-brand` — color palette (RGB + CMYK hex codes extracted from `.cclibs` library files), Reckless + Greycliff typography, logo usage rules, iconography, image style. 12 wordmark/monogram SVGs + 14 icon SVGs + 3 sample marketing photos copied into `assets/`.
- `marley-context` — company overview, market/ICP, pipeline state (current through March 2024 source decks). Distilled from 11 context PDFs + 11 investor updates + 3 payer decks + 3 fundraise decks.

**Task skills**
- `memo` — single skill with two variants (general + investor-update), routed by audience cues. Investor-update KPI conventions distilled from 9 monthly updates Sept 2021 → Nov 2022. General-memo variant has a flagged source gap (no internal-strategy-memo exemplars in source).
- `payer-pitch-deck` — canonical 3-act narrative arc + evidence-citation conventions, drawn from the March 2024 BCBS FL deck.
- `product-scoping-deck` — analytical-scenario format + the "What would you have to believe to get to X?" pattern, drawn from the August 2023 Clinical Design deck.
- `fundraise-pitch-deck` — investor-pitch arc + three-pillar traction frame + risks-paid-down/underwriting ask framing, drawn from the March 2024 Sapphire deck.

**Sub-agent**
- `chris-critic` — read-only review agent applied after every task-skill draft. Persona, sources-to-load, baseline checks, focus areas, output template, failure modes — all encoded per spec.

**Known gaps flagged**
- `memo` general variant has no source exemplar (the two files in `memos/` were reclassified to payer + fundraise per inventory decision).
- `marley-principles/decision-frameworks.md` flags clinical-protocol decisions, pricing-across-segments, hiring rubric, and vendor-selection as un-formalized.
- `marley-voice/banned-phrases.md` and `preferred-phrases.md` are partly inferred (no formal lists existed in source).
- `marley-visual-brand` clear-space, minimum-size, and numeric type scale are sensible defaults — not from a formal brand book.
- All examples are redacted for confidentiality per the policy.

---

When iterating: bump version in `plugins/marley-foundation/plugin.json`, add a new entry here with a brief note on what changed and why.
