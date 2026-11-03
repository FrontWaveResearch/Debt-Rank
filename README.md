# Front Wave Debt Review

Static site: `index.html` + `league.json` (effective cost of debt from FY exchange filings of 1,343 listed Indian companies, pulled 30 Oct 2026, with data-quality flags).

A CFO can (1) search a listed company, (2) enter a few numbers, or (3) upload/paste a loan schedule from Excel.
The review shows: cost position vs clean comparables, fair rate, named cheaper peers, 12-month runway/funding gap,
and an indicative before/after if Front Wave aggregates and refinances the book. All computation is in the browser.

## Deploy on GitHub Pages
1. Create a public repository (e.g. `debt-review`).
2. Upload `index.html` and `league.json` to the root; commit.
3. Settings -> Pages -> Source "Deploy from a branch" -> main / root -> Save. Live in ~2 min at https://<user>.github.io/<repo>/.

## Wire the contact buttons
In `index.html`, find near the top of the script:
    const DESK={site:"https://frontwaveresearch.com",email:"",whatsapp:""};
Add the desk email and WhatsApp number (digits with country code, e.g. "9198xxxxxxxx").
With whatsapp set, a "WhatsApp the desk" button sends the visitor's full review text to that number.

## Updating the data
Replace `league.json` with a fresh pull and commit; keep the PULLED constant in index.html in sync.
