# SVG Logo Builder

Use this workflow when the user asks for a logo, mark, emblem, wordmark, badge, favicon, app icon, brand symbol, or editable SVG identity concept.

## Goal

Create clean, editable vector logo concepts as standalone SVG. Prefer simple geometry, clear silhouettes, and reusable structure over decorative complexity.

## Workflow

1. Clarify only essential missing details: brand name, industry, mood, colors, and whether the output should be icon-only, wordmark-only, or icon plus wordmark.
2. If direction is vague, propose 2-3 visual directions before final SVG.
3. Use a fixed `viewBox`: `0 0 512 512` for icon-only marks or `0 0 1200 400` for logo lockups.
4. Use editable SVG elements: `path`, `rect`, `circle`, `polygon`, `line`, `text`, and `g`.
5. Avoid embedded images, base64, external fonts, JavaScript, and remote assets.
6. Group important parts with IDs such as `mark`, `wordmark`, `accent`, and `background`.
7. Return the complete SVG in one fenced `svg` code block.

## Design Rules

- Make the mark recognizable at 32 px.
- Use no more than 2-3 brand colors unless asked otherwise.
- Prefer flat fills and simple strokes.
- Use generic font-family fallbacks such as `Inter, Arial, sans-serif`.
- Explain that final production logos should convert text to outlines in a vector editor.
- Avoid copying trademarked logos, copyrighted characters, or existing brand identities.
- Do not claim legal trademark clearance.

## Response Format

```text
Concept: [short name]
Use case: [where it works best]

```svg
<svg ...>
  ...
</svg>
```

Edit notes:
- Colors: ...
- Text is editable in the `wordmark` group.
- Save as `brand-name-logo.svg`.
```

## Quality Check

Before final answer, verify:

- Complete `<svg>` root and valid `viewBox`.
- No external or raster dependencies.
- Mark remains legible when small.
- Colors are consistent.
- Group IDs make editing easier.
