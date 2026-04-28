# PPT Master Integration

Use this file when generating slides with PPT master.

## Deck Defaults

- Aspect ratio: 16:9
- Canvas: `1280 x 720`
- Background: `#FFFFFF` or `#F7F3EE`
- Primary text: `#2F2F2F`
- Muted blue: `#A7C7E7`
- Dusty orange: `#E8A87C`
- Divider: `#DED8D1`
- Pale blue: `#EAF4FC`
- Pale orange: `#FCE8DA`

## SVG Spec Lock

Every slide should follow these constraints:

- Use `viewBox="0 0 1280 720"`.
- Use embedded text, not rasterized text.
- Keep text within safe margins.
- Use explicit fills and strokes.
- Use simple gradients only when they improve illustration softness.
- Use filters only for very light, local illustration shadow if the PPT workflow supports them; otherwise use pale flat ellipses as shadows.
- Avoid external image links unless intentionally bundled.
- Prefer simple SVG primitives and paths.

## Design Process

1. Read the source and identify the key idea per slide.
2. Decide the visual metaphor before drawing.
3. Choose a slide pattern from `slide-patterns.md`.
4. Place typography first, then illustration, then secondary labels.
5. Keep illustrations calm and balanced.
6. Run the QA checklist before export.

## Text Density

- Cover: title, subtitle, one metadata line.
- Content slide: one main idea and 2-4 support points.
- Body copy: 8-18 words per block.
- Avoid long bullet lists.

## Illustration Production Rules

- Keep paths clean and shapes editable.
- Use layered vector forms rather than raster images when possible.
- Use gradients sparingly.
- Ground figures with pale soft ellipses instead of heavy shadows.
- Use simplified people without cartoon exaggeration.

## Forbidden Treatments

- 3D realism
- Heavy shadows
- Cartoon mascot styling
- Neon palettes
- Dense dashboards
- Overly literal clipart
- Busy full-canvas scenes
- Excessive gradients
