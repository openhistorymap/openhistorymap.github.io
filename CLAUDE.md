# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

The Hugo source for the Open History Map institutional site (`www.openhistorymap.org`, served via GitHub Pages from the `gh-pages` branch). Content authoring + light layout customization on top of the `ananke` theme. There is no application code, no test suite, no linter — changes are content (`content/**/*.md`) or template tweaks (`layouts/`).

The "real" OpenHistoryMap apps live on other subdomains referenced from `config.toml` (`map.`, `index.`, `blog.openhistorymap.org`); this repo does not contain them.

## Commands

- `hugo server -D` — local preview with drafts.
- `hugo --minify` — production build into `public/` (matches CI exactly).
- `hugo new conference/<slug>.md` — scaffold from `archetypes/conference.md`. Same pattern for `paper`, `event`, `post`.
- First-time clone: `git submodule update --init --recursive` (the `ananke` theme is a submodule; the `dimension` submodule listed in `.gitmodules` points at a placeholder URL and is not actually used).

Hugo **extended** is required (matches `peaceiris/actions-hugo@v2` with `extended: true`).

## Deploy

`.github/workflows/gh-pages.yml` runs on push to `master`: checkout with submodules → `hugo --minify` → publish `public/` via `peaceiris/actions-gh-pages@v3`. There is no staging — merging to `master` is the deploy. The committed `public/` directory is a leftover artifact and is not what gets served.

## Content architecture

Custom sections beyond Hugo defaults: `conference`, `paper`, `event`, `tech`. Each non-`tech` section has its own archetype in `archetypes/` and matching templates in `layouts/<section>/` (`list.html`, `single.html`, `summary.html`, `summary-with-image.html`). When adding a new section, mirror that quartet or it will fall back to ananke defaults.

`layouts/index.html` drives the homepage feed off `Site.Params.mainSections` (defaults to `conference` — see `config.toml`'s commented-out `mainSections` if a switch is needed). `recent_posts_number` in `[params]` controls how many summary cards appear before the "more" list.

`config.toml` is the single source of truth for the top nav (`[[menu.main]]` entries link out to the sibling subdomains) and for ananke theme params (logo, social links, color classes from Tachyons).

`static/CNAME` pins the custom domain — do not delete or rename when editing files in `static/`.

## Design

Design context lives in `.impeccable.md` (root). Read it before any visual or template work. Short version: cartographic / surveyor register for an academic-DH audience; Bagnard + Hanken Grotesk + PT Mono; warm-paper light theme with a dark counterpart via `light-dark()`; terracotta accent used sparingly. Anti-references include the current ananke skin — replace, don't iterate.
