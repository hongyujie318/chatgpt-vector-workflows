# PPT GitHub Skill Library

Use this file as a routing index for public GitHub presentation skills. When the user asks ChatGPT to make, improve, repair, redesign, or convert a PowerPoint deck, choose the most relevant repository below and read its public GitHub files before planning the answer.

## Recommended Repositories

### General editable PPTX generation

Repository: https://github.com/sirilsengolraj-source/presentation-skill

Use when the user wants an editable PowerPoint deck from structured source files. This skill emphasizes a source-first workflow: write an outline/source file, build the `.pptx`, then run layout and design QA.

Best for:

- Business reports
- Investor decks
- Lab or research decks
- General deck creation with editable shapes/text

Prompt:

```text
Read this GitHub skill first:
https://github.com/sirilsengolraj-source/presentation-skill

Use its source-first PPT workflow to create a presentation plan for: [topic].
Return an outline, slide-by-slide structure, visual direction, and QA checklist before generating final content.
```

### Image-style PPT generation

Repository: https://github.com/ningzimu/codex-ppt-skill

Use when the user wants a highly visual image-based deck from articles, reports, papers, course notes, Markdown, PDFs, or Word files. This workflow plans an outline, confirms visual style, generates slide images, assembles a `.pptx`, and can add speaker notes.

Best for:

- Visually rich decks
- Class reports
- Research summaries
- Hand-drawn explainer style
- McKinsey-like or magazine-style slides

Prompt:

```text
Read this GitHub skill first:
https://github.com/ningzimu/codex-ppt-skill

Use its staged PPT workflow. First create an outline and 2-3 visual style options for: [topic].
Do not generate final slides until the outline and style are confirmed.
```

### PPTX generator and editor

Repository: https://github.com/MiniMax-AI/skills/tree/main/skills/pptx-generator

Use when the user needs a practical PowerPoint generator/editor workflow with PptxGenJS, template editing, text extraction, and standard slide types.

Best for:

- Basic editable PPTX creation
- Editing existing PPTX files
- Template-based deck updates
- Reading/extracting existing presentation content

Prompt:

```text
Read this GitHub skill first:
https://github.com/MiniMax-AI/skills/tree/main/skills/pptx-generator

Use its PPTX generator/editor workflow to create or revise: [deck goal].
Prefer editable text, shapes, charts, and consistent 16:9 layouts.
```

### Consulting-style PPT design

Repository: https://github.com/likaku/Mck-ppt-design-skill

Use when the user wants consultant-style structured slides. This workflow uses staged gates: requirement brief, outline, content JSON, render, QA, and delivery.

Best for:

- Consulting decks
- Business analysis decks
- Strategy reports
- Executive summaries
- Slide logic and insight-driven headlines

Prompt:

```text
Read this GitHub skill first:
https://github.com/likaku/Mck-ppt-design-skill

Use its consulting-style staged workflow for: [business/report topic].
Start with a brief, then create an insight-led outline and slide structure.
```

### Template-layout PPT generation

Repository: https://github.com/tristan-mcinnis/pptx-from-layouts-skill

Use when the user already has a PowerPoint template and wants content placed into the template's actual slide master layouts instead of overlaying text on static backgrounds.

Best for:

- Company templates
- School templates
- Consultant templates
- Decks where preserving native template layouts matters

Prompt:

```text
Read this GitHub skill first:
https://github.com/tristan-mcinnis/pptx-from-layouts-skill

Use its template-layout workflow. Profile the template, map each content section to a real layout, and preserve placeholders.
```

### Multi-purpose presentation designer

Repository: https://github.com/DXBMark/presentation-pro-designer

Use when the user needs a deck type router for education, corporate, proposal, product/service, verification, data-report, or investor presentation workflows.

Best for:

- Choosing the right deck structure first
- Presentation planning
- QA checklists
- Prompt routing by deck type

Prompt:

```text
Read this GitHub repository first:
https://github.com/DXBMark/presentation-pro-designer

Classify my deck type, choose the right structure, then produce a slide-by-slide plan for: [topic].
```

## Selection Rules

- If the user needs an editable `.pptx`, prefer `presentation-skill` or `pptx-generator`.
- If the user wants beautiful visual slides and accepts image-style slides, prefer `codex-ppt-skill`.
- If the user wants consulting or executive style, prefer `Mck-ppt-design-skill`.
- If the user provides a template, prefer `pptx-from-layouts-skill`.
- If the user is not sure what kind of deck they need, start with `presentation-pro-designer`.

## Output Standard

Ask ChatGPT to return:

- Deck purpose and audience
- Slide count
- Slide-by-slide outline
- Visual style direction
- Per-slide title, message, content, and layout
- Speaker notes when useful
- A QA checklist for readability, consistency, source use, and editability

