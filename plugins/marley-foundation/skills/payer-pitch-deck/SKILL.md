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

- Cover slide: payer name + date
- State-specific evidence: emphasize Marley evidence in payer's primary states if available
- "Easy contracting" slide: reference existing payer-family contracts (BCBS / Anthem / etc.) when applicable
- Patient-selection criteria: tune to payer's likely target population (commercial / MA / Medicaid)

## Step 5 — Hand to chris-critic for review

After drafting, hand the draft to `chris-critic` for review. Read the review returned. Incorporate the highest-impact recommendations into a revised draft. Show the user the revised draft followed by the full review block as an appendix so they can see what was flagged and what changed.

## Step 6 — Cite materially-shaping decisions in a footnote

At the end of the deck (or as a brief note for the user), name the principles / voice rules / context decisions / visual brand choices that materially shaped the output. Example:

> *Drafted with: marley-principles #2 (specialized care) + #6 (fast feedback loops); marley-voice (payer register, no consumer wit); marley-context/market.md (cardiometabolic ICP), pipeline.md (Nov 2023 outcomes); marley-visual-brand (purple-on-cream slide canvas, Reckless display + Greycliff body); payer-pitch-deck/evidence-conventions (Ettehad Lancet citation for downstream-risk reduction).*

## Files

- `narrative-arc.md` — canonical 3-act structure with slide-by-slide breakdown.
- `evidence-conventions.md` — how to cite clinical and economic claims.
- `templates/README.md` — pointer to master PPT.
- `examples/bcbs-fl-march-2024-slide-by-slide.md` — canonical reference deck (redacted as appropriate).
- `source-refs.md` — extraction notes.
