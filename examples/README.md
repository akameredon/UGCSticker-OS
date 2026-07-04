# Examples

This folder holds real, completed examples of the UGCSticker-OS pipeline in action. Each example proves out the framework against a real customer's assets and captures what worked, so future generations (and future rule-file updates) can learn from it.

## Folder convention

One subfolder per example, named `<industry>-<short-product-name>/`, e.g. `restaurant-jollof-sauce/`, `juice-mango-blend/`, `cosmetics-shea-butter/`.

Inside each subfolder:

```
<example-name>/
├── 01-input-sticker.png     <- the original die-cut sticker artwork
├── 02-input-product.png     <- the original product/container photo
├── 03-input-model.png       <- the approved UGC model reference
├── 04-output-hero.png       <- the final accepted hero render
├── 05-output-lifestyle.png  <- (optional) additional accepted output types
└── notes.md                 <- see template below
```

Only include the **final accepted** output(s) — this folder is a reference library of what "good" looks like, not a dumping ground for every attempt.

## notes.md template

```markdown
# <Example Name>

**Industry template used:** templates/<Industry>.md
**Prompt file used:** prompts/<Type>Prompt.md
**Date:** YYYY-MM-DD

## Inputs
- Sticker: brief description (shape, finish, key colours)
- Product: brief description (container type, material)
- Model: which approved model reference was used

## What worked
- Notable wins in composition, lighting, or realism

## What needed correction
- Any rule that had to be reinforced or any failure mode hit during generation
  (e.g. "first attempt distorted the QR code — re-ran Stage 3 with explicit
  perspective-only instruction")

## Rule file impact
- Did this example reveal a gap in any rules/ file? If so, note it here and
  update the relevant rule file, bumping SKILL.md's version/changelog.
```

## Why this matters

Every example added here should make the *next* generation better — either by giving future prompts a proven reference point, or by surfacing a rule gap that gets fixed in `/rules`. Treat this folder as the framework's test suite, not just a portfolio.
