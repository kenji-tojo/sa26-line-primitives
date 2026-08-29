# Inverse Rendering for Modeling with Line Primitives

Project page for the SIGGRAPH Asia 2026 (ACM TOG) paper.

- Page: https://kenji-tojo.github.io/sa26-line-primitives/
- Code: https://github.com/kenji-tojo/inverse-line-primitives
- Dataset: https://huggingface.co/datasets/kenji-tojo/fuzzy_dataset

## Setup

Enable GitHub Pages: *Settings -> Pages -> Source: Deploy from a branch -> `main` / `(root)`.

`index.html` holds all the page's own CSS inline in `<style>` — no jQuery, no build step.
The only external stylesheet is a self-hosted copy of Font Awesome 5 Free
(`assets/css/fontawesome-all.min.css` + `assets/webfonts/`), used for the Resources icons,
taken from `kenji-tojo.github.io`. Nothing is loaded from a CDN.

## Notes

- The paper and supplemental PDFs are served from the `paper` release, not from the repo tree
  (`uploads/*.pdf` is gitignored).
- `images/teaser.jpg` is 724 KB / 3106x650; consider downscaling for faster loads.
- `assets/webfonts/` ships all formats (~2.8 MB). Browsers only ever fetch the `.woff2`,
  so the `.eot`/`.svg`/`.ttf` files can be deleted if you want a leaner repo.
