---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true

# What kind of artifact this is. Free-form, but stick to a small vocabulary
# so the listing reads consistently:
#   app · api · library · plugin · extension · spec · stack · dataset · cli
category: "app"

# Implementation language (single string, used as a small badge in the listing).
language: ""

# Maturity. One of: stable · active · beta · experimental · archived
status: "active"

# Where the source lives. Required for anything to show up as a tool.
repo: ""

# Where it runs / is documented (live URL). Optional.
homepage: ""

# Where to download or install (release page, marketplace, package, etc.). Optional.
download: ""

# Optional one-line subtitle. Falls back to the description.
description: ""
---

