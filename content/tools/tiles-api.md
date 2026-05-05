---
title: "Tiles API"
date: 2026-05-05
draft: false
category: "api"
language: "Python"
status: "active"
repo: "https://github.com/openhistorymap/tiles-api"
homepage: ""
download: ""
description: "Time-aware tile server — serves vector tiles indexed by space, time and thematic layer."
---

The tiles API is the server that backs the map. Standard XYZ tile servers
key tiles by `(z, x, y)`; OHM data also has a temporal axis, so the API
adds time-window filtering and per-layer grouping on top of the usual
spatial pyramid.

It is the longest-running piece of OHM-specific infrastructure and
underpins every map view we publish.
