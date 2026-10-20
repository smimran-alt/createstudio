# CreateStudio — Free design platform MVP

A responsive, original design platform inspired by the *category* of online brand-design products (not a copy of their source code, trademarks, or paid templates).

## Included (working now)
- Homepage and category browsing
- 6 starting compositions each for logo, business card, social post and flyer (24 category/template combinations)
- Editable name, tagline, color palette, background/text/accent colors, graphic motif and font category
- Live vector preview
- Free, watermark-free SVG and 2× PNG export
- Saved designs in browser `localStorage` (up to 50; no cross-device syncing)
- Mobile-friendly layout, no accounts, API keys, paid plugins or build tools

## Deploy on GitHub Pages (free)
1. Create a **public** repository on GitHub (for example `createstudio`).
2. Upload `index.html`, `styles.css` and `app.js` **to the root** of the repository. Do not upload the ZIP as a single file.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**; choose `main` and `/(root)`, then **Save**.
5. When GitHub finishes publishing, your site will be at `https://YOUR-USERNAME.github.io/createstudio/` (substitute exact username/repository casing).
6. To update the site, edit and commit the files. Your published site updates after the Pages deployment completes.

## Run locally
Double-click `index.html` to open in a browser, or run `python -m http.server 8000` here and open `http://localhost:8000`.

## Known limitations / next milestones
- Not AI generated: current designs are programmable SVG templates. True AI image generation needs a model/service and appropriate compute.
- No user registration, shared cloud gallery, checkout or website publishing; all are future phases.
- Saved designs exist **only in the browser** on this device. Export SVG to preserve the artwork.
- SVG text remains text rather than outlined paths; font fallback may vary on different devices.
- For business-card production printing, add bleed, trim and PDF/CMYK workflows in a future phase.
- The downloadable PNG has a background; transparent background export is not implemented yet.

## Security & publishing notes
No secrets should ever be committed to GitHub Pages JavaScript. When backend features are added, use server-side secrets and appropriate authentication, rate limits, data handling and storage access rules.

## Project tree
```
createstudio/
  index.html
  styles.css
  app.js
  README.md
```
