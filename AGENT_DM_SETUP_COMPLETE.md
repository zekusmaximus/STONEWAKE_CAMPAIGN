# Agent DM Setup — Complete

**Status:** Ready for agent-driven D&D sessions

---

## What Was Created

Your Stonewake campaign repository now has a **comprehensive bootstrap system** that allows coding agents (Claude, Codex, etc.) to act as your DM with full context and consistent gameplay.

### New Files Created

1. **[system/bootstrap_prompt.md](system/bootstrap_prompt.md)** — **EXPANDED (374 lines)**
   - Core identity and tone calibration
   - Startup sequence (which files to read in order)
   - Session flow (opening, active play, transitions, ending)
   - Clock advancement triggers (explicit conditions for all 5 clocks)
   - NPC motivation cheat sheet (inline quick reference)
   - Companion control rules (Valmore & Snik social/combat behavior)
   - Conflict resolution style hierarchy (economic → legal → institutional → combat)
   - Decision presentation format (how to offer choices)
   - Canon governance (append-only, errata procedures)
   - Session end output format (unified diffs)
   - Quick reference checklist for DM agents

2. **[system/npc_motivation_quick_ref.md](system/npc_motivation_quick_ref.md)** — **NEW**
   - Detailed motivation profiles for all major NPCs
   - What each NPC wants, how they pursue it, what makes them act
   - Tone guidance for each character
   - NPC agency guidelines (when they act independently vs. react to Luno)
   - Quick decision matrix for DM agents

3. **[system/open_threads_active.md](system/open_threads_active.md)** — **NEW**
   - All 8 current open threads with status
   - Priority order for NPC actions
   - What requires player action vs. what advances independently
   - Session 08 opening context (ready to paste)
   - Guidelines for when to advance threads off-screen

4. **[system/conflict_resolution_procedures.md](system/conflict_resolution_procedures.md)** — **NEW**
   - Explicit procedures for economic, legal, institutional, and combat conflicts
   - Player tools vs. NPC tools for each conflict type
   - Resolution mechanics and clock impact guidance
   - Conflict escalation ladder (5 steps from info gathering to open conflict)
   - Special section on infernal contract conflicts
   - Examples from campaign history

5. **[system/session_pacing_guide.md](system/session_pacing_guide.md)** — **NEW**
   - Session structure (4 phases: opening, active play, transitions, wrap-up)
   - Pacing principles (tight narration, player agency, meaningful choices, clock-driven)
   - Scene length guidelines (short/medium/long)
   - When to force decisions vs. let player explore
   - Handling downtime and balancing multiple threads
   - Immersion techniques (dice transparency, tactical language, consequence framing)

6. **[system/dm_interaction_protocol.md](system/dm_interaction_protocol.md)** — **NEW**
   - Decision presentation format (standard template)
   - How to request rolls (skill checks, attacks, saves)
   - Handling different types of player input (clear, vague, creative, indecisive)
   - Combat decision flow (initiative-based)
   - NPC reaction format
   - Consequence narration templates
   - Session end protocol

---

## How to Use This System

### Step 1: Start a New Agent Session

Open a new chat with Claude, Claude Code, Codex, or another coding agent.

### Step 2: Paste the Bootstrap Prompt

Copy the entire contents of **[system/bootstrap_prompt.md](system/bootstrap_prompt.md)** into the agent.

The bootstrap will instruct the agent to:
1. Read all necessary context files in order
2. Understand the campaign state and mechanics
3. Begin play immediately after Session 07
4. Follow all system rules (clocks, NPCs, conflicts, pacing)

### Step 3: Play Begins

The agent will present the opening scene with:
- Current location and time
- Who's present (Luno, Valmore, Snik, NPCs)
- Immediate context and active threats
- Clear decision point with 3-4 options

### Step 4: Agent Maintains Context

The agent will:
- Track all resources (HP, spell slots, gold, inventory)
- Advance clocks only when explicit triggers are met
- Drive NPCs according to their motivations
- Present conflicts using the hierarchy (economic → legal → institutional → combat)
- Maintain tone (tactical realism, bureaucratic horror, gritty subtlety)
- Record all consequential rolls

### Step 5: Session End

When you're ready to end, the agent will:
- Summarize outcomes (XP, clock ticks, threads)
- Update resource tracking
- Output unified diffs for:
  - New session log
  - World state updates
  - Clock advances
  - Character sheet updates
  - Errata (if needed)

You can then commit these changes to the repository to preserve state.

---

## Key Features of This System

### 1. Full Context Preservation
- All campaign history, NPCs, mechanics, and rules are in the repository
- Agents can reset/restart without losing state
- Session logs provide complete audit trail

### 2. Explicit Clock Management
- All 5 clocks have explicit triggers listed in bootstrap
- Agents advance clocks only when conditions are met (not arbitrarily)
- Clock ticks create natural story escalation

### 3. NPC Agency & Motivation
- Every major NPC has clear goals and methods
- NPCs act independently when player is occupied elsewhere
- Competent adversaries (Ashfall, Captain Kain) adapt and plan

### 4. Conflict Resolution Hierarchy
- Economic and legal tools prioritized over combat
- Infernal agents prefer delegated enforcement and contracts
- Combat is surgical and purposeful, not default

### 5. Immersive Decision Presentation
- Every major choice has clear mechanical stakes
- Options include pros/cons/risks/requirements
- Consequences are narrated immediately and tracked

### 6. Tactical Realism Tone
- NPCs are competent and act rationally
- No contrived solutions or deus ex machina
- Logistics, payment, communication delays matter
- Violence has costs and consequences

### 7. Bureaucratic Horror Theme
- Ashfall operates through contracts and procedures, not brute force
- Power is institutional and professional, not theatrical
- Threats are implied through legal/economic pressure

---

## Example Usage Flow

### You Start a Session:
```
[Paste system/bootstrap_prompt.md into agent]
```

### Agent Responds:
```
# Day 21 — Morning

### Location: Brindlecross Garrison Command Hall

The map table is covered with patrol routes and incident reports. Captain Kain
stands with arms crossed, watching you review the latest intelligence...

[Full scene context with 3-4 clear options]

**What does Baron Luno do?**
```

### You Choose:
```
Option 1: Interrogate the detained coordinator
```

### Agent Runs Interrogation:
```
### Interrogation Scene — Coordinator Detention Cell

[Scene narration with NPC reactions]

**Available Interrogation Approaches:**
1. Legal Pressure [Persuasion check]
2. Fear & Certainty [Intimidation check]
3. Deal-Making [Persuasion check, binds you to protection]
4. Other [specify]

**What does Baron Luno do?**
```

### Session Continues...

Combat encounters use initiative blocks with dice rolls.
Social scenes track NPC motivations and reactions.
Clocks advance only when explicit triggers are met.

### Session Ends:
```
## SESSION END — Session 08

[Summary, XP, resource updates, next session hooks]

### Unified Diffs Output:
[New session log, world state updates, clock advances, character updates]
```

---

## Testing the System

### Recommended First Session Test

1. **Start with the bootstrap prompt**
2. **Choose a simple objective** (e.g., "Interrogate the detained coordinator")
3. **Verify the agent:**
   - Presents clear options
   - Tracks resources accurately
   - Advances clocks only when triggered
   - Maintains tone and NPC consistency
   - Outputs proper diffs at session end

### If Issues Arise

- Check that the agent read all required files (bootstrap lists them in order)
- Verify the agent is using RAW D&D 5e mechanics
- Ensure clocks are only advancing when explicit triggers are met
- Confirm NPCs are acting according to their motivations in `npc_motivation_quick_ref.md`

---

## File Reference Summary

### Core Bootstrap (Paste This to Start)
- **[system/bootstrap_prompt.md](system/bootstrap_prompt.md)** — Primary agent instructions

### Supporting System Files (Referenced by Bootstrap)
- **[system/npc_motivation_quick_ref.md](system/npc_motivation_quick_ref.md)** — NPC goals and behaviors
- **[system/dm_interaction_protocol.md](system/dm_interaction_protocol.md)** — How to present decisions
- **[system/open_threads_active.md](system/open_threads_active.md)** — Current active storylines
- **[system/conflict_resolution_procedures.md](system/conflict_resolution_procedures.md)** — Non-combat conflict guidance
- **[system/session_pacing_guide.md](system/session_pacing_guide.md)** — Session structure and flow

### Existing System Files (Already in Repo)
- **[system/live_play_protocol.md](system/live_play_protocol.md)** — Dice, canon discipline, turn flow
- **[system/dm_rules.md](system/dm_rules.md)** — RAW enforcement, companion control
- **[system/combat_state_template.md](system/combat_state_template.md)** — Initiative combat format
- **[system/session_log_template.md](system/session_log_template.md)** — Log standardization

### World Context (Agent Reads These)
- **[sessions/session_log_07.md](sessions/session_log_07.md)** — Latest session
- **[world/world_state.md](world/world_state.md)** — Canonical world snapshot
- **[world/active_clocks.md](world/active_clocks.md)** — 5 tension clocks
- **[characters/baron_luno.md](characters/baron_luno.md)** — PC sheet
- **[characters/valmore_and_snik.md](characters/valmore_and_snik.md)** — Companion sheets

---

## What Makes This System Unique

### 1. Append-Only Canon
- No retroactive changes; corrections via Errata
- Full audit trail in session logs
- Agents can't accidentally break continuity

### 2. Clock-Driven Narrative
- Story escalates organically based on player choices
- NPCs act independently; world doesn't wait for player
- Explicit triggers prevent arbitrary tension

### 3. Institutional Conflict Focus
- Economic and legal warfare prioritized over combat
- Infernal bureaucracy as primary antagonist
- Reflects real-world power dynamics (contracts, leverage, reputation)

### 4. Agent-Friendly Design
- Explicit checklists and decision matrices
- Clear formatting and templates
- Separation of concerns (clocks, NPCs, conflicts, pacing)

### 5. Player Agency Respect
- No railroading; genuine choices with real consequences
- Creative approaches are evaluated fairly
- Agents present options but never force actions

---

## Next Steps

1. **Test the bootstrap** with a short session (30-60 minutes)
2. **Verify outputs** match expected format (session log, diffs, resource tracking)
3. **Adjust as needed** (add Errata entries if rules need clarification)
4. **Play regularly** — the system is designed for consistent agent-driven sessions

---

## Credits

**System Design:** Based on your existing Stonewake campaign structure with tactical realism, append-only canon, and clock-driven pacing.

**Expansion Focus:** Explicit guidance for AI agents to maintain consistency, track state, drive NPCs, and present immersive decisions like your example session.

**Result:** A self-contained D&D campaign that can run autonomously with coding agents as DM while maintaining quality, consistency, and player agency.

---

**Your campaign is ready. Good luck, Baron Luno. Stonewake awaits.**
