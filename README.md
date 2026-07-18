# Arpita Saha — Portfolio

A single-page, responsive portfolio site for Arpita Saha (Molecular Biology, Bioinformatics & Pharmacology research profile).

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The site — markup, styles, and layout in one self-contained file. |
| `arpita.jpeg` | Profile photo, referenced by `index.html`. Keep the filename as-is or update the `<img src>` in the hero section if you rename it. |
| `arpita.md` | Source content (education, experience, certifications, references) that the site is built from. Edit this first when updating info, then mirror the change into `index.html`. |

## Running locally

No build step or dependencies — it's plain HTML/CSS.

**Quickest:** double-click `index.html` to open it directly in a browser.

**With a local server** (recommended, avoids any `file://` quirks):

```bash
npx serve .
```

Then open the URL it prints (e.g. `http://localhost:3000`).

## Structure

The page is a single scrolling document with a sticky top navigation bar linking to each section:

- **About** — research focus summary
- **Education** — degrees, in reverse chronological order
- **Experience** — internship / research roles
- **Skills** — instrumental, compliance, wet-lab, and QA/QC competencies
- **Certifications** — training courses and awarded certificates
- **Contact** — email CTA and academic references

Navigation collapses into a hamburger menu below 760px; layout further adapts at 620px and 420px breakpoints for tablet and mobile.

## Customizing

- **Content:** edit the relevant `<section>` in `index.html` directly.
- **Colors:** all colors are CSS custom properties defined in `:root` at the top of the `<style>` block, with a dark-mode override under `@media (prefers-color-scheme: dark)`.
- **Photo:** replace `arpita.jpeg` with a new image of the same filename, or update the `src` attribute in the `.portrait img` element.

## Deploying

The site is fully static, so it can be published as-is to any static host (GitHub Pages, Netlify, Vercel, etc.) — just upload `index.html` and `arpita.jpeg` together.
