# Inverse Rendering for Modeling with Line Primitives

Project page for the SIGGRAPH Asia 2026 (ACM TOG) paper.

- Page: https://kenji-tojo.github.io/sa26-line-primitives/
- Code: https://github.com/kenji-tojo/inverse-line-primitives
- Dataset: https://huggingface.co/datasets/kenji-tojo/fuzzy_dataset

## Setup

Enable GitHub Pages: *Settings -> Pages -> Source: Deploy from a branch -> `main` / `(root)`.

The page is a single dependency-free `index.html` — no jQuery, no webfonts, no build step;
all CSS is inline in `<style>`. Only `images/teaser.jpg` is loaded locally.

## Notes

- The paper and supplemental PDFs are served from the `paper` release, not from the repo tree
  (`uploads/*.pdf` is gitignored).
- `images/teaser.jpg` is 724 KB / 3106x650; consider downscaling for faster loads.
