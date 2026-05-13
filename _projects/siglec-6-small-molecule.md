---
title: "Siglec-6 small-molecule binding"
slug: siglec-6-small-molecule
lead: "Computationally screen and dock candidate analogues against Siglec-6 to improve on the lab's existing weak (~75 µM) lead — promising hits get synthesised and validated wet-lab (SPR for K_d, CETSA in live cells)."
lead_author: "Julien Lee Heberling"
lead_affiliation: "Huang Lab, Scripps Research"
theme: "Virtual screening, immunology"
compute: "Modest — AutoDock Vina docking workflows"
repo: ""
team: []
---

## Why this project

Siglec-6 (CD327, OB-BP1) is a poorly understood Siglec family member —
expression is restricted to memory B cells, mast cells, and
trophoblasts, and it's upregulated in chronic lymphocytic leukaemia,
acute myeloid leukaemia, and preeclampsia. The Huang lab has
preliminary binding data on a small molecule that interacts with
Siglec-6 but at a weak affinity (K_d ≈ 75 µM). The hackathon goal is
to use computation to suggest analogues with markedly improved binding,
so the wet-lab can prioritise synthesis and validation.

## What a team could build

- Set up an AutoDock Vina docking workflow against the AlphaFold model
  of Siglec-6.
- Generate or curate a SMILES library of analogues around the current
  ~75 µM lead.
- Score and rank candidates, then surface a short list of promising
  poses with rationale.

Minimum viable demo: a ranked list of analogue candidates with docking
scores, pose visualisations, and a one-pager arguing why the top hits
are worth synthesising.

## Stretch directions

- Pull a protein-language-model embedding for Siglec-6 (e.g. via
  OpenProteinSet on AWS) and use it as an additional feature for
  filtering candidates.
- Generative analogue design (e.g. via fragment growing) rather than a
  static SMILES library.
- Compare Vina against a free-energy or ML-based rescoring step.

## Data

- AlphaFold PDB of Siglec-6 (~50 kDa, unglycosylated).
- SMILES strings of small-molecule candidates (~300–600 amu).

Pull the AlphaFold structure / UniProt annotations from
[UniProt on AWS](https://registry.opendata.aws/uniprot/), and the
[OpenProteinSet AWS mirror](https://registry.opendata.aws/openfold/)
if teams want PLM embeddings as a representation-learning baseline.

## Wet-lab follow-up

Promising hits are synthesised by the lab and validated:

- **SPR** for K_d measurement.
- **CETSA** for protein perturbation in live cells.

## Skills you'll build

Protein–ligand docking with AutoDock Vina; virtual screening from
SMILES libraries; structure-based rational design of small-molecule
analogues; reading docking poses against experimental binding-affinity
data.
