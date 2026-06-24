# SVG Icon Set Builder

Use this workflow when the user asks for icons, an icon pack, SVG icons, vector icons, pictograms, UI symbols, line icons, filled icons, or a consistent visual system for multiple small symbols.

## Goal

Create coherent SVG icon sets with consistent geometry, stroke weight, corner radius, spacing, and naming. The output should be easy to paste into code, Figma, Illustrator, or Inkscape.

## Workflow

1. Identify requested icons and target style: outline, filled, duotone, solid, rounded, sharp, playful, technical, or minimal.
2. Default to a `24 x 24` viewBox for UI icons or `64 x 64` for presentation icons.
3. Define shared style tokens before drawing: `stroke-width`, `stroke-linecap`, `stroke-linejoin`, fill behavior, and color.
4. Create every icon with the same `viewBox` and consistent visual weight.
5. Return each icon as a standalone SVG unless the user asks for a sprite.
6. Include a compact manifest listing icon names and intended meanings.

## SVG Rules

- Avoid embedded raster images, base64 data, external CSS, external fonts, scripts, and remote links.
- Prefer paths and simple primitives.
- Use `currentColor` for single-color UI icons.
- Add `<title>` only when icons will be used standalone.
- Keep icons optically centered.
- Do not mix filled and outline styles in one set unless variants are requested.

## Response Format

```text
Icon system:
- Grid: 24 x 24
- Style: rounded outline
- Stroke: 1.75
- Color: currentColor

Manifest:
- search: magnifier for search fields
- upload: arrow into tray

```svg
<!-- search.svg -->
<svg ...>...</svg>
```
```

## Quality Check

Before final answer, verify:

- Every SVG uses the same `viewBox`.
- Stroke widths and line caps match.
- Icon names are filesystem-safe.
- No icon depends on raster images or external resources.
- Icons have enough negative space for small sizes.
