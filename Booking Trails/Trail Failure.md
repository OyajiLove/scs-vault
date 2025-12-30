# Trail Failure

📛 **MECHANIC:** Trail Failure
🔗 **PARENT SYSTEM:** [[_Booking Trails Index|Booking Trails]]
🧭 **CATEGORY:** Booking & Simulation / Long-Term Planning
🔑 **KEYWORDS:** trail failure, abandoned arc, booking interruption, storyline collapse
📌 **ORIGIN:** Vol 5, Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Trails can fail or be abandoned. This is not always bad (pivots can create new opportunities), but unplanned failures have consequences for [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] and worker morale.

---

## Failure Causes

| Cause | Example |
|-------|---------|
| **Worker leaves** | Contract expires, injury, firing |
| **Booking change** | New booker, corporate mandate |
| **Fan rejection** | Crowd turns on arc |
| **Emotional burnout** | Trail dragged too long |
| **Real-world interference** | Scandal, no-show, shoot incident |

---

## Failure Outcomes

| Outcome | Effect |
|---------|--------|
| **Trail marked abandoned** | Logged in booking history |
| **Fan Memory impact** | "Remember when they teased that feud and never delivered?" |
| **Worker morale** | Participants may resent wasted build |
| **Booking trust penalty** | AI/player credibility affected |
| **Salvage opportunity** | Some failures can pivot to new trails |

---

## Planned vs Unplanned Abandonment

**Planned Abandonment:**
- Booker decides arc isn't working
- Clean pivot to new direction
- Minimal memory damage if handled well

**Unplanned Abandonment:**
- External factors force stoppage
- Hanging threads in fan memory
- May need explicit closure segment later

---

## Recovery Options

| Option | When to Use |
|--------|-------------|
| **Reframe as heel work** | "They were stringing us along" |
| **Callback later** | Revisit "unfinished business" when workers available |
| **Acknowledge in-universe** | Promo references the abandoned angle |
| **Let it fade** | Sometimes silence is best |

---

## Connected Mechanics

- [[Trail Planning]] - where failures originate
- [[Trail Milestones]] - missed milestones trigger failure
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory Engine]] - failures create negative memories

---

## Open Questions

- Failure severity scaling (minor vs catastrophic)?
- Recovery timeline requirements?

---

## Implementation Notes

```json
{
  "trail_id": "tr_001",
  "status": "abandoned",
  "failure_cause": "worker_injury",
  "failure_date": "2025-03-20",
  "milestones_completed": 3,
  "milestones_total": 6,
  "memory_impact": "moderate_negative",
  "recovery_attempts": []
}
```
