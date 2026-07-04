# Quality Control — Self-Scoring Checklist

Before any output is presented as final, score the render against every item below. If any item fails, redo the render internally — never present a failing image as final.

```
1.  Sticker shape/contour intact?            100/100 required
2.  Typography legible and unaltered?         100/100 required
3.  Colour accurate to source artwork?        100/100 required
4.  QR code (if present) crisp and intact?    Pass/Fail
5.  Container proportions realistic?          Pass/Fail
6.  Hero sticker fully readable?              Pass/Fail
7.  Background believable for the industry?   Pass/Fail
8.  Hand/finger placement natural & unobtrusive? Pass/Fail
9.  Perspective/projection correct?           Pass/Fail
10. Shadows and reflections physically correct? Pass/Fail
11. Overall commercial/advertising quality?    Pass/Fail
```

**Rule:** All items must pass before output. If any item fails twice in a row on the same asset set, stop and flag the issue rather than continuing to regenerate blindly — this usually means the input assets need re-checking (e.g. low-resolution sticker upload) rather than a prompt problem.

## Escalation

If a render repeatedly fails the same checklist item across attempts, log it as a known issue and consider whether a rule file needs updating (see Versioning in `SKILL.md`).
