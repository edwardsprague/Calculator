[README.md](https://github.com/user-attachments/files/32938441/README.md)
# Calculator# Deal Analyzer — Ironheart Commercial

A self-contained, single-file real estate deal analysis tool. No build step, no dependencies, no backend — it's one `index.html` file with everything (HTML, CSS, and JavaScript) inline.

## What's inside

| # | Tab | Covers |
|---|-----|--------|
| 00 | Cap Rate Calculator | NOI, cap rate, reverse valuation |
| 01 | Purchase & Hold | IRR, DSCR, cash-on-cash, year-by-year cash flow |
| 02 | Discounted Purchase | Below-market / distressed acquisitions with rehab |
| 03 | Fix & Flip | Project cost, profit, ROI, annualized ROI |
| 04 | Portfolio | Rollup across all current holdings |
| 05 | Property Comparison | Side-by-side underwriting on competing targets |
| 06 | Retirement | Years to replace a target passive income |
| 07 | Settlement Statement | Buyer/seller debits & credits, AZ arrears tax proration |
| 08 | Seller Carry | Amortization, balloon, early note-sale discounting |
| 09 | Multifamily Underwriting | Full 13-module underwriting & prospecting suite |

Data you enter in the Portfolio, Compare, unit mix, and comps tables is saved to **your own browser's local storage** — it's per-device/per-browser, not shared across your team, and nothing is sent to a server.

## How to host this on GitHub Pages

1. Create a new repo (or use an existing one) and add this `index.html` to the root (or to a `/docs` folder — your choice).
2. Commit and push:
   ```bash
   git add index.html README.md
   git commit -m "Add Deal Analyzer tool"
   git push
   ```
3. In the repo: **Settings → Pages** → under "Build and deployment," set **Source** to "Deploy from a branch," pick your branch (e.g. `main`) and the folder (`/root` or `/docs`), then save.
4. GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/` — that's your live, shareable link. It updates automatically every time you push a new `index.html`.

## How to just run it locally (no GitHub needed)

Double-click `index.html`, or drag it into any browser window. Works fully offline except for loading the two Google Fonts (Fraunces, IBM Plex Sans/Mono) — if those fail to load, the tool still works, it just falls back to system fonts.

## Making changes

Everything lives in the one file — there's no separate CSS or JS file to track down. Search for the relevant tab's HTML `<section class="panel" id="panel-...">` block to find its fields, and its matching `function calc...()` further down in the `<script>` tag to find its math.
