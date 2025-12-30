# Gimmick vs Tags

📛 **MECHANIC:** Gimmick vs Tags
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** gimmick distinction, tags distinction, character vs performer, kayfabe vs shoot
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 1-3 | Tags System developed; gimmick concept referenced but distinction not formalized |
| v1.5 | Vol 4 | Hidden Personality system solidified separation between "real performer" and "presented character" |
| v2.0 | Vol 6 | **LOCKED** - Explicit distinction codified: Tags = who you are underneath, Gimmick = who fans see. Conceptual framing formalized |

---

## Overview

One of the most important conceptual distinctions in SCS. Confusing Gimmicks and Tags leads to broken booking logic and unrealistic character behavior.

---

## The Core Distinction

| Aspect | Tags | Gimmick |
|--------|------|---------|
| **What it represents** | The actual performer underneath | The character fans see |
| **Persistence** | Permanent (personality, background) | Can change (repackage, evolution) |
| **Visibility** | Hidden from audience | Publicly presented |
| **Example** | "Loyal," "Anxious," "Former Amateur" | "The Undertaker," "Stone Cold" |

---

## Conceptual Framing

**Tags = Who you are underneath**
- Your [[Hidden_Personality|Hidden Personality]] traits
- Your background and training
- Your real psychological makeup
- What drives your decisions when the cameras aren't rolling

**Gimmick = Who the fans see**
- Your ring name and presentation
- Your alignment (face/heel)
- Your signature catchphrases and mannerisms
- The story you're telling in the ring

---

## Why It Matters

### Booking Logic

A worker with the Tag "Loyal" might:
- Refuse to turn heel even if booked to
- Generate [[Push Resistance]] if forced into betrayal angles
- Need special handling for heel turns (injury angle, desperation)

But their Gimmick can still be a villain if the character is written that way.

### Character Consistency

A worker with the Tag "Anxious" playing a confident heel gimmick:
- Promos might crack under pressure
- Big match nerves affect performance
- Authentic moments bleed through the character

### Memory and Legacy

[[Fan Memory Engine/_Fan Memory Index|Fan Memory]] tracks:
- Gimmick moments (the character's story)
- Tag-driven moments (when the real person showed through)

The most memorable moments often come from Tag bleeding into Gimmick.

---

## Examples

| Worker | Tags (Underneath) | Gimmick (Presented) |
|--------|-------------------|---------------------|
| Mick Foley | Intelligent, Pain Tolerance High, Loyal | Mankind (deranged), Cactus Jack (hardcore), Dude Love (comedy) |
| Glenn Jacobs | Professional, Business-Minded, Team Player | Kane (monster heel/face) |
| Mark Calaway | Locker Room Leader, Professional, Reserved | The Undertaker (supernatural icon) |

---

## Connected Mechanics

- [[Tags_System]] - the 394 tags defining workers
- [[Hidden_Personality]] - psychological traits underneath
- [[Gimmick Attributes]] - what defines the presented character
- [[Gimmick Management]] - changing the presented character

---

## Open Questions

- Tag/Gimmick conflict resolution rules (when they clash, what wins?)
- Can Tags change over career (growth, trauma)?

---

## Implementation Notes

Tags and Gimmicks are stored separately and cross-referenced:

```json
{
  "worker_id": "w_001",
  "tags": ["loyal", "locker_room_leader", "pain_tolerance_high"],
  "hidden_personality": {
    "drive": 18,
    "ego": 12,
    "loyalty": 16
  },
  "active_gimmick": {
    "gimmick_id": "gim_003",
    "ring_name": "The Undertaker",
    "alignment": "tweener"
  }
}
```
