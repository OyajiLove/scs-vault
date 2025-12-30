# Buzz Scale

📛 **MECHANIC:** Buzz Scale
🔗 **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
🧭 **CATEGORY:** Booking & Simulation / Momentum Tracking
🔑 **KEYWORDS:** buzz rating, momentum scale, 1-20, hot, cold, crowd engagement
📌 **ORIGIN:** Vol 5 (renamed from "Heat"), Vol 6 (refined)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

The Buzz Scale is a 1-20 rating measuring short-term crowd engagement and momentum. Unlike [[Popularity_System|Popularity]] (0-100, slow-moving), Buzz is volatile and changes weekly based on booking decisions and crowd response.

---

## The 1-20 Scale

| Buzz Rating | Label | Meaning |
|-------------|-------|---------|
| 1-4 | Cold | Losing momentum, audience disengaged |
| 5-8 | Lukewarm | Some attention, but not catching fire |
| 9-12 | Warm | Solid momentum, crowd invested |
| 13-16 | Hot | Strong buzz, audience reacting weekly |
| 17-20 | On Fire | Major hype, cultural presence, likely push incoming |

---

## Momentum States (#100)

Qualitative descriptions of momentum trajectory:

| State | Indicators | Effects |
|-------|------------|--------|
| **Rising** | Win streak, crowd growing | +5% to reactions |
| **Hot** | Peak momentum | +15% to reactions |
| **Plateaued** | Stable but not climbing | Baseline |
| **Cooling** | Losses, poor booking | -5% to reactions |
| **Cold** | Extended losing, no direction | -15% to reactions |
| **Dead** | Completely directionless | Needs repackage |

**Recovery:** Hot → Cold can happen fast; Cold → Hot requires careful rebuild.

---

## Buzz Generation Sources (#99)

| Buzz Source | Duration |
|-------------|----------|
| **Great Match** | 2-4 weeks |
| **Viral Promo Moment** | 1-3 months |
| **Shocking Turn** | 2-6 months |
| **Title Win** | Variable by title prestige |
| **Social Media Incident** | 1-4 weeks |
| **Mainstream Crossover** | 3-12 months |

**Buzz Decay:** Faster than overness if not reinforced.  
**Buzz Conversion:** Can convert to permanent overness with sustained booking.

---

## Buzz Subtypes

These don't get separate scores; they influence the main Buzz rating:

| Subtype | Description |
|---------|-------------|
| **Live Buzz** | Crowd reaction score from match engine |
| **Booking Momentum** | Win/loss streaks, title contention |
| **Promo Resonance** | Segments remembered over time |
| **Cultural Heat** | Controversy, social media (modern feds only) |
| **Emotional Investment** | Sympathy, betrayal arcs, redemption stories |

---

## Connected Mechanics

- [[Buzz Inputs]] - what raises/lowers Buzz
- [[Buzz to Pop Conversion]] - how sustained Buzz becomes Popularity
- [[Buzz Decay]] - how momentum fades over time

---

## Open Questions

- Regional Buzz variation (does Japan track differently than US?)
- Subtype weighting formula not specified

---

## Implementation Notes

```json
{
  "worker_id": "w_001",
  "current_buzz": 14,
  "buzz_tier": "hot",
  "buzz_subtypes": {
    "live": 15,
    "booking_momentum": 12,
    "promo_resonance": 14,
    "cultural_heat": 8,
    "emotional_investment": 16
  }
}
```
