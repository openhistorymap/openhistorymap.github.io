---
title: "GeoContext Editor"
date: 2026-05-20
draft: false
category: "app"
language: "Svelte"
status: "beta"
repo: "https://github.com/openhistorymap/geocontext-app"
homepage: ""
download: "https://github.com/openhistorymap/geocontext-app/releases"
description: "Desktop editor for Geocontext repositories — a Tauri + SvelteKit app for building and curating gcx.json bundles and their datasets outside of QGIS."
---

A standalone desktop application — built with Tauri v2 and SvelteKit — for
working on Geocontext repositories directly, following the same `FORMAT.md` as
the [Geocontext Front-End](/tools/geocontext-front/).

Where the QGIS plugin captures a bundle from an existing GIS project and the
web front-end renders one for readers, the editor sits in between: open a
`gcx.json`, edit its manifest and datasets, and commit the result — no QGIS
session required.
