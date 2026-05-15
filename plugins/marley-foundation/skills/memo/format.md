# Memo format — General + Investor Update variants

This skill handles two memo variants. **Variant selection happens via audience cues** before drafting — see [[audience-cues]] for routing logic.

Both variants share the same Marley voice (see `../marley-voice/voice.md`). The variants differ in **structure**, **length**, and **content conventions** — not in tone.

---

# Variant A — General Memo (default) — "Decision Memo"

The general-memo variant is the **Decision Memo** — Marley's canonical format for documenting non-trivial decisions: strategic, operational, organizational, technical. Use it whenever the memo's purpose is to make or document a decision, not just to inform.

Marley has a written template (`examples/general-template-decision-memo.md`) and a worked-example draft (`examples/general-decision-memo-disease-focus.md`). Read both before drafting.

## Title format

`Decision Memo: [question or topic]`

If still in draft, prefix with `DRAFT`: `DRAFT Decision Memo: [topic]`.

## Canonical structure — 7 sections

Use these section headers verbatim. Bare nouns, no question marks, no fluff.

### 1. Goal

Single paragraph (~3–6 sentences). Explain why we're making a decision on this question or topic and how it's important to Marley. Frame the stakes.

> *Example: "For Marley's first launch, we need to deliberately select which disease to support. While we will be able to pivot and expand later, there could be significant time and cost penalties to do so."*

### 2. Stakeholders

Short block. Two parts:

- **Who/what is impacted by this decision** — usually one sentence naming the affected groups.
- **RACI frame for the decision itself** — explicit named callouts:
  - *"[Name] (role) is **Responsible**"* — the person doing the work to execute the decision
  - *"[Name] is **Accountable**"* — the single decider; the person whose call this is
  - *"[Name], [Name] are **Consulted**"* — people whose input is sought before deciding (have voice, not veto)
  - *"[Name], [Name] are **Informed**"* — people who need to know the decision after it's made

RACI is Marley's canonical stakeholder frame for new Decision Memos (per `../marley-principles/decision-frameworks.md` Q6). Older Marley memos used a 3-role RAPID abbreviation (Recommending / Agreeing / Deciding) — historical examples are preserved in this format; new memos should use RACI.

### 3. Context

Short framing (~1 paragraph + optional bulleted considerations). Cover:
- Broader business context for the decision
- What we've previously decided that connects, or what we'll have to decide in the future based on this
- The core considerations that matter — when applicable, name them explicitly (e.g. *"Desirability / Viability / Feasibility"*, or whatever framework applies)

### 4. Decision (or "Proposal" in draft state)

The decision as a **declarative statement** — not "we believe we should consider" but *"We should launch in Hypertension."* Pair the declaration with a brief 2–4 sentence summary of "why" — the headline reasoning that the Rationale section will then unpack.

If the memo is still in draft and the decision isn't final, use header "Proposal" instead of "Decision" and frame as a recommendation.

### 5. Rationale

The longest section. Walks through the reasoning that supports the decision. Structure:

- **Name the framework** applied (if any) — e.g. *"Desirability / Viability / Feasibility"*, the 7-question decision framework from `../marley-principles/decision-frameworks.md`, or whatever lens fits. Name it at the top of the section.
- **For each framework dimension, present the analysis** — usually a **table comparing options across that dimension**. Marley uses tables aggressively here; if the decision involves comparing 3+ options across 3+ criteria, a table is almost always the right move.
- **Be quantitative** wherever possible. Specific numbers, named sources, dated data.
- **Honest commentary** is fine and welcomed — *"Afib scored surprisingly low across the board, perhaps due to..."* Plain-language observation in the analysis is on-voice.
- **Risks and mitigants** — name the risks of the chosen path and how each is mitigated. If a risk has no mitigant, say so directly.
- **Takeaways** — close the section with a brief synthesis paragraph or summary table that pulls the analysis into the case for the decision.

### 6. Alternatives Considered

Optional but expected for any non-trivial decision. List the realistic alternatives that were not selected. For each:
- Name the option
- One short paragraph (2–4 sentences) on what makes it appealing, why it wasn't picked, and any conditions under which it might be revisited

Don't strawman — each alternative should be one a reasonable person could pick. If you find yourself dismissing alternatives in one sentence each, the analysis is shallow.

### 7. Final Decision Date & Decider

Sign-off block. Names + date when the decision was committed. While in draft, this block can be a placeholder.

## Length

- **Short Decision Memo**: 600–1,200 words. Suitable for tactical decisions with 2–3 alternatives, modest analysis.
- **Standard Decision Memo**: 1,500–3,000 words. Most strategic decisions land here. Tables and frameworks pull weight.
- **Deep Decision Memo**: 3,000–5,000 words. Use when the decision deserves heavy analysis (initial-disease-focus type calls, fundraise structure, major partnership commits).

## Voice notes (specific to this variant)

- Standard Marley voice (see `../marley-voice/voice.md`)
- More analytical and quantitative than consumer copy
- **Declarative on the decision** — *"We should launch in Hypertension"*, not "we recommend considering"
- **Honest on uncertainty** — *"Hypothyroidism scored surprisingly..."*, *"More work is needed to..."*
- **Tables when comparing options** — almost always the right format for the Rationale section
- **Name your framework** at the top of Rationale
- **No "Memo:" prefix on the title** — the format is `Decision Memo: [topic]`, not "Memo: Decision on..."

## What this format is NOT for

- Periodic investor updates → use Variant B instead.
- Standalone information memos (no decision being made) → consider a one-pager, briefing doc, or just an email. The Decision Memo format is overkill if there's no decision.
- External-facing communications → drafts for payers, investors, or partners go through the respective deck/pitch skills.
- Inbound legal/compliance memos from outside counsel — Marley *receives* these; the memo skill is for what Marley *authors*.

---

# Variant B — Investor Update

The investor-update variant is for periodic (typically monthly) updates to Marley's investor list. Distilled from the 9 investor updates in source (Sept 2021 → Nov 2022).

## Canonical structure (drawn from actual past updates)

1. **Title block** — "Marley Medical Investor Update — [Month Year]"

2. **tl;dr** — lowercase section header. **2–4 paragraphs.** This is the most important section. It should:
   - Lead with the headline event of the period (a launch, a milestone, a hard learning)
   - State current focus and what's coming next
   - Honestly summarize what's working and what isn't
   - Close with macro / cash / fundraise framing if relevant

3. **The Plan** — visual / chart showing where we are vs. plan. One-slide concept reproduced as a brief section.

4. **Help Requests** — explicit list of asks. Format:
   > - We are looking for [specific thing]
   > - Intros at [specific orgs / names of payers / specific roles]
   > - Ideas for [specific challenge we are working on]

5. **Team and Hiring Updates** — current org chart at fairly fine granularity (MSO team + Clinic team), open roles, recent hires/departures.

6. **Section-by-section progress on key initiatives** — variable, drawn from what mattered this period. Recurring section topics across past updates:
   - Product / offering launch + status
   - Patient acquisition / funnel performance
   - GTM / state expansion
   - Partnership status (table format)
   - Clinical outcomes / patient population profile
   - Patient stories / NPS quotes

7. **Financials** — recurring burn, one-time costs, cash position. Specific. Numbers stated, not buried.

8. **Cash-out analysis** — scenario table. Multiple scenarios (base / expanded / accelerated) showing months to cash out.

9. **Fundraising Strategies and Questions** — *numbered* open questions for investors to weigh in on. Examples from past updates: *"When and how should we think about fundraising?", "Can we raise more now and have more capacity to wait?"*

10. **Topics for Discussion** — bullet list anchoring the upcoming investor call. 3–5 bullets.

## Length
- Typical: 6–11 pages of formatted PDF
- 1,500–4,000 words of narrative text + tables/charts

## Cadence
- Monthly is the default cadence (per the numbered series in source)
- Occasional gap months are fine if there's no material change

## Voice notes (specific to this variant)
- Same Marley voice + investor-update register
- "tl;dr" lowercase as the opening section header
- Honest about hard problems immediately — don't bury bad news
- Colloquial warmth ("hunker down", "come out strong", "lots of duct tape", "a worthy and fun problem to solve") — these are the Marley signal in investor comms
- Specific numbers always — never "significant growth", always "63 patients up from 21"
- Numbered open questions invite engagement — don't fake confidence on things still being worked out
- See `examples/investor-update-*.md` for tone reference

## KPI conventions for this variant
**See [[kpi-conventions]]** — the canonical list of which metrics Marley reports in every investor update and in what format.

---

## See also

- [[audience-cues]] — how to detect which variant to use
- [[kpi-conventions]] — investor-update-specific KPI reporting standards
- `examples/` — exemplars of both variants
- [[source-refs]] — extraction notes
