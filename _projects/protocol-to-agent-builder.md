---
title: "Protocol-to-Agent Builder"
slug: protocol-to-agent-builder
lead: "Turn any protocol — wet-lab SOP, microscopy workflow, computational pipeline — into a grounded, queryable assistant that can answer practical execution questions and produce checklists."
theme: "Research tooling & AI agents"
lead_author: ""
lead_affiliation: ""
repo: ""
team: []
---

## Why this project

Protocols at Scripps live as PDFs, methods sections, SOPs, and slide
decks — formats that aren't structured for an agent to reason over.
Lifting them into a structured, queryable form is broadly useful across
the institute and directly aligned with the hackathon's AI-tooling
premise.

## What a team could build in one day

A prototype that:

- Ingests protocols from PDFs, text, spreadsheets, or web pages.
- Extracts steps, materials, timings, parameters, hazards, and
  dependencies.
- Normalizes them into a structured representation.
- Exposes the result through chat, checklist, or workflow-card views.
- Answers grounded questions with links back to the source passages.

Minimum viable demo: one real protocol ingested end to end, with a user
asking practical execution questions and getting source-grounded answers.

## How Claude and AWS help

- **Claude** is central — extraction, normalization, grounding, and
  question answering all use it.
- **AWS** hosts storage, retrieval, embeddings, and the lightweight app
  infrastructure to make the assistant usable during the event.

## Stretch directions

- Compare two versions of a protocol and surface the diff.
- Generate reagent / shopping lists.
- Produce execution checklists or calendarized task sequences.
- Support multiple protocol types with shared templates.
