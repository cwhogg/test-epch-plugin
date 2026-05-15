# Marley Medical Typography

From the typography licenses and font files in `visual brand/Brand Assets/Marley Typography/`.

## Font stack

### Primary: Reckless

**Reckless** is Marley's primary typeface. It's a contemporary serif with character — modern but warm, confident but not corporate. Licensed for desktop and web (`Brand Assets/Marley Typography/Primary Fonts/Reckless/License/`).

Weights available:
- Reckless Regular
- Reckless Regular Italic
- Reckless Medium
- Reckless Medium Italic

Formats available in the brand library: OTF, TTF, WOFF, WOFF2.

**Use Reckless for:** display headlines, deck titles, brand-forward marketing copy, hero text, anywhere the brand voice needs to come through visually.

### Primary (sans-serif companion): Greycliff

**Greycliff** is licensed from Adobe Fonts (`Brand Assets/Marley Typography/Primary Fonts/Greycliff_Adobe Fonts.txt`). It's a humanist geometric sans — clean, friendly, modern.

**Use Greycliff for:** UI text, body copy in product, dashboards, anywhere readability and density matter more than brand-warmth. Pairs cleanly with Reckless.

### Backup fonts (system / web-safe fallbacks)

If Reckless or Greycliff aren't available (some web contexts, some client systems):

- **Newsreader** — serif backup for Reckless. Available at `Brand Assets/Marley Typography/Backup Fonts/Newsreader/` (Italic + Medium TTF).
- **Poppins** — sans backup for Greycliff. Available at `Brand Assets/Marley Typography/Backup Fonts/Poppins/` (Regular, SemiBold, Bold TTF).

Both Newsreader and Poppins are free Google Fonts and a safe fallback in any web context.

---

## Type hierarchy (suggested, since source brand library does not specify a numeric scale)

These are recommended scales for decks and longer documents. Adjust to the specific medium.

| Role | Font | Weight | Approx size |
|---|---|---|---|
| Slide / page title | Reckless | Medium | 36–48pt |
| Section header | Reckless | Medium | 24–28pt |
| Sub-header | Reckless | Regular Italic | 18–20pt |
| Body | Greycliff (or Poppins fallback) | Regular | 14–16pt |
| Caption / footnote | Greycliff | Regular | 10–12pt |
| Pull quote | Reckless | Regular Italic | 22–28pt |
| Data label | Greycliff | SemiBold | 12–14pt |

## Pairing rules

- **Reckless + Greycliff** is the canonical Marley pairing. Reckless for warmth and brand-voice; Greycliff for clarity and density.
- **Never set body copy in Reckless** at small sizes — the serif details get noisy below ~14pt.
- **Never set display headlines in Greycliff** when Reckless is available — Greycliff is the workhorse, not the lead.
- Italic Reckless is reserved for pull quotes, patient quotes, and emphasis — not for body.

## What's NOT in source

The source brand library provides the fonts and their licenses, but does not provide:
- A formal numeric type scale
- Line-height / leading rules
- Letter-spacing / tracking rules
- A web-CSS rule set

The scale above is a sensible default. If formalized brand guidance ever lands, replace this section.

---

## See also

- [[colors]] — color rules apply to type too (e.g. don't set Reckless headlines in red on a peach surface).
- [[logo-usage]] — the wordmark uses its own letterform; do not re-set "Marley Medical" in Reckless to substitute for the wordmark.
- [[source-refs]] — where this was extracted from.
