# Patent Publication Companion Site

This repository contains a plain HTML, CSS, and JavaScript GitHub Pages site for a patent publication companion page centered on deterministic gather over logically managed live inference state.

The site is intentionally restrained and technical. It is designed to read like a serious architecture publication page rather than a startup landing page or generic product site.

## Included Files

```text
/
  index.html
  styles.css
  script.js
  robots.txt
  sitemap.xml
  README.md
  .nojekyll
```

Expected asset paths:

```text
/assets/patent.pdf
/assets/architecture-overview.svg
/assets/gather-flow.svg
/assets/figures/...
/assets/favicon.svg
```

## What the Site Presents

The homepage is organized into these sections:

1. Overview / Hero
2. Problem
3. Core Invention
4. Why Deterministic Gather Matters
5. Architecture
6. Why It Matters
7. Differentiation
8. Method / Execution Flow
9. Artifacts
10. Contact
11. Footer

## Metadata and Status Editing

The publication metadata is intentionally easy to edit directly in `index.html`.

Look for the metadata grid in the hero and update fields such as:

- `Status`
- `Jurisdiction`
- `Publication / Filing Type`
- `Year`
- `Domain`
- `Category`

Suggested edits:

- replace `[Jurisdiction]` with the actual jurisdiction
- update the publication wording to match the actual record
- update the year if needed

## Contact Placeholder Editing

The contact section uses deliberate editable placeholders instead of fake live data.

In `index.html`, replace:

- `[professional-email@example.com]`
- `[GitHub repository link]`

The contact section is intentionally presented as a professional reference block rather than a call-to-action panel.

## Asset Placement

Place the real publication files here:

```text
/assets
  patent.pdf
  architecture-overview.svg
  gather-flow.svg
  favicon.svg
  /figures
```

Recommended usage:

- `patent.pdf`: published patent or published application PDF
- `architecture-overview.svg`: primary architecture figure
- `gather-flow.svg`: execution flow or gather-path figure
- `favicon.svg`: small square favicon
- `figures/`: supplemental figure set

## GitHub Pages Deployment

This site requires no framework and no build step.

### Branch-based Pages deployment

1. Push the repository to GitHub.
2. Open `Settings` -> `Pages`.
3. Under `Build and deployment`, choose:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
4. Save.

### Optional GitHub Actions deployment

The site also works with GitHub Actions Pages workflows, but Actions are not required for normal deployment.

## Why `.nojekyll` Is Included

GitHub Pages can run Jekyll automatically. This project is plain static hosting and does not require Jekyll. The `.nojekyll` file ensures the site is served directly without Jekyll processing.

## SEO / Crawlability

The site includes:

- `robots.txt`
- `sitemap.xml`
- canonical metadata
- Open Graph metadata
- Twitter card metadata

If you later change the domain or move the repo, update:

- canonical URL in `index.html`
- Open Graph and Twitter image URLs in `index.html`
- `sitemap.xml`
- `robots.txt`

## Customization Notes

### Repo and artifact links

Update these links in `index.html` as needed:

- `./assets/patent.pdf`
- `./assets/architecture-overview.svg`
- `./assets/gather-flow.svg`
- `./assets/figures/`
- repository URLs

### Typography and color system

Edit theme variables at the top of `styles.css` to customize:

- background tones
- card surfaces
- text colors
- accent color
- line colors
- shadows and radius values

The current typography uses:

- `IBM Plex Sans` for body text
- `Fraunces` for headings

### JavaScript behavior

`script.js` is intentionally minimal. It handles:

- reveal-on-scroll
- active navigation highlighting
- footer year update

The core page content remains fully readable without JavaScript.

## Publishing Checklist

Before sharing publicly:

- replace the asset placeholders with real files
- replace the contact placeholders
- confirm metadata wording against the actual publication record
- confirm the repository URL
- confirm the GitHub Pages URL

## Design Intent

This site is intended to feel like a publication-grade architecture microsite for a serious systems patent.

It is deliberately:

- dark
- restrained
- technical
- diagram-friendly
- engineer-readable
- framework-free

It is deliberately not:

- a startup landing page
- a pricing page
- a generic portfolio
- a marketing-heavy product site


