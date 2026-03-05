---
title: Gameplay
description: Camp actions, GM profiles, and survival strategy for Escape the Valley.
sidebar:
  order: 2
---

## Overview

You lead a party of settlers through a procedurally generated valley. Each turn you choose a camp action, then the game engine resolves events, weather, encounters, and resource changes. The goal is to reach the valley exit before your supplies or your people give out.

The world uses seeded generation -- pass `--seed 42` to get the same terrain, weather patterns, and event deck every time. Useful for comparing strategies or sharing challenges.

## Camp actions

Every turn at camp, you choose one action:

| Action | What it does |
|--------|-------------|
| **Travel** | Move toward the exit. Every turn not moving burns supplies for nothing. |
| **Rest** | Recover health and morale. Chance to cure conditions. |
| **Hunt** | Forage for food. Best results in forests and plains. |
| **Repair** | Fix wagon damage before it strands you. |
| **Ration** | Cut to half-rations when food is scarce. Costs morale. |
| **Abandon** | Drop cargo weight for speed. Last resort only. |

The tension is always between moving forward and keeping your party healthy. Travel too hard and people break down. Rest too long and you starve.

## GM profiles

The AI Game Master narrates your journey using one of three storytelling voices. The GM shapes the tone, not the mechanics -- all three profiles use the same underlying rules engine.

| Profile | Tone | Best for |
|---------|------|----------|
| **Chronicler** | Dry, factual, historical | Players who want the facts straight |
| **Fireside** | Warm, folksy storyteller | First playthrough (default) |
| **Lantern-Bearer** | Eerie, atmospheric, foreboding | Experienced players looking for tension |

Choose a profile at launch:

```bash
trail tui --gm chronicler
trail tui --gm fireside
trail tui --gm lantern-bearer
```

The GM runs locally via [Ollama](https://ollama.com/). If Ollama is not installed or not running, the game falls back to built-in narration.

## World generation

Each run generates terrain, weather, encounters, and event decks from a seed. Two runs with the same seed produce the same world, letting you:

- Compare strategies on identical maps
- Share seeds with friends for challenge runs
- Reproduce and report bugs reliably

The twist deck introduces 10-15% weird folklore events -- strange encounters that bend the rules in unexpected ways.

## XRPL Ledger Backpack

An optional feature for Phase 2: every supply change (food, water, medicine, ammo, parts) is tracked as a token on the XRPL Testnet. After your run, the trail ledger shows an on-chain receipt of your entire journey.

```bash
trail ledger   # print the on-chain trail ledger
```

This feature requires a testnet connection and is entirely optional. The game works fully offline without it.
