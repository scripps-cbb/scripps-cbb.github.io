---
title: "Caspar–Klug T-Number Explorer"
slug: caspar-klug-capsids
lead: "An interactive tool for exploring the geometry of viral icosahedral capsids — T-number, triangular subdivisions, pentamers and hexamers, and how simple rules generate complex viral shells."
theme: "Structural biology & visualization"
lead_author: ""
lead_affiliation: ""
repo: ""
team: []
---

## Why this project

Many viral capsids have icosahedral symmetry built from repeating protein
subunits. The Caspar–Klug triangulation number, **T**, defines how many
smaller triangles tile each face of the icosahedron — and so how many
subunits the capsid has, and how pentamers and hexamers are organized.
A good interactive visualization makes the relationship between T, lattice
structure, and capsid architecture immediate. Inspiration:
[foldavirus.org](https://foldavirus.org/).

## What a team could build in one day

An interactive viewer that lets users:

- Pick a T-number (T=1, 3, 4, 7, …) and see the corresponding icosahedral
  lattice render in real time.
- Toggle layers: underlying icosahedron, triangular subdivision, asymmetric
  units, capsomers, pentamers/hexamers.
- See the 12 required pentameric positions highlighted on the topology.
- Compare how subunit count and complexity grow with T.

The minimum viable demo is selecting a few T-values and getting clear,
labeled geometry.

## Educational value

This is useful for biology, structural biology, virology, and chemistry
education — it turns a piece of math that often appears as static figures
into something students can manipulate.

## Stretch directions

- Map real PDB capsids onto the lattice and highlight the asymmetric unit.
- Cut-away / cross-section views.
- Annotated guided tours (e.g. "build T=3 from T=1").
- Export figures or short animations for teaching.
