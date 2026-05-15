# Scope-section template

How Marley structures the scenario slides specifically. Each scenario in a product-scoping deck follows this template.

---

## Scenario slide layout

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Scenario Title — honest, often colloquial]

Assumptions:
●  [Structural choice 1 — e.g. panel size per MD]
●  [Structural choice 2 — e.g. cadence for risk group 1]
●  [Structural choice 3 — e.g. cadence for risk group 2]
●  [Structural choice 4 — e.g. who does what]
●  [Structural choice 5 — e.g. what's excluded / deferred]



      [Metric 1]            [Metric 2]            [Metric 3]
      [VALUE]               [VALUE]               [VALUE]
      [unit]                [unit]                [unit]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Title conventions
- Honest and memorable
- Use internal colloquial labels — "Getting greedy", "Where we were before Minnesota"
- Use the "What would you have to believe to get to X?" pattern for ambitious-target scenarios
- Don't title scenarios with corporate-flat labels ("Scenario A", "Option 2")

### Assumptions block
- Always bulleted, parallel structure
- Each assumption is a *structural choice*, not a conclusion
- 4–7 assumptions per scenario is the sweet spot
- Make panel-size / population-size / cadence / staffing explicit
- Make the *deferral / exclusion* explicit (e.g. "46% of patients with no readings deferred")

### Output metrics
- Display 2–4 key output metrics, large and prominent
- Use the metrics that map to the **required attributes** named in Slide 3
- For a clinical-design scenario, this is reviews/day, follow-ups/day, hours of messaging
- For a unit-economics scenario, this would be margin/patient, CAC payback, gross margin
- For a panel-modeling scenario, this is panel size, MD count required, scaling factor

### Output-metric format
- Single number per metric, prominent
- Label below in small type
- No charts on this slide — charts go in the appendix
- Consistent metric set across all scenarios in the deck (so they can be visually compared)

---

## The "What would you have to believe to get to X?" pattern

This is the signature Marley scoping move. The pattern:

1. **Pick an ambitious target.** A panel size, a margin, a patient count, a CAC, a timeline.
2. **Title the scenario:** *"What would you have to believe to get to [target]?"*
3. **Write the assumption set** that would have to be true for the target to be achievable.
4. **Display the output metrics** the scenario produces.
5. **Discuss in the room** whether the assumption set is plausible.

This is more honest than "Here's our forecast" — it makes the path-dependency explicit and turns the question from "is this number right?" to "do you believe these assumptions?"

---

## Cross-scenario summary slide (recommended)

After the scenario walkthrough, a single summary slide comparing all scenarios across the same metric set is high-value:

| Scenario | Panel size | Reviews/day | F/U visits/day | Hours messaging |
|---|---|---|---|---|
| Before Minnesota | 400 | 25 | — | — |
| Minnesota Protocol | 400 | 8 | 3.6 | 0.7 |
| Minnesota v2 | 400 | 5 | — | — |
| At capacity | 800 | 13 | 7 | 1.2 |
| Get to 1,500 | 1,500 | 11 | 7 | 1.5 |
| Get to 2,000 | 2,000 | 15 | 9 | 0.5 |

This kind of summary table lets the reader compare assumption sets and identify which scenarios pass the "required attributes" filter from Slide 3.

---

## See also

- [[narrative-arc]] — overall deck structure
- [[source-refs]] — extraction notes
