---
title: "Tiles API (Rust)"
date: 2026-05-12
draft: false
category: "api"
language: "Rust"
status: "beta"
repo: "https://github.com/openhistorymap/tileserver_rust"
homepage: ""
download: ""
description: "A read-only Rust port of the OHM vector-tile API — axum, deadpool-postgres and MVT — built to serve the same time-aware tiles with a smaller footprint."
---

A reimplementation of the [Tiles API](/tools/tiles-api/) in Rust: same
time-, space- and layer-aware vector tiles, served read-only through `axum`
over a `deadpool-postgres` connection pool, emitting standard MVT.

The goal is the same contract as the Python server at a lower resource cost —
a drop-in tile back-end for high-traffic or constrained deployments. It is the
newer of the two and still being hardened against the original.
