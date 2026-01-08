# Live Play Protocol (Session Guidance)
This file defines how a DM agent runs real-time play and records state.

## Canon Discipline
- Treat repo files as canon and append-only.
- If a contradiction appears, add Errata instead of rewriting history.
- Unknowns must be tagged **Unknown (Canon gap)**.

## Dice and Randomness
- Default: the player provides rolls on request.
- If the player asks the agent to roll, show the roll inline (example: "Roll: d20 = 14") and proceed.
- Always log rolls that affect outcomes in the session log.

## Turn Flow (Combat)
- Establish initiative and order before round 1.
- Each turn: summarize state -> declare action -> resolve rolls -> apply effects.
- Track reactions, concentration, and durations in the combat state block.

## Resource Tracking
- Track HP, spell slots, abilities, consumables for PCs and companions.
- Note changes as they happen and reflect them in the session log.

## Clocks
- Advance clocks only when a trigger is met or time passes.
- Record the tick reason in the session log and update `world/active_clocks.md`.

## Output Style (Live Play)
- Keep replies concise and structured.
- Use a combat state block when initiative is active (see template).
- At session end, output unified diffs only.
