---
title: "Index API"
date: 2026-05-17
draft: false
category: "api"
language: "Python"
status: "active"
repo: "https://github.com/openhistorymap/ohm-index-api"
homepage: "https://index.openhistorymap.org"
download: ""
description: "Back-end for the OHM data index — a Zotero connector that turns the curated Zotero library into the searchable index of sources behind index.openhistorymap.org."
---

OHM's sources live in Zotero, tagged with `ohm:*` descriptors by the
[Zotero plugin](/tools/ohm-zotero/). This API is what turns that library into
a public, queryable index: it connects to Zotero, reads the curated items and
their descriptors, and serves them as the searchable catalogue behind
`index.openhistorymap.org`.

Pair it with the [Index Front-End](/tools/ohm-index-front/) for the browser
side of the same service.
