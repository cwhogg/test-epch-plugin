# Clinical Design and Clinic Capacity Analysis — August 2023 (slide-by-slide reference)

**Source:** `product decks/Marley Medical Clinical Design - August 2023.pdf`
**Why this example:** the most fully realized product-scoping deck in source. Reference for canonical scenario-modeling structure including the signature "What would you have to believe to get to X?" framing.

This is an internal deck (not redacted — the content is internal-team analysis, not externally-sensitive).

---

## Slide 1 — Cover
**Marley Medical — Clinical Design and Clinic Capacity Analysis — August 2023**

## Slide 2 — The Problem
*"The volume of clinical reviews, patient follow up and messaging is becoming overwhelming with growth."*

Single-sentence problem framing.

## Slide 3 — Required attributes / criteria for the solution
*We need a revised clinical protocol that is:*
- Evidence-based and effective
- Championed by the clinical team
- Data-driven and proactive
- Something we can implement efficiently with technology
- A clinical model that generates a sufficient panel size per MD to be a viable business

5-bullet list naming the constraints/criteria before any scenario evaluation. This is the filter Slides 6+ scenarios will be judged against.

## Slide 4 — The Analysis (methodology)
*"We analyzed various potential clinical protocols systematically, and modeled the volume of visits and clinical reviews required by each."*

One slide explaining methodology before scenarios.

## Slide 5 — Key Learnings
Bulleted meta-findings *before* the scenario walk-through:
- All the options we looked at were similar in design and ended up similar in capacity requirements
- 46% of patients with no readings in last 2 weeks — pushing these reviews out immediately reduces review burden
- All scenarios allowed for a group of "High Risk" patients reviewed 2x per month (usually 5%); >15% of population on 2x monthly reviews breaks capacity
- As panel size increases, low-risk patients must be reviewed by non-MDs and escalated to MDs when needed

## Slide 6 — "Where we were before Minnesota" (baseline scenario)
**Assumptions:**
- 400 patient panel per MD
- 25% reviewed every 2 weeks
- 75% reviewed every 4 weeks
- All primary clinical reviews conducted by MDs
- MDs spending time on patients with incomplete data
- MDs spending time on chase activities

**Output:** **25** Reviews per day

## Slide 7 — "Implementing the 'Minnesota Protocol'"
**Assumptions:**
- 400 patient panel per MD
- 5% (high risk) reviewed every 2 weeks
- 11% (med risk) reviewed every 4 weeks
- 38% (low risk/at goal) reviewed every 8 weeks
- 46% (no readings) not reviewed and deferred
- All primary clinical reviews still conducted by MDs
- Non-MDs responsible for chase activities

**Output:** **8** Reviews per day

## Slide 8 — "Implementing the 'Minnesota Protocol' v2"
**Assumptions:**
- Same as Slide 7 plus:
- Low risk review by non-MD with 25% escalation rate
- Non-MDs responsible for chase activities

**Output:** **5** Reviews per day

## Slide 9 — "Running efficiently at capacity"
**Assumptions:**
- **800 patient panel per MD**
- 10% (high risk) reviewed every 2 weeks by MD
- 30% (med risk) reviewed every 4 weeks by non-MD + escalated
- 35% (low risk/at goal) reviewed every 8 weeks by non-MD + escalated
- 25% (no readings) deferred
- Non-MDs responsible for chase activities

**Output:** **13** Reviews per day · **7** Follow-up visits per day

## Slide 10 — "Low risk patients managed by non-MDs"
**Assumptions:** Same as Slide 9 + low-risk reviews escalate to non-MD instead of MD

**Output:** **11** Reviews per day · **7** Follow-up visits per day

## Slide 11 — "Getting greedy"
**Assumptions:**
- **1,000 patient panel per MD**
- Same risk stratification as Slide 9

**Output:** **14** Reviews per day · **9** Follow-up visits per day

## Slide 12 — "What would you have to believe to get to 1,200?"
**Assumptions:**
- **1,200 patient panel per MD**
- 5% (high risk) reviewed every 2 weeks by MD
- 20% (med risk) reviewed every 4 weeks by non-MD + escalated
- 50% (low risk/at goal) reviewed every 8 weeks by non-MD + escalated
- 25% (no readings) deferred
- Low risk patients managed by non-MDs with annual MD visit
- Leverage midlevel providers for clinical reviews

**Output:** **9** Reviews per day · **8** Follow-up visits per day

## Slide 13 — "What would you have to believe to get to 2,000?"
**Assumptions:**
- **2,000 patient panel per MD**
- 5% (high risk) reviewed every 2 weeks by MD
- 20% (med risk) reviewed every 4 weeks by non-MD + escalated
- 50% (low risk/at goal) reviewed every 8 weeks by non-MD + escalated
- 25% (no readings) not reviewed and no annual visit (inactive)
- Low risk patients managed by non-MDs with annual MD visit
- Leverage midlevel providers for reviews

**Output:** **15** Reviews per day · **9** Follow-up visits per day

## Appendix — Risk groups breakdowns
Four alternative risk-stratification methodologies shown side by side:
1. Risk groups based on points away from BP goal
2. Risk groups based on BP thresholds + goal/not at goal
3. Risk groups based on BP thresholds only
4. Risk groups based on at goal / not at goal only

## Appendix — Summary of proposals
Cross-scenario summary slide allowing visual comparison across all scenarios.

## Companion deck: Prescriber evolution (panel-build trajectory)
10 slides modeling clinical-staffing evolution from 50 patients → 1,000 patients per panel, showing how reviews/day, NPVs/day, follow-ups/day, and hours-for-messaging shift as panel grows. Same scenario-template structure applied to a different question.

---

## What to learn from this example

- **Single-sentence problem (Slide 2)** — no preamble, just the constraint. *"The volume of clinical reviews, patient follow up and messaging is becoming overwhelming with growth."*
- **5-bullet required attributes (Slide 3) becomes the filter** — every scenario in Slides 6+ should be judged against these criteria. A scenario that fails one of them should be flagged in the deck, not silently included.
- **Scenario titles are honest and colloquial** — *"Where we were before Minnesota"*, *"Getting greedy"*. Not corporate-flat ("Scenario A", "Option 2"). The names reflect how the team actually thinks about each option.
- **Two scenarios use the "What would you have to believe to get to X?" framing** — for ambitious targets (1,200 and 2,000 patient panels). The framing inverts: instead of "is this possible?" the question is "what assumptions make this possible?" Then the room debates whether the assumption set is plausible.
- **Consistent output-metric set** — Reviews/day appears on every scenario; Follow-up visits/day on most; Hours messaging when relevant. This consistency lets the reader compare scenarios visually.
- **All scenarios assume "Non-MDs responsible for chase activities"** — a structural choice carried across the analysis. Calling out shared assumptions like this is important for the reader to see what's being held constant.
- **Appendix shows the alternatives that were considered and not selected** (4 risk-stratification methodologies) — transparent about the path not taken.
- **No recommendation slide at the end.** The deck doesn't end with "We propose Scenario X". It ends with the summary and lets the room decide. This is intentional — product-scoping decks lay out the option space; the decision happens in the discussion.
