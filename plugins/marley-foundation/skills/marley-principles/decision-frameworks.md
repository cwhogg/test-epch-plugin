# Marley decision framework

## When to use this framework
Use this framework whenever Marley makes a non-trivial decision — strategic, operational, organizational, technical. It applies equally to "should we hire this person", "should we contract with this payer", "should we build this feature in-house", "should we change our pricing model". For trivial decisions (reversible, low-stakes, narrow scope), this is overkill — apply judgment about when the rigor is worth the time.

## The 7 questions

For any significant decision, walk through these in order. Write the answers down — that's the decision memo.

### 1. What is the decision?
Define it in a single sentence — be specific. Generic framings ("how should we approach X") produce generic answers. Sharp framings ("how do we price for self-funded employers vs. fully-insured payers given our 2026 cost structure") produce sharp answers. If you can't write the decision in one specific sentence, you don't yet know what you're deciding.

### 2. What are the possible outcomes?
Enumerate the realistic options. Don't strawman — each option should be one a reasonable person could pick. Usually 2–4 options. If there's only one option, you don't have a decision to make; if there are more than 5, you haven't done the work to narrow down.

### 3. What is needed to execute each outcome?
For each option: what resources, time, dependencies, capabilities does it require? This is where unrealistic options get filtered — an option that requires capacity Marley doesn't have isn't really an option.

### 4. What are the main downsides of each possible outcome?
For each option: what could go wrong, and what's the impact on the rest of the business? Be honest about second-order effects — a pricing change has implications for sales motion, brand positioning, and customer trust. A vendor choice has implications for hiring, integration cost, and switching cost. Naming the downsides explicitly is how you avoid surprise later.

### 5. Is the decision reversible (two-way door) or permanent (one-way door)?
Two-way door: if we're wrong, we can change course in weeks or months at modest cost. One-way door: reversal is expensive, slow, or impossible. Two-way doors should be made fast — speed matters more than perfect choice. One-way doors deserve more analysis, more consultation, and a higher bar of confidence before committing.

### 6. Who decides, and who needs to be consulted?
Be explicit about authority (RACI: who is Responsible, Accountable, Consulted, Informed). Most decision failures aren't about the substance — they're about ambiguity over who actually had the call. Name the decider. Name who needed to weigh in but didn't have veto. Name who needs to know after.

> **Note on stakeholder frames:** RACI (Responsible / Accountable / Consulted / Informed) is the canonical Marley frame going forward — use this in new Decision Memos. Older Marley artifacts (notably the December 2021 *Disease Focus* draft) used a 3-role RAPID abbreviation (Recommending / Agreeing / Deciding); preserved verbatim in `../memo/examples/general-decision-memo-disease-focus.md` for historical reference, but not the going-forward convention.

### 7. How do we track outcomes?
What metric or signal tells us in 30/90/180 days whether the decision was right? Without this, we don't learn — we just keep deciding. The tracking commitment is part of the decision; if you can't articulate how you'll know, you're not really committed to evaluating.

---

## Cross-references

- `principles.md` — the 12 operating principles that should shape *what's considered* in any decision. The framework above is the *process*; the principles are the *content* that informs each answer.
- `../memo/format.md` (Variant A — Decision Memo) — the Rationale section of a Marley Decision Memo should walk through this framework explicitly. Name "the 7-question decision framework" at the top of Rationale; structure the section around the seven answers.
- `../memo/examples/general-decision-memo-disease-focus.md` — worked example of a Marley Decision Memo. Note the framework used in that memo is *Desirability / Viability / Feasibility* (a different lens — that was a market-fit decision, not a generic decision). The 7-question framework is the meta-framework that applies regardless of which substantive framework gets named inside Rationale.
