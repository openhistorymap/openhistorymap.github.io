---
title: "HGTFS — Historical General Transit Feed Specification"
date: 2026-05-05
draft: false
category: "spec"
language: ""
status: "active"
repo: "https://github.com/hgtfs"
homepage: "https://hgtfs.github.io"
download: ""
description: "A GTFS-based specification for historical transit networks: stops, routes, edges and operators with explicit time-of-validity (date_opened / date_closed), honest date uncertainty, a network graph, and historical-context events."
---

GTFS describes today's transit networks; HGTFS is the equivalent for
*historical* ones. Every stop, route, network edge and operator carries an
explicit time-of-validity, so a network can be reconstructed for any chosen
date — and where the historical record is uncertain, the dates say so
(`date_opened` bounded by min/max, closures asserted only on evidence).

The specification is developed in the open at
**[hgtfs.github.io](https://hgtfs.github.io)** — a full field reference plus a
time-aware web **[viewer](https://hgtfs.github.io/viewer/)** that scrubs a feed
through time and recolours the network as operators change. It grew out of the
earlier, archived [openhistorymap/HTFS](https://github.com/openhistorymap/HTFS)
draft and is the basis for transit layers inside OHM.
