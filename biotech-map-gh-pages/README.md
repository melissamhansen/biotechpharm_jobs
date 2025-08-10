# Biotech Map (GitHub Pages)

This folder is ready to publish your R `leaflet` map with **GitHub Pages**.

## Quick publish (2 minutes)

1. In your R script, make sure you save your map as:
   ```r
   saveWidget(map, file = "geocoded_map.html", selfcontained = TRUE)
   ```

2. Download this zip and unzip it locally. Copy **your** `geocoded_map.html` into the unzipped folder (same level as `index.html`).

3. Create a new public GitHub repo, e.g., `biotech-map`.
   - Upload all files from this folder (including `.nojekyll`, `index.html`, `404.html`, and your `geocoded_map.html`).

4. Enable Pages:
   - Go to **Settings → Pages**.
   - **Source:** `Deploy from a branch`.
   - **Branch:** `main` and **/ (root)**. Save.

5. Your site will be live in ~30–60 seconds at:
   - `https://<your-username>.github.io/<repo-name>/`

   The `index.html` redirects to `geocoded_map.html` automatically.

## Notes
- Because `selfcontained = TRUE`, a single file is enough.
- If your map doesn't load on Pages, double-check that `geocoded_map.html` is in the repo root (not inside a subfolder).
- The blank `.nojekyll` file tells GitHub Pages not to try to process assets.

Enjoy!
