# Wiretex demo website
Static site (HTML, CSS, JavaScript) that works on GitHub Pages. No build step.

## Publish on GitHub Pages
1. Create a repo and upload the **contents** of this folder (not the folder itself). Keep `.nojekyll` and `images/.gitkeep`. Hidden files are skipped by drag-and-drop, so use `git add .` or add `.nojekyll` via *Add file → Create new file*.
2. Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
3. After a minute the site is live at `https://<user>.github.io/<repo>/`. All links are relative, so it works in a project subfolder too.
4. Custom domain: add it under Settings → Pages (GitHub creates a `CNAME` file).

## Make it theirs
- **Contact details:** open `app.js`, fill `CONFIG` at the top (`phone`, `whatsapp` e.g. `2547XXXXXXXX`, `email`, `location`). Empty items stay hidden. Quote requests are sent to WhatsApp, or email if no WhatsApp is set.
- **Products and text:** edit the lists (`PRODUCTS`, `FAQ`, `STEPS`, `WHY`, `APPS`) in `app.js`. The copy is sample industry text; replace it with Wiretex's real specifications, sizes and standards before launch.
- **Photos:** product art is drawn in code. To use real photos, add files to `images/` named `product1.jpg` … `product11.jpg` (in the order of the product list) and `gabion1.jpg`, `gabion2.jpg`, `gabion3.jpg`. They appear automatically over the drawings.
- **Colours:** variables at the top of `styles.css`.

## Features
Product range with filters, quote list (persisted in the browser), gabion calculator, gabion comparison table, applications, process, FAQ, quote form, mobile menu.
