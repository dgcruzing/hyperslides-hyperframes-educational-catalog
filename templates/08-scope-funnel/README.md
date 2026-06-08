# Scope Funnel

Status: planned

Category: Scope visual

Purpose: Visual metaphor for narrowing possible work into approved scope.

## Files

- `composition.html` - HyperFrames variable-native boilerplate.
- `template-variables.schema.json` - Declared variables used by the composition.
- `sample-vars.json` - Sample render values matching the style review batch.

## HyperFrames Variable Pattern

This boilerplate declares variables on the `<html>` root with `data-composition-variables`, then reads them at runtime with `window.__hyperframes.getVariables()`.

Use CLI overrides with:

```powershell
npx hyperframes render composition.html --variables-file sample-vars.json --strict-variables --output 08-scope-funnel.mp4
```
