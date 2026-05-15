# docs-source/

This folder is for the **original source documents** that the plugin's skills were distilled from. It is intentionally separate from the plugin itself.

## Why this is here

Skills in `plugins/marley-foundation/skills/` were distilled from a body of source PDFs, decks, and brand assets that live in Chris's local directory `~/epch-claude/`. When iterating on the plugin (refining a voice rule, updating a narrative arc, adding a new principle), you'll want to know which source doc to go back to.

Each skill folder has a `source-refs.md` file that names the source documents used. Together those source-refs files form a directory of where every distilled piece came from.

## raw/

`docs-source/raw/` is the staging folder for source documents. **It is currently empty by design.** The source documents live at `~/epch-claude/` in the curated folders described in `~/epch-claude/INVENTORY.md`. Copying them all into the plugin repo would:
- Bloat the repo with large binaries (multi-MB PDFs, .pptx files)
- Duplicate the canonical source location
- Make it ambiguous which copy is the truth

**The canonical source-of-truth lives at `~/epch-claude/`**. Use `raw/` if you want to:
- Stage a new document you're about to distill into the plugin
- Keep a redacted version of a source doc when the original has confidential content
- Stash a one-off reference doc that doesn't belong in the curated `~/epch-claude/` folders

## How distillation works (the iteration loop)

When refreshing source material:

1. Drop the new/updated source file into the appropriate `~/epch-claude/` folder.
2. Update `~/epch-claude/INVENTORY.md` if the new file changes the category mapping.
3. Re-distill the affected skill (read the source, update the skill's content files).
4. Update the skill's `source-refs.md` to reference the new source.
5. Bump `plugins/marley-foundation/plugin.json` version and add a CHANGELOG entry.

## Source folders (as of v0.1.0 scaffold)

The source documents currently feeding the plugin live at:

| Source folder | Feeds skill |
|---|---|
| `~/epch-claude/principles/` | `marley-principles` |
| `~/epch-claude/marley medical voice/` | `marley-voice` |
| `~/epch-claude/visual brand/` | `marley-visual-brand` |
| `~/epch-claude/context/` | `marley-context` |
| `~/epch-claude/memos/` | reclassified: → `payer-pitch-deck` + `fundraise-pitch-deck` |
| `~/epch-claude/investor updates/` | `memo` (investor-update variant) |
| `~/epch-claude/payer pitch decks/` | `payer-pitch-deck` |
| `~/epch-claude/product decks/` | `product-scoping-deck` |
| `~/epch-claude/fundraising decks/` | `fundraise-pitch-deck` |
