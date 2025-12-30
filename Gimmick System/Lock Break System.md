# Lock Break System

📛 **MECHANIC:** Lock Break System
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** lock break, shattered gimmick, catastrophic failure, legacy damage
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 6 | **LOCKED** - Break triggers defined (scandal, burial, shoot incident, criminal conviction, company collapse). Severity levels (Cracked → Erased) and recovery paths specified. Real-world examples codified |

**Note:** Introduced alongside Iconic Lock and Decay in Vol 6 as the failure-state mechanic. The Benoit example establishes the "Erased" tier as canonical.

---

## Overview

When [[Iconic Lock Decay]] reaches critical levels, or a catastrophic event occurs, the lock can shatter entirely. This is rare but devastating, fundamentally changing how fans perceive the gimmick.

---

## Break Triggers

| Trigger | Severity |
|---------|----------|
| **Major scandal** | Immediate break risk |
| **Sustained burial** | Gradual break over months |
| **Shoot incident** | Context-dependent |
| **Criminal conviction** | Near-automatic break |
| **Company collapse** | Regional break (WCW death affecting WCW-only icons) |
| **Death under bad circumstances** | Complex (can freeze or break) |

---

## Break Severity Levels

| Level | Effect |
|-------|--------|
| **Cracked** | Lock weakened, recovery possible |
| **Fractured** | Significant damage, difficult recovery |
| **Shattered** | Lock destroyed, gimmick becomes liability |
| **Erased** | Promotion pretends gimmick never existed |

---

## Post-Break States

| State | Description |
|-------|-------------|
| **Rebuild possible** | Worker can attempt new Iconic Lock with same or new gimmick |
| **Diminished legacy** | Gimmick remembered but with asterisk |
| **Toxic association** | Any mention damages associated workers/promotions |
| **Selective memory** | Fans remember peak, ignore fall |

---

## Recovery Paths

| Path | Requirements |
|------|--------------|
| **Time heal** | Extended absence, let memories fade |
| **Reinvention** | New gimmick, distance from old |
| **Redemption arc** | Acknowledge fall, earn back trust |
| **Context shift** | New promotion, new audience |
| **Death freeze** | Passing can freeze legacy at last good point |

---

## Real-World Examples

| Worker | Break Type | Recovery |
|--------|------------|----------|
| Hulk Hogan (2015) | Scandal | Partial rebuild, diminished |
| Chris Benoit | Catastrophic | Erased, no recovery |
| Ric Flair (late career) | Gradual decay | Selective memory |
| Ultimate Warrior | Company conflict | Time heal + death freeze |

---

## Connected Mechanics

- [[Iconic Lock]] - what's being broken
- [[Iconic Lock Decay]] - the process leading to break
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - break creates negative memories
- [[Cultural Immortality]] - can be lost via break

---

## Open Questions

- Can broken locks ever fully recover to previous peak?
- Inheritance effects (does breaking Hogan affect nWo members?)
- Simulation ethics: how to handle real-world tragedies?

---

## Implementation Notes

```json
{
  "gimmick_id": "gim_001",
  "lock_break": {
    "status": "fractured",
    "break_date": "2015-07-24",
    "break_trigger": "scandal",
    "pre_break_legacy": 92,
    "post_break_legacy": 65,
    "recovery_attempts": [
      {"date": "2018-04-08", "event": "wrestlemania_return", "result": "partial"}
    ],
    "toxic_association": false
  }
}
```
