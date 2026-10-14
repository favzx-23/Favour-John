# Favour John – Design Portfolio

Full-screen, scrollable graphic design portfolio for Favour John (Favz Graphix):
cover → about → seven featured projects → logofolio → filterable design gallery → skills → contact.

`index.html` holds all styles and scripts; artwork lives in `images/` as WebP
(`name.webp` full size, `name-t.webp` thumbnail). There is nothing to build:
open `index.html` in a browser to view it locally.

## Adding a design

1. Export it as WebP twice: up to 1400 px on the long side (`my-design.webp`) and 560 px (`my-design-t.webp`), and put both in `images/`.
2. Copy one `<figure>` line in the gallery section of `index.html`, change `data-img`, the `src`, the alt text and caption, and set `data-c` to `social`, `events` or `print`.

## Publishing

`.github/workflows/pages.yml` deploys the site to GitHub Pages on every push to `main`.
One-time setup: **Settings → Pages → Source: GitHub Actions**. The site will then be at
`https://favzx-23.github.io/Favour-John/`.
