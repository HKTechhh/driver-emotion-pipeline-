# Driver Emotion Pipeline

A single static page walking through how the [driver-emotion](https://github.com/HKTechhh/driver-emotion)
project's two emotion-recognition models are built, trained, evaluated, and fine-tuned for
in-car use.

This is a standalone copy of that project's technical explainer doc, kept as its own
repository so it can be deployed independently (e.g. on Vercel) without pulling in the full
research codebase, model files, or datasets.

## Deploying

The whole site is one file, `index.html`, with no build step and no dependencies beyond two
Google Fonts loaded over CDN. Any static host works; on [Vercel](https://vercel.com):

1. Import this repository as a new Vercel project.
2. Leave the framework preset as "Other" and the build command empty — Vercel serves
   `index.html` directly from the repo root.
3. Deploy.

To preview locally, just open `index.html` in a browser, or serve the directory with any
static file server, e.g. `python3 -m http.server`.

## Source of truth

Every number on the page is pulled from the main project's `results/` and
`docs/experiment_log.md`. If those change, update `index.html` to match.
