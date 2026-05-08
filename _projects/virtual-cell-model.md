---
title: "Training a 'virtual cell' model for gene expression inference"
slug: virtual-cell-model
lead: "Train a virtual-cell model from public scRNA-seq perturbation data and benchmark it against entries from the November 2025 Virtual Cell Challenge."
theme: "Single-cell, transcriptomics, machine learning"
compute: "High — STATE base model takes ~2 hr on an A100"
repo: ""
team: []
---

## Why this project

The Virtual Cell Challenge is a fresh, well-defined benchmark with
harmonized public data — exactly the kind of target a hackathon team can
ship something measurable against in three days.

## What a team could build in one day

- Stand up the **STATE** base model from Arc Institute's harmonized
  datasets (a video tutorial walks through the setup).
- Run inference on a held-out perturbation set.
- Compare predictions to challenge baselines and the published entries.

Minimum viable demo: trained model + a small evaluation report against
one or two challenge tasks.

## Stretch directions

- Novel architectures or multi-task heads.
- Data augmentations.
- Mixed real + simulated perturbation training.

## Resources

- [Arc Institute harmonized datasets](https://arcinstitute.org/) and the
  Virtual Cell Atlas GitHub repo.
- STATE base-model setup tutorial.

## Compute

High — STATE training is ~2 hours on an A100. Inference is much cheaper.
