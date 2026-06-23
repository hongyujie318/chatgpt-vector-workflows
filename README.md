# ChatGPT Vector SVG Workflow Pack

This repository is a GitHub-readable workflow pack for ChatGPT Deep Research or ChatGPT with the GitHub connector.

It is not a native ChatGPT Skill upload. Use it when your ChatGPT account can connect GitHub repositories but does not show the Skills upload/editor UI.

## How To Use

1. Create a GitHub repository, for example `chatgpt-vector-workflows`.
2. Upload this folder to that repository.
3. In ChatGPT, connect the GitHub repository.
4. Start a prompt like:

```text
Use the GitHub repository `chatgpt-vector-workflows` as my vector workflow library.
Read `skills/svg-logo-builder.md`, then create an editable SVG logo for [brand name].
Return complete SVG code only, with short edit notes.
```

For icon sets:

```text
Read `skills/svg-icon-set-builder.md`.
Create a consistent SVG icon set for: search, upload, settings, user, notification.
Use a 24x24 viewBox and currentColor.
```

For diagrams:

```text
Read `skills/svg-diagram-illustrator.md`.
Create an editable SVG process diagram explaining [topic].
Use a 1200x800 viewBox and grouped, labeled elements.
```

## Files

- `skills/svg-logo-builder.md` - logos, marks, badges, wordmarks, app icons.
- `skills/svg-icon-set-builder.md` - consistent SVG icon systems.
- `skills/svg-diagram-illustrator.md` - diagrams, infographics, flows, architecture visuals.
- `prompts/quick-prompts.md` - copy-paste prompts for ChatGPT.

## Output Standard

Ask ChatGPT to return:

- A complete `<svg>` document.
- No raster images, base64 data, external fonts, JavaScript, or remote assets.
- Meaningful group IDs.
- A valid `viewBox`.
- Short edit notes.
