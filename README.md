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

- The reconstruction viewer is self-contained in `index.html` (inline CSS and JavaScript).
  It uses the following captures; each row needs `<scene>_gt_<photo>.png`,
  `<scene>_<photo>.png`, and `<scene>_view<view>_25.png` from `images/capture_results/`.
  Scenes are listed alphabetically, with Cactus 1 selected initially.
  The photo/view mappings are embedded in the script; the original `images/views/`
  JSON files are not needed to serve the page.

  | Scene | Photo | View |
  | --- | --- | --- |
  | cactus1 | P6A1794 | 1 |
  | cactus2 | P6A1046 | 1 |
  | dinosaur | P6A1540 | 2 |
  | flowers | P6A1147 | 1 |
  | fur | P6A1649 | 1 |
  | kiwi | P6A1291 | 1 |
  | tawashi | P6A1406 | 2 |
  | textiles | P6A1978 | 1 |

- The paper and supplemental PDFs are served from the `paper` release, not from the repo tree
  (`uploads/*.pdf` is gitignored).
- `images/teaser.jpg` is 724 KB / 3106x650; consider downscaling for faster loads.
- `assets/webfonts/` ships all formats (~2.8 MB). Browsers only ever fetch the `.woff2`,
  so the `.eot`/`.svg`/`.ttf` files can be deleted if you want a leaner repo.
