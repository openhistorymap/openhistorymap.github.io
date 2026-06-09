---
title: "Tiles Archive"
date: 2026-05-06
draft: false
category: "cli"
language: "Python"
status: "active"
repo: "https://github.com/openhistorymap/tiles_archive"
homepage: ""
download: ""
description: "Builds per-time-partition PMTiles archives from the OHM tile store and publishes them to Cloudflare R2 — static, cacheable snapshots of the map for any time window."
---

The live [Tiles API](/tools/tiles-api/) generates tiles on demand; this tool
bakes them. It slices the data by time partition, writes each slice out as a
single-file PMTiles archive, and publishes the result to Cloudflare R2.

The payoff is static hosting: a PMTiles file on object storage serves a whole
time window straight to the client, no tile server in the loop — cheaper to
run and trivial to cache or mirror.
