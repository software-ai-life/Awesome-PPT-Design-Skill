# PPT Master Integration

Use this file when generating slides with PPT master.

## Deck Defaults

- Aspect ratio: 16:9
- Canvas: `1280 x 720`
- Background: `#FFFFFF`
- Primary text: `#2B2B2B`
- Accent: `#2F6BFF`
- Grid/divider: `#E6EAF2`
- Secondary text: `#6B6B6B`
- Pale module fill: `#F7F9FC`

## SVG Spec Lock

Every slide should follow these constraints:

- Use `viewBox="0 0 1280 720"`.
- Use embedded text, not rasterized text.
- Keep text within safe margins.
- Use real text elements for all readable content.
- Use explicit fills and strokes.
- Do not use filters, blur, shadows, gradients, or external image links.
- Prefer simple SVG primitives: `rect`, `line`, `path`, `circle`, `text`, `polyline`.

## Design Process

1. Read and summarize the source document.
2. Decide the 3-5 slide narrative before drawing.
3. Assign each slide one slide pattern from `slide-patterns.md`.
4. Create the visual hierarchy first: title, signal, structure, support.
5. Add grid fragments and data-inspired details last.
6. Run the QA checklist before exporting to PPTX.

## Text Density

- Cover: title plus one short subtitle.
- Content slide: maximum 1 main idea, 3-5 modules.
- Body copy: prefer 8-16 words per block.
- Avoid full paragraphs unless quoting a source.

## Icon And Chart Rules

- Use thin outline icons only when they clarify meaning.
- Avoid decorative icon rows.
- Charts should be flat and directly labeled.
- Blue marks the key signal; graphite provides context.

## Forbidden Treatments

- Shadows
- Glow effects
- Glassmorphism
- Claymorphism
- 3D geometry
- Warm paper texture
- Decorative blobs
- Heavy rounded cards
- Dense tables with full grid borders
