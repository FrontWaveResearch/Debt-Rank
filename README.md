# Front Wave Debt Rank

A static page: `index.html` + `league.json` (effective cost of debt computed from FY exchange filings of 1,364 listed Indian companies, pulled 29 Oct 2026).

## Deploy on GitHub Pages
1. Create a new public repository (e.g. `debt-rank`).
2. Upload `index.html` and `league.json` to the repository root and commit.
3. Settings -> Pages -> Source: "Deploy from a branch" -> Branch: `main`, folder `/ (root)` -> Save.
4. After ~1-2 minutes the site is live at `https://<username>.github.io/debt-rank/`.

## Custom domain (optional)
In Settings -> Pages add e.g. `debtrank.frontwaveresearch.com`; at your DNS, add a CNAME record pointing that subdomain to `<username>.github.io`; tick "Enforce HTTPS".

## Updating the data
Replace `league.json` with a fresh pull and commit - nothing else changes. Keep the "pulled" date in index.html's PULLED constant in sync.
