# KPI conventions — investor-update variant only

**This file applies only to the investor-update variant of the memo skill.** General memos can use whatever metrics serve the argument.

Extracted from the recurring KPI patterns across 9 investor updates (Sept 2021 → Nov 2022) and the March 2024 Sapphire deck.

---

## Always include in every investor update

### Patient count
- **Format:** total patients enrolled, with change since last update.
- **Example:** *"We are currently at 63 patients, up from 21 at the last update."*
- **Pace of growth:** also report the most recent enrollment cadence — *"adding 10–15 new patients per week"* — and a brief "days per X patients" pattern when noteworthy (*"100 days to first 10, 33 days to next 10, 15 days to next 10, currently 10 every 5.8 days"*).

### Clinical outcomes
- **Format:** average BP reduction (systolic AND diastolic), plus distribution.
- **Example:** *"For patients with >4 weeks of data, we see an average BP reduction of 6.2 mmHg systolic and 3.6 mmHg diastolic."*
- **Distribution breakdowns** to include:
  - % who reduced BP > 0 mmHg
  - % who reduced BP > 10 mmHg
  - % who reduced their BP risk classification
  - % who increased their BP risk classification (don't hide this)

### Engagement
- **NPS** — average score from completed surveys. Always include sample size. (*"Average NPS: 95 (64 completed surveys)"*)
- **Patient activity** — % active in last 30 days
- **Retention** — when sample size allows (1-year retention preferred)
- **Interaction cadence** — synchronous visits per patient per month, async messages per patient per week
- **Device readings** per patient per week

### Patient demographics + profile
- **Mean / median / range age**
- **Mean / median chronic conditions count**
- **% with mental health diagnosis**
- **% overweight or obese / % clinical-level obesity**
- **% with existing PCP**
- **SDOH callouts** when material (disability, financial stress, occupation patterns)

### Cash position + burn
- **Total cash remaining** — specific dollar amount, dated.
- **Recurring monthly burn** — separate from one-time expenses.
- **Months to cash out** — base case, plus 1–2 alternate scenarios in a table.
- **Format:** scenario table with column headers like "Total Headcount" or "2024 Spend (mo)" + "Months to Cash Out"

### Patient-acquisition funnel
When acquisition is in motion (always relevant for early-stage updates):
- **Cohort table by month:** Digital Ads → Lead Qual Form (%) → Schedule Sales Call (%) → Complete Sales Call (%) → New Patient → Overall Conversion %
- **CAC** by channel, with trend
- **Lead channels active** — Facebook, Google, partnerships, etc.

---

## Include when applicable

### State / geographic expansion
- States currently live
- States in process (with timeline)
- Network contracts active / in progress per state
- Lead and patient distribution by state

### Partnership / B2B status
- Table format: Partner name | Status | Notes
- Recurring named partners: Impilo (devices), Truepill (pharmacy), Canvas (EMR), Source (messaging), Quest (labs), CertifyOS (credentialing)
- Active B2B targets when relevant

### Product / offering progress
- New capabilities launched
- Current builds in progress with rough timing
- Self-described maturity state (recent example: *"functional, but neither pretty nor delightful"*)

### Hiring
- Current FTE count + PT contractors
- Recent hires (named, with role)
- Open roles being actively recruited
- Departures (be honest)

---

## Reporting standards — how numbers should be framed

- **Absolute + delta.** Always give both the absolute number and the change since last report. *"63 patients (up from 21)"* — not just "63."
- **Sample size for any rate or average.** *"Average NPS: 95 (64 completed surveys)"* — not just "NPS 95."
- **Time-bounded.** *"In the last 30 days"*, *"as of Nov 27, 2023"*, *"April 2022 cohort"* — always anchor numbers to a window.
- **No vague qualifiers.** *"Significant growth"*, *"strong retention"*, *"high engagement"* — replace with specific numbers.
- **Direction of any miss stated plainly.** If a metric got worse, say so. Don't omit it; don't soften it.

---

## What to do when a metric is unavailable

Don't fake it. Common honest framings from past updates:
- *"We don't have a lot of data on retention yet, but it is a key metric we are tracking."*
- *"In 1–2 months we will see how this new bolus of patients performs, and should have enough data to see our true early retention."*
- *"I think we can safely say it is not horrible so far."*

Better to say "we don't have it yet" than to publish a noisy or misleading number.

---

## See also

- [[format]] — full investor-update structure
- [[audience-cues]] — when to use the investor-update variant
- `../marley-voice/voice.md` — investor-update voice register
