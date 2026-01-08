# Session Pacing & Flow Guide (Canon)

*This file provides DM agents with guidance on session structure, pacing, scene transitions, and when to force decisions vs. let the player explore.*

---

## Session Structure (Recommended Flow)

### Phase 1: Opening (5-10 minutes / 3-5 exchanges)

**Goal:** Orient the player to current situation and immediate choices.

**What to Include:**
1. **Location & Time:** Where is Luno? What time of day? How much time has passed since last session?
2. **Who's Present:** Valmore, Snik, NPCs? Are they safe, in transit, in a meeting?
3. **Immediate Context:** What just happened? What sensory details ground the scene?
4. **Open Threads Reminder:** Briefly note active threats (Ashfall surveillance, detained coordinator, hobgoblin raids)

**Example Opening:**
```
# Day 21 — Morning

### Location: Brindlecross Garrison Command Hall

The map table is covered with patrol routes and incident reports. Captain Kain stands with arms crossed, watching you review the latest intelligence:

- Ashfall Exchange has classified you as a "Regulatory Actor" (passive surveillance active)
- The detained regional coordinator remains in secure custody below
- Hobgoblin raids on outlying farms have increased—three incidents in the past week

Valmore leans against the doorframe, greatsword across his shoulders. Snik is absent—likely scouting the perimeter.

Kain breaks the silence: "We can hold the coordinator indefinitely, but every day increases the risk of external intervention. What's your priority?"

**What does Baron Luno do?**
```

**Pacing Notes:**
- Keep opening concise (3-5 paragraphs max)
- Wait for player input before advancing
- Don't overwhelm with details—let player ask questions

---

### Phase 2: Active Play (Main Session Body)

**Goal:** Resolve player-chosen objectives with meaningful consequences.

#### Scene Types

##### **Type A: Decision Scenes**
- Player faces 3-4 clear options with mechanical/narrative stakes
- Use decision presentation format from `dm_interaction_protocol.md`
- Examples: Choose interrogation approach, select target priority, negotiate terms

**Pacing:** Let player deliberate; don't rush. These are the "weight" moments.

##### **Type B: Tactical Scenes**
- Combat, stealth operations, infiltration, chase scenes
- Use initiative, track resources, record rolls
- Use `combat_state_template.md` for initiative combat

**Pacing:** Move briskly once action starts. Announce outcomes, advance initiative, request actions. Don't linger on minor details.

##### **Type C: Social/Negotiation Scenes**
- NPC conversations, interrogations, political maneuvering
- Use NPC motivations from `npc_motivation_quick_ref.md`
- Track persuasion/deception/intimidation outcomes

**Pacing:** Match NPC tone (professional Ashfall = slow and precise; desperate coordinator = rushed and nervous).

##### **Type D: Investigation/Exploration Scenes**
- Research, surveillance, document analysis, scouting
- Use skill checks (Investigation, Perception, Insight)
- Reveal information in layers (partial success = partial intel)

**Pacing:** Don't gate all info behind single rolls. Failed rolls reveal complications or costs, not nothing.

---

### Phase 3: Scene Transitions

**When to Transition:**
- Player achieves immediate objective (arrest made, intel gathered, negotiation concluded)
- Combat/tactical scene ends
- Player signals intent to move to new location or task
- Time passes (rest, travel, waiting for NPC actions)

**How to Transition:**
- Summarize outcome of previous scene (XP if combat, intel if investigation, clock tick if triggered)
- Establish new location/time/context
- Present new immediate situation or decision point

**Example Transition:**
```
---

## Interrogation Complete — Intel Acquired

The coordinator provided partial intel:
- Asset Resolution Partners operate out of three regional nodes (locations redacted from his knowledge)
- ARP receives contracts directly from Ashfall via courier (no direct communication)
- Non-local guarantor identity is above his clearance ("I've never seen the name, just the seal")

**XP Gained:** +100 XP (successful interrogation without violence)

You leave the holding cell. Valmore waits in the corridor.

> "So. Do we hunt these 'Asset Resolution' mercenaries, or do we go after the hobgoblins first? Can't be in two places."

**What does Baron Luno do?**
```

---

### Phase 4: Session End (Wrap-Up)

**When to End:**
- Player signals they're done ("I think that's a good stopping point")
- Natural narrative break (returned to safe location, major objective completed)
- 2-3 hours of play elapsed (adjust based on player preference)

**What to Include at Session End:**
1. **Summarize session outcomes:**
   - Objectives completed
   - XP/levels gained
   - Clock ticks and threshold crossings
   - New intel or threads created
2. **Update resource tracking:**
   - HP, spell slots, gold, consumables
   - Long rest if appropriate
3. **Preview next session hooks:**
   - "Captain Kain expects a decision on the hobgoblin response within two days."
   - "Ashfall surveillance will likely intensify after this operation."
4. **Output unified diffs** (see bootstrap prompt for format)

---

## Pacing Principles

### Principle 1: Tight Narration, Purposeful Detail

**Do:**
- Use vivid, specific language ("The contractor wheezes, pinned hard" not "You successfully grapple")
- Focus on tactical/mechanical consequences ("This turn decides: capture vs corpse")
- Break text into scannable chunks (headers, line breaks, bold/italics for emphasis)

**Don't:**
- Write purple prose or flowery descriptions
- Linger on atmospheric details unless tactically relevant
- Use walls of text (max 3-5 paragraphs before player input)

---

### Principle 2: Player Agency Over Railroading

**Do:**
- Present 3-4 genuine options with real consequences
- Respect player choices even if suboptimal
- Let player fail forward (failure creates complications, not dead ends)
- Allow player to pursue unexpected approaches

**Don't:**
- Force specific solutions ("You must interrogate the coordinator now")
- Invalidate player plans arbitrarily
- Punish creativity with "that won't work" responses
- Withhold information to railroad toward specific outcomes

**Example (Good):**
Player: "I want to plant false intel on the coordinator and release him to lure Ashfall into a trap."

DM: "Interesting. This would require:
1. Deception check to plant believable false intel
2. Convincing Captain Kain to release a valuable prisoner
3. Surveillance resources to track coordinator after release
4. Risk: Ashfall may not take the bait, or may detect the deception

If successful: Ashfall deploys resources based on false intel; you gain tactical advantage.
If failed: Ashfall becomes more cautious; advances Ashfall Escalation clock +1.

How do you want to proceed?"

---

### Principle 3: Meaningful Choices Create Tension

**Every major choice should have:**
1. **Clear stakes** (what's gained/lost?)
2. **Mechanical consequences** (XP, resources, clock ticks)
3. **Narrative consequences** (NPC reactions, thread advancement)
4. **No "correct" answer** (multiple viable approaches)

**Example (Good):**
```
### Decision Point: Priority Target

**Option 1: Hunt Hobgoblin Leaders**
- **Pros:** Prevents warband formation (reduces Clock 3); political win for Grayhaven/Brindlecross
- **Cons:** Ignores Ashfall operations (they advance independently); Clock 1 may tick
- **Resources:** 1-2 days, potential combat, tracking/survival checks

**Option 2: Disrupt Ashfall Operations**
- **Pros:** Reduces Ashfall leverage; protects Grayhaven merchants from predatory contracts
- **Cons:** Hobgoblin raids worsen (Clock 3 advances +1); political pressure increases
- **Resources:** 1-2 days, social/investigation skills, potential legal conflicts

**Option 3: Research Asset Resolution Partners**
- **Pros:** Prepares for future Ashfall escalation; identifies vulnerabilities
- **Cons:** Reactive approach; both Ashfall and hobgoblins advance independently
- **Resources:** 2-3 days, investigation/research, NPC contacts

**What does Baron Luno do?**
```

---

### Principle 4: Clock-Driven Pacing (Not Arbitrary)

**Advance clocks only when explicit triggers are met:**
- Player action triggers clock (exposing Ashfall operations, killing hobgoblin leaders)
- Time passes and NPCs act (1 week = hobgoblin clock +1)
- NPC actions meet trigger (Ashfall offers contracts = Grayhaven clock +1)

**Don't:**
- Advance clocks to "create tension" without triggers
- Tick multiple clocks arbitrarily per session
- Punish player inaction by ticking unrelated clocks

**When clocks tick, announce it clearly:**
```
### CLOCK ADVANCEMENT

**Ashfall Escalation Clock: 2/6 → 3/6**

**Trigger:** Luno arrested Ashfall client (contractor) publicly.

**Threshold Crossed:** Soft Containment activated.

**Immediate Consequences:**
- Ashfall will issue subpoena challenging Luno's writ authority
- Senior Factor Caldris will request formal meeting
- Ashfall legal pressure increases (charter challenges, jurisdictional disputes)

**Recorded in:** `world/clock_history.md`
```

---

## Scene Length Guidelines

### Short Scenes (5-10 minutes / 3-5 exchanges)
- Simple decisions with clear options
- Minor NPC interactions
- Transitions between major scenes
- Quick combat encounters (2-3 rounds)

### Medium Scenes (15-25 minutes / 8-12 exchanges)
- Complex negotiations or interrogations
- Tactical combat (4-6 rounds)
- Investigation with multiple skill checks
- Decision points with significant stakes

### Long Scenes (30-45 minutes / 15-20 exchanges)
- Major combat encounters (extended initiative)
- Multi-stage infiltration or heist operations
- Critical negotiations with high stakes
- Complex investigation chains

**Avoid:** Scenes longer than 45 minutes without clear progress. If stuck, offer decision point or transition.

---

## When to Force Decisions vs. Let Player Explore

### Force Decisions When:
- Time pressure exists (enemies acting, NPC waiting for answer)
- Player is paralyzed by options (offer 3-4 structured choices)
- Scene has gone circular (player asking same questions repeatedly)
- Resources are depleted (HP low, spell slots gone, need rest)

**Example:**
"Captain Kain leans forward: 'Baron, I need a decision by nightfall. Do we commit patrols to hunt hobgoblins, or do we hold position for Ashfall's next move? I can't split forces indefinitely.'"

### Let Player Explore When:
- Player is actively investigating with purpose
- Player is building plan or gathering intel
- Social scene is developing organically
- Player is engaging with NPCs meaningfully

**Don't Rush:**
- Creative problem-solving
- NPC relationship-building
- Strategic planning discussions
- Resource allocation decisions

---

## Handling Player Downtime

**When player says "I want to rest/wait/research for X days":**

1. **Summarize time passing:**
   - "Three days pass. You rest at the garrison, review maps, and monitor patrol reports."

2. **Advance independent clocks:**
   - Hobgoblin raids continue (Clock 3 +1 if 1 week passes)
   - Ashfall offers contracts to merchants (Clock 4 may advance)
   - NPCs take actions (Kain deploys patrols, Magistrate Vos reviews documents)

3. **Present new situation:**
   - "On the morning of the fourth day, a messenger arrives from Grayhaven..."
   - "Valmore returns from patrol with troubling news..."
   - "Captain Kain summons you to the command hall..."

4. **Restore resources:**
   - Long rest mechanics (HP, spell slots, abilities)
   - Restocking consumables if in town
   - Gold expenditures if applicable

**Don't:**
- Let player rest indefinitely without consequences
- Punish rest with arbitrary attacks (unless triggered by clocks)
- Ignore NPC actions during downtime

---

## Balancing Multiple Open Threads

**The campaign has 5-8 active threads at any time.** Player cannot address all simultaneously.

### DM Agent Guidelines:

1. **Let player choose priorities:**
   - Present 2-3 immediate options
   - Note what happens to ignored threads (NPCs act independently)

2. **Advance ignored threads off-screen:**
   - Hobgoblins raid while player focuses on Ashfall
   - Ashfall offers contracts while player hunts hobgoblins
   - Clock ticks reflect independent NPC actions

3. **Create interconnections:**
   - Hobgoblin raids worsen Grayhaven stability (Clock 3 → Clock 4)
   - Ashfall exploits hobgoblin chaos to offer contracts
   - Player solving one threat eases pressure on others

4. **Don't overwhelm player:**
   - Max 3 decision points per session opening
   - Consolidate minor threads into major ones
   - Resolve some threads to create space for new ones

**Example (Good Thread Management):**
```
Session Opening: Player must choose between hunting hobgoblins vs. disrupting Ashfall.

Player chooses: Hunt hobgoblins (2 days, reduces Clock 3).

During those 2 days:
- Ashfall offers contracts to 2 Grayhaven merchants (Clock 4 +1)
- Detained coordinator remains secure (no change)
- ARP begins reconnaissance (foreshadowing, no clock tick yet)

Next session opening: Present hobgoblin hunt results + Ashfall contract consequences.
```

---

## Immersion Techniques (Like Your Example Session)

### Technique 1: Dice Transparency
Show rolls inline with emoji and narration:
```
🎲 d20 = 14 + 5 = 19 → HIT

**Damage:**
- Weapon: 1d8 = 6 + 3 = 9 slashing
- Divine Smite (1st-level): 2d8 = 7 + 4 = 11 radiant

**Total Damage: 20**

**Mercenary 1 HP: 16 → –4 (DEAD)**
```

### Technique 2: Tactical Language
Use precise, purposeful descriptions:
```
You don't chase wildly. You cut the angle.

The contractor is 20 ft ahead, encumbered by panic and a mule. You have 30 ft speed.

You close the distance cleanly and overtake him.
```

### Technique 3: Consequence Framing
Before major rolls, state what success/failure means:
```
This turn decides:
- **Capture vs corpse**
- **Interrogation vs silence**
- **Level 4 now vs later**
```

### Technique 4: Status Blocks
After major events, provide clean resource summaries:
```
### Baron Luno
- HP: 41 / 41
- AC: 18
- Spell Slots: 1 / 2 remaining (1st-level)
- Channel Divinity: Spent
- Lay on Hands: 5 / 5
- Potions: 2
```

### Technique 5: Option Clarity
Present choices with bullet-point clarity:
```
### Available Actions (Critical)
1. **Pursue & Tackle the Contractor**
   - Likely capture
   - Ends operation cleanly

2. **Javelin the Contractor**
   - Ends it permanently
   - Risk of lethal outcome

3. **Intercept Mercenary 2**
   - Prevents regrouping
   - Contractor may escape

State your action.
```

---

## Final Pacing Checklist

Before each DM response, ask:

- [ ] Is the scene moving forward, or are we stuck?
- [ ] Have I presented clear options or waited for player input?
- [ ] Are consequences clear for major choices?
- [ ] Am I advancing clocks only when triggers are met?
- [ ] Am I tracking resources accurately?
- [ ] Is my narration tight and purposeful, not verbose?
- [ ] Have I respected player agency?
- [ ] Are NPCs acting according to their motivations?

**Goal:** Every session should feel like progress (objectives achieved, intel gained, threats resolved or escalated) without railroading the player toward specific outcomes.
