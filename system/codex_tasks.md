# Codex Task Prompts (Operational Playbook)
Use these prompts as copy/paste tasks for Codex. Each task must output unified diffs only (no full file rewrites unless creating a new file).

## A) Session log creation
Prompt:
You are Codex. Create a new session log in `sessions/session_log_XX.md` using the provided notes.
Requirements:
- Structured sections: Date Anchor, Party, Summary (Detailed), Mechanical Notes, World State Changes, Open Threads.
- Use `system/session_log_template.md` as the formatting baseline.
- Include mechanical outcomes, world consequences, NPC knowledge changes, and open threads.
- Keep it detailed but concise.
- Output a unified diff only. If the session log is new, add it as a new file in the diff.
Input notes:
<paste narrative snippets or bullet notes here>

## B) Clock advancement
Prompt:
You are Codex. Update `world/active_clocks.md` based on the specified clock changes.
Requirements:
- Increment the clock(s) with justification tied to a session or event.
- If a threshold triggers, note the outcome.
- Minimal diff; append-only behavior.
- Output a unified diff only.
Input:
Clock(s) advanced:
Reason(s):

## C) World state mutation
Prompt:
You are Codex. Update `world/world_state.md` with the factual changes provided.
Requirements:
- Minimal diff, append-only where required.
- Add new NPCs/locations/factions with status and first appearance session.
- If changes affect NPCs, locations, or factions, update the mirror files (`world/npc_roster.md`, `world/locations.md`, `world/factions.md`) in the same diff.
- Mark unknowns as **Unknown (Canon gap)**.
- Output a unified diff only.
Input changes:
<paste factual changes here>

## D) End-of-session all updates bundle
Prompt:
You are Codex. Produce unified diffs for a full session update bundle.
Requirements:
- New `sessions/session_log_XX.md`
- Update `world/world_state.md`
- Update `world/active_clocks.md`
- Update relevant `characters/` files
- Minimal diffs, append-only where required.
Input:
Session number:
Session notes (bullets):
Clocks advanced:
Character/resource changes:
