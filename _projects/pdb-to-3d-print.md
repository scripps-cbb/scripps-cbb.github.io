---
title: "PDB to 3D Print"
slug: pdb-to-3d-print
lead: "One-click conversion from any PDB ID or uploaded structure file to a printable, mesh-repaired 3D file — with a short scientific 'structure card' to go with it."
theme: "Structural biology & outreach"
lead_author: ""
lead_affiliation: ""
repo: ""
team: []
---

## Why this project

Immediately visual, broadly understandable, and genuinely useful for
education, outreach, lab communication, and rapid prototyping. It sits at
the intersection of structural biology, geometry processing, and
scientific communication — and a BambuLab P2S printer will be on site to
print the best results live.

## What a team could build in one day

A small web app or CLI that:

- Fetches a structure from the PDB or accepts an upload.
- Generates one or two print-friendly geometry styles (e.g. surface mesh
  or stylized backbone) with sane defaults for thickness, scale, and
  stability.
- Repairs fragile geometry and exports STL, OBJ, or 3MF.
- Renders a preview image.
- Produces a short structure card describing the molecule and the
  steps taken to make it printable.

The minimum viable demo is one-click conversion for a small set of
example structures, plus a downloadable print-ready file.

## How Claude and AWS help

- **Claude** to scaffold the parsing/export workflow, write per-structure
  explanatory text, and propose labeling or domain-highlight ideas.
- **AWS** for preview rendering, queueing conversions, and batch
  generation across small curated structure collections.

## Stretch directions

- Multicolor or multipart models for assembly.
- Auto-highlight binding pockets or domains.
- Suggest the best print orientation.
- Batch-convert a curated library for teaching or outreach.
