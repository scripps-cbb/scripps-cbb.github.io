---
title: "Peptide–MHC binding affinity vs. viral evolution in COVID-19"
slug: peptide-mhc-covid-evolution
lead: "Test whether peptide–MHC binding affinity correlates with viral mutation rates in SARS-CoV-2 across the pandemic."
theme: "Immunology"
compute: "Low – moderate"
repo: ""
team: []
---

## Why this project

A clean immunology hypothesis with a clear directional question: if
highly variable sites also bind MHC well, that suggests MHC pressure
isn't suppressing variability — and would constrain models of immune
evasion. The tools and data are all public.

## What a team could build in one day

- Pull SARS-CoV-2 sequences across waves (early variants through more
  recent ones).
- Run **NetMHCPan** (or **UniPMT**) to predict peptide affinities for
  each variant.
- Score per-position variability across the lineage.
- Correlate variability with predicted binding strength and visualize.

Minimum viable demo: a correlation plot for one HLA allele across at
least two variant time points.

## Stretch directions

- Multiple HLA alleles weighted by population frequency.
- Compare against influenza or other RNA viruses for a baseline.
- Consider T-cell vs. B-cell epitope contexts separately.

## Tools and data

- Peptide–MHC predictors: [NetMHCPan](https://services.healthtech.dtu.dk/),
  UniPMT.
- Public SARS-CoV-2 sequence collections (GISAID, NCBI Virus).
