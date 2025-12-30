# Garbage Throwing

📛 **MECHANIC:** Garbage Throwing
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** garbage throwing, riot, crowd escalation, physical response, ECW, territory
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

Certain crowd cultures escalate to physical response. This is rare, era-locked, and region-locked. When it happens, it's a major event that affects booking, memory, and worker morale.

---

## Triggers

| Trigger Type | Effect |
|--------------|--------|
| **Cultural Flag Active** (Southern US) | Enables throwing |
| **Heat Overflow** | Heel does too good a job or commits sacred betrayal |
| **Booking Violation** | Workrate star buried, local hero humiliated |
| **Nostalgia Betrayal** | [[Gimmick System/Cultural Immortality|Immortal]] insulted, mask destroyed |
| **Fan Culture Type** | Hothead, Traditionalist = increased chance |

---

## Era/Region Gate

| Region | Era | Throwing Behavior |
|--------|-----|-------------------|
| **Southern US** | 1980s | Rare, mostly verbal hostility |
| **Southern US** | 1995-2001 | Active, especially Nitro, PPVs |
| **Mexico** | Any | Rare, used for betrayals or rudo excess |
| **Japan** | Any | Almost never; total crowd shame if it happens |
| **Modern US** | 2000s-Now | Disabled by default unless chaos-friendly fed |

---

## Simulation Response

| Response | Description |
|----------|-------------|
| **Match Summary** | "Security struggled to hold back the crowd as plastic bottles rained down..." |
| **Commentary** | Adapts by AI booker type |
| **Booking Fallout** | AI may panic and pivot if throwing escalates |
| **Player Warning** | "The fans' reaction was nuclear. Proceed carefully." |

---

## Historical Examples

| Event | Context |
|-------|---------|
| **Bash at the Beach '96** | Hogan heel turn, garbage thrown |
| **ECW regularly** | Built into the culture |
| **Various Nitro episodes** | NWO heat at peak |

---

## Consequences

| Outcome | Effect |
|---------|--------|
| **Heel push may be derailed** | AI reconsiders |
| **Title change may be reversed** | Panic booking |
| **[[Fan Memory Engine/_Fan Memory Index|Memory Snapshot]] created** | "The night the ring filled with trash" |
| **Worker morale boost** | Heel knows they're doing their job |

---

## Connected Mechanics

- [[Region Era Profiles]] - gates when throwing is possible
- [[Heat vs Hate]] - throwing usually means true Hate, not just Heat
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - throwing creates permanent snapshots
- [[Booking Trails/_Booking Trails Index|Booking Trails]] - may cause trail failure or pivot

---

## Open Questions

- Safety/injury mechanics if throwing gets out of hand
- Promotion reputation effects (ECW embraces it, WWE avoids it)
- Player control over throwing culture in custom feds

---

## Implementation Notes

```json
{
  "garbage_event": {
    "show_id": "show_nitro_1996_07_07",
    "segment_id": "seg_main_event",
    "trigger": "nostalgia_betrayal",
    "worker_target": "w_hogan",
    "intensity": 20,
    "memory_snapshot_created": true,
    "booking_fallout": {
      "ai_panic": true,
      "pivot_suggested": false
    },
    "commentary_note": "This crowd has completely lost it!"
  }
}
```
