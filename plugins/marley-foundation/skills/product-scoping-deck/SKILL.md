---
name: product-scoping-deck
description: Build a Marley Medical product-scoping deck — an internal analytical deck that models scenarios, evaluates trade-offs, and supports a product/operational/clinical decision. Triggers on "scope this", "scoping deck for [X]", "capacity analysis", "model scenarios for [X]", "what would we have to believe to get to [target]", "clinical design deck", "PRD-style deck", or any request to think through a product/operational decision via scenario modeling.
---

# Product-scoping deck skill

This skill produces an internal analytical deck for thinking through a product, operational, or clinical decision. **Not for external audiences** (payer / investor / partner) — those route to their respective skills.

## Step 1 — Confirm the scoping question

A product-scoping deck answers a specific decision question. Confirm with the user:
- What is the decision being made?
- What are the constraints / required attributes?
- What scenarios should be modeled?

If the question is vague ("scope our product"), push back: ask for the specific decision.

## Step 2 — Load foundation skills

Before drafting:
- Read `../marley-principles/principles.md` and `decision-frameworks.md` — product-scoping decks reflect how Marley actually reasons about decisions; load these before drafting
- Read `../marley-voice/voice.md` — internal register: most candid, most operationally honest
- Read `../marley-context/pipeline.md` — current-state numbers anchor scenario assumptions
- Read `../marley-visual-brand/colors.md`, `typography.md`, `logo-usage.md` — scoping decks are still visual artifacts; brand still applies

## Step 3 — Draft

Reference `examples/clinical-design-august-2023-slide-by-slide.md` for the canonical worked example. Follow the canonical structure in [[narrative-arc]]:
1. Cover
2. The Problem (what's not working today)
3. Required attributes / criteria for the solution
4. The Analysis (methodology)
5. Key Learnings (meta-takeaways before scenarios)
6. Scenario walkthrough — one slide per scenario using [[scope-template]]
7. (Recommended) Cross-scenario summary table
8. Appendix

For each scenario slide, use the scenario template in [[scope-template]]:
- Title (honest, often colloquial — e.g. "What would you have to believe to get to 2,000?")
- Assumptions block (4–7 structural choices)
- Output metrics (2–4, displayed prominently, consistent across scenarios)

## Step 4 — Use the "What would you have to believe" pattern

When the scoping question involves an ambitious target, use the signature Marley framing:
> *"What would you have to believe to get to [target]?"*

Then write the assumption set required for the target, display the output metrics, and let the room discuss whether the assumption set is plausible.

## Step 5 — Hand to chris-critic for review

After drafting, hand the draft to `chris-critic` for review. Read the review returned. Incorporate the highest-impact recommendations into a revised draft. Show the user the revised draft followed by the full review block as an appendix so they can see what was flagged and what changed.

The critic has product-scoping-deck-specific scrutiny encoded in its variant-awareness block — assumption parallelism, output-metric consistency, math reconciliation, required-attributes filter, and honest-about-the-math checks all happen automatically.

## Step 6 — Cite materially-shaping decisions in a footnote

> *Drafted with: marley-principles #1 (plans are hypotheses) + #11 (eliminate friction); marley-voice (internal register, most candid); product-scoping-deck/narrative-arc (problem → required attributes → scenarios), scope-template ("What would you have to believe" framing for ambitious targets); marley-context/pipeline.md (current panel size, current outcomes for scenario anchoring).*

## Files

- `narrative-arc.md` — overall structure.
- `scope-template.md` — slide-level template for scenarios, plus the "What would you have to believe" pattern.
- `templates/README.md` — pointer to master PPT.
- `source-refs.md` — extraction notes.
