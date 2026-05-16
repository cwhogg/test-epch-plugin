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

## v0.5.0 — Slide composition patterns extracted from all 5 source payer decks

v0.4.0 added named layouts (the structural skeleton) and per-slide asset specification. But "Layout: TITLE_AND_BODY" + "Surface: Cream" still leaves wide latitude for what a slide actually *looks like* — the same layout can host an annotated timeline, a 4-box grid, or a radial team diagram. The missing middle layer is the **composition pattern**: the recurring visual templates that give Marley payer decks their look.

This release adds that pattern vocabulary, extracted by walking all 5 source payer decks slide-by-slide and identifying patterns that recur across them.

**Foundation — new file `marley-visual-brand/slide-patterns.md`**

Distilled from all 5 payer-deck PDFs (BCBS FL March 2024, OSF March 2024, Feb 13 2024 generic, Jan 10 2024 generic, UHC Accelerator May 2023). Each pattern entry includes: composition rules (element count, asset role, surface tendencies), when-to-use, host layout, source-slide references across all 5 decks.

15 most-used patterns (3+ decks):
- `horizontal-process-flow` (14 occurrences) — narrative-box / patient-journey / claim-circle sub-variants
- `2-column-pivot` (8) — the canonical pivot slide (Peach left / Sky right)
- `positioning-diagram` (8) — Marley elevated middle band between Specialists / PCPs
- `paper-thumbnails` (8) — citation thumbnails as background credibility props
- `3-column-option-compare` (7) — three contracting structures / three acquisition paths
- `logos-row` (7) — investor / payer / press-credibility row
- `hero-photo-with-overlay` (6) — the canonical Welcome treatment (every deck)
- `headline-only-section-divider` (6)
- `multi-chart-grid + stat-strip` (5) — the canonical clinical-results slide
- `n-box-equal-grid (4-box)` (5) — selection criteria / value-prop summary
- `n-box-equal-grid (6-box)` (4) — payer-fit grid
- `hero-stat-grid` (4) — canonical position-4 problem-framing slide
- `stat-stack` (4) — engagement KPIs (always Purple cards, no icons)
- `annotated-timeline` (4) — canonical patient-case slide (8–9 dots, 4 colored zones)
- `radial-team-diagram` (4) — 6 satellite role labels around Marley m-diamond center

Customer-specific patterns (1–2 decks; invoke when audience calls for them):
- `geographic-map` (health-system / multi-state-payer audiences)
- `gantt-chart` (B2B contracting pipeline — OSF only; health-system audiences)
- `diagram-with-arrows (FFS→VBC upgrade)` (OSF only; contract-economics narratives)
- `2-column-photo-overlay` (illustrative patient photo — mostly demoted to appendix)
- `logos-grid (payer portfolio)` (only in generic decks; awkward in customer-specific decks)
- `metric-over-time-chart` (rarer than expected; usually subsumed by `multi-chart-grid + stat-strip`)
- `two-stat-emphasis` (single giant number; paired with paper-thumbnail substantiation)
- `bulleted-toc` (longer / more formal customer decks only)

Dropped patterns (May 2023 only; replaced in Jan 2024 redesign — don't reach for these):
- `checklist-vs-status-table`, `tabbed-card`, `9-icon services grid`, `distribution-bar-breakdown` ROI waterfall, `8-box n-grid`, `radial-ecosystem-diagram`

Plus pattern → host layout and pattern → surface tendency tables, plus evolution notes (May 2023 → Jan → Feb → March 2024).

**Foundation — supporting updates**
- `marley-visual-brand/SKILL.md` — description and load steps include slide-patterns; files section adds it.
- `marley-visual-brand/source-refs.md` — documents the 5-deck pattern-extraction provenance (extracted 2026-05-16) and notes that pattern names are coined for this skill (Marley has no formal pattern-naming convention) and composition rules are extracted from observed repetition across decks.

**Task skill — `payer-pitch-deck`**
- `SKILL.md` Step 2 loads `slide-patterns.md`. Step 3 now requires a `Pattern` field in the per-slide visual spec alongside Layout / Surface / Icon / Photo / Logo. Adds pattern-diversity target (6+ distinct patterns across ~26 slides), customer-specific-pattern guidance, and dropped-pattern avoidance.
- `narrative-arc.md` — every slide in all 3 acts (cover + 25 content slides + 10 appendix) gets a `Pattern:` line in its Visual spec block naming the specific composition pattern that fits the slide's communicative job.
- `examples/bcbs-fl-march-2024-slide-by-slide.md` — 5 representative retrofitted slides now include Pattern lines (cover, hero-stat-grid slide 4, patient-journey slide 11, patient-case slide 14, 2-column-pivot slide 16). New footer note enumerates the ~10 distinct patterns the BCBS deck uses across its slides.

**Sub-agent — `chris-critic`**
- "Any deck" conditional-load list now includes `slide-patterns.md`.
- "Any deck — visual specificity" variant-awareness block expanded with: pattern-named-per-slide check, layout-and-pattern-diversity check (≥4 layouts + 6+ patterns), pattern-fit-per-slide-job check (e.g. hero-stat-grid only at position 4; stat-stack only on engagement-KPI slides; annotated-timeline only on patient-case slides; radial-team-diagram only on care-team slides), customer-specific-pattern appropriateness check, dropped-pattern avoidance check.
- Diagnostics output template's `Visual specificity (decks only)` line now references pattern naming alongside layout and asset naming.

**What this doesn't do (deferred):** fundraise-pitch-deck and product-scoping-deck per-slide Pattern annotations (they benefit transitively from `slide-patterns.md` but their own narrative-arc files weren't retrofitted this pass). No Pattern-line retrofit on the other ~21 BCBS example slides beyond the original 5.

---

## v0.4.0 — Per-slide visual specificity + named layouts vocabulary

End-to-end test of the payer-pitch-deck skill via Claude Cowork surfaced two visual-design weaknesses: generated decks used uniform layouts (mostly one-column text blocks) and named no specific brand assets per slide (generic "a clinical icon", "a hero photo"). Root cause: the visual-brand skill documented *what* the brand contains but never gave Claude a vocabulary for *how to compose with it* per slide. This release adds that vocabulary and makes per-slide visual specification required.

**Foundation — `marley-visual-brand`**
- New file `layouts.md` — extracts the 13 raw PPT layouts from `Marley_Presentation_MasterTemplate.pptx` and collapses them to **7 conceptual layout types** (`TITLE_FAMILY`, `TITLE_AND_BODY`, `TITLE_1_2` 2-panel, `SECTION_DIVIDER`, `HERO_STATS`, `CUSTOM`, `BLANK`). Each entry includes canonical PPT layout name(s), description, when-to-use guidance, palette pairings, and asset-pairing hints. Includes a deck-level layout-diversity rule (≥4 distinct layouts across a ~25-slide deck).
- `SKILL.md` — description updated to mention "7 named slide layout types"; load step added for `layouts.md`; files section updated.
- `colors.md` — added "Deck-level palette diversity" section with target distribution (~40% Cream / ~25% Peach / ~25% Sky / ~10% Red-accent) and a slide-type → surface quick-reference table.
- `image-style.md` — replaced the bare list of 13 icons with a **semantic icon mapping table** (one row per icon: SVG filename + when-to-use), with the 4 highest-frequency icons bolded (`Marley_blood_pressure.svg`, `Marley_heart.svg`, `Marley_pill.svg`, `Marley_stethoscope.svg`). Same treatment for the 7 marketing photos (JPG filename + when-to-use). New "Don't refer to assets generically" rule — always name the file.
- `source-refs.md` — noted the .pptx-as-zip XML extraction and the 13→7 collapse; flagged that pattern guidance is punted until exported PNGs exist; flagged that semantic mappings are extrapolated from observed practice, not from a brand-agency mapping document.

**Task skill — `payer-pitch-deck`**
- `SKILL.md` Step 2 loads `layouts.md`. Step 3 has a new "Per-slide visual specification (required)" subsection mandating Layout / Surface / Icon / Photo / Logo per slide, with layout-diversity (≥4 distinct) and palette-diversity targets.
- `narrative-arc.md` — every slide across all 3 acts (cover, hero stats, PCP-burden, new-category, panel-profile, patient-journey, engagement metrics, patient case, clinical results, payer-needs 2-col pivot, easy-to-work-with, three-stages, three-contracting-structures + visualizations, thank-you, plus appendix) now includes a "Visual spec" block naming the layout, surface color, semantic icon (when applicable), hero photo (when applicable), and logo lockup variant.
- `examples/bcbs-fl-march-2024-slide-by-slide.md` — retrofitted 5 representative slides with full Visual spec blocks (cover, hero stats, patient journey hero photo, patient case timeline, payer-needs pivot) to demonstrate the convention on the canonical reference deck.
- `templates/README.md` — added a workflow step tying PowerPoint's Slide Layout panel names to `layouts.md`.

**Sub-agent — `chris-critic`**
- "Any deck" conditional-load list now includes `image-style.md` and `layouts.md`.
- New "Any deck — visual specificity" variant-awareness block checks: layout named per slide, layout diversity (≥4 distinct), surface named per slide, palette diversity (no >70% single color), assets named by filename, asset semantic fit per `image-style.md` mapping.
- Diagnostics output template gains `Visual specificity (decks only): pass / partial / fail` line.

**What this doesn't do (deferred):** fundraise-pitch-deck and product-scoping-deck per-slide annotations (they benefit transitively from the foundation changes — `layouts.md`, semantic icon/photo mappings, palette diversity rule — but their own narrative-arc files weren't retrofitted this pass). Pattern guidance still punted (no exported PNG patterns in source). Per-slide font sizing intentionally not duplicated (typography.md owns the scale).

---

## v0.3.2 — Plugin directory structure + YAML frontmatter fixes

Three issues uncovered by `claude plugin validate` that were causing Cowork's "Marketplace sync failed":

- **`plugin.json` was at `plugins/marley-foundation/plugin.json`** instead of inside its own `.claude-plugin/` directory. The validator requires `plugins/marley-foundation/.claude-plugin/plugin.json`. Moved via `git mv`.
- **`marley-voice/SKILL.md` and `memo/SKILL.md` had unquoted `: ` (colon-space) mid-description**, which YAML parses as a key:value separator and silently drops the entire frontmatter. Both descriptions converted to YAML folded-scalar (`>-`) form. Other 6 SKILL.md descriptions were fine but those two contained phrases like *"writing: marketing copy"* and *"non-trivial decisions: Goal..."* that broke parsing.
- **`plugin.json` missing `author` field** (validator warning, not error). Added `{"name": "Chris Hogg", "email": "cwhogg@gmail.com"}`.

Local `claude plugin validate .` and `claude plugin validate ./plugins/marley-foundation` both now return `✔ Validation passed`.

## v0.3.1 — Marketplace.json schema fix

Two schema corrections in `.claude-plugin/marketplace.json` that were causing "Failed to add marketplace" in Cowork:

- `owner` was a string (`"Chris Hogg"`); per the Claude Code plugin marketplace spec it must be an object with a `name` field — fixed to `{"name": "Chris Hogg"}`.
- Plugin reference field was `path`; the spec requires `source` (with a `./` prefix for paths relative to repo root) — fixed to `"source": "./plugins/marley-foundation"`.

No plugin content changes; this is a manifest-only fix.

## v0.3.0 — Memo general-variant rebuild + Decision Framework v1

Two related additions in one pass.

**Fix 1 — Memo general variant rebuilt from real Marley exemplars.** Previously the general-memo variant had a flagged source gap (no canonical internal-strategy memos in source). Chris added 5 files to `memos/`; we used 2 of them (the Marley-authored Decision Memo TEMPLATE and the December 2021 Disease Focus draft) to fully ground the variant. The other 3 (2 inbound Foley & Lardner legal memos, 1 internal Quality Manual) are explicitly excluded as different genres — documented in source-refs.md.

- `memo/format.md` — Variant A fully rewritten. Now anchored in Marley's canonical 7-section Decision Memo structure (Goal / Stakeholders / Context / Decision / Rationale / Alternatives Considered / Final Decision Date & Decider). Investor-update variant untouched.
- `memo/examples/general-placeholder.md` — deleted (placeholder retired, real exemplars now exist).
- `memo/examples/general-template-decision-memo.md` — new. Marley's canonical Decision Memo template, distilled with RACI stakeholder block.
- `memo/examples/general-decision-memo-disease-focus.md` — new. Fully worked example (the December 2021 disease-selection decision). Preserves historical RAPID terminology with a clear "use RACI going forward" note.
- `memo/SKILL.md` — description tightened to include "decision memo" trigger phrases and name the 7-section structure. Step 1 source-gap warning removed (no longer applies). Files-section updated.
- `memo/audience-cues.md` — added explicit "Decision Memo" trigger phrases under the general-variant list. Added a new "Adjacent artifact types — route elsewhere" section calling out inbound legal memos and standards documents as not-memos-this-skill-handles.
- `memo/source-refs.md` — general-variant section now properly populated with the 2 distilled exemplars. The 3 excluded files (2 Foley legal memos + Quality Manual) explicitly documented as different genres.
- `agents/chris-critic.md` — new memo-general-variant scrutiny block. Checks for: declarative Decision statement, RACI stakeholder block, named framework in Rationale, tables for option comparison, quantitative claims source-tied, alternatives genuinely considered, risks named with mitigants, correct title format.

**Fix 2 — Decision Framework v1 authored by Chris.** Replaces the prior `decision-frameworks.md` placeholder. The 7 questions are Chris's verbatim text; surrounding framing is minimal (cross-references and a RACI/RAPID reconciliation note).

- `marley-principles/decision-frameworks.md` — fully rewritten. The 7 questions (What is the decision / Possible outcomes / Execution requirements / Downsides / Reversibility (two-way vs. one-way door) / Who decides + consulted (RACI) / How we track outcomes). Cross-references to `principles.md`, memo format.md Variant A, and the Disease Focus example.
- `marley-principles/SKILL.md` — Step 2 of "What to do when this skill loads" now explicitly directs Claude to apply the 7-question framework for any non-trivial decision; walk the user through it if they haven't structured their thinking that way.
- `marley-principles/source-refs.md` — new "Authored content (not source-distilled)" section recording the framework as Chris-authored on 2026-05-14. Replaces the prior "What's MISSING from source" gap-list with a "single canonical framework — no per-area sub-frameworks" note.
- `agents/chris-critic.md` — Operational-questions section in primary critique focus expanded with explicit 7-question coverage. The critic now draws operational questions from the framework when reviewing artifacts that involve decisions; surfaces 2–3 questions where the document has a real gap (not all 7 on every artifact).

**RACI as canonical stakeholder frame.** Chris decided RACI (over RAPID) is the going-forward Marley convention for stakeholder authority. Ripple changes applied:
- Decision Frameworks Q6 reconciliation note positions RACI as canonical, RAPID as historical-only.
- `memo/format.md` Variant A Section 2 — RAPID frame replaced with RACI frame; historical-convention note added.
- `memo/examples/general-template-decision-memo.md` — RAPID format reference in Stakeholders section updated to RACI.
- `memo/examples/general-decision-memo-disease-focus.md` — preserves historical RAPID verbatim (faithful reproduction) with a clear "convention has since changed to RACI" callout at the top.
- `agents/chris-critic.md` memo-general-variant block — checks for RACI; notes historical RAPID is OK in historical documents.

**Gap closures (vs. v0.2.0).** Two of the seven scaffold-time gaps are now closed:
- ~~General-memo variant has no real exemplar~~ → closed (template + worked example now distilled from source).
- ~~`decision-frameworks.md` flags 4 un-formalized frameworks~~ → closed (7-question meta-framework is the single canonical framework; per-area sub-frameworks intentionally not maintained).

Remaining gaps (4): visual-brand defaults validation, payer FAQ/objection-handling, fundraise FAQ/objection-handling, no forward-looking product-vision deck. All require Chris's input or new source artifacts.

---

When iterating: bump version in `plugins/marley-foundation/plugin.json`, add a new entry here with a brief note on what changed and why.
