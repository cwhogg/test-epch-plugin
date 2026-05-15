# DRAFT Decision Memo: Initial Disease Focus

**Source:** `memos/DRAFT Decision Memo - Initial Disease Focus v21.12.13.docx` (December 2021)
**Why this example matters:** the most fully realized Marley Decision Memo in source. Demonstrates the canonical 7-section structure with real comparative analysis (4 candidate diseases × Desirability / Viability / Feasibility framework × heavy use of tables). Use this as the worked example when drafting any new Decision Memo.

Preserved verbatim from source.

> **Historical-convention note:** the Stakeholders section in this example uses a 3-role RAPID abbreviation (Recommending / Agreeing / Deciding). This was Marley's stakeholder frame in 2021. Marley's current canonical frame is RACI — see `../format.md` Variant A Section 2 and `../../marley-principles/decision-frameworks.md` Q6. When drafting new Decision Memos, use RACI; preserve RAPID terminology only when faithfully reproducing historical documents.

---

## Goal

For Marley's first launch, we need to deliberately select which disease to support. While we will be able to pivot and expand later, there could be significant time and cost penalties to do so.

## Stakeholders

The full Marley team is impacted by this decision. Disease selection impacts our product, our future clinical team composition and the partners we prioritize.

- Commercial Strategy (Sibel Sayiner) is **Recommending** this decision.
- Business (Joe Slavinsky) and Operations (David Hubanks) are **Agreeing** to this decision.
- Chris Hogg is **Deciding** this decision.

## Context

Each disease has its own clinical complexities and population dynamics, creating different needs and different product solutions. Though we expect to expand our scope over time, we believe that our initial disease should provide a strong foundation, with sufficient initial market and opportunity to scale.

The core considerations in this decision are:
- Are there enough interested patients? — **Desirability**
- Will unit economics make sense, at a disease level? — **Viability**
- Can we execute clinically? — **Feasibility**

## Proposal

We should launch in Hypertension. It has a significant prevalence and patient interest, shown in the solid CAC and CTR+Conversion Rate from our marketing tests. It provides a good opportunity for immediate commercialization, given its mid-tier outpatient costs while still having some emergency spend that we can reduce over time. Finally, from a clinical perspective, it's primarily med-managed through known treatment algorithms determined by blood pressure, making it exceptionally portable to virtual care.

## Rationale

### Research Process

We started with four potential disease targets:
- Atrial Fibrillation (Afib)
- Congestive Heart Failure (CHF)
- Hypertension
- Hypothyroidism

Broad research was conducted into each disease's prevalence, cost research, and clinical protocols.

### Desirability

We needed to ensure there was a sufficient volume of patients who were interested in an offering. To do that, we considered diseases by prevalence, % who are clinically in need of help and market interest, as shown in marketing tests.

| | Afib | CHF | Hypertension | Hypothyroidism |
|---|---|---|---|---|
| Prevalence — Total | 1–2% | 2% | 45% | 5% (~2.5% subclinical) |
| Prevalence — 60+ | 4–6% | 12% | 75% | 16% |
| % uncontrolled | N/A — Escalation in care until rate control achieved | N/A — Progressive disease | 66% | 30% |

Prevalence & clinical need research indicates the largest opportunity in hypertension, with CHF being second largest.

| | Afib | CHF | Hypertension | Hypothyroidism |
|---|---|---|---|---|
| CPM | $70.45 | $30.27 | $19.74 | $50.75 |
| CPC | $6.21 | $3.77 | $1.76 | $3.28 |
| CTR | 1.13% | 0.80% | 1.12% | 1.55% |
| Conversion Rate | 5.95% | 9.55% | 14.73% | 13.25% |
| Total Leads | 17 | 30 | 812 | 62 |
| Cost per Lead | $104 | $39 | $12 | $25 |

All of these market tests show a reasonable cost per lead (<$100). Given the higher prevalence of hypertension, its costs (CPC and Cost per Lead) are lowest. The CTR (clickthrough rate) and conversion rate demonstrate a level of engagement or velocity through the ad and survey. When looking at those two together, Hypothyroidism has the largest velocity, with Hypertension second. Afib scored surprisingly low across the board, perhaps due to the fact that most patients are actively managed until they achieve rate control.

### Viability

We need to ensure that the economics behind the disease is reasonable, both in the short term and in the long term. For that, we need to consider the annual cost burden associated with each disease and its breakdown.

| | Afib | CHF | Hypertension | Hypothyroidism |
|---|---|---|---|---|
| Annual Spend | ~$12,000 | ~$24,400 | ~$9,100 | ~$2,600 |
| Pharmacy Spend | ~$1,200 | ~$2,400 | ~$2,400 | ~$200 |
| Outpatient Spend | ~$3,600 | ~$1,200 | ~$2,800 | ~$1,000 |
| Emergency Spend | ~$7,200 | ~$20,800 | ~$3,000 | ~$1,300 |
| Would RPM apply? | Yes | Yes | Yes | No |

In the immediate terms, we can potentially capture annual outpatient spend per patient. We would want to leverage codes like RPM to provide that care more comprehensively. RPM, fully billed, is ~$1,500 a year. Afib and Hypertension are squarely above that, enabling us to deliver value on RPM outpatient alone. The low ratio of outpatient care to overall spend in CHF is concerning: we would clearly be tackling a very small portion of the care burden. Conversely, in Hypothyroidism, outpatient is a decent portion of total costs, but it's so small, it's not a good base to grow on.

As we get more sophisticated, we will look to capturing more of the emergency spending bucket (i.e. drive savings). Here, Afib and CHF look very promising. The significant cost burdens to payers would also make our value-based pitch attractive.

### Feasibility

We need to ensure that this is a clinical process that we can execute on, especially in early days.

| | Afib | CHF | Hypertension | Hypothyroidism |
|---|---|---|---|---|
| Clinical care primarily based on | Meds, until need for pacemaker | Meds and diet/lifestyle | Meds | Meds |
| Primary clinical endpoints | Ventricular Rate | Symptoms, LV Ejection Fraction | Blood Pressure | Serum TSH Concentration |
| Clear treatment algorithm to optimize? | Yes | Somewhat. Mainly diet based. | Yes | Yes |
| Primary mgmt steps reimbursed virtually? | Earlier (meds) yes; later (rhythm) no | Regular mgmt yes; cardiac testing potentially | Yes | Commercial only — Medicare doesn't cover labs at home |
| Who primarily manages | Cardiologist | ⅔ PCP, ⅓ Cardiologist | PCP | PCP |
| Need for escalation/referrals | Med — decent chance of AEs | High — large need for ER | Low — AEs are fairly rare | Med — complex cases go to Endo |
| Competition | Low — Hardware plays, less care | Low — Few competitors | Medium — Hello Heart, Livongo | Low — Few competitors |

Hypertension and Hypothyroidism, with their easy clinical endpoint, PCP management and lower competition are both attractive from a feasibility perspective.

### Takeaways

Put all together:

| | Afib | CHF | Hypertension | Hypothyroidism |
|---|---|---|---|---|
| Desirability | Low | Medium | **High** | High |
| Viability | High | Medium | **High** | Low |
| Feasibility | Low | Medium | **High** | High |

Based on these criteria, we believe Hypertension is the best candidate for initial disease launch.

## Alternatives Considered

- **Launch in Hypothyroidism.** Hypothyroidism seems to have a strong pull from a patient perspective and would be potentially feasible in a commercial environment. However, the economics make it un-interesting. It's not a big enough budget item to attract commercial payers for disease-specific deals, and Medicare doesn't cover the primary check-point clinically (labs) if delivered at home.

- **Launch in CHF.** There is a lot to like in CHF. It has a high potential value capture, is clearly underserved by the market from a competition standpoint and can be primarily managed through high-touch dietician care and medication management. However, the patient interest seems to be lower, and more clinical expertise will be required to deliver a strong showing. Since the emergency spending is so high, we know that health systems love to own these patients, since so much revenue flows through them. This would be a great expansion disease state, once Marley is more confident in our process and clinical ops.

## Final Decision Date & Decider

[Details on who signed off on the decision and when.]

---

## What to learn from this example

- **Title format** — `DRAFT Decision Memo: Initial Disease Focus` — "DRAFT" prefix for in-draft state, colon-separated topic.
- **Goal is a single tight paragraph** — frames the stakes and the cost of getting it wrong.
- **Stakeholders uses explicit RAPID** — Recommending / Agreeing / Deciding spelled out with names. No ambiguity about who's calling the shot.
- **Context names the framework** — Desirability / Viability / Feasibility is named explicitly as the structure the Rationale will follow. The reader knows what's coming.
- **Proposal is declarative** — *"We should launch in Hypertension"*, not "we recommend exploring".
- **Rationale section uses one table per framework dimension** — D/V/F gets a comparative table each, plus a Takeaways summary table. This is the highest-leverage move in Marley decision memos.
- **Honest commentary in the analysis** — *"Afib scored surprisingly low across the board, perhaps due to..."* On-voice, not hedging.
- **Alternatives Considered isn't a strawman section** — Hypothyroidism and CHF each get a real paragraph naming what's appealing about them and why they weren't picked. CHF gets a "this is a great expansion disease state" — a real future-conditional consideration.
- **Final Decision Date & Decider is a placeholder in the draft** — that's fine. The block exists; it gets filled in when the decision is finalized.
