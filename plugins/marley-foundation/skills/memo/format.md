# Memo format — General + Investor Update variants

This skill handles two memo variants. **Variant selection happens via audience cues** before drafting — see [[audience-cues]] for routing logic.

Both variants share the same Marley voice (see `../marley-voice/voice.md`). The variants differ in **structure**, **length**, and **content conventions** — not in tone.

---

# Variant A — General Memo (default)

The general-memo variant is for internal strategy memos, one-pagers, board-update memos, partnership-pitch memos, and any narrative document for an audience that is **not specifically the investor list on a periodic cadence**.

## ⚠️ Source-thin variant
The source folder `memos/` did not contain canonical internal/strategy memo examples — only a payer 2-pager (BCBS) and a fundraise Series A memo, both reclassified to their respective task skills. **The general-memo format below is a sensible scaffold based on Marley's voice and other Marley narrative artifacts. Update it once Chris drops one or two real internal/strategy memos into source.**

## Structure (recommended scaffold)

1. **Title** — direct statement of subject. No "Memo:" prefix.
2. **Opening framing** (2–4 sentences) — what this memo is about and why now. Skip TL;DR/Executive Summary jargon; just write the framing.
3. **The argument** — body sections, each with a short header. Use 2–5 sections, named for the substantive content, not by structural role ("The market opportunity" not "Background").
4. **What we're proposing / what we believe** — the recommendation or decision the memo is asking for.
5. **Open questions / what we'd want feedback on** — explicit list of where the writer is genuinely uncertain.

## Length
- One-pager: 400–700 words
- Strategy memo: 1,000–2,500 words
- Long-form thought piece: up to 4,000 words; rare

## Voice notes (specific to this variant)
- Marley voice (see `../marley-voice/voice.md`)
- More analytical than consumer copy — facts, numbers, qualified claims
- Honest about uncertainty: "Our current best guess is…", "We believe but don't yet have evidence…"
- Numbered lists for open questions
- Open with the recommendation if it exists; bury the lede only when you genuinely don't have one yet

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
