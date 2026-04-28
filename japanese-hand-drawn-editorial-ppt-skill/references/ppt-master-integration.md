# PPT Master Integration

Use this file when generating slides with PPT master.

## Deck Defaults

- Aspect ratio: 16:9
- Canvas: `1280 x 720`
- Background: `#F8F6F2`
- Primary text: `#2B2B2B`
- Secondary text: `#6C6C6C`
- Soft gray: `#BDBDBD`
- Muted indigo: `#6C7A89`
- Pale wash: `#EAE7E1`

## SVG Spec Lock

Every slide should follow these constraints:

- Use `viewBox="0 0 1280 720"`.
- Use embedded text, not rasterized text.
- Keep text inside safe margins.
- Use explicit fills and strokes.
- Use mostly simple SVG primitives and paths.
- Use slight irregularity in line paths to imply hand-drawn craft.
- Avoid heavy filters, glossy effects, strong shadows, and external image links.

## Design Process

1. Summarize the source into one message per slide.
2. Select a soft illustration metaphor.
3. Choose a slide pattern from `slide-patterns.md`.
4. Place text and illustration asymmetrically.
5. Add small annotations and pale wash last.
6. Run QA before exporting.

## Text Density

- Cover: title, subtitle, one small metadata line.
- Content slide: one main idea and 2-3 support notes.
- Body copy: 8-18 words per block.
- Avoid dense bullets.

## Illustration Production Rules

- Use editable SVG paths where possible.
- Use uneven line paths and imperfect curves.
- Keep fills pale and transparent-looking.
- Keep annotations small and quiet.
- Avoid clean tech iconography and perfect geometric diagrams.

## Forbidden Treatments

- Heavy contrast
- Bold saturated colors
- Glossy effects
- 3D realism
- Sharp tech grids
- Dashboard styling
- Cartoon mascots
- Dense full-canvas scenes
