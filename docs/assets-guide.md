# 🖼️ Assets Guide

Every SVG in this repository is **handcrafted** using pure vector graphics. No raster images, no Canva exports.

## Asset Inventory

| File | Dimensions | Purpose |
|:---|:---|:---|
| `logo.svg` | 200×200 | UT monogram in cyberpunk hexagon |
| `banner.svg` | 1200×400 | Full-width hero banner |
| `background.svg` | 1200×40 | Subtle dot-grid background tile |
| `divider.svg` | 1200×30 | Section divider with gradient line |
| `footer.svg` | 1200×200 | Footer with wave and attribution |
| `profile-card.svg` | 480×320 | Glassmorphic developer card |
| `timeline.svg` | 800×620 | Journey and hackathon timeline |
| `projects.svg` | 900×580 | Portfolio project showcase |
| `tech-icons.svg` | 900×480 | Tech stack grid |

## SVG Techniques Used

### Gradients
All SVGs use `<linearGradient>` and `<radialGradient>` for the neon color effects.

### Gaussian Blur
`<feGaussianBlur>` creates the neon glow effects on nodes, borders, and text.

### Masks & Clipping
`<mask>` and `<clipPath>` are used for fade effects, wave shapes, and avatar circles.

### Reusable Symbols
`<symbol>` and `<use>` minimize duplication — tech chips, timeline nodes, and priority labels all use shared definitions.

### Color Matrix
`<feColorMatrix>` tints the blur output to match the neon color palette.

## Modifying SVGs

1. Open the SVG in any text editor (VS Code recommended)
2. Find the `<defs>` section — this contains all gradients, filters, and symbols
3. Modify colors by changing `stop-color` values in gradients
4. Modify text by editing `<text>` elements directly
5. Save and verify rendering in a browser

## GitHub SVG Constraints

GitHub's SVG renderer has restrictions:
- ❌ No `<script>` tags
- ❌ No `<foreignObject>`
- ❌ No external resources (fonts, images, stylesheets)
- ❌ No CSS `@import`
- ✅ Inline styles work
- ✅ `<defs>`, `<symbol>`, `<use>` work
- ✅ Filters (`<filter>`) work
- ✅ Gradients work
- ✅ System fonts work
