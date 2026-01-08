# DM Interaction Protocol (Canon)

*This file defines how DM agents should present decisions, ask for rolls, handle player input, and maintain immersion. This is the "player interface" for agent-driven DMing.*

---

## Core Principle: Player Agency + Clear Stakes

**The player should always know:**
1. What options are available
2. What each option might achieve or cost
3. What rolls/resources are required
4. What consequences follow their choice

**The DM should never:**
- Force specific actions ("You must do X")
- Hide critical information arbitrarily
- Invalidate creative approaches without justification
- Make decisions for the PC (Luno's choices are player's choices)

---

## Decision Presentation Format

### When to Use This Format
- Major tactical decisions (combat options, target selection)
- Strategic choices (priority targets, resource allocation)
- Social decisions (negotiation approaches, interrogation methods)
- Moral/ethical choices (lethal vs. non-lethal, law vs. expediency)

### Standard Format

```markdown
## SCENE CONTEXT — [Location/Situation]

[2-4 paragraphs of concise scene-setting: where, who, what just happened, immediate threats/opportunities]

### Available Options ([Descriptor: Critical/Immediate/Strategic])

1. **[Option Name]**
   - [What this option involves]
   - [Primary benefit or goal]
   - [Risk or cost]
   - [Mechanical requirement if relevant]

2. **[Option Name]**
   - [What this option involves]
   - [Primary benefit or goal]
   - [Risk or cost]
   - [Mechanical requirement if relevant]

3. **[Option Name]**
   - [What this option involves]
   - [Primary benefit or goal]
   - [Risk or cost]
   - [Mechanical requirement if relevant]

4. **Other**
   - Be specific

[Optional: "This choice determines: X vs Y vs Z" framing]

**What does Baron Luno do?**
```

### Example (From Your Sample Session)
```markdown
## ROUND 2 — BARON LUNO ACTS SOON

This is now **control**, not combat.

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

4. **Command Surrender**
   - Intimidation check
   - Might freeze both

State your action.

This turn decides:
- **Capture vs corpse**
- **Interrogation vs silence**
- **Level 4 now vs later**

**What does Baron Luno do?**
```

---

## Requesting Rolls

### When to Ask for Rolls
- Player declares action with uncertain outcome
- Opposed check required (grapple, stealth vs. perception, deception vs. insight)
- Combat (attack rolls, saves, damage)
- Skill challenges (persuasion, investigation, athletics)

### Standard Roll Request Format

```markdown
**[Check Type]: [Skill/Save] ([DC/Opposed])**

[Brief explanation of what success/failure means]

**Request:** Roll [die] + [modifier]
```

### Example 1: Skill Check
```markdown
**Grapple Check: Athletics (Contested)**

You need to overpower the contractor before he reaches cover.

- **Your Roll:** d20 + 5 (STR Athletics)
- **His Roll:** d20 + 1 (DEX Acrobatics)

**Request:** Roll d20 for your Athletics check.
```

### Example 2: Attack Roll
```markdown
**Attack Roll: Longsword + Divine Smite**

**Target AC:** 15
**Advantage:** Yes (Vow of Enmity)

Roll **2d20** (take higher) + 5 for attack.

If you hit, declare whether you're using Divine Smite.
```

### Example 3: Saving Throw
```markdown
**Saving Throw: Dexterity (DC 14)**

The mercenary hurls a flask of alchemist's fire.

- **Success:** Half damage (2d6 fire / 2)
- **Failure:** Full damage (2d6 fire)

**Request:** Roll d20 + 1 (DEX save).
```

---

## Alternative: Agent Rolling (When Requested)

If the player asks the agent to roll:

```markdown
**Agent Rolling: [Check Type]**

🎲 d20 = 14 + 5 = **19 → SUCCESS**

[Immediate narration of result]
```

### Example (Agent Rolls Initiative)
```markdown
## INITIATIVE ROLLS

### Baron Luno
🎲 d20 –1 = 13 → **Initiative: 12**

### Mercenary 1 (Crossbow)
🎲 d20 +2 = 9 → **Initiative: 9**

### Mercenary 2 (Spear)
🎲 d20 +2 = 15 → **Initiative: 15**

### Contractor
🎲 d20 +0 = 6 → **Initiative: 6**

---

## INITIATIVE ORDER
1. Mercenary 2 (Spear) — 15
2. Baron Luno — 12
3. Mercenary 1 (Crossbow) — 9
4. Contractor — 6
```

---

## Handling Player Input

### Type 1: Clear, Actionable Input

**Player:** "I pursue and tackle the contractor."

**DM Response:**
```markdown
### Action Chosen: Pursue & Tackle the Contractor

You don't chase wildly. You cut the angle.

**Movement:** 30 ft speed; contractor is 20 ft away (encumbered).

You close the distance cleanly and overtake him.

**Grapple Check (Contested):**
- **You:** Athletics +5
- **Contractor:** Acrobatics +1

**Request:** Roll d20 for Athletics.
```

---

### Type 2: Vague or Incomplete Input

**Player:** "I want to deal with Ashfall."

**DM Response:**
```markdown
### Clarification Required

"Dealing with Ashfall" could mean several approaches:

1. **Disrupt their client operations** (arrest more contractors, sabotage contracts)
2. **Research their structure** (investigate Asset Resolution Partners, guarantor identity)
3. **Legal counterattack** (work with Magistrate Vos to challenge jurisdiction)
4. **Build political coalition** (unite Grayhaven/Brindlecross against Ashfall contracts)

Which approach interests you? Or do you have a different method in mind?
```

---

### Type 3: Creative/Unexpected Input

**Player:** "I want to plant false intel on the coordinator and release him to bait Ashfall into a trap."

**DM Response:**
```markdown
### Creative Approach: False Intel Bait Operation

Interesting. This is not a standard option, but it's viable. Here's what it would require:

**Requirements:**
1. **Deception Check (DC 16):** Plant believable false intel without coordinator detecting deception
2. **Persuasion Check (Captain Kain, DC 14):** Convince Brindlecross to release valuable prisoner
3. **Surveillance Resources:** Track coordinator after release (Snik can handle this with Stealth checks)
4. **Time Investment:** 2-3 days to set up and execute

**Potential Outcomes:**
- **Success:** Ashfall deploys resources based on false intel; you gain tactical advantage (ambush, intel on ARP methods)
- **Partial Success:** Coordinator released but Ashfall detects deception; advances Ashfall Escalation clock +1
- **Failure:** Coordinator warns Ashfall immediately; they become more cautious (hardens future operations)

**Risks:**
- Ashfall may not take the bait (they're professionally paranoid)
- Coordinator may leverage freedom to disappear entirely
- Captain Kain's trust depends on your justification

**Do you want to proceed with this plan? If so, what false intel do you want to plant?**
```

---

### Type 4: Indecisive or Paralyzed Input

**Player:** "I don't know what to do. There are too many threats."

**DM Response:**
```markdown
### Strategic Assessment: Priority Triage

You're right—there are multiple active threats. Here's a quick summary with recommendations:

**Immediate Threats (Next 2-3 Days):**
1. **Detained Coordinator** → Interrogate now before rescue attempts (Recommended: High Priority)
2. **Ashfall Surveillance** → Passively advancing; no immediate action required

**Short-Term Threats (Next 1-2 Weeks):**
3. **Hobgoblin Raids** → Worsening but not yet critical (Recommended: Medium Priority)
4. **Asset Resolution Partners** → Not yet deployed; research can wait

**From a tactical perspective:**
- **Interrogate coordinator first** (time-sensitive; gains intel on other threats)
- **Then address hobgoblins** (prevents warband formation)
- **Then research ARP** (prepares for future Ashfall escalation)

**However:** You don't have to follow this order. What feels most urgent to you?

Alternatively, if you want to delegate:
- Captain Kain can handle hobgoblin patrols (with mixed success)
- Brindlecross intel can interrogate coordinator (but you'll get better results personally)

**What's your instinct?**
```

---

## Handling Combat Decisions

### Initiative-Based Combat Flow

```markdown
## ROUND [X] — [Character Name] ([Initiative #])

[Brief situation summary: positioning, threats, allies, resources]

### Current Status
- **HP:** [current] / [max]
- **AC:** [value]
- **Resources:** [spell slots, abilities, reactions, concentration]
- **Conditions:** [prone, grappled, poisoned, etc.]

### Tactical Situation
[1-2 sentences describing immediate threats, opportunities, positioning]

### Available Actions
[List standard action options + any special context-specific options]

**Standard Options:**
- **Attack:** [weapon options with modifiers]
- **Cast Spell:** [available spells with effects]
- **Dash/Disengage/Dodge:** [movement/defense]
- **Use Item:** [potions, equipment]
- **Help/Grapple/Shove:** [support actions]

**Context-Specific:**
- [Any special tactical opportunities based on terrain, positioning, enemy state]

**What does Baron Luno do?**
```

### Example (Combat Decision Point)
```markdown
## ROUND 2 — BARON LUNO (Initiative 12)

Mercenary 1 is dead (Divine Smite). Mercenary 2 is Disengaging toward the contractor. Contractor is fleeing with the ledger satchel.

### Current Status
- **HP:** 41 / 41
- **AC:** 18
- **Spell Slots:** 1 / 2 (1st-level)
- **Channel Divinity:** Spent (Vow of Enmity)
- **Lay on Hands:** 25 / 25
- **Reaction:** Available

### Tactical Situation
You're 20 ft from the fleeing contractor (encumbered, panicking). Mercenary 2 is between you and him, retreating. This is now **control**, not combat.

### Available Actions

**Movement Options:**
1. **Pursue Contractor** (30 ft speed; can overtake him)
2. **Intercept Mercenary 2** (20 ft; blocks his retreat)
3. **Hold Position** (defensive stance)

**Combat Options:**
4. **Javelin the Contractor** (ranged attack; 30 ft; risk of lethal damage)
5. **Attack Mercenary 2** (melee; prevents his escape)
6. **Grapple Contractor** (if pursued; Athletics check)

**Social Options:**
7. **Command Surrender** (Intimidation check; might freeze both)

**This turn decides:**
- **Capture vs corpse**
- **Interrogation vs silence**
- **XP threshold for Level 4**

**What does Baron Luno do?**
```

---

## Presenting NPC Reactions

### When NPCs Respond to Player Actions

**Format:**
```markdown
### [NPC Name] Reacts

[1-2 sentences describing NPC's emotional/tactical response]

> "[Direct quote from NPC]"

[NPC's action or decision]

[Mechanical consequence if relevant: clock tick, new thread, resource change]
```

### Example 1: Friendly NPC
```markdown
### Captain Kain Reacts

Kain leans back, arms crossed, considering your plan.

> "Bold. Risky. But if you can pull it off, we'll have actionable intel on Asset Resolution Partners. You'll need Magistrate Vos to sign off on the release—she won't approve without ironclad justification."

**Mechanical Note:** Requires Persuasion check (DC 14) to convince Magistrate Vos.
```

### Example 2: Adversarial NPC
```markdown
### Senior Factor Caldris Reacts

Caldris's expression doesn't change, but his fingers tap the desk twice—a tell.

> "How... industrious. You've arrested one of our clients. That does complicate matters. We'll need to review jurisdictional authority. Expect formal correspondence within three days."

**CLOCK ADVANCEMENT: Ashfall Escalation 2/6 → 3/6**
**Trigger:** Arrest of Ashfall client
**Consequence:** Soft containment begins (subpoenas, legal harassment)
```

### Example 3: Desperate NPC
```markdown
### Regional Coordinator Reacts

The coordinator's eyes widen. His voice cracks.

> "You don't understand—if I tell you everything, the Hellsbind activates. I've seen what happens. But... but if you can protect me, really protect me, not just lock me in a cell... I'll tell you about the couriers. About the nodes. About the *seal*."

**Decision Point:** Do you offer protection (binds you to his safety) or press without guarantees?
```

---

## Consequence Narration

### When Player Actions Have Outcomes

**Format:**
```markdown
## [Outcome Type] — [Consequence Summary]

[Immediate result narration]

**Mechanical Effects:**
- [XP, resources, clock ticks, NPC reactions]

**Narrative Effects:**
- [New threads, changed relationships, intel gained]

[Transition to next scene or decision point]
```

### Example 1: Combat Victory
```markdown
## COMBAT ENDS — CONTRACTOR CAPTURED

You bind the contractor's hands and drag him off the road. The mercenary with the spear is gone—fled into the fields. No witnesses. The mule has bolted, but the ledger satchel is intact.

**Mechanical Effects:**
- **XP Gained:** +450 XP (mercenary neutralized, contractor captured, clean operation)
- **Total XP:** 1,750 → 2,200 XP
- **LEVEL UP:** Baron Luno reaches **Level 4** (apply after rest)
- **Resources Spent:** 1 spell slot (Divine Smite), Channel Divinity (Vow of Enmity)

**Narrative Effects:**
- **Contractor is captive:** Interrogation opportunity (immediate or transport to Brindlecross)
- **Ledger secured:** Contains evidence of consortium operations
- **Mercenary escaped:** Will report to consortium; advances enemy awareness

**What does Baron Luno do next?**
1. Interrogate contractor immediately (field interrogation)
2. Transport to Brindlecross for formal detention
3. Search ledger for immediate intel
```

### Example 2: Social Victory
```markdown
## MAGISTRATE VOS CONVINCED — LEGAL COVER SECURED

Magistrate Vos reviews your documentation, then signs the writ extension.

> "Your arrests are legally sound. Ashfall will challenge jurisdiction, but they'll lose. Keep your operations clean, and I'll keep providing cover."

**Mechanical Effects:**
- **Brindlecross Legitimacy Clock:** No change (legal cover maintained)
- **New Resource:** Magistrate Vos as active ally (legal guidance, document access)

**Narrative Effects:**
- **Ashfall legal challenge weakened:** Jurisdiction dispute will favor Luno
- **Magistrate Vos trusts Luno:** Future requests will be easier (DC –2)
- **Grayhaven officials aware:** Some will view Luno as legitimate; others as threat

**Next Scene:** Captain Kain awaits your report at Brindlecross garrison.
```

### Example 3: Failure with Complications
```markdown
## INTERROGATION INCOMPLETE — COORDINATOR RESISTS

The coordinator clams up. He's calculating, testing how much he can withhold.

> "I told you—I'm just an accountant. I don't know where the Asset Resolution Partners operate. That's above my clearance."

**Mechanical Effects:**
- **Intel Gained:** Partial (confirms ARP exists, but no locations/leaders)
- **Time Spent:** 1 hour (no other resource cost)

**Narrative Effects:**
- **Coordinator remains uncooperative:** Requires different approach (intimidation, deal-making, time pressure)
- **Ashfall rescue window narrows:** Each day of detention increases rescue/elimination risk
- **Captain Kain watching:** Will judge your interrogation effectiveness

**Available Options:**
1. **Intimidation approach** (Intimidation check, DC 14; risk: damages future cooperation)
2. **Offer protection deal** (Persuasion check, DC 12; binds you to his safety)
3. **Let him stew** (wait 1-2 days; he may break under isolation)
4. **Other approach**

**What does Baron Luno do?**
```

---

## Session End Protocol

### When Player Signals End or Natural Break Occurs

```markdown
## SESSION END — [Session Number]

### Session Summary
- **Objectives Completed:** [list major accomplishments]
- **XP Gained:** [total for session]
- **Clock Advances:** [list any clock ticks with triggers]
- **New Threads Created:** [list any new open threads]

### Resource Update
**Baron Luno:**
- **HP:** [current] / [max]
- **Spell Slots:** [current] / [max per level]
- **Lay on Hands:** [current] / [max]
- **Channel Divinity:** [spent/available]
- **Potions/Consumables:** [list]
- **Gold:** [amount]

**Valmore & Snik:**
- [HP and resource updates if relevant]

### Long Rest (If Applicable)
- All HP restored
- All spell slots restored
- All short rest abilities restored
- [Any long rest restrictions or conditions]

### Next Session Hooks
- [2-3 immediate threads or decision points for next session]

**Next session opens with:** [brief scene setup]

---

### Unified Diffs Output
[Wait for player confirmation before outputting diffs]

Output format:
1. `sessions/session_log_XX.md`
2. `world/world_state.md` (minimal diffs)
3. `world/active_clocks.md` + `world/clock_history.md`
4. Character sheets (resource updates)
5. `system/errata.md` (if needed)
```

---

## Final Checklist for DM Agents

Before each response to the player:

- [ ] Have I presented clear options with mechanical stakes?
- [ ] Have I requested specific rolls if actions are uncertain?
- [ ] Have I narrated consequences immediately after resolution?
- [ ] Have I respected player agency (no forced actions)?
- [ ] Have I maintained tone (tactical realism, bureaucratic horror, gritty subtlety)?
- [ ] Have I tracked resources accurately?
- [ ] Have I advanced clocks only when triggers are met?
- [ ] Have I ended responses with clear player decision point?

**Goal:** The player should always know what their options are, what the stakes are, and what happens next. No ambiguity, no railroading, no missing information.
