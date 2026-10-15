# Favour John – Design Portfolio

Full-screen, scrollable graphic design portfolio for Favour John (Favz Graphix):
hero with scrolling work strips → about → services → nine selected projects → "More work"
gallery (filterable, 64 designs) → toolkit → process → contact. Light and dark themes follow the
visitor's system setting.

`index.html` holds all styles and scripts plus the selected-project images (inlined); the
"More work" gallery images live in `images/` as WebP (`name.webp` full size, `name-t.webp` thumbnail). There is nothing to build:
open `index.html` in a browser to view it locally.

## Adding a design

1. Export it as WebP twice: up to 1400 px on the long side (`my-design.webp`) and 560 px (`my-design-t.webp`), and put both in `images/`.
2. Copy one `<figure>` line in the `#gallery` section of `index.html`, change `data-full`, the `src`, the alt text and caption, and set `data-c` to `social`, `events`, `brand` or `print`.

## Publishing

`.github/workflows/pages.yml` deploys the site to GitHub Pages on every push to `main`.
One-time setup: **Settings → Pages → Source: GitHub Actions**. The site will then be at
`https://favzx-23.github.io/Favour-John/`.
