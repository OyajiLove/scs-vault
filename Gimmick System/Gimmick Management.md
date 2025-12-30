# Gimmick Management

📛 **MECHANIC:** Gimmick Management
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** repackage, gimmick change, evolution, reversion, dual identity
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 1-4 | Repackaging and character changes discussed in context of booking decisions; "dual identity" (e.g., Mankind/Cactus Jack) referenced informally |
| v2.0 | Vol 6 | **LOCKED** - Full management action set defined: Repackage, Evolution, Reversion, Dual Identity, AI Override, Worker-Driven Shift. Memory effects specified |

---

## Overview

Tools and options for modifying a worker's gimmick over time. Gimmicks aren't static; they can evolve, be replaced, or return from the past.

---

## Management Actions

| Action | Description |
|--------|-------------|
| **Repackage** | Complete gimmick replacement (new name, look, alignment) |
| **Evolution** | Gradual change within same identity (darker Stone Cold) |
| **Reversion** | Return to previous gimmick (Cactus Jack returns) |
| **Dual Identity** | Worker alternates between gimmicks (Finn/The Demon) |
| **AI Override** | System forces change due to crowd rejection |
| **Worker-Driven Shift** | Worker's [[Hidden_Personality|personality]] causes organic change |

---

## Repackage

Full gimmick replacement:

| Factor | Consideration |
|--------|---------------|
| **When to use** | Burnout stage, failed debut, major storyline shift |
| **Risk** | Crowd may reject new character |
| **Benefit** | Fresh start, escape bad booking history |
| **Memory effect** | Old gimmick enters [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] as separate entity |

---

## Evolution

Gradual shift within same identity:

| Factor | Consideration |
|--------|---------------|
| **When to use** | Stagnation, natural character growth, heel/face drift |
| **Risk** | May feel forced if too sudden |
| **Benefit** | Maintains continuity, feels organic |
| **Memory effect** | Same gimmick, new chapter |

---

## Reversion

Return to previous gimmick:

| Factor | Consideration |
|--------|---------------|
| **When to use** | New gimmick failed, nostalgia play, special occasion |
| **Risk** | Diminishing returns on repeated reversions |
| **Benefit** | Nostalgia pop, proven commodity |
| **Memory effect** | Reactivates old memories, potential callback feuds |

---

## Dual Identity

Worker maintains two active gimmicks:

| Example | Normal | Alter Ego |
|---------|--------|-----------|
| Finn Bálor | Technical face | The Demon (special matches only) |
| Mick Foley | Mankind | Cactus Jack (hardcore mode) |
| Keiji Mutoh | Technical ace | Great Muta (paint, mist, brutality) |

Rules:
- Only one active at a time
- Switching has cooldown period
- Each identity tracks separate Buzz/memory
- Alter ego typically reserved for big matches

---

## AI Override

System forces gimmick change when:

- Crowd rejection sustained over X weeks
- Buzz drops below threshold despite push
- Worker personality conflicts with current gimmick

Override options:
- Suggest repackage to booker
- Organic heel/face drift
- Forced time off for "injury" reset

---

## Worker-Driven Shift

Worker's Tags/Personality cause organic change:

| Tag | Potential Shift |
|----|-----------------|
| "Egotist" | Heel drift if not pushed properly |
| "Loyal" | Resists heel turn booking |
| "Chaotic" | Unpredictable character evolution |
| "Methodical" | Slow, deliberate gimmick changes |

---

## Connected Mechanics

- [[Gimmick Lifecycle]] - management actions move between stages
- [[Gimmick Attributes]] - what changes during management
- [[Turn_Engine]] - alignment shifts processed separately

---

## Open Questions

- Repackage success rate formula?
- Dual Identity limits (max 2? 3?)
- Worker consent mechanics for forced changes?

---

## Implementation Notes

```json
{
  "management_action": {
    "worker_id": "w_001",
    "action_type": "repackage",
    "old_gimmick_id": "gim_001",
    "new_gimmick_id": "gim_002",
    "reason": "burnout_recovery",
    "date": "2025-03-15",
    "success_probability": 0.65
  }
}
```
