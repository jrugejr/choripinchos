# Choripinchos — Mismo sabor. Menos trabajo. Más brasas.

A bilingual (English / Español), offline-ready progressive web app for making **Choripinchos**: Colombian-inspired, kabob-style chorizo made from a seasoned beef mixture shaped onto wide flat skewers and grilled over charcoal.

## Features

- Scale recipes by number of skewers or meat-and-fat weight.
- Adjust lean/fat ratio and hand-diced versus coarse-ground portions.
- Editable seasonings, measured in grams per kilogram of meat/fat.
- Practical shopping estimates (pounds/ounces, garlic cloves, scallion stalks/bunches, pantry spoon equivalents).
- Grocery checklist, recipe copy and batch notes.
- Local-only saved batches; no account or backend.
- Installable PWA using a service worker and manifest.

## Publish on GitHub Pages

Open **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/(root)**, then save. Your eventual URL should be `https://jrugejr.github.io/choripinchos/`.

PWA installation and offline support need HTTPS, which GitHub Pages provides. The service worker caches all local app assets after the first online visit. Google Fonts are decorative and not required for offline functionality.

## Notes on measurements

The default recipe is an *experimental starting point*, not a verified family recipe. Meat/fat values refer to **trimmed lean meat + separately measured raw beef fat**; account for fat in store-bought ground beef. The calculator targets approximate finished raw mixture weight when scaling by count, accounting for ingredient additions; actual yields vary. Produce counts and spoons are estimates, not substitutes for weighing salt or additives. Trimmed produce yields and market package sizes vary.

Food safety: treat as raw fresh sausage. Keep refrigerated at or below 40°F / 4°C; cook or freeze within 1–2 days; cook to an internal temperature of **160°F / 71°C**. Do not attempt uncontrolled fermentation/drying.

## Development

Pure HTML/CSS/vanilla JS: serve the directory over HTTP(S), e.g. `python -m http.server 8080`. PWA installation requires `localhost` or HTTPS.

Licensed under MIT (see LICENSE).
