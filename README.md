# Stonewake Campaign SSOT
This repository is the Single Source of Truth (SSOT) for the Stonewake D&D 5e campaign. All facts, mechanics, and outcomes that appear here are canon unless explicitly marked as draft. This repo is the memory that survives context resets.

## What "canon" means
- Canon is the authoritative record of what happened and what is true in the campaign.
- Canon changes only by appending new facts or adding Errata (never rewriting history).
- Unknowns are labeled as **Unknown (Canon gap)** until resolved by play or a ruling.
- If a contradiction is found, do **not** edit past entries; use Errata per `system/schemas.md`.

## Repo layout
- `characters/` player and companion sheets (mechanical state and loadouts)
- `world/` world state, factions, clocks, and strategic situation
- `sessions/` immutable session logs
- `system/` governance, DM rules, bootstrap prompt, and Codex task prompts

Key files:
- `characters/party_state.md` shared party resources
- `world/locations.md`, `world/npc_roster.md`, `world/factions.md` quick-access mirrors
- `world/clock_history.md` append-only clock tick log
- `system/errata.md` central Errata index

## Quickstart
1) Read `sessions/index.md` and the latest `sessions/session_log_XX.md`.
2) Read `world/world_state.md` and `world/active_clocks.md`.
3) Read `characters/baron_luno.md` and any companions in `characters/`.
4) Read `system/rules_assumptions.md` for RAW baselines.
5) Read `system/live_play_protocol.md` for runtime procedure.
6) Start play immediately after the latest log.

## How to start a new DM chat session
- Tell the model to treat all repo files as canon and append-only.
- Point it at `system/bootstrap_prompt.md` and the latest session log.
- Do not paste full files; reference the repo files directly and request diffs.

## Update workflow (session -> diff -> review -> commit)
1) Play the session.
2) Capture bullet notes or transcript snippets.
3) Generate unified diffs that update:
   - `sessions/` (new log)
   - `world/world_state.md` (facts changed)
   - `world/active_clocks.md` (clock ticks)
   - `characters/` (resource changes)
4) Review diffs against canon rules in `system/schemas.md`.
5) Commit once the diffs are correct.

## How to resume after a context reset
- Re-read `system/bootstrap_prompt.md`.
- Load the latest session log and current world state.
- Use the clocks and character sheets as the mechanical baseline.
- If anything is unclear, mark it as **Unknown (Canon gap)** and add an Errata note.
