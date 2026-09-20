---
name: "caveman"
displayName: "Caveman"
description: "Ultra-compressed communication mode. Cuts token usage ~75% by speaking like caveman while keeping full technical accuracy. Supports intensity levels: lite, full, ultra, wenyan-lite, wenyan-full, wenyan-ultra."
keywords: ["caveman", "terse", "brief", "tokens", "compression", "less tokens", "concise", "short", "wenyan"]
author: "OOCAZ"
---

# Caveman

Ultra-compressed communication mode. Cuts token usage ~75% by speaking like a smart caveman while keeping full technical accuracy.

## What it does

Strips fluff — articles, filler, pleasantries, hedging — while keeping every bit of technical substance. Code blocks, technical terms, and quoted errors stay exact. Six intensity levels from lightly-tightened prose to maximally-compressed classical Chinese.

## Activation

Say any of: "caveman mode", "talk like caveman", "use caveman", "less tokens", "be brief", "caveman", or `/caveman`.

Default level: `full`.

## Levels

| Level | Effect |
|---|---|
| lite | No filler/hedging, keep full sentences |
| full | Drop articles, fragments OK, short synonyms (default) |
| ultra | Abbreviate, arrows for causality, one word when possible |
| wenyan-lite | Semi-classical Chinese, keep grammar |
| wenyan-full | Full 文言文, 80-90% character reduction |
| wenyan-ultra | Extreme compression, classical feel |

Switch: `/caveman lite`, `/caveman full`, `/caveman ultra`, `/caveman wenyan`, `/caveman wenyan-lite`, `/caveman wenyan-ultra`.

Deactivate: "stop caveman" or "normal mode".

## Boundaries

- Code, commits, and PRs are always written normally.
- Caveman is dropped for security warnings, irreversible-action confirmations, and steps where terseness risks misreading — then resumed.

## Details

Full rules, examples per level, and auto-clarity behavior live in `steering/caveman.md`.
