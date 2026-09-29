# commonblock.co

Static site for CommonBlock. No build step.

- `index.html` — the homepage.
- `deck.html` — the overview deck (links from the homepage's "Deck" / "View the deck").
- `white-paper.html` — the white paper (links from "White paper" / "Read the white paper").
- `CNAME` — custom domain for GitHub Pages.
- `.nojekyll` — tells GitHub Pages to serve files as-is.

Each page is a self-contained bundle (fonts and scripts embedded); it needs JavaScript to display.

## Deploy on GitHub Pages
1. Upload every file in this folder to the repo root, including `CNAME` and `.nojekyll`.
2. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Settings → Pages → Custom domain: `commonblock.co`, then "Enforce HTTPS" once the certificate is issued.
4. At the DNS registrar: four A records for `commonblock.co` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153, and a CNAME record for `www` pointing to `<your-github-username>.github.io`.

## Updating
Replace a page and commit. Keep the filenames the same so the links between pages keep working.
