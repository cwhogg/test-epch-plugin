# Product-scoping deck — canonical narrative arc

Extracted from `product decks/` — primarily the **Clinical Design and Clinic Capacity Analysis (August 2023)** deck, with cross-reference to the **Patient Journey** deck and **Clinic Economics** deck. The product-scoping pattern at Marley is **analytical and scenario-modeled**, not aspirational.

The Marley product-scoping deck is structured as a **structured decision document**: problem → required attributes → analysis methodology → key learnings → scenario-by-scenario walkthrough → conclusion / recommendation. This is the inverse of a sales deck — it's a deck for thinking out loud and showing the work.

---

## Canonical structure

### Slide 1 — Cover
- Marley Medical wordmark
- Title of the scoping question / analysis (e.g. "Clinical Design and Clinic Capacity Analysis", "Patient Journey")
- Date / month

### Slide 2 — The Problem
1–3 sentences naming what's not working today, framed concretely:
> *The volume of clinical reviews, patient follow up and messaging is becoming overwhelming with growth.*

### Slide 3 — Required attributes / criteria for the solution
A bulleted list of what the solution must do or be. Each bullet is a constraint or selection criterion. From the Clinical Design deck:
- Evidence-based and effective
- Championed by the clinical team
- Data-driven and proactive
- Implementable efficiently with technology
- Generates a sufficient panel size per MD to be a viable business

This slide is doing important work: it makes the trade-off space explicit before any scenario evaluation.

### Slide 4 — The Analysis (methodology)
One slide explaining how the analysis was done. From the Clinical Design deck:
> *We analyzed various potential clinical protocols systematically, and modeled the volume of visits and clinical reviews required by each.*

If there's an analysis framework, name it here.

### Slide 5 — Key Learnings
3–6 bullet-point findings *before* the scenario walk-through. These are the meta-takeaways that frame how to read the scenarios. From Clinical Design:
- *All the options we looked at were similar in design and ended up similar in capacity requirements*
- *We have a ton (46%) of patients with no readings in last 2 weeks, and all of these reviews should get pushed out, which will immediately reduce review burden*
- *All scenarios allowed for a group of 'High Risk' patients who were reviewed 2x per month (usually 5%)*

### Slides 6–N — Scenario walkthrough
Each scenario gets its own slide with a consistent structure:

**Title** — named scenario, often colloquial:
- "Where we were before Minnesota"
- "Implementing the 'Minnesota Protocol'"
- "Implementing the 'Minnesota Protocol' v2"
- "Running efficiently at capacity"
- "Low risk patients managed by non-MDs"
- "Getting greedy"
- **"What would you have to believe to get to 1,200?"** — signature Marley framing
- **"What would you have to believe to get to 2,000?"**

**Assumptions block** — bulleted list of the model's inputs / structural choices:
- 400 patient panel per MD
- 5% of patients (high risk) reviewed every 2 weeks
- 11% of patients (med risk) reviewed every 4 weeks
- 38% of patients (low risk/at goal) reviewed every 8 weeks
- 46% of patients (no readings) not reviewed and deferred
- All primary clinical reviews still conducted by MDs
- Non-MDs responsible for chase activities

**Output metrics** — the model's results, displayed prominently. For the Clinical Design deck:
- Reviews per day
- Follow-up visits per day
- Hours for messaging/other
- NPVs per day (when relevant)

### Final scenario slide
The "what would you have to believe to get to X" framing is Marley-signature — it inverts the modeling question and explicitly names the assumption-set required to hit an ambitious target.

### Appendix
Whatever supporting analysis didn't make it into the main flow:
- Alternative risk-stratification approaches
- Summary tables comparing scenarios
- Sensitivity analyses
- Detailed breakdowns by sub-cohort

### End slide
Just "END" — minimal.

---

## Marley-specific narrative moves to use

### "What would you have to believe to get to X?"
This is the signature scoping move. Instead of asking "what's possible?", invert: "to hit X, what assumptions would have to be true?" Then test the assumption-set against reality.

### Named scenarios
Marley names its scenarios with internal-colloquial labels — "Where we were before Minnesota", "Getting greedy", "Running efficiently at capacity". These are not slides for external audiences; they're for the team to think clearly. Names should be honest and memorable, not corporate-flat.

### Honest about the math
Marley scoping decks **show the math** — they don't bury assumptions, and they don't fudge the output. If a scenario requires unrealistic assumptions, the deck says so. The reviewer should be able to recompute the conclusion from the assumptions.

### Trade-off framing, not solution-pushing
Product scoping decks are not for selling a recommendation. They're for laying out the option space, the constraints, and the trade-offs. The deck should give the reader enough to disagree with the recommendation if they want to.

---

## When to use this deck format

- Capacity / staffing decisions
- Protocol changes
- Build-vs-buy / tooling decisions
- Patient-segment expansion decisions
- Pricing / packaging analyses
- Anything where a *decision* is the output, not a *pitch*

**Not for:** investor / payer / partner-facing artifacts (those are pitches; use those skills instead).

---

## See also

- [[scope-template]] — slide-level template for the recurring scenario structure
- [[source-refs]] — extraction notes
- `examples/` — past product-scoping decks (redacted as needed)
- `../marley-context/pipeline.md` — current operational state to anchor scenario assumptions
- `../marley-voice/voice.md` — internal/team register: most candid, most operationally honest
