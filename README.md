# Hyperslides HyperFrames Educational Catalog

Reusable HyperFrames-style educational motion templates for trainer-led videos, module introductions, project management concepts, decision-making explainers, and VET learning support.

This catalog is designed as a small playground: each style has a variable-native HTML composition, a schema, sample values, and a short preview render.

## Built For HyperFrames

HyperFrames is the open-source HTML-to-video framework from HeyGen:

- GitHub: https://github.com/heygen-com/hyperframes
- Variables documentation: https://hyperframes.heygen.com/concepts/variables

These examples follow the HyperFrames variable pattern:

- variables declared with `data-composition-variables`
- runtime values read with `window.__hyperframes.getVariables()`
- sample values stored beside each composition as `sample-vars.json`
- fixed render settings kept outside the variable layer

## What Is Included

```text
templates/
  assets/                         shared base plates used by the samples
  01-base-flip-cards/
    composition.html
    template-variables.schema.json
    sample-vars.json
    README.md
  ...
previews/
  hyperslides_style_*.mp4          short preview renders
docs/
  variable-catalog-validation-report.md
catalog.manifest.json
```

## Styles

1. Base 01 - Voice-Paced Flip Cards
2. Base 02 - Drop/Slide Rows
3. Paragraph Build
4. Colour-Coded Meaning Signals
5. Right Way / Wrong Way Columns
6. Checklist Reveal
7. Cost Number Counter
8. Scope Funnel
9. Cost Stack
10. Triple Constraint
11. Gantt Bar Growth
12. Cost S-Curve
13. Decision Fork
14. Decision Matrix

## Try A Template

Install or clone HyperFrames from the upstream project, then render any composition with its sample variables.

Example:

```powershell
npx hyperframes render templates/07-number-counter/composition.html `
  --variables-file templates/07-number-counter/sample-vars.json `
  --strict-variables `
  --output renders/07-number-counter.mp4
```

If your local HyperFrames CLI uses different command names or flags, follow the current upstream docs.

## Build With An AI Coding Agent

These templates are intentionally plain HTML, CSS, JavaScript, and JSON, so they are easy to adapt with an AI coding agent such as Codex, Claude Code, Cursor, or another local coding assistant.

A useful workflow is:

1. Pick a style from `templates/`.
2. Open its `README.md`, `composition.html`, and `sample-vars.json`.
3. Ask your agent to adapt the sample variables for your lesson, topic, or course.
4. Keep the variable schema intact unless you are deliberately creating a new reusable variant.
5. Render a short preview, review the timing and text fit, then iterate.

Example prompt:

```text
Use templates/10-triple-constraint as the base. Keep the HyperFrames variable pattern intact, but adapt sample-vars.json for a short project management lesson about scope, time, cost, and quality. Keep the wording trainer-led and suitable for adult learners.
```

The agent should treat `composition.html` as the reusable template and `sample-vars.json` as the editable lesson data.

## Why These Exist

These templates came out of an ACS/Hyperslides workflow for clear, trainer-led educational videos. The goal is to make repeatable motion blocks that are easy to adapt by changing text, colours, labels, amounts, and simple state variables.

The preview MP4s are examples only. The reusable source is in `templates/<style>/composition.html`.

## Notes Before Publishing

- This catalog is released under the MIT License.
- Replace or remove the sample base plate images if you do not want to publish this visual look.
- These templates are community examples and are not affiliated with or endorsed by HeyGen.
- Do a final privacy/IP review before pushing to GitHub.
