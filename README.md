# Otipo Safaris

Website for Otipo Safaris, Premium Kenya Safari Tours & Wildlife Adventures.
Live site: https://seemaletoluo260-collab.github.io/Otipo-Safaris/

This repo holds the production build of the site (static HTML/CSS/JS plus media),
so any static host can serve it as-is.

## Structure

- `index.html`: entry page (SEO meta, Open Graph, JSON-LD)
- `assets/`: compiled JavaScript and CSS bundle
- `gallery/`: safari photos and the hero video
- `favicon.ico`, `robots.txt`, `placeholder.svg`

## Run locally

```bash
python -m http.server 8080
```

Then open http://localhost:8080

## Deploy

The site is published with **GitHub Pages** from the `main` branch (root folder).
Every push to `main` updates https://seemaletoluo260-collab.github.io/Otipo-Safaris/
within a minute or two.

Paths are relative, so the same files also work on a custom domain
(e.g. otiposafaris.com) or on Vercel / Netlify with no build step.
