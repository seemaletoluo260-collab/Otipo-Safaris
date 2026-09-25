# Otipo Safaris

Website for Otipo Safaris, Premium Kenya Safari Tours & Wildlife Adventures.
Migrated from https://otiposafaris.lovable.app

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

The site uses absolute paths (`/assets/...`, `/gallery/...`), so it must be served
from the domain root, for example:

- **Vercel / Netlify / Cloudflare Pages**: import this repo, no build command, output directory `.`
- **GitHub Pages**: works only with a custom domain (e.g. otiposafaris.com), not at `/Otipo-Safaris/`

`vercel.json` and `_redirects` send unknown routes to `index.html` (SPA fallback).
