---
title: "Protein language model embeddings for property prediction"
slug: plm-property-prediction
lead: "Extract embeddings from protein language models, train prediction heads on a chosen property, and benchmark across PLMs and head architectures."
theme: "Protein engineering, machine learning"
compute: "Moderate — basic ML GPU (Nvidia T4 or above)"
repo: ""
team: []
---

## Why this project

Embedding-based property prediction is one of the cleanest applied uses
of protein language models. Common targets like stability and solubility
have been benchmarked extensively — but less-studied properties like
optimum pH, enzyme activity, or protein flexibility could yield a more
interesting benchmark, if the right datasets exist.

## What a team could build in one day

- Implement a clean **embed → prediction head** pipeline.
- Run a small set of PLMs (ESM2, ESM3, ProtT5, etc.) against one chosen
  property dataset.
- Compare a few head architectures: linear, shallow MLP, attention pooling.
- Produce a benchmark table with held-out evaluation.

Minimum viable demo: at least two PLMs, one property dataset, one head
architecture — with held-out results.

## Stretch directions

- More PLMs and more property datasets for a real benchmark.
- Transfer-learning and multi-task heads.
- Compare to ESM-IF or structure-aware models on the same task.

## Resources

- Protein language models: ESM2 / ESM3, ProtT5, Ankh, ProGen.
- Datasets: TAPE / FLIP / PEER suites, plus more specific datasets for
  optimum pH or enzyme activity if findable.
