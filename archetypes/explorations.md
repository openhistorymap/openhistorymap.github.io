---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true

# What kind of exploration this is. Free-form, but stick to a small vocabulary
# so the listing reads consistently:
#   atlas · map · gallery · timeline · street view
category: "atlas"

# Temporal (or spatial) scope, set in the meta register. Free text, kept short:
#   "753 BC → AD 476" · "Antiquity → 18th c." · "1914 → 1918" · "Present day"
coverage: ""

# Where the data comes from. Rendered as small badges:
#   Wikidata · Wikipedia · OpenStreetMap · THOR · …
sources: []

# Maturity. One of: active · beta · experimental · archived
status: "active"

# The live site — these are public-facing data editions, so this is the
# primary call to action. Required for anything to show up as an exploration.
homepage: ""

# Where the source lives. Optional but encouraged.
repo: ""

# Optional one-line subtitle. Falls back to the description.
description: ""
---

