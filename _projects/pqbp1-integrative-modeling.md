---
title: "PQBP1 as a central regulator of inflammation in neurodegeneration"
slug: pqbp1-integrative-modeling
lead: "Use integrative modelling (HADDOCK) to build structural hypotheses for how PQBP1 — a small disordered adapter — recognises oligomeric ligands (HIV-1 capsid, Tau fibrils, α-syn fibrils) and recruits cGAS to drive inflammation."
lead_author: "Dale Allen"
lead_affiliation: "Chanda Lab, Scripps Research"
theme: "Integrative structural modelling, innate immunity"
compute: "Modest — HADDOCK (preferably 3.0) with online dependencies; data under 1 GB"
repo: ""
team: []
---

> **Confidentiality.** This dataset is near submission. All data shared
> with the team must be kept confidential until publication. Talk to
> Dale about sharing additional data beyond what's in the starter pack.

## Why this project

PQBP1 is a 265-aa, largely disordered adapter that's been impossible to
pin down by cryo-EM or crystallography. The Chanda lab has assembled
NMR, HDX-MS, XL-MS, and biochemistry data on how PQBP1 interacts with
oligomeric ligands and recruits cGAS to trigger inflammation — a
mechanism implicated in Alzheimer's and Parkinson's. The piece that's
still missing is a structural picture, and the hackathon outputs feed
directly into a manuscript in preparation.

## What a team could build

- Convert the lab's NMR, HDX-MS, and XL-MS restraints into HADDOCK
  constraint files.
- Run HADDOCK across the three target ligands (HIV-1 hexamer, Tau
  fibrils, α-syn fibrils) and assess convergence with MDanalysis and
  TM-comparison.
- Generate many models without user bias — let the data and the
  scoring drive ensemble selection.

Minimum viable demo: converged HADDOCK ensembles for the PQBP1 WW
domain against at least one oligomeric ligand, plus a short writeup
comparing binding surfaces across targets.

## Stretch directions

- Model the tri-molecular complex of PQBP1 (265 aa) + HIV-1 hexamer
  (221 aa × 6) + human cGAS (522 aa).
- Coarse-grained simulations of how PQBP1 senses ligands through
  conformational selectivity.
- Cross-check HADDOCK ensembles against the lab's existing Alphalink2
  XL-MS model of unbound PQBP1.

## Data

Mix of PDB, plain text, and FASTA — primarily structural restraints
plus reference structures. The starter pack pairs published WW-domain
constraints (Nat. Commun. 2021) with the lab's NMR, HDX-MS, and XL-MS
data, and includes an Alphalink2 model of unbound PQBP1. Preliminary
low-confidence cryo-EM maps are available on request.

Reference structures (PQBP1, HIV-1 capsid, Tau, α-syn, cGAS) can be
pulled from [UniProt on AWS](https://registry.opendata.aws/uniprot/).

## Background reading

- <https://pubmed.ncbi.nlm.nih.gov/35809572/>
- <https://pubmed.ncbi.nlm.nih.gov/26046437/>
- <https://www.nature.com/articles/s41467-021-26851-2>
- <https://www.mdpi.com/1999-4915/16/8/1340>
- <https://pmc.ncbi.nlm.nih.gov/articles/PMC3318138/>
- <https://www.nature.com/articles/srep30293>

## Skills you'll build

Integrative structural modelling with HADDOCK; ingesting NMR, HDX-MS,
and XL-MS restraints into 3D models; structural-bioinformatics
workflows with MDanalysis and TM-comparison; reasoning from sparse
experimental data toward biophysical mechanism.
