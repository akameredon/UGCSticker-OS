# UGCSticker-OS

A reusable creative "operating system" for AI-assisted commercial product advertising, built for **Sleekblue Media Houz**.

UGCSticker-OS teaches any capable AI model to consistently generate the same advertising style — the Sleekblue signature look — regardless of which customer, sticker, or product is involved.

## What it does

Given three immutable inputs:

1. **Customer's die-cut sticker** (artwork must never be altered)
2. **Customer's product / container**
3. **Approved UGC model** (the recurring "face" of the brand)

...the framework produces commercial-grade UGC advertising imagery that follows a fixed set of composition, realism, manufacturing, and quality-control rules — every single time, for every industry.

## Repo structure

```
UGCSticker-OS/
│
├── README.md                 <- you are here
├── SKILL.md                  <- Main Brain / entry point instructions
│
├── rules/                    <- Hard rules the AI must always obey
│   ├── sticker_rules.md
│   ├── composition_rules.md
│   ├── realism_rules.md
│   ├── camera_rules.md
│   ├── manufacturing_rules.md
│   ├── quality_control.md
│   ├── rejection_rules.md
│   ├── lighting_rules.md
│   ├── typography_rules.md
│   └── output_rules.md
│
├── templates/                <- Industry-specific creative direction
│   ├── Restaurant.md
│   ├── Juice.md
│   ├── Cosmetics.md
│   ├── Food.md
│   ├── Fashion.md
│   ├── Pharmaceutical.md
│   ├── Household.md
│   └── General.md
│
├── prompts/                  <- Ready-to-use prompt templates per output type
│   ├── HeroPrompt.md
│   ├── LifestylePrompt.md
│   ├── AmazonPrompt.md
│   ├── ShopifyPrompt.md
│   ├── SocialAdsPrompt.md
│   └── BillboardPrompt.md
│
└── examples/                 <- Reference input/output sets (add your own)
```

## How to use it

1. Start with `SKILL.md` — it's the operating system's main brain and tells the AI how to process the three inputs, in what order, and against which rule files.
2. Pick the right `templates/<Industry>.md` file for the customer's business category.
3. Pick the right `prompts/<Type>Prompt.md` for the output you need (hero shot, lifestyle shot, Amazon listing image, Shopify banner, social ad, billboard).
4. Feed `SKILL.md` + the relevant template + the relevant prompt + your three assets into the AI model of choice.
5. The AI runs the Stage 1 → Stage 4 pipeline (Analyze Sticker → Analyze Product → Apply Sticker → Quality Check) defined in `SKILL.md`, referencing the `rules/` files at each stage.

## Versioning

This framework is meant to evolve. Every time a better composition rule, a fix for a recurring defect, or a new industry template is discovered, bump the version and commit it so all future generations inherit the improvement.

```
v1 → v2 → v3 → ... → v10 → ... → v100
```

## Status

🚧 v1 — initial scaffold based on Sleekblue Media Houz's internal creative direction.
