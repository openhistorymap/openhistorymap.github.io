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

# Numeric bounds used to plot this edition as a band on the section's shared
# deep-time chart. Years are integers; BC is negative (753 BC → -753), and
# there is no year zero (AD 1 is 1). For an edition that spans all of history,
# use the chart's full range (-3500 to 2000). The plotted axis runs
# 3500 BC → AD 2000; "now" lives in the ongoing register.
era_from: 0
era_to: 0

# Set true for live, continuously-refreshed editions (present-day datasets or
# all-period harvests). These render in the "ongoing" register beneath the
# bounded historical editions, with a distinct band style.
ongoing: false

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

