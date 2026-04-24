# ppt-master Integration

Use this reference when applying either Japanese editorial style inside `ppt-master`.

## Eight Confirmations Defaults

1. Canvas format: `PPT 16:9`, `0 0 1280 720`.
2. Page count: choose fewer pages than a dense consulting deck; protect negative space.
3. Target audience: define whether the deck is executive, brand, humanities, internal sharing, or proposal.
4. Style objective: usually `General Consulting` for business clarity, or `General Versatile` for brand story.
5. Color scheme: choose either Style 1 (paper + charcoal + indigo) or Style 2 (white + charcoal + burnt orange).
6. Icon usage: built-in `tabler-outline`, minimal inventory.
7. Typography: Style 1 uses editorial serif title; Style 2 uses bold elegant sans-serif headings.
8. Image usage: prefer existing images or vector diagrams; avoid AI imagery unless the user asks for atmospheric background assets.

## design_spec.md Language

Use the standard `ppt-master` design spec structure. In section III, describe:

- "Japanese minimalist washi paper texture"
- "soft off-white tactile background"
- "thin gray architectural rules"
- "single indigo accent"
- "professional editorial warmth"

For Style 2, describe:

- "High-end Japanese lifestyle magazine editorial"
- "Stark white background"
- "Bold but elegant sans-serif headings"
- "Structured grid layout with generous negative space"
- "Burnt orange and charcoal gray accents"
- "Asymmetric edge-pressed image composition"

## Style 1 spec_lock.md Defaults

Use this as a starting point and adjust only when needed:

```markdown
## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- bg: #F5F5F5
- bg_secondary: #EFEDEA
- primary: #2C3E50
- accent: #2C3E50
- text: #333333
- text_secondary: #6B6B6B
- text_tertiary: #9A9690
- border: #D8D6D0
- soft_lavender: #D5D0DB
- wisteria: #B3AFCB
- blue_gray: #8995B7
- moss_gray: #777F6C
- clay_rose: #AA6F5F

## typography
- font_family: Microsoft YaHei, PingFang SC, Arial, sans-serif
- title_family: Georgia, Microsoft YaHei, serif
- emphasis_family: Georgia, Microsoft YaHei, serif
- code_family: Consolas, Courier New, monospace
- body: 20
- title: 34
- subtitle: 24
- annotation: 15
- cover_title: 64
- chapter: 44
- hero_number: 38
- footnote: 11

## icons
- library: tabler-outline
- inventory: target, circle-check, chart-bar, notes, feather, leaf, sparkle, route, template, users
```

Before finalizing the icon inventory, verify icon filenames exist in `skills/ppt-master/templates/icons/tabler-outline`.

## SVG Execution Rules

- Re-read `spec_lock.md` before every page.
- Build paper texture with SVG circles/lines or low-opacity paths; do not use filters that may export poorly.
- Use `fill-opacity` / `opacity` attributes, not `rgba()`.
- Use thin rules and open frames instead of many filled cards.
- Keep titles assertion-like and concise.
- Include source footers in a quiet monospace style.

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

Adjust rhythm based on source content. Do not add breathing pages as filler.

## Style 2 spec_lock.md Defaults

Use this when the user asks for the second style:

```markdown
## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- bg: #FFFFFF
- bg_secondary: #F4F2EF
- primary: #CC5500
- accent: #CC5500
- text: #333333
- text_secondary: #6B6B6B
- text_tertiary: #8A8580
- border: #D9D9D6
- deep_clay: #71362B
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
- chapter: 46
- hero_number: 42
- footnote: 11

## icons
- library: tabler-outline
- inventory: arrow-right, circle-check, chart-bar, layout-grid, photo, route, template, users
```

For Style 2 SVG execution:

- Use `#FFFFFF` as the dominant background.
- Use burnt orange only for small active accents, not broad fills.
- Use asymmetric edge-pressed images when images exist.
- If no images exist, simulate magazine energy through cropped geometric blocks, vertical type labels, and precise grid rules.
- Keep 16:9 throughout.
