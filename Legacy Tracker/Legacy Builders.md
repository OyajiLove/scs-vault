# Legacy Builders

📛 **MECHANIC:** Legacy Builders
🔗 **PARENT SYSTEM:** [[_Legacy Tracker Index|Legacy Tracker]]
🧭 **CATEGORY:** Career & Recognition
🔑 **KEYWORDS:** legacy growth, title reigns, iconic matches, milestone events
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

Events and achievements that increase a worker's [[Legacy Scale|Legacy Score]]. Unlike [[Buzz Inputs|Buzz]], Legacy grows slowly and accumulates over years.

---

## Major Legacy Builders

| Event | Legacy Gain |
|-------|-------------|
| World title reign | +5 to +15 (based on reign quality) |
| Iconic match | +3 to +8 (5-star caliber, memorable) |
| Career-defining feud | +3 to +5 |
| Cross-promotional appearance | +2 to +4 |
| Mainstream crossover | +5 to +10 |
| Mentoring future star | +2 to +5 |
| Innovation (move, match type) | +3 to +8 |

---

## Title Reign Quality

Not all title reigns build equal Legacy:

| Reign Type | Legacy Gain |
|------------|-------------|
| Transitional (< 1 month) | +1 to +2 |
| Standard (1-6 months) | +3 to +5 |
| Dominant (6+ months, quality defenses) | +8 to +12 |
| Record-breaking | +10 to +15 |
| Forgettable (no memorable moments) | +1 |

---

## Match Legacy

Matches that build Legacy:

| Match Type | Legacy Gain |
|------------|-------------|
| 5-star classic | +5 to +8 |
| MOTY candidate | +3 to +5 |
| Historically significant (first of its kind) | +5 to +10 |
| Career-defining (Undertaker's Streak matches) | +3 to +5 each |
| Retirement match (good send-off) | +3 to +8 |

---

## Cultural Impact Builders

| Event | Legacy Gain |
|-------|-------------|
| Catchphrase enters popular culture | +5 to +10 |
| Referenced in non-wrestling media | +2 to +5 |
| Magazine covers, mainstream interviews | +2 to +4 |
| Movie/TV appearances | +3 to +8 |
| Political/social significance | +5 to +15 |

---

## Connected Mechanics

- [[Legacy Scale]] - what's being built
- [[Legacy Modifiers]] - affects growth rate
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - major builders create snapshots

---

## Open Questions

- Dark match/house show Legacy building?
- Social media era Legacy building (modern feds)?
- Negative event Legacy damage amounts?

---

## Implementation Notes

```json
{
  "legacy_event": {
    "worker_id": "w_001",
    "event_type": "world_title_reign",
    "event_date": "2024-04-07",
    "base_gain": 8,
    "quality_modifier": 1.25,
    "final_gain": 10,
    "reign_details": {
      "title": "WWE Championship",
      "length_days": 245,
      "defenses": 8,
      "memorable_moments": 3
    }
  }
}
```
