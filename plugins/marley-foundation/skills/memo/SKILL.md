---
name: memo
description: Draft a Marley Medical memo — either a Decision Memo (default — Marley's canonical 7-section format for documenting non-trivial decisions: Goal / Stakeholders / Context / Decision / Rationale / Alternatives / Decider), or a periodic investor update memo. Triggers on "decision memo", "write a memo", "draft a memo on [X]", "document the decision to [X]", "need to decide [X] — write it up", "investor update", "monthly investor memo", "quarterly update", or similar. Variant selection happens inside the skill based on audience cues; when ambiguous, the skill will ask which variant before drafting.
---

# Memo skill — handles two variants

This skill produces written memo deliverables. It has **two variants**: general/strategy memo (default) and investor-update memo. Variant routing happens at the top of the skill based on audience cues.

## Step 1 — Detect variant

Read `audience-cues.md` and apply its routing logic. That file is the single source of truth for trigger-phrase lists, disambiguation rules, and the "what is NOT a memo" routing-elsewhere logic. When variant is ambiguous, ask the user — see the example clarifying question in `audience-cues.md`.

Both variants are now well-grounded in source: the general variant (Decision Memo) is anchored in Marley's own template + a fully worked example (Disease Focus draft, Dec 2021); the investor-update variant is anchored in 10 monthly updates spanning Sept 2021 → Nov 2022.

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

Use `format.md` for the structural template. Match the variant to its scaffold:
- **Variant A (general)**: title → framing → argument sections → recommendation → open questions.
- **Variant B (investor update)**: title → tl;dr → The Plan → Help Requests → Team → section-by-section progress → Financials → Cash-out → Fundraising Q's → Topics for discussion.

Apply Marley voice — but pick the right register for the variant:
- **Variant A** → standard Marley voice (see `../marley-voice/voice.md` general voice characterization). Plainspoken, contractions, specific numbers, no corporate hedging.
- **Variant B** → investor-update register specifically (see `../marley-voice/voice.md` section *"Investor-update voice (same DNA, more operational)"*). Same DNA as standard voice plus: lowercase `tl;dr` section header, operational candor (*"hunker down"*, *"lots of duct tape"*, *"a worthy and fun problem to solve"*), numbered fundraising questions, scenario tables for cash-out, every numeric claim tied to source.

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
  - `general-template-decision-memo.md` — Marley's own Decision Memo template (verbatim from source).
  - `general-decision-memo-disease-focus.md` — fully worked Decision Memo example (Disease Focus draft, Dec 2021).
  - `investor-update-december-2021.md` — redacted pre-launch update.
  - `investor-update-may-2022.md` — redacted post-launch update.
- `source-refs.md` — extraction notes.
