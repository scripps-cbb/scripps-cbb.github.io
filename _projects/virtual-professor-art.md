---
title: "Virtual Professor Art"
slug: virtual-professor-art
lead: "Talk to a virtual scientific mentor in mixed reality — real-time conversation, synthesized voice, and an animated avatar that can react to what the headset sees."
theme: "Mixed reality & conversational AI"
lead_author: ""
lead_affiliation: ""
repo: ""
team: []
---

## Why this project

It pulls together mixed reality, conversational AI, voice synthesis, avatar
animation, and science education into one demo. The scope is naturally
tiered: a text-to-speech conversational loop is already useful on day one,
while avatars, lip sync, and headset-aware context are great stretch
goals. A handful of Meta Quest headsets will be available on site.

## What a team could build in one day

A real-time conversation loop where a student speaks to (or types at) the
Virtual Professor in a Unity / Meta Quest scene and gets a spoken answer
back. Concretely:

- An AWS-hosted server that takes user input, calls an LLM, and streams
  the response through text-to-speech.
- A Unity client on Meta Quest with microphone capture and audio playback.
- A simple avatar that "speaks" the response (basic mouth open/close is
  enough for the MVP).
- A short `personality.md` that grounds tone, expertise, and limits — so
  the agent answers in a consistent voice. Reference audio of Prof. Art
  Olson would be used **only with explicit permission**.

## How Claude and AWS help

- **Claude** for grounded, age-appropriate explanations, drafting the
  personality file, and scaffolding the conversational pipeline.
- **AWS** for the real-time conversation server, STT/TTS services,
  streaming, and hosting the Unity client's backend.

## Stretch directions

- Lip sync, facial animation, gesture, and idle behavior on the avatar.
- Send headset screenshots to the server so the professor can comment on
  what the student is looking at.
- A small library of guided demonstrations.
- Multiple "virtual mentor" personalities for different domains.
