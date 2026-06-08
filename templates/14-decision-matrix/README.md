# Decision Matrix

Status: planned

Category: Decision support

Purpose: Weighted option table with configurable criteria and scores.

## Files

- `composition.html` - HyperFrames variable-native boilerplate.
- `template-variables.schema.json` - Declared variables used by the composition.
- `sample-vars.json` - Sample render values matching the style review batch.

## HyperFrames Variable Pattern

This boilerplate declares variables on the `<html>` root with `data-composition-variables`, then reads them at runtime with `window.__hyperframes.getVariables()`.

Use CLI overrides with:

```powershell
npx hyperframes render composition.html --variables-file sample-vars.json --strict-variables --output 14-decision-matrix.mp4
```
