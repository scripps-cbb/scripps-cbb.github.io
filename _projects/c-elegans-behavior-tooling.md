---
title: "Tooling for C. elegans behavior analysis"
slug: c-elegans-behavior-tooling
lead: "Apply or build behavioral analysis tools to study how specific motor neurons shape C. elegans behavior, using a perturbation video dataset."
theme: "Behavioral analysis, machine learning"
compute: "High — large storage required"
repo: ""
team: []
---

## Why this project

Worm behavior is one of the most tractable, widely-used systems for
mapping neural circuits to behavior, and there's a great public dataset
of perturbation videos to work with — about 300 videos at ~27,000 frames
each, with motor-neuron perturbations included.

## What a team could build in one day

- Get the videos loading and indexed.
- Run an existing tracker (e.g. Tierpsy or DeepLabCut) on a subset.
- Extract per-frame behavioral features.
- Look for motor-neuron-perturbation effects in the basic statistics
  (speed, posture, frequency of reversals, etc.).

Minimum viable demo: tracking output + a handful of summary plots
showing perturbation effects.

## Stretch directions

- Train a new tracker or behavior classifier.
- Contrastive embeddings of behavior across perturbations.
- Unsupervised clustering of behavioral motifs.

## Compute

High — the dataset is large and storage is the practical bottleneck.
Plan to subset early in the day.
