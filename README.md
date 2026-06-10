# Hyperslides HyperFrames Educational Catalogue

Reusable HyperFrames-style educational motion templates for trainer-led videos, module introductions, project management concepts, decision-making explainers, and VET learning support.

Start with the newer V4 template set in `templates_10_26/`. It includes 19 base templates plus approved variants, each with a variable-native HTML composition, a schema, sample values, and matching preview assets.

## Start Here: V4 Templates

Use `templates_10_26/` as the current more robust release set.

It contains:

- 19 base educational motion templates.
- 12 approved variant templates.
- `previews/` with the matching preview MP4s and selected proof frames.
- self-contained template folders with `composition.html`, `template-variables.schema.json`, `sample-vars.json`, and `README.md`.

The older `templates/` folder is still included as the original 14-style catalogue.

## Dummies Guide

If you are new to this workflow, start with the plain-English Google Slides guide:

- Dummies guide slides: https://docs.google.com/presentation/d/e/2PACX-1vT8RKiLMCS5sSL5t-RqPpQZB_8I7usiKG7a1o6O3Qy3SsaB5BlUAk-ansl81jC1mb-S_XgbNaHenGxe/pub?start=false&loop=false&delayms=3000

## Built On HyperFrames

This catalogue is built on top of HyperFrames. A lot of the base composition pattern, render workflow, and HTML-to-video approach comes from the HyperFrames project:

- HyperFrames site: https://www.hyperframes.dev/
- GitHub: https://github.com/heygen-com/hyperframes
- Variables documentation: https://hyperframes.heygen.com/concepts/variables

This repository is a template catalogue for education and training use. It is not a replacement for the base HyperFrames project.

## Claude Cowork And HyperFrames MCP

You can also use these templates as a starting base inside Claude Cowork with the HyperFrames MCP. Grab a folder from `templates_10_26/`, load the `composition.html`, `sample-vars.json`, and schema into your Cowork context, then use the MCP to adapt, preview, edit, and render the composition conversationally.

HyperFrames MCP guide: https://hyperframes.heygen.com/guides/mcp

For local rendering, beginners should have both:

1. The base HyperFrames project from HeyGen.
2. This educational template catalogue.

These examples follow the HyperFrames variable pattern:

- variables declared with `data-composition-variables`
- runtime values read with `window.__hyperframes.getVariables()`
- sample values stored beside each composition as `sample-vars.json`
- fixed render settings kept outside the variable layer

## Beginner Setup Checklist

Before you try to render a video, make sure you have:

- A local copy of HyperFrames: https://github.com/heygen-com/hyperframes
- A local copy of this catalogue: https://github.com/dgcruzing/hyperslides-hyperframes-educational-catalog
- Node.js installed.
- A graphics card suitable for local video rendering.
- Recommended minimum for local rendering: a GPU with at least 4 GB VRAM.
- More GPU memory is better for heavier renders, longer videos, and smoother iteration.

If you only want to look around, start with the preview MP4s in `previews/`. You do not need to render anything just to understand the styles.

## What Is Included

```text
templates_10_26/
  01-achievements-challenges/
    composition.html
    template-variables.schema.json
    sample-vars.json
    README.md
  ...
  previews/
    *.mp4                          preview renders and proof frames

templates/
  assets/                          shared base plates used by the original samples
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

## V4 Base Templates

The current V4 set is in `templates_10_26/`:

1. Achievements Challenges
2. Circle Lift
3. Code of Ethics
4. Contingency Plan
5. Contrasting Grid
6. Curved Timeline
7. Executive Summary
8. FAQs
9. Four Ways Skills
10. Freelancer Tips
11. Gap Analysis
12. Johari Window
13. Medical Tabs
14. Process Flow
15. Terms Definitions
16. Transformation Map
17. Trial Flow
18. Tuckman Model
19. Value Innovation

## V4 Variants

The V4 folder also includes these approved variant styles:

1. Contrasting Grid Ripple
2. Executive Summary Signal Board
3. FAQs Light Leak
4. Four Ways Skills Contingency Style
5. Freelancer Tips Chromatic Radial
6. Freelancer Tips Claude Editorial
7. Johari Window SafeX Cockpit
8. Medical Tabs SDF Iris
9. Process Flow Bounce Wow
10. Terms Definitions Edu Whip
11. Transformation Map Flight Mode
12. Trial Flow Three D Reveal

## Try A Template

Install or clone HyperFrames from the upstream project first, then place or reference this catalogue where your HyperFrames render workflow can find it.

Plain-English version:

1. Get HyperFrames.
2. Get this catalogue.
3. Pick one folder in `templates_10_26/`.
4. Edit that folder's `sample-vars.json`.
5. Preview.
6. Render only when the wording fits.

Example:

```powershell
npx hyperframes render templates_10_26/15-process-flow/composition.html `
  --variables-file templates_10_26/15-process-flow/sample-vars.json `
  --strict-variables `
  --output renders/process-flow.mp4
```

If your local HyperFrames CLI uses different command names or flags, follow the current upstream docs.

## Build With An AI Coding Agent

These templates are intentionally plain HTML, CSS, JavaScript, and JSON, so they are easy to adapt with an AI coding agent such as Codex, Claude Code, Cursor, or another local coding assistant.

A useful workflow is:

1. Pick a style from `templates_10_26/`.
2. Open its `README.md`, `composition.html`, and `sample-vars.json`.
3. Ask your agent to adapt the sample variables for your lesson, topic, or course.
4. Keep the variable schema intact unless you are deliberately creating a new reusable variant.
5. Render a short preview, review the timing and text fit, then iterate.

Example prompt:

```text
Use templates_10_26/15-process-flow as the base. Keep the HyperFrames variable pattern intact, but adapt sample-vars.json for a short project management lesson about scope, time, cost, and quality. Keep the wording trainer-led and suitable for adult learners.
```

The agent should treat `composition.html` as the reusable template and `sample-vars.json` as the editable lesson data.

## Why These Exist

These templates came out of an ACS/Hyperslides workflow for clear, trainer-led educational videos. The goal is to make repeatable motion blocks that are easy to adapt by changing text, colours, labels, amounts, and simple state variables.

The preview MP4s are examples only. The reusable V4 source is in `templates_10_26/<style>/composition.html`.

## Notes

- This catalogue is released under the MIT License.
- The base code pattern and render workflow are heavily informed by HyperFrames: https://www.hyperframes.dev/
- These templates are community examples and are not affiliated with or endorsed by HeyGen or HyperFrames.

