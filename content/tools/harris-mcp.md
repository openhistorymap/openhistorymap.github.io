---
title: "Harris MCP"
date: 2026-05-18
draft: false
category: "api"
language: "Python"
status: "active"
repo: "https://github.com/openhistorymap/harris-mcp"
homepage: ""
download: ""
description: "A Model Context Protocol server for reading and auditably editing Harris matrices — archaeological stratigraphy — with a changelog-backed write surface."
---

The Harris matrix is how archaeologists record stratigraphy: the ordered
relationships between the layers and cuts of an excavation. `harris-mcp`
exposes those matrices to LLM agents through the Model Context Protocol, with
adapters for the common interchange formats — HMDP, CSV, XLSX and HMC/HMCX.

The read surface is tuned for language models; the write surface is
changelog-backed, so every edit an agent makes is auditable and reversible.
Corpus-level tools let it reason across a whole set of documents at once.
