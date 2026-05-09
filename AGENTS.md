# AGENTS.md

## Repo shape
- This repo is a plain static site for GitHub Pages. There is no package manager, build step, test runner, or CI config.
- The live site is served directly from root files: `index.html`, `styles.css`, `script.js`, and the profile image in the repo root.

## GitHub Pages constraints
- This repo is a project site, not a `username.github.io` site. The published URL is `https://toei-piyamon.github.io/Toei_Web/`.
- Keep asset references relative, such as `./styles.css`, `./script.js`, and `./image.jpg`. Do not switch them to root-absolute paths like `/styles.css`, or the site will break under `/Toei_Web/`.

## Editing notes
- Main content and section structure live in `index.html`.
- All styling is in `styles.css`; the visual language is a light modern pastel theme with rounded cards and soft gradients.
- `script.js` is intentionally tiny and only handles nav-link active state on click.
- The current profile image filename contains spaces and is URL-encoded in `index.html` as `./LINE_ALBUM_Shanghai-Beijing%2015-22112025_260509_1.jpg`. If you rename or move the image, update the `src` exactly.

## Verification
- There is no automated verification in this repo.
- Best check is to open `index.html` in a browser and confirm the layout, anchor navigation, and image path still work.

## Deploy
- Push changes to `main`.
- GitHub Pages should be configured as `Deploy from a branch` using `main` and `/ (root)`.
