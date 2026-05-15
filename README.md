# marley-foundation — a Claude plugin for Marley Medical

A personal-demo plugin representing **Marley Medical**, Chris Hogg's virtual-first cardiometabolic care company. Foundation skills capture company principles, voice, visual brand, and context. Specific skills cover the four deliverables Chris actually creates: investor update memos, payer pitch decks, product-scoping decks, and fundraise pitch decks. A `chris-critic` sub-agent reviews every task-skill draft before it goes back to the user.

---

## What's in this plugin

**8 skills + 1 sub-agent.**

- **Foundation skills** (always-on background context — load whenever any Marley work is in flight):
  - `marley-principles` — 12 operating principles + decision frameworks
  - `marley-voice` — brand voice, banned phrases, preferred phrases, exemplars
  - `marley-visual-brand` — colors, typography, logos, iconography, photography style
  - `marley-context` — company, market, ICP, current pipeline state

- **Task skills** (fire on specific deliverable requests):
  - `memo` — single skill with general + investor-update variants
  - `payer-pitch-deck` — visual pitch for a named health plan
  - `product-scoping-deck` — internal analytical scenario-modeling deck
  - `fundraise-pitch-deck` — visual pitch for a named investor / named round

- **Sub-agent:**
  - `chris-critic` — read-only review agent invoked after every task-skill draft

---

## Installing in Claude Code

```bash
/plugin marketplace add ~/epch-claude/plugin
/plugin install marley-foundation@marley-personal
```

The first command registers this folder as a local marketplace. The second installs the `marley-foundation` plugin from that marketplace.

After install, try the test prompts below to verify each skill triggers correctly.

---

## Installing in Cowork

1. Push this repo to a private GitHub repo (e.g. `github.com/cwhogg/marley-claude-plugins`).
2. In Cowork → Customize → Plugins → Add marketplace.
3. Point it at the GitHub URL.
4. Install the `marley-foundation` plugin.

---

## The iteration loop

The skill *descriptions* (in each `SKILL.md` YAML frontmatter) are the highest-leverage strings in the system — they determine when Claude loads the skill. Iterate on them based on actual usage:

1. **Use a skill** with a test prompt.
2. **Inspect** what loaded vs. what didn't. Did Claude pick up `marley-voice` on a copy task? Did `payer-pitch-deck` fire on the right phrasing?
3. **Refine the description** in `plugins/marley-foundation/skills/<skill>/SKILL.md`. Make it more specific. Add the trigger phrases that you actually use.
4. **Bump version** in `plugins/marley-foundation/plugin.json` and add a CHANGELOG entry.
5. **Reinstall** (in Claude Code: `/plugin reinstall marley-foundation@marley-personal`).
6. **Re-test.**

---

## 9 test prompts (one per skill + a memo-variant routing test)

Use these in Claude Code to verify each skill triggers correctly and produces Marley-quality output on the first prompt.

### 1. `marley-principles` (ambient — should load alongside any Marley work)
> *"Why is Marley going broad-in-network with payers instead of doing narrow B2B carve-outs? Walk me through the reasoning from first principles."*

Should load `marley-principles` and answer using Principles #3 (B2C2B) and #8 (broad in-network).

### 2. `marley-voice` (any written output)
> *"Write 3 new Marley brand headlines on the theme of 'feeling more like yourself again with blood pressure under control'. Keep them Marley voice."*

Should load `marley-voice` and produce headlines in the canonical Marley register (contractions, plainspoken-confident, possibly a witty move).

### 3. `marley-visual-brand` (visual artifact)
> *"I need to mock up a landing-page hero section for Marley. Give me the color, type, and layout decisions you'd make and why."*

Should load `marley-visual-brand` and apply Marley Purple `#5A38B2`, Cream `#FDF7EF` background, Reckless display + Greycliff body.

### 4. `marley-context` (positioning / market work)
> *"Walk me through Marley's competitive positioning vs. Galileo, Hello Heart, and Oak Street. What's the ICP for each?"*

Should load `marley-context` and reference the canonical competitive table.

### 5. `memo` — general variant
> *"Draft a 1-pager strategy memo on why Marley is expanding from hypertension to broader cardiometabolic disease."*

Should load `memo`, route to general variant (no investor-update cues), apply the Variant A scaffold. **Note:** the general-memo variant has a flagged source gap — no canonical internal-strategy memos in source. The output will exercise the scaffold but won't be source-grounded the way investor-update memos are. Treat this prompt as a scaffold-validation test, not a "this is what Marley general memos always look like" test.

### 6. `memo` — investor-update variant (variant-routing test)
> *"Draft this month's Marley investor update. We hit 80 patients this month, signed a new payer in Ohio, and we're starting to think about a bridge round."*

Should load `memo`, route to investor-update variant (periodic cadence + "investor update" trigger), apply the Variant B scaffold with tl;dr / Help Requests / Team / Section progress / Financials / Fundraising Q's / Topics for Discussion.

### 7. `payer-pitch-deck`
> *"Build a payer pitch deck for Anthem Ohio. We have a conversation in two weeks."*

Should load `payer-pitch-deck`, apply the 3-act narrative arc, customize for Anthem Ohio (state-specific evidence, "easy contracting" line referencing any existing Anthem-family contracts), and hand to `chris-critic` after drafting.

### 8. `product-scoping-deck`
> *"Scope a deck on what we'd have to believe to support a 1,200-patient-per-MD panel in 2025."*

Should load `product-scoping-deck`, recognize the "What would you have to believe to get to X?" signature framing, apply the scenario-modeling structure.

### 9. `fundraise-pitch-deck`
> *"Build a Series B deck for Bessemer. $20M raise, want to position as the next-gen virtual primary care for chronic disease."*

Should load `fundraise-pitch-deck` (NOT the memo skill's investor-update variant — this is a visual deck for a named firm), apply the canonical fundraise arc with the risks-paid-down/underwriting ask framing. **Validation check:** the output should use $20M / Bessemer / Series B (not stale $6–8M / a16z / Series A numbers from the Sapphire example), AND should pull current Marley numbers (patient count, payer count, PPPM rate) from `pipeline.md` "Most current source-attested numbers" table — not copy-paste 2024 numbers verbatim.

---

## What to do tomorrow

The tightest learning loop is **exercise one task skill end-to-end** before broadening.

**Recommended starting skill:** `memo` (investor-update variant).

Why this one first:
- It's the most format-strict of the four task skills (multiple required sections, KPI conventions, source-tied numbers) — so if the skill works, you learn a lot about whether the system can hold structure.
- It has 9 source exemplars (vs. 1–3 for the deck skills) — the model has the most pattern signal here.
- The chris-critic review on a memo has a tight feedback loop — you can read the draft, the review, and the revision side-by-side in one prompt window.
- It exercises the variant-routing logic (the trickiest part of the memo skill).

**The end-to-end exercise:**
1. Prompt Claude with test prompt #6 above.
2. Inspect what loaded (which foundation skills came in alongside `memo`?).
3. Read the draft and the chris-critic review.
4. Note where the draft missed Marley voice / KPI conventions / format expectations.
5. Refine the relevant files (`memo/format.md`, `memo/kpi-conventions.md`, `marley-voice/voice.md`).
6. Repeat. Aim for a draft that needs minimal revision after critic on the second pass.

Once that's tight, broaden to the deck skills (which depend heavily on the visual-brand foundation skill).

---

## Repo structure

```
plugin/
├── .claude-plugin/
│   ├── marketplace.json
│   └── CHANGELOG.md
├── plugins/
│   └── marley-foundation/
│       ├── plugin.json
│       ├── skills/
│       │   ├── marley-principles/
│       │   ├── marley-voice/
│       │   ├── marley-visual-brand/
│       │   ├── marley-context/
│       │   ├── memo/
│       │   ├── payer-pitch-deck/
│       │   ├── product-scoping-deck/
│       │   └── fundraise-pitch-deck/
│       └── agents/
│           └── chris-critic.md
├── docs-source/
│   ├── README.md
│   └── raw/
├── README.md
└── .gitignore
```

Source documents live at `~/epch-claude/` (one level up). See `docs-source/README.md` for the source-distillation mapping.
