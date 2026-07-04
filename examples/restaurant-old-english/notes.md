# Restaurant — Old English Bar & Grills

**Industry template used:** templates/Restaurant.md
**Prompt file used:** prompts/HeroPrompt.md
**Date:** 2026-07-04

## Inputs
- **Sticker:** Rounded-rectangle die-cut, glossy finish. Red background, white "OLD ENGLISH" wordmark arched over a black "BAR & GRILLS" ribbon, two antelope-head logo marks, small flame icon, "Scan Here" QR code bottom-left, address/phone/social contact block on the right, secondary "Exclusive by Cubana" line.
- **Product:** Translucent plastic take-out container with a snap-fit lid; sticker applied flat and centered on the lid's top panel.
- **Model:** Approved reference — young woman, black off-shoulder bodycon dress, bun updo, warm natural smile, neutral studio backdrop in the source photo (background to be replaced per the Restaurant template in the final render).

## Generated Prompt (Hero Shot)

```
A high-end commercial hero photograph. A young Nigerian woman with her hair in a bun, wearing
a black off-shoulder fitted dress, holds an Old English Bar & Grills take-out container toward
the camera with a warm, genuine smile. The die-cut sticker on the container's lid is fully
visible and perfectly readable, occupying approximately 40% of the frame: red background,
white arched "OLD ENGLISH" wordmark, black "BAR & GRILLS" ribbon banner, two antelope-head
logo marks, small flame icon above the wordmark, "Scan Here" QR code on the left, and the
address/phone/social contact block on the right — all rendered exactly as the source artwork,
zero redesign. The translucent plastic container occupies approximately 20% of the frame, held
naturally at chest height, with realistic reflections and a soft contact shadow. Background: a
warm, busy Nigerian bar & grill setting — diners eating and laughing in soft focus, a visible
grill station, warm string lighting or ambient evening tones. Lighting: warm, natural, ambient
restaurant light, no flat studio lighting. Ultra photorealistic, 8K, commercial advertising
quality, natural skin texture, correct material physics on the translucent plastic, sticker
sharp and legible even against the busy background.
```

## What worked
- Locking the sticker's exact contact-info block and dual-logo layout up front (Stage 1) avoids the model "cleaning up" or simplifying the contact details, which is a common failure mode with busy stickers.
- Naming the container material explicitly ("translucent plastic," "snap-fit lid") gets more accurate reflections than a generic "container" description.

## What needed correction
- The raw reference photos include background artifacts (an HP laptop logo, a rough wooden table) that must NOT carry into the final render — called out explicitly so the image AI doesn't treat them as intended set dressing.
- Reference model photo has a neutral studio background; the prompt explicitly overrides this with the Restaurant template's busy bar & grill setting rather than defaulting to the studio look.

## Rule file impact
- None yet — first pass. If the QR code or contact block gets distorted/simplified across multiple generation attempts, that would justify adding an explicit "dense text block" sub-rule to `rules/typography_rules.md` for stickers carrying a lot of small print.
