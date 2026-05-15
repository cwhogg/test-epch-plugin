# Audience cues — picking the memo variant

The memo skill has two variants. Pick based on user cues before drafting. If ambiguous, ask.

---

## Investor-update variant — triggers

Use the investor-update variant when the user's request contains any of:

- The literal phrase "investor update", "monthly investor update", "quarterly update", "investor memo"
- Periodic framing: "this month", "monthly", "May update", "update for the period", "Q1 update"
- Audience explicitly named as investors / the cap table / "our board" *in a periodic-cadence context*
- "Update for the investors", "update for the round", "memo to investors"
- Recurrence cue: the user references prior updates ("for the next update", "follow up to last month's")

When investor-update variant is selected:
- Use the structure in [[format]] — tl;dr + Plan + Help Requests + Team + Section progress + Financials + Cash-out + Fundraising Q's + Topics for discussion
- Apply [[kpi-conventions]] for KPI formatting
- Voice: investor-update register (see `../marley-voice/voice.md` "Investor-update voice")

---

## General-memo variant — triggers

Use the general-memo variant when the user's request contains any of:

- "Memo", "one-pager", "strategy memo", "internal memo", "thought piece"
- "Pitch memo for [non-investor party]" (e.g. partnership memo)
- "Write up [topic]" without a specific audience cue
- Audience is named but not the investor list: "memo for the team", "memo for [partner / advisor]"
- One-off framing — no periodic-cadence cue

When general-memo variant is selected:
- Use the recommended scaffold in [[format]]
- KPI conventions don't apply — use whatever metrics serve the argument
- Voice: standard Marley voice (see `../marley-voice/voice.md`)

---

## Disambiguation — ask the user when:

- The trigger phrase is ambiguous ("write a memo about the new payer contract" — investor update? internal? for the partner?)
- The user names a periodic cadence but the audience is not investors ("monthly memo to the team")
- The user says "update" without a specific audience

Example clarifying question:
> *Quick check — is this a periodic investor update (monthly/quarterly investor memo cadence) or a standalone strategy memo? I'll structure it differently for each.*

---

## When in doubt, default to general-memo variant

If you can't tell after one clarifying question, the general-memo variant is the safer default — it's lower-stakes in structure (more flexible) and easier to upgrade to investor-update format if needed than vice versa.

---

## What is NOT a memo

Some requests look memo-adjacent but should route elsewhere:

- **"Pitch deck for investors"** / **"fundraise deck"** → route to `fundraise-pitch-deck` skill, not memo.
- **"Payer deck"** / **"deck for [health plan]"** → route to `payer-pitch-deck` skill, not memo.
- **"Scoping deck for [product]"** → route to `product-scoping-deck` skill.

A *deck* is visual / slide-based. A *memo* is prose / narrative.

The Series A *memo* in source (Marley Medical Series A Memo, Jan 2024) is a narrative document — that's a fundraise-pitch artifact and lives in fundraise-pitch-deck examples per the inventory.
