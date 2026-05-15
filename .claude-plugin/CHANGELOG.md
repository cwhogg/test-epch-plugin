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

## v0.2.0 — Self-review pass

Self-review identified 20 high+medium-impact improvements applied in one pass. Major changes:

**Foundation-skill descriptions** — stripped "Load whenever…" imperative tails from all 4 foundation SKILL.md descriptions (`marley-principles`, `marley-voice`, `marley-visual-brand`, `marley-context`). Skill matching is similarity-based against user prompts, so descriptions are now purely descriptive of what the skill contains and what kinds of work it's used for. Should improve trigger reliability.

**`marley-voice` self-contradictions fixed** — `banned-phrases.md` had banned "world-class", "seamless", "robust" as self-descriptions, but those exact words appear in canonical Marley source (elevator pitches, May 2021 narrative). Added a new "Phrases with nuance" section that allows them when grounded with concrete substantiation and bans them only when used as standalone vague filler. Same nuance for "best-in-class" and "comprehensive". Added "comprehensive" and "integrated" to `preferred-phrases.md` as Marley-coded words.

**`memo/SKILL.md`** — Step 1 no longer duplicates trigger phrases inline; now points to `audience-cues.md` as single source of truth. Step 3 disambiguates voice register per variant (standard vs. investor-update register). Step 1 also explicitly flags the general-variant source gap.

**`fundraise-pitch-deck/SKILL.md`** — de-hardcoded Sapphire-specific numbers from Step 3 (was: "$6–8M led by a16z", "13 payers, 77% coverage", "$75 PPPM, 35% margin"). Now references `pipeline.md` for current numbers and `examples/sapphire-march-2024-slide-by-slide.md` for the worked example. Footnote example uses bracketed placeholders.

**`payer-pitch-deck/SKILL.md`** — fixed wrong date in footnote example ("Nov 2023" → bracketed placeholder). Step 4 ("Customize per payer") expanded with concrete payer-family knowledge: BCBS plans are independent licensees, Florida Blue is BCBS FL, Anthem rebrand to Elevance Health 2022, MA-specific framing guidance.

**`chris-critic.md`** —
- Always-load list trimmed (moved `market.md` and `pipeline.md` to conditional loading; always-load is now just `company.md` plus principles + voice).
- Added a full variant-awareness block for product-scoping-deck (assumption parallelism, output-metric consistency, math reconciliation, required-attributes filter, honest-about-the-math).
- Added variant-awareness blocks for payer and fundraise that surface what was previously only in the calling SKILL.md files.
- Verdict "No" renamed to "Don't ship" for clarity.
- "Repeating prior critiques" failure mode softened to acknowledge no persistent memory across reviews — only fires when prior critique is passed back as input.

**`product-scoping-deck`** — added `examples/clinical-design-august-2023-slide-by-slide.md` (canonical worked example, parallel to other deck skills' examples files). Fixed awkward Step 2 phrasing.

**`product-scoping-deck/SKILL.md` and `fundraise-pitch-deck/SKILL.md`** — removed inline "critic should pay attention to..." lists that duplicated what chris-critic's own variant-awareness block now covers. Single source of truth for variant-specific scrutiny lives in chris-critic.

**`marley-context/pipeline.md`** — added a "Most current source-attested numbers" summary table at the top, so any artifact pulling current Marley numbers has a single-glance reference.

**`README.md`** — test prompt #5 (general-memo variant) now warns about the source-thin status. Test prompt #9 (fundraise deck) now includes validation criteria for the de-hardcoding fix.

**`marketplace.json`** — added marketplace-level description.

---

When iterating: bump version in `plugins/marley-foundation/plugin.json`, add a new entry here with a brief note on what changed and why.
