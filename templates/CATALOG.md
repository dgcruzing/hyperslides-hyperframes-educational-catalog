# Hyperslides HyperFrames Variable Catalog

Status: full variable-native boilerplate catalog.

Source docs: [HyperFrames Variables](https://hyperframes.heygen.com/concepts/variables)

## What This Catalog Contains

Each style folder contains:

- `composition.html`
- `template-variables.schema.json`
- `sample-vars.json`
- `README.md`

## Styles

1. [Base 01 - Voice-Paced Flip Cards](./01-base-flip-cards/README.md) - Default ACS module-intro pattern with two voice-paced flip cards.
2. [Base 02 - Drop/Slide Rows](./02-drop-slide-rows/README.md) - Row-by-row reveal for topic slides that need more than two card ideas.
3. [Paragraph Build](./03-paragraph-build/README.md) - Line-by-line reveal for narrated explanation.
4. [Colour-Coded Meaning Signals](./04-meaning-signals/README.md) - Show approved, warning, caution, and neutral states with colour.
5. [Right Way / Wrong Way Columns](./05-comparison-columns/README.md) - Side-by-side contrast between preferred and poor practice.
6. [Checklist Reveal](./06-checklist-reveal/README.md) - Step-by-step checklist reveal for evidence or process cues.
7. [Cost Number Counter](./07-number-counter/README.md) - Animated count-up for budget or cost impact.
8. [Scope Funnel](./08-scope-funnel/README.md) - Visual metaphor for narrowing possible work into approved scope.
9. [Cost Stack](./09-cost-stack/README.md) - Stacked budget categories with configurable labels and proportions.
10. [Triple Constraint](./10-triple-constraint/README.md) - Animated triangle showing scope, time, cost, and quality.
11. [Gantt Bar Growth](./11-gantt-bars/README.md) - Horizontal bar growth for schedule sequence.
12. [Cost S-Curve](./12-s-curve/README.md) - Animated cumulative cost curve.
13. [Decision Fork](./13-decision-fork/README.md) - Forked path showing positive and negative consequences.
14. [Decision Matrix](./14-decision-matrix/README.md) - Weighted option table with configurable criteria and scores.

## Notes

- Dimensions and FPS remain fixed in the composition/render command, not variables.
- Text, colours, booleans, numbers, enum options, and media URLs are variables.
- Complex lists are expressed as named primitive fields rather than array variables so the Studio UI can render useful controls.
