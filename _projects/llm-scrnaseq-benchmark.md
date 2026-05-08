---
title: "Benchmarking LLMs for automated scRNA-seq analysis"
slug: llm-scrnaseq-benchmark
lead: "Test which LLM produces the fastest, most accurate cell-type annotation pipeline using expert-curated public scRNA-seq datasets as ground truth."
theme: "Single-cell, transcriptomics, LLMs"
compute: "Low — 16 GB RAM, standard CPU"
repo: ""
team: []
---

## Why this project

Cell-type annotation is one of the most time-consuming steps in scRNA-seq
analysis. LLMs are now capable enough to either generate full pipelines
end-to-end or do zero-shot annotation directly from marker genes. A clean
head-to-head benchmark — same data, same prompts, expert-annotated ground
truth — would be a useful contribution.

## What a team could build in one day

- Pick a small set of well-annotated public datasets (the 10X / Seurat
  PBMC tutorial data is a clean starting point).
- Run several LLMs (Claude, GPT, open-weights models) under matched
  prompts — both the "generate a pipeline" framing and the "zero-shot
  annotation from marker genes" framing.
- Score against expert annotations and produce a leaderboard.

Minimum viable demo: a comparison table for one dataset across 2–3 LLMs.

## Stretch directions

- Extend across tissues and conditions for a broader benchmark.
- Multi-step agentic pipelines (LLM as orchestrator over sklearn / scanpy).
- Cost vs. latency vs. accuracy comparisons.

## Compute

Low — 16 GB RAM and a standard CPU should suffice. Most work is API calls.
