# Match Simulation

📛 **MECHANIC:** Match Simulation (In-Match Flow)
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Match Simulation / Core Gameplay
🔑 **KEYWORDS:** match simulation, momentum meter, grapple timing, Fire Pro, move selection, spots, near falls
📌 **ORIGIN:** Vol 1 (conceptual), scattered references
✅ **STATUS:** 🔨 EXPLORATORY (Not Locked)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔨 EXPLORATORY |

---

## ⚠️ STATUS WARNING

This mechanic is **EXPLORATORY**. The vision exists but detailed specifications are not locked. This document captures the design intent for future development.

**What's Locked:**
- [[Match Inputs]] - booking decisions
- [[Match Processing]] - quality evaluation
- [[Match Consequences]] - outcome effects

**What's Exploratory:**
- Moment-to-moment match flow
- Move selection and execution
- Timing windows and counters
- AI decision trees

---

## Design Vision

From Vol 1: "Fire Pro-style grapple timing + AI logic trees + emergent storytelling"

The goal is matches that feel like they're happening organically, with crowd reactions, momentum swings, and narrative moments emerging from gameplay rather than being scripted.

---

## Conceptual Components

### Momentum Meter

| Concept | Description |
|---------|-------------|
| **Scale** | 0-100 for each worker |
| **Starts at** | Neutral (50-50) or asymmetric based on story |
| **Swings** | Successful moves increase, failed moves decrease |
| **Threshold effects** | At 80+, finisher becomes viable; at 20-, risk of loss |

### Grapple Timing (Fire Pro Style)

| Concept | Description |
|---------|-------------|
| **Lock-up** | Workers engage in grapple |
| **Timing window** | Input determines who gets advantage |
| **Move selection** | Winner of exchange picks move |
| **Counters** | Defender may reverse with good timing |

### Move Selection

| Factor | Influence |
|--------|-----------|
| **Worker skills** | Available moves in repertoire |
| **Momentum level** | Bigger moves at higher momentum |
| **Match type** | Some moves only in certain types |
| **Opponent condition** | Targeting injured body parts |
| **House style** | Promotion norms affect selection |

### Spot Execution

| Element | Description |
|---------|-------------|
| **Signature moves** | Worker's known sequences |
| **Finishers** | Protected moves that can end match |
| **High spots** | Risk/reward spectacular moves |
| **Callbacks** | References to past matches |
| **Botches** | Failed execution, injury risk |

### Signature Spot System (#211)

**Core Concept:** Workers have signature sequences fans expect.

| Spot Type | Pop Effect |
|-----------|------------|
| **Signature Setup** | Recognition pop when initiated |
| **Signature Spot** | Full pop on execution |
| **Finisher Tease** | Massive pop on kickout |
| **Stolen Finisher** | Huge pop, used rarely |
| **Tribute Move** | Nostalgic pop, context-dependent |

**Freshness:** Using same spots repeatedly diminishes returns.  
**Innovation:** New spots can become signatures over time.

---

## Crowd Reaction Flow

Crowds react to in-match moments:

| Moment | Reaction |
|--------|----------|
| **Big move lands** | Pop based on move impact |
| **Near fall** | Escalating drama |
| **Kickout** | Relief or frustration |
| **Comeback** | Building energy |
| **Finisher tease** | Major pop |
| **Finisher hit** | Climax |
| **Heel cheating** | Boos/heat |
| **Face overcoming** | Cheers/hope |

---

## AI Worker Behavior

Workers as autonomous agents:

| Behavior | Description |
|----------|-------------|
| **Competitive** | Trying to win within kayfabe |
| **Professional** | Following agenting/layout |
| **Selfish** | Protecting themselves, no-selling |
| **Giving** | Putting over opponent |
| **Chaotic** | Going off-script |

Hidden Personality affects behavior:
- High Ego → May no-sell or hog offense
- High Loyalty → Follows booking exactly
- High Risk-Taking → Attempts dangerous spots

---

## Implementation Path

### MVP (Abstract Resolution)

For MVP, matches are resolved abstractly:
1. Take [[Match Inputs]]
2. Apply [[Match Processing]] modifiers
3. Generate [[Match Consequences]]
4. LLM describes key moments narratively

No moment-to-moment simulation. Quality determined by inputs + RNG + modifiers.

### Future (Detailed Simulation)

Post-MVP, add:
1. Turn-based or real-time match flow
2. Move databases for each worker
3. Timing windows and counters
4. Visual match representation
5. Commentary integration

---

## Fire Pro Inspiration

Elements to potentially adapt:

| Fire Pro Element | SCS Adaptation |
|------------------|----------------|
| **Grapple timing** | Skill-based move advantage |
| **Spirit meter** | Momentum + fighting spirit |
| **CPU logic** | Hidden Personality influences |
| **Edit mode** | Worker creator with move sets |
| **Critical system** | Finisher protection |

---

## Open Questions (Many)

- Is this turn-based, real-time, or hybrid?
- How much player input vs AI control?
- Move database scope (hundreds? thousands?)
- Animation/visual representation
- Match length mechanics
- Stamina/fatigue modeling
- Injury system integration
- Tag team coordination
- Multi-man match flow

---

## Connected Mechanics

- [[Match Inputs]] - locked, feeds simulation
- [[Match Processing]] - locked, evaluates result
- [[Match Consequences]] - locked, propagates effects
- [[Worker_Skills|Worker Skills]] - base capabilities
- [[Hidden_Personality|Hidden Personality]] - AI behavior

---

## Implementation Notes

```json
{
  "match_simulation_concept": {
    "status": "exploratory",
    "mvp_approach": "abstract_resolution",
    "future_approach": "detailed_simulation",
    "inspiration": "fire_pro_wrestling",
    "key_elements": [
      "momentum_meter",
      "grapple_timing",
      "move_selection",
      "crowd_reactions",
      "ai_behavior"
    ],
    "open_design_questions": 10,
    "estimated_scope": "post_mvp"
  }
}
```
