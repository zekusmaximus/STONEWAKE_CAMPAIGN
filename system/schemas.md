# Schemas and Canon Governance (Append-Only)
This file defines the rules for what can change and how changes are recorded. Treat it as enforceable policy.

## Canon rules (global)
- Canon is append-only. Never rewrite or delete past canon.
- Corrections go into Errata, never by editing earlier text.
- New facts must be timestamped by session or date anchor.
- Unknowns are labeled **Unknown (Canon gap)** until resolved.

## Errata format (append-only)
Add an Errata section at the end of the relevant file (or append to an existing Errata section).

```
## Errata (Append-only)
- [YYYY-MM-DD or Session XX] Issue: <brief contradiction or correction>
  - Canon-safe resolution: <what is now true without rewriting history>
  - Impacted files: <list of files>
```

## Session log rules
- Session logs are immutable once written.
- New sessions are new files: `sessions/session_log_XX.md`.
- Use two-digit numbering and increment by 1.
- If a log needs correction, add Errata to the log file.

## World state update rules
- `world/world_state.md` is append-only in spirit: add new facts or add an Errata entry.
- Do not delete locations, NPCs, or factions; mark as inactive, deceased, or dissolved.
- Status fields should be one of: `active`, `inactive`, `unknown`, `destroyed`, `merged`, `sealed`, `compromised`.
- New NPCs/locations/factions must include: name, role/summary, status, and first appearance session.

## Active clocks rules
- Every clock must include:
  - Name
  - Current tick (X/Y)
  - What it measures
  - What advances it
  - Threshold outcomes
  - How to reduce/redirect
- Tick increments must include justification tied to a session or event.
- Resolving a clock is append-only: mark it resolved and create a new clock if needed.

## Naming conventions
- NPCs: `First Last` or `Title Name` with consistent spelling.
- Factions: `Formal Name` (short label optional).
- Locations: `Location Name` with region in parentheses if ambiguous.

## Canon gap procedure
When something is unknown:
1) Record it as **Unknown (Canon gap)** in the relevant file.
2) Add a note in the next session log explaining why it is unknown.
3) Resolve only through play or a formal Errata ruling.
