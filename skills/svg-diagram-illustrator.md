# SVG Diagram Illustrator

Use this workflow when the user asks for a vector diagram, SVG infographic, process chart, architecture diagram, flow visual, editable illustration, timeline, comparison visual, or explanatory graphic.

## Goal

Turn concepts into crisp, editable SVG diagrams and explanatory vector illustrations. Prefer semantic layout, clear labels, and structured groups over decorative artwork.

## Workflow

1. Identify the diagram type: flow, timeline, comparison, hierarchy, architecture, cycle, funnel, map-like layout, or explanatory illustration.
2. Choose a fixed canvas: `viewBox="0 0 1200 800"` for landscape diagrams or `0 0 800 1200` for vertical posters.
3. Build layout first with regions, connectors, and label areas; add refinement after.
4. Group related elements with IDs such as `header`, `step-1`, `connector-2`, `legend`, and `annotations`.
5. Use readable text sizes and avoid tight text containers.
6. Return a complete standalone SVG in one fenced `svg` code block.

## Diagram Rules

- Use only editable SVG primitives, paths, text, gradients, masks, and simple filters.
- Avoid raster images, base64 data, scripts, and external assets.
- Use a restrained palette with strong contrast.
- Use arrows and connectors consistently.
- Keep text as SVG `<text>` unless outlined text is requested.
- Align elements to an implicit grid with consistent spacing.
- If real numbers are involved, state assumptions and represent values proportionally.

## Response Format

```text
Diagram: [title]
Layout: [flow/timeline/comparison/etc.]

```svg
<svg ...>
  <defs>...</defs>
  ...
</svg>
```

Edit notes:
- Main labels live in `text` elements.
- Color tokens are defined near the top.
- Resize by changing width/height while keeping the viewBox.
```

## Quality Check

Before final answer, verify:

- Valid `viewBox`.
- Labels are readable.
- Connectors point in the intended direction.
- Repeated components have consistent size and spacing.
- No external or raster dependencies.
