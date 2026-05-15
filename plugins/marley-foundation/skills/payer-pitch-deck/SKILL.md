---
name: payer-pitch-deck
description: Build a Marley Medical payer-facing pitch deck — a visual deck prepared for a named health plan, MA plan, MCO, or risk-taking provider. Triggers on "payer deck for [X]", "pitch deck for [health plan]", "BCBS deck", "MA deck", "deck for [payer name]", "Florida Blue deck", "Anthem deck", or any request to build a deck pitching Marley to a payer audience.
---

# Payer pitch deck skill

This skill produces a slide deck pitching Marley to a named payer audience.

## Step 1 — Confirm the audience

A payer deck is **prepared for a specific named entity**. Confirm which payer the deck is for before drafting:
- Health plan / MA plan / MCO / Medicaid / risk-taking provider
- Specific state market(s) relevant to the payer
- Whether the payer is part of a larger BCBS family / Anthem family / etc. — affects the "Easy contracting" slide framing

If the user hasn't named the payer, ask.

## Step 2 — Load foundation skills

Before drafting:
- Read `../marley-principles/principles.md`
- Read `../marley-voice/voice.md` — payer register: more clinical precision, less consumer wit
- Read `../marley-voice/banned-phrases.md`
- Read `../marley-context/company.md`, `market.md`, and `pipeline.md` — current-state numbers matter
- Read `../marley-visual-brand/colors.md`, `typography.md`, `logo-usage.md`, `image-style.md` — payer decks are visual artifacts; brand fidelity matters

## Step 3 — Draft

Follow the canonical 3-act structure in [[narrative-arc]]:
1. Marley Medical Overview (slides 1–15)
2. How Marley Works with Payers (slides 16–25)
3. Appendix: Clinical Data Deep Dive

Apply [[evidence-conventions]] for clinical and economic claims — cite specific sources, frame outcomes honestly, never use vague qualifiers.

Reference `examples/bcbs-fl-march-2024-slide-by-slide.md` for the canonical structure and slide-level content patterns.

Use the master PPT template at `~/epch-claude/visual brand/Marley_Presentation_MasterTemplate.pptx` as the visual starting point.

## Step 4 — Customize per payer

- **Cover slide:** payer name + date
- **State-specific evidence:** emphasize Marley evidence in payer's primary states if available
- **"Easy contracting" slide:** reference existing payer-family contracts when applicable. Marley payer-family awareness to apply:
  - **BCBS plans** are independent licensees — a contract with one BCBS plan does NOT automatically extend to others. *Florida Blue is BCBS FL; Highmark covers PA / WV / DE / NY (parts); Anthem Blue Cross is a BCBS licensee in some states.* Reference the specific BCBS-affiliate Marley has worked with, not "BCBS" generically.
  - **Anthem / Elevance Health** — Anthem rebranded as Elevance Health (parent) in 2022, but the Anthem brand persists on consumer-facing health plans. The relationship to BCBS Anthem-affiliate plans is specific to each state.
  - **Humana, UnitedHealthcare, Aetna, Cigna** — national for-profit payers. Contract with one MA segment doesn't extend to commercial segment automatically.
  - **MA-specific framing** — pitching an MA plan? Emphasize Star Ratings, MLR reduction in the polychronic 5%, and the engagement gap (up to 30% of MA membership unengaged). These are the highest-leverage points in MA contracting.
- **Patient-selection criteria:** tune to payer's likely target population (commercial / MA / Medicaid). Marley currently excludes Medicaid (per Nov 2022 update — verify current state in `pipeline.md`).

## Step 5 — Hand to chris-critic for review

After drafting, hand the draft to `chris-critic` for review. Read the review returned. Incorporate the highest-impact recommendations into a revised draft. Show the user the revised draft followed by the full review block as an appendix so they can see what was flagged and what changed.

## Step 6 — Cite materially-shaping decisions in a footnote

At the end of the deck (or as a brief note for the user), name the principles / voice rules / context decisions / visual brand choices that materially shaped the output. Example:

> *Drafted with: marley-principles #2 (specialized care) + #6 (fast feedback loops); marley-voice (payer register, no consumer wit); marley-context/market.md (cardiometabolic ICP), pipeline.md ([dated clinical outcomes — pull current date and metrics from pipeline.md at draft time]); marley-visual-brand (purple-on-cream slide canvas, Reckless display + Greycliff body); payer-pitch-deck/evidence-conventions (Ettehad Lancet citation for downstream-risk reduction).*

## Files

- `narrative-arc.md` — canonical 3-act structure with slide-by-slide breakdown.
- `evidence-conventions.md` — how to cite clinical and economic claims.
- `templates/README.md` — pointer to master PPT.
- `examples/bcbs-fl-march-2024-slide-by-slide.md` — canonical reference deck (redacted as appropriate).
- `source-refs.md` — extraction notes.
