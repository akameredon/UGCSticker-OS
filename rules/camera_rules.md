# Camera Rules

## Framing

- Default to a shot that reads naturally as a phone-shot UGC photo/video frame, not a studio product shoot, unless the prompt file (e.g. `BillboardPrompt.md`) calls for a formal ad composition.
- Eye-level or slightly above-eye-level angle for hero/hand-held shots — avoid extreme low or high angles unless the industry template calls for drama (e.g. billboard hero shots).

## Lens & Depth of Field

- Simulate a natural phone/mirrorless lens look: shallow-to-moderate depth of field, subject and hero sticker in sharp focus, background softly blurred.
- Never blur the sticker itself, even when background blur is heavy — the sticker must remain the sharpest, most legible element in frame alongside the model's face.

## Stability

- No motion blur on the sticker or product.
- Slight, natural handheld framing imperfection is acceptable for authenticity in UGC-style shots; studio/billboard shots should be perfectly level and centered.

## Aspect Ratio by Output Type

Match aspect ratio to the intended platform (see matching file in `/prompts/`):
- Social ads / Reels / TikTok: 9:16
- Amazon / Shopify listing images: 1:1 or 4:5
- Billboard: wide format appropriate to placement (e.g. 16:9 or wider)
