# PPT Master Integration

Use this file when generating slides with PPT master.

## Deck Defaults

- Aspect ratio: 16:9
- Canvas: `1280 x 720`
- Background: `#F5EFE6`
- Primary text: `#3A3A3A`
- Accent: `#A68A64`
- Divider: `#D8CCBD`
- Muted text: `#746F68`
- Pale fill: `#FBF7F1`

## SVG Spec Lock

Every slide should follow these constraints:

- Use `viewBox="0 0 1280 720"`.
- Use embedded text, not rasterized text.
- Keep text within safe margins.
- Use explicit fills and strokes.
- Avoid filters, blur, shadows, gradients, and external image links.
- Prefer simple SVG primitives: `rect`, `line`, `path`, `circle`, and `text`.

## Design Process

1. Read the source document and extract the premium narrative.
2. Reduce each slide to one message.
3. Choose a pattern from `slide-patterns.md`.
4. Apply large margins before adding details.
5. Use subtle dividers and soft brown accents only after the hierarchy is clear.
6. Run the QA checklist before exporting to PPTX.

## Text Density

- Cover: title plus one subtitle or metadata line.
- Content slide: one main idea, 2-4 supporting blocks.
- Body copy: 8-18 words per block.
- Avoid long bullet lists; use editorial statements and concise labels.

## Typography Rules

- Use serif for title-level hierarchy.
- Use sans-serif for body and labels.
- Do not mix more than two font families.
- Keep line spacing generous.

## Forbidden Treatments

- Heavy cards
- Thick borders
- Drop shadows
- Glow effects
- Bright saturated colors
- Dense dashboards
- Decorative icon rows
- Busy photo collages
- Gradient backgrounds
