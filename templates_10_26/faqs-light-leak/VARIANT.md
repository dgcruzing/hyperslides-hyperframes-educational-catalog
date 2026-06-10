# FAQ Light Leak Variant

Status: accepted-locked

Source reference:
- Reference concept: Light Leak shader sample with navy background, orange flare, subtle grid, and warm directional transition energy.

Implementation notes:
- Kept the accepted FAQ information architecture intact.
- Changed the variant palette to navy `#001524` and orange `#fb8b24`.
- Added a render-safe GSAP/CSS light-leak layer behind the FAQ card instead of embedding the full WebGL shader, so the variant stays easy to edit and less brittle in Hyperframes.
- Used `overwrite: "auto"` on the new light overlay tweens.

Proof outputs:
- `..\..\renders\faqs-light-leak.mp4`
- `..\..\renders\faqs-light-leak-frame-3s.png`

Known render warnings:
- Existing FAQ panel swap animations still trigger unresolved GSAP overlap lint warnings.
- Google Fonts warning remains from the base template pattern.

Lock notes:
- 2026-06-10: Daniel accepted this as a locked style base for future FAQ style experiments.
- Future experiments should copy this folder to a new sibling under `variants\` and leave `variants\light-leak` intact.
