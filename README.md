# Patron Executive Dashboards

Public host for **The Patron Group's** executive-facing dashboards.

**Live site:** https://dadbod87.github.io/patron-executive-dashboards/

---

## What this repository is

This repository exists for **one purpose**: publishing executive dashboards to a
stable, bookmarkable public URL via GitHub Pages. The first dashboard is the
**Work Impact Dashboard** (served at the site root, `index.html`). Additional
executive dashboards may be added over time.

## What this repository is NOT

- It is **not** the source of truth. The dashboards are built and maintained in a
  **private** repository (Project Atlas); this repo only holds the *published copy*.
- It contains **no** Atlas documentation, memory, architecture, decisions,
  roadmap, source data, or internal notes — only the published dashboard HTML and
  this scaffolding.

## Do not edit here

`index.html` is **generated** — it is copied verbatim from the private source by an
allowlisted publish script and overwritten on every publish. Edit the dashboard in
the private Atlas repository and re-publish; changes made directly here will be lost.

## How updates happen

A publish script in the private repo copies **only** the dashboard HTML into this
repo as `index.html`, runs a safety scan, and pushes. Publishing is
**manual and approval-gated** — it never happens automatically. GitHub Pages then
redeploys the site at the URL above.

## Files

| File | Purpose |
|---|---|
| `index.html` | The published Work Impact Dashboard (generated — do not edit) |
| `.nojekyll` | Serve files as-is (skip Jekyll processing) |
| `robots.txt` | Discourage search-engine indexing of this internal-facing site |
| `README.md` | This file |
