# diff-tool

Interactive prototype of the **Import / Merge postprocessor** window for ENCY (CAM/CNC, dark theme).

A single self-contained `index.html` (no build step) that shows a one-directional import/merge:
pull commands and subprograms from an imported postprocessor (left, read-only source) into the
current one (right, editable). Line-level and character-level diffs are computed live (LCS).

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deployment

Published via GitHub Pages (GitHub Actions). Pushing to `main` runs
[`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml), which deploys the
static site. The live page is served from the repository root (`index.html`).
