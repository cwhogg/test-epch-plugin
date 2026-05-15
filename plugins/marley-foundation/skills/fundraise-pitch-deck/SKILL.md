---
name: fundraise-pitch-deck
description: Build a Marley Medical fundraise pitch deck — a visual investor-facing deck for a named round or named firm. Triggers on "fundraise deck", "Series A deck", "Series B deck", "pitch deck for [investor firm]", "deck for [VC name]", "investor pitch deck for the round", "a16z deck", "Sapphire deck". Distinct from the memo skill's investor-update trigger — a fundraise deck is a visual artifact for a specific round, NOT a written periodic update to existing investors.
---

# Fundraise pitch deck skill

This skill produces a visual investor-facing pitch deck for a named round or named firm.

## ⚠️ Don't collide with investor-update memo

If the user says "investor update" or any periodic-cadence framing — that's the **memo skill (investor-update variant)**, not this skill.

If the user says "pitch deck", "fundraise deck", "Series X deck", or names a specific firm/round — that's this skill.

If ambiguous, ask:
> *"Quick check — is this a visual pitch deck for a specific firm / named round (e.g. Series A deck for Sapphire), or a periodic written investor update memo? I'll structure it differently for each."*

## Step 1 — Confirm the audience and the round

- Which firm is this deck prepared for?
- Which round? (Series A / Series B / bridge / etc.)
- Is there a named lead investor?
- Round-size target?

## Step 2 — Load foundation skills

Before drafting:
- Read `../marley-principles/principles.md`
- Read `../marley-voice/voice.md` — investor-pitch register: confident, plainspoken, specific numbers, no corporate hedging
- Read `../marley-voice/banned-phrases.md`
- Read `../marley-context/company.md`, `market.md`, `pipeline.md` — current-state numbers anchor traction
- Read `../marley-visual-brand/colors.md`, `typography.md`, `logo-usage.md`, `image-style.md`

## Step 3 — Draft

Follow the canonical structure in [[narrative-arc]]:

**First half (similar to payer deck):** What Marley is, the problem, the new category, the model, clinical evidence.

**Second half (fundraise-specific):**
- B2C2B GTM strategy (5 steps)
- Patient growth trajectory (multi-year bar chart with multipliers)
- AI / platform roadmap (Fetch + LLM-assisted functions)
- Payer contracts (13 payers, 77% coverage, 31M lives, $75 PPPM, 35% margin)
- Contract upgrade path (FFS → outcomes-based: $75 → $150 PPPM, 35% → 65% margin)
- B2B pipeline (named targets)
- The Plan (Growth / Revenue / Partnerships / Unit economics quadrants)
- Team (Propeller heritage)
- **The Ask** — risks paid down vs. risks being underwritten

Apply [[traction-conventions]] for the three-pillar traction frame (patient growth + clinical evidence + payer contracting).

Reference `examples/sapphire-march-2024-slide-by-slide.md` for the canonical structure.

## Step 4 — Customize per firm

- Cover slide: firm name + date
- Named lead investor on the ask slide
- Investor track-record / team slide tuned to firm's thesis (consumer brand → Roman/Hims framing; clinical → Galileo/Firefly; value capture → Oak/ChenMed)
- B2B pipeline: emphasize targets relevant to firm's portfolio

## Step 5 — Hand to chris-critic for review

After drafting, hand the draft to `chris-critic` for review. Read the review returned. Incorporate the highest-impact recommendations into a revised draft. Show the user the revised draft followed by the full review block as an appendix so they can see what was flagged and what changed.

The critic should pay extra scrutiny to:
- Whether traction framing is specific and source-tied (no vague growth claims)
- Whether the ask is clearly framed and properly disarmed via risks-paid-down/underwriting
- Whether the multi-year plan is internally consistent (patients × PPPM → ARR math holds)
- Whether the team slide says something specific (Propeller exit details) vs. generic credentialing

## Step 6 — Cite materially-shaping decisions in a footnote

> *Drafted with: marley-principles #3 (B2C2B) + #8 (broad in-network); marley-voice (investor-pitch register, specific numbers, no hedging); marley-context/pipeline.md (1,250 patients enrolled / 13 payer contracts / $75 PPPM); fundraise-pitch-deck/traction-conventions (three-pillar traction, risks-paid-down vs. underwriting frame); marley-visual-brand (purple-on-cream slide canvas, Reckless display + Greycliff body).*

## Files

- `narrative-arc.md` — canonical slide-by-slide structure.
- `traction-conventions.md` — three-pillar traction frame, multi-year plan format, risks framing, CAC discipline, team-narrative pattern.
- `templates/README.md` — pointer to master PPT.
- `examples/sapphire-march-2024-slide-by-slide.md` — canonical reference deck.
- `source-refs.md` — extraction notes.
