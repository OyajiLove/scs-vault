# Push Resistance

📛 **MECHANIC:** Push Resistance
🔗 **PARENT SYSTEM:** [[Buzz System/_Buzz System Index|Buzz System]]
🧭 **CATEGORY:** Booking & Simulation / Crowd Psychology
🔑 **KEYWORDS:** push resistance, buzz pop gap, manufactured heat, organic over, crowd rejection, false popularity
📌 **ORIGIN:** Vol 5-6 (conceptual references)
✅ **STATUS:** Stub (concept referenced, mechanics not formally specified)

---

## Overview

Push Resistance describes the friction that occurs when there's a significant gap between a worker's **Buzz** (short-term momentum from booking) and their **Popularity** (long-term organic overness). This gap creates both crowd psychology effects and backstage political tension.

---

## The Buzz/Pop Gap Problem

| Scenario | Crowd Effect | Backstage Effect |
|----------|--------------|------------------|
| **High Buzz, Low Pop** ("Being Pushed") | Crowd rejects manufactured heat, "go away" chants | Other workers resent unearned spotlight |
| **Low Buzz, High Pop** ("Coasting") | Fans loyal but restless, "push them" chants | Worker may be entitled, resistant to new talent |
| **High Buzz, High Pop** (Aligned) | Maximum engagement, everything works | No resistance, smooth booking |
| **Low Buzz, Low Pop** (Jobber) | Indifference | No political capital |

---

## High Buzz / Low Pop: The Roman Reigns Problem

When booking pushes someone the crowd hasn't organically embraced:

| Effect | Description |
|--------|-------------|
| **Crowd Rejection** | Boos intended babyface, cheers heels against them |
| **Diminishing Returns** | Each push segment generates less Buzz |
| **Anchor Damage** | Negative memories form around forced moments |
| **Backstage Resentment** | Other workers see unearned push |
| **Management Stubbornness** | AI bookers may double down (reality accurate) |

### Resolution Paths
- Turn heel (embrace the rejection)
- Repackage and rebuild organically
- Time off to reset expectations
- Wait for circumstances to align (Shield reunion effect)

---

## Low Buzz / High Pop: The Coasting Legend Problem

When established stars aren't currently featured:

| Effect | Description |
|--------|-------------|
| **Fan Restlessness** | "Push [Name]" chants during other segments |
| **Entitlement Risk** | Worker may resist putting over new talent |
| **Booking Tension** | Fans reject whoever beats them |
| **Political Capital** | High Pop = high leverage in negotiations |

### Resolution Paths
- Feature them in meaningful feuds
- Use them to elevate new talent (torch passing)
- Part-time legends schedule
- Retirement arc if appropriate

---

## Connected Mechanics

- [[Buzz System/_Buzz System Index|Buzz System]] - Short-term momentum tracking
- [[Popularity_System|Popularity System]] - Long-term overness
- [[Crowd_Memory|Crowd Memory]] - Gaps create negative memory anchors
- [[Contract System/Worker Resistance|Worker Resistance]] - Backstage friction from gaps
- [[Backstage Politics System/_Backstage Politics System Index|Backstage Politics]] - Political consequences
- [[Hidden_Personality|Hidden Personality]] - Ego affects how workers handle gaps

---

## Open Questions

- [ ] Exact threshold for "significant gap" triggering effects
- [ ] Decay rate of crowd rejection
- [ ] AI booker behavior when facing push resistance
- [ ] How many failed pushes before giving up
- [ ] Regional variation in tolerance for manufactured pushes

---

## Implementation Notes

```json
{
  "push_resistance_check": {
    "worker_id": "w_001",
    "current_buzz": 16,
    "current_pop": 45,
    "gap": 11,
    "gap_direction": "buzz_exceeds_pop",
    "resistance_active": true,
    "effects": {
      "crowd_rejection_modifier": -0.15,
      "backstage_resentment": true,
      "diminishing_returns": 0.8
    }
  }
}
```

---

**Document Status:** Stub (needs formal mechanics from future design work)
**Last Updated:** 2025-12-22
**Next Review:** Formalize gap thresholds and effect calculations
