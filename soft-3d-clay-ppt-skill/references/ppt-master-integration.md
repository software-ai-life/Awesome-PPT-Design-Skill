# ppt-master Integration

Use this reference when applying Soft 3D / Claymorphism inside `ppt-master`.

## Eight Confirmations Defaults

1. Canvas format: `PPT 16:9`, `0 0 1280 720`.
2. Page count: protect whitespace; avoid too many dense pages.
3. Target audience: define whether the deck is business, product, brand, or internal training.
4. Style objective: usually `General Versatile` for visual warmth or `General Consulting` for business clarity.
5. Color scheme: warm beige + sage + warm pink + charcoal.
6. Icon usage: built-in `tabler-outline`, minimal inventory.
7. Typography: clean sans-serif title and body, monospace labels.
8. Image usage: use existing screenshots/photos when useful; otherwise use vector soft 3D geometry.

## design_spec.md Language

Use the standard `ppt-master` design spec structure. In section III, describe:

- "Minimalist professional presentation"
- "Soft 3D / Claymorphism aesthetic"
- "Soft matte geometric shapes floating in corners"
- "Pastel beige, sage green, and Morandi warm pink palette"
- "Airy modern UI-like layout"
- "Sophisticated soft shadows and high-end illustration feel"

## spec_lock.md Defaults

```markdown
## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- bg: #FDF5E6
- bg_secondary: #FFF9EF
- primary: #B2AC88
- accent: #DBADAD
- text: #333333
- text_secondary: #6B6B6B
- text_tertiary: #9A9288
- border: #E7DAC8
- sage: #B2AC88
- warm_pink: #DBADAD
- shadow: #C8BBA8
- white: #FFFFFF

## typography
- font_family: Microsoft YaHei, PingFang SC, Arial, sans-serif
- title_family: Arial, Microsoft YaHei, sans-serif
- emphasis_family: Arial, Microsoft YaHei, sans-serif
- code_family: Consolas, Courier New, monospace
- body: 20
- title: 38
- subtitle: 24
- annotation: 14
- cover_title: 68
- chapter: 44
- hero_number: 42
- footnote: 11

## icons
- library: tabler-outline
- inventory: circle-check, chart-bar, cube, sphere, layout-grid, route, sparkles, template, users
```

Before finalizing icon inventory, verify icon filenames exist in `skills/ppt-master/templates/icons/tabler-outline`.

## SVG Execution Rules

- Re-read `spec_lock.md` before every page.
- Build soft 3D shapes with layered SVG geometry, not external images unless requested.
- Do not use `rgba()`.
- Avoid filters if they create export problems; approximate soft shadows with low-opacity offset shapes.
- Keep 3D accents out of text-heavy zones.
- Use 16:9 throughout unless the user explicitly overrides.

## Suggested Page Rhythm

```markdown
## page_rhythm
- P01: anchor
- P02: breathing
- P03: dense
- P04: dense
- P05: breathing
- P06: dense
- P07: dense
- P08: breathing
- P09: dense
- P10: anchor
```
