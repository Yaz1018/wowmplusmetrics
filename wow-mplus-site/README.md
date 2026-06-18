# WoW Midnight Season 1 — Mythic+ Dashboards

Static, self-contained interactive dashboards. No build step, no server. Each HTML file works on its own; `index.html` is a landing page linking the two.

- `index.html` — landing page
- `dashboard.html` — all-roles class/spec performance
- `tanks.html` — weighted Tank Success Index (+12 to +18)
- `.nojekyll` — tells GitHub Pages to serve the files as-is

## Publish to GitHub Pages

Create an empty repo on GitHub first (no README), then from this folder:

```bash
git init
git add .
git commit -m "WoW Midnight S1 Mythic+ dashboards"
git branch -M main
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin main
```

Then in the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main`, folder: `/ (root)` → Save.**

After about a minute your site is live at:

```
https://<USERNAME>.github.io/<REPO>/
```

Direct links to share on Discord:
- Tank index: `https://<USERNAME>.github.io/<REPO>/tanks.html`
- Full breakdown: `https://<USERNAME>.github.io/<REPO>/dashboard.html`

## Notes

Data is a point-in-time snapshot (~June 2026); Mythic+ tuning shifts weekly. Methodology and sources are documented inside each dashboard.
