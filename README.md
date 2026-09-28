# commonblock.co

Static site for CommonBlock. No build step.

- `index.html` — the explainer page with the interactive model (self-contained; fonts load from Google Fonts).
- `docs/` — PDFs of the deck, white paper and State of Play, linked from the page.
- `CNAME` — custom domain for GitHub Pages.

## Deploy on GitHub Pages
1. Create a repo (e.g. `commonblock-site`) and upload every file in this folder to its root, including `CNAME` and `.nojekyll`.
2. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Settings → Pages → Custom domain: `commonblock.co`, then "Enforce HTTPS" once the certificate is issued.
4. At the DNS registrar: four A records for `commonblock.co` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153, and a CNAME record for `www` pointing to `<your-github-username>.github.io`.

## Updating
Replace `index.html` or the PDFs in `docs/` and commit. Keep the filenames in `docs/` the same so the links on the page keep working.
