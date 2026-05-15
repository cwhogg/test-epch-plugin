---
name: memo
description: Draft a Marley Medical memo — either a strategy/internal memo (default), or a periodic investor update memo. Triggers on "write a memo", "draft an investor update", "monthly investor memo", "quarterly update", "one-pager on", "strategy memo", "update for the investors", "memo to the team", or similar. Variant selection happens inside the skill based on audience cues; when ambiguous, the skill will ask which variant before drafting.
---

# Memo skill — handles two variants

This skill produces written memo deliverables. It has **two variants**: general/strategy memo (default) and investor-update memo. Variant routing happens at the top of the skill based on audience cues.

## Step 1 — Detect variant

Read [[audience-cues]] and detect which variant the user wants.

- **Investor-update triggers**: "investor update", periodic-cadence framing, audience explicitly named as investors on a recurring cadence → use Variant B.
- **General-memo triggers**: "memo", "one-pager", "strategy memo", audience is not the investor list → use Variant A.
- **When ambiguous**: ask the user. *"Quick check — is this a periodic investor update, or a standalone strategy memo?"*

## Step 2 — Load foundation skills

Before drafting any memo:
- Read `../marley-principles/principles.md` — let principles shape framing.
- Read `../marley-voice/voice.md` — voice is non-negotiable. Plainspoken, contractions, no corporate hedging.
- Read `../marley-voice/banned-phrases.md` — avoid these phrases.
- Read `../marley-context/company.md` (and `pipeline.md` if current state matters).

If the variant is **investor-update**, also read:
- `../marley-voice/examples/03-investor-update-voice-sample.md` — investor-update register.
- [[kpi-conventions]] — the KPI patterns to include.
- `examples/investor-update-may-2022.md` and `examples/investor-update-december-2021.md` — for cadence and structure reference.

## Step 3 — Draft

Use [[format]] for the structural template. Match the variant to its scaffold:
- **Variant A (general)**: title → framing → argument sections → recommendation → open questions.
- **Variant B (investor update)**: title → tl;dr → The Plan → Help Requests → Team → section-by-section progress → Financials → Cash-out → Fundraising Q's → Topics for discussion.

Apply Marley voice throughout. Specific numbers, no hedging, "tl;dr" lowercase for investor updates.

## Step 4 — Hand to chris-critic for review

After drafting, hand the draft to `chris-critic` for review. Read the review returned. Incorporate the highest-impact recommendations into a revised draft. Show the user the revised draft followed by the full review block as an appendix so they can see what was flagged and what changed.

## Step 5 — Cite materially-shaping decisions in a footnote

At the end of the memo (or in a brief footnote), name the principles / voice rules / context decisions that materially shaped the output. Example:

> *Drafted with: marley-voice (investor-update register; "tl;dr" lowercase, no corporate hedging), memo/kpi-conventions (patient count + delta, BP outcomes, NPS with sample size, scenario-based cash-out table), marley-principles #12 (honest framing of open problems).*

## Files

- `format.md` — both-variant structural templates.
- `audience-cues.md` — variant-routing logic.
- `kpi-conventions.md` — KPI reporting standards (investor-update variant only).
- `examples/` — exemplars:
  - `general-placeholder.md` — placeholder noting source-thin variant.
  - `investor-update-december-2021.md` — redacted pre-launch update.
  - `investor-update-may-2022.md` — redacted post-launch update.
- `source-refs.md` — extraction notes.
