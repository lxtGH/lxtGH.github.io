# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A personal academic homepage for **Xiangtai Li** built on Jekyll, forked from `RayeRen/acad-homepage.github.io`. Deployed via GitHub Pages from the `main` branch at `lxtGH.github.io`. Day-to-day edits are content updates (publications, news, intro), not framework changes.

## Local development

Requires Ruby + Bundler (Jekyll's GitHub Pages stack).

```bash
bundle install              # one-time, installs github-pages gem
bash run_server.sh          # = bundle exec jekyll serve
```

Server runs on port `4001` (set in `_config.yml`, not the Jekyll default 4000 — the README is wrong about this). Livereload picks up edits to `_pages/**`, `_includes/**`, `_sass/**`, and `assets/**` automatically. **`_config.yml` changes require a server restart.**

## Where content lives

The site is rendered from a single page (`_pages/about.md`) that `include_relative`s four content fragments — these are the files you almost always edit:

- `_pages/includes/intro.md` — bio, role, research interests, contact / hiring blurbs.
- `_pages/includes/news.md` — recent news (currently empty).
- `_pages/includes/pubs.md` — publication list. Hand-authored `<li>` entries with `<strong>` for the author's name, a colored `<span>` venue/highlight tag, and trailing `<a>` links for code/project pages. Match this structure when adding new entries.
- `_pages/includes/others.md` — honors, awards, and other tail sections.

Project landing pages live under `project/<name>/index.html` (e.g. `project/sa2va/`, `project/omg_seg/`) and are linked to from `pubs.md`.

Site-wide layout lives in `_layouts/default.html` + `_includes/` (masthead, sidebar, author profile, SEO, analytics). Styling is SCSS under `_sass/`. Touching these is rare — prefer content edits unless the user explicitly asks for a layout/style change.

## Google Scholar citation pipeline

Per-paper citation counts are injected client-side, not at build time:

1. `.github/workflows/google_scholar_crawler.yaml` runs `google_scholar_crawler/main.py` daily (08:00 UTC) and on `page_build`. It uses the `GOOGLE_SCHOLAR_ID` repo secret and force-pushes `gs_data.json` + `gs_data_shieldsio.json` to a separate `google-scholar-stats` branch.
2. `_includes/fetch_google_scholar_stats.html` fetches that JSON via jsDelivr CDN (`site.google_scholar_stats_use_cdn: true` in `_config.yml`) and fills any element with class `show_paper_citations`, using its `data` attribute as the Google Scholar paper ID (`citation_for_view=...`).

To show a paper's citation count anywhere in markdown:
```html
<span class='show_paper_citations' data='SCHOLAR_PAPER_ID'></span>
```

The crawler script and `google_scholar_crawler/` are excluded from the Jekyll build (see `exclude:` in `_config.yml`).

## Conventions when editing pubs.md

- `<strong>Xiangtai Li</strong>` is always bolded in author lists; co-first authors get a trailing `*`, with `\* means equal contribution.` noted at the top of the file.
- Venue tags follow the form `<strong>[VENUE-YEAR]<span style="color:red"> one-line highlight </span> </strong>`.
- Trailing links are plain `<a href="...">Code</a>` / `Project Page` / `Model and Data`, separated by spaces (not pipes inside the `<li>`).
- New "Recent Works" go to the top of that section; older ones drop into "Several Other Previous works".
