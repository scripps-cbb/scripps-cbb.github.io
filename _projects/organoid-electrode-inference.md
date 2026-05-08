---
title: "Inferring brain organoid structure from electrode recordings"
slug: organoid-electrode-inference
lead: "Reverse-infer the structure of a brain organoid from multi-electrode recordings using computational models and machine learning."
theme: "Neuroscience, machine learning, computational modeling"
compute: "High"
repo: ""
team: []
---

## Why this project

Recovering structure from spiking patterns is a foundational neuroscience
problem and a great test bed for hybrid model + ML approaches. Public
recordings exist, and a base modeling toolkit is available on site.

## What a team could build in one day

- Load the organoid recordings.
- Fit a baseline model — e.g. connectivity inference from spike
  cross-correlations — and evaluate against the structural ground truth.
- Visualize inferred vs. true structure.

Minimum viable demo: a working pipeline from recording → inferred
connectivity → comparison plot for at least one organoid.

## Stretch directions

- Deep generative models of latent neural dynamics.
- End-to-end structure inference from raw recordings.
- Per-organoid variability and population-level summaries.

## Resources

- Methods preprint:
  [bioRxiv 2023.12.29.573646](https://www.biorxiv.org/content/10.1101/2023.12.29.573646v2.full).
- Recordings on
  [DANDI](https://dandiarchive.org/dandiset/000732). *Note: the dataset
  is currently being republished under a new ID due to federal compliance
  changes — check the DANDI archive for the live URL at the time of the
  hackathon.*

## Compute

High — multi-electrode recordings are large; budget for storage and a
GPU for any deep-learning extensions.
