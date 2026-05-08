---
title: "Natural-Language Control for Molstar"
slug: molstar-llm-control
lead: "Drive the Molstar molecular viewer with chat — generate MolViewSpec scenes (and, as a stretch, MolViewStories) from plain-English requests."
theme: "Visualization & AI agents"
lead_author: ""
lead_affiliation: ""
repo: ""
team: []
---

## Why this project

[Molstar](https://molstar.szbl.ac.cn/viewer/) is a powerful viewer, but
its full configuration surface (representations, selections, colors,
camera) is hard to discover. A chat layer that compiles user intent into
**MolViewSpec** would make the tool more accessible — and a natural fit
for AI-assisted exploration of molecular structures.

## What a team could build in one day

A chatbot front-end (hosted on AWS, backed by Qwen, Ollama, or an existing
Claude / OpenAI account) that:

- Accepts plain-language requests like "show the binding pocket as
  surface, color by hydrophobicity, hide waters."
- Generates a corresponding MolViewSpec configuration.
- Loads it into a live Molstar viewer.

Minimum viable demo: a working round-trip where a user describes a scene
and Molstar reflects the requested view.

## Stretch directions

- Extend to **MolViewStories** for interactive, multi-step narratives.
- Suggest improvements ("would you like to also highlight the active
  site?") based on the loaded structure.
- Library of saved prompt → scene templates for teaching.
