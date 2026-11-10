# KATA — Concept Site

A single-page concept website for KATA (Dubai Mall Waterfront Promenade), built to
show what a dedicated site for the restaurant could look like. No build step —
`index.html` is a fully self-contained static page (fonts load from Google Fonts;
every photo is embedded directly in the file).

## Run locally

Just open `index.html` in a browser — no server or install needed.

## Deploy on Netlify

**Option A — connect this GitHub repo (recommended, auto-deploys on every push):**

1. Push this repo to GitHub (see below).
2. On [netlify.com](https://app.netlify.com), click **Add new site → Import an existing project**.
3. Pick this repository. Build settings are already set via `netlify.toml`
   (publish directory `.`, no build command needed) — just click **Deploy**.

**Option B — drag and drop (fastest, no GitHub needed):**

Go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag `index.html` onto
the page.

## Push this repo to GitHub

```bash
git init
git add .
git commit -m "KATA concept site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

(Create the empty repo on GitHub first at github.com/new — don't initialize it with a
README, since this folder already has one.)

## Notes

- Address, phone, hours, and Google rating were not provided for this one, so they
  were looked up (Tripadvisor + Google) rather than scraped from a Google Maps
  screenshot like the other prototypes — worth double-checking they're still current:
  Lower Ground Floor, Fashion Avenue, Dubai Mall Waterfront Promenade · 054 582 9933 ·
  4.7★ (1,019 Google reviews) · Mon–Thu 10am–12am, Fri–Sun 10am–1am.
- The in-store menu photos captured were only 140px wide and not legible. The menu on
  this page is built from the real named dish photos you provided (Ramen, Salmon
  Teriyaki, Wagyu Sliders, etc.) plus the category headers that were readable and one
  confirmed signature dish (Popcorn Shrimp, mentioned in public reviews). Confirm items
  and pricing against the current KATA menu before sharing this externally.
- Source photos used to build the page are kept locally but excluded from git via
  `.gitignore` (already baked into `index.html` as compressed images).
