---
title: "Geocontext QGIS Plugin"
date: 2026-04-28
draft: false
category: "plugin"
language: "Python"
status: "active"
repo: "https://github.com/openhistorymap/geocontext-qgis"
homepage: ""
download: "https://github.com/openhistorymap/geocontext-qgis/releases"
description: "QGIS plugin that exports the current map view as a Geocontext bundle (gcx.json + GeoJSON datasets) and pushes it to a GitHub repository."
---

A QGIS plugin aimed at researchers who already work in QGIS and want to
publish a slice of their project as an open, shareable bundle.

The plugin captures the current view — extents, layers and selected
datasets — and writes them out as a `gcx.json` manifest plus
`datasets/*.geojson`, then optionally pushes the result to a GitHub
repository via the system `git`. The matching front-end (see
*Geocontext Front-End*) renders these bundles back to a browser.
