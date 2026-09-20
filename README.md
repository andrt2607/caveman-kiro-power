# Caveman — Kiro Power

Ultra-compressed communication mode for [Kiro](https://kiro.dev). Cuts token usage ~75% by having the agent speak like a smart caveman while keeping full technical accuracy. Fluff dies, substance stays.

Code blocks, technical terms, and quoted errors are always preserved exactly. Ships six intensity levels, from lightly-tightened prose to maximally-compressed classical Chinese (文言文).

## Why use it

- **Fewer tokens** — strips articles, filler, pleasantries, and hedging. Roughly 75% reduction on prose.
- **Same accuracy** — technical terms, code, commit messages, and PRs stay exact.
- **Tunable** — six levels let you pick how aggressive the compression is.
- **Safe by default** — auto-drops caveman for security warnings and irreversible-action confirmations, then resumes.

## What's in this repo

```
caveman-kiro-power/
├── POWER.md            # Power manifest (metadata, quick reference)
├── steering/
│   └── caveman.md      # Full behavior rules, levels, examples
└── README.md           # This file
```

## Install

A Kiro Power is a folder containing a `POWER.md` manifest and a `steering/` directory. Install it by placing this repo in your Kiro powers directory.

### Option 1 — Clone into the powers directory

**User level (available in every workspace):**

```bash
git clone <repo-url> ~/.kiro/powers/caveman
```

**Workspace level (available in one project only):**

```bash
git clone <repo-url> .kiro/powers/caveman
```

### Option 2 — Copy manually

Copy the `caveman-kiro-power` folder into either location:

- `~/.kiro/powers/caveman` — user level, all workspaces
- `.kiro/powers/caveman` — workspace level, current project only

After installing, reload Kiro (or reopen the workspace) so the power is picked up. Confirm it loaded by checking the installed powers list in Kiro.

## Usage

### Activate

Say any of the following, or use the slash command:

- "caveman mode"
- "talk like caveman"
- "use caveman"
- "less tokens"
- "be brief"
- "caveman"
- `/caveman`

Default level on activation is `full`.

### Switch levels

| Command | Level |
|---|---|
| `/caveman lite` | No filler/hedging, keep full sentences |
| `/caveman full` | Drop articles, fragments OK, short synonyms (default) |
| `/caveman ultra` | Abbreviate, arrows for causality, one word when possible |
| `/caveman wenyan-lite` | Semi-classical Chinese, keep grammar |
| `/caveman wenyan` / `/caveman wenyan-full` | Full 文言文, 80–90% character reduction |
| `/caveman wenyan-ultra` | Extreme compression, classical feel |

### Deactivate

Say "stop caveman" or "normal mode". The level persists until you change it or the session ends.

## Levels at a glance

Question: *"Why does my React component re-render?"*

| Level | Response |
|---|---|
| lite | "Your component re-renders because you create a new object reference each render. Wrap it in useMemo." |
| full | "New object ref each render. Inline object prop = new ref = re-render. Wrap in useMemo." |
| ultra | "Inline obj prop → new ref → re-render. useMemo." |
| wenyan-lite | 組件頻重繪，以每繪新生對象參照故。以 useMemo 包之。 |
| wenyan-full | 物出新參照，致重繪。useMemo Wrap之。 |
| wenyan-ultra | 新參照→重繪。useMemo Wrap。 |

## Boundaries

- **Code, commits, and PRs** are always written normally, regardless of level.
- Caveman is dropped for **security warnings**, **irreversible-action confirmations**, and steps where terseness risks a misread — then resumed automatically.

## How it works

`POWER.md` declares the power's metadata and keywords so Kiro can surface it. `steering/caveman.md` holds the full instruction set: activation triggers, the compression rules, all six intensity levels with examples, and the auto-clarity behavior. When the power is active, Kiro loads these steering rules into context and applies them to its responses.

## Author

OOCAZ
