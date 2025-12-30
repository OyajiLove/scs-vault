# Gimmick Lifecycle

📛 **MECHANIC:** Gimmick Lifecycle
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** gimmick lifecycle, debut, peak, stagnation, burnout, rebirth, legacy echo
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 1-4 | Character arcs discussed informally; concept of "gimmick freshness" emerged in booking discussions |
| v2.0 | Vol 6 | **LOCKED** - Formal lifecycle stages defined: Debut, Climb, Peak, Stagnation, Burnout, Rebirth, Legacy Echo. Stage transition triggers and Buzz modifiers specified |

---

## Overview

Every gimmick follows a natural arc from debut to potential burnout. Understanding this lifecycle helps bookers time pushes, pivots, and retirements.

---

## Lifecycle Stages

| Stage | Description |
|-------|-------------|
| **Debut** | Introduction period. Crowd forming first impressions. High variance in reception. |
| **Climb** | Building momentum. Wins matter more. Character definition solidifying. |
| **Peak** | Maximum overness for this gimmick. Crowd fully invested. Best time for title runs. |
| **Stagnation** | Diminishing returns. Same beats feel repetitive. Buzz harder to maintain. |
| **Burnout** | Crowd actively tired of the character. Negative reactions to familiar spots. |
| **Rebirth** | Gimmick evolution or repackage. Fresh start with lessons learned. |
| **Legacy Echo** | Post-active period. Gimmick remembered, can return for nostalgia pops. |

---

## Stage Transitions

| Transition | Trigger |
|------------|---------|
| Debut → Climb | Positive crowd response sustained over 4+ appearances |
| Climb → Peak | [[Buzz Scale|Buzz]] reaches 15+ and holds, title contention |
| Peak → Stagnation | Buzz plateaus despite continued push |
| Stagnation → Burnout | Buzz drops, crowd rejection signals |
| Burnout → Rebirth | Repackage, heel/face turn, time off |
| Any → Legacy Echo | Retirement or extended absence |

---

## Stage Effects

| Stage | Buzz Modifier | Booking Notes |
|-------|---------------|---------------|
| Debut | High variance | Test different opponents/segments |
| Climb | +1 bonus to positive events | Momentum is your friend |
| Peak | Stable ceiling | Don't overexpose |
| Stagnation | -1 penalty to repetitive beats | Need fresh angles |
| Burnout | -2 penalty, negative crowd risk | Consider time off |
| Rebirth | Reset baseline, fresh start | Old baggage fades |
| Legacy Echo | Nostalgia bonus on returns | Diminishing with each return |

---

## GIMMICK EVOLUTION SYSTEM (#212)

📌 **Source:** Vol 1 Extraction #212

### Core Concept

Gimmicks can evolve naturally or be forcibly changed.

| Evolution Type | Requirements |
|----------------|-------------|
| **Organic Growth** | High crowd acceptance, worker buy-in |
| **Heel/Face Shift** | Turn mechanics trigger (see [[Turn_Engine]]) |
| **Repackage** | Failed gimmick, needs fresh start |
| **Character Deepening** | Adding layers to existing persona |
| **Era Adaptation** | Adjusting to changing times |

**Risk:** Forced evolution without setup = rejection.

---

## GIMMICK HEAT/POP SOURCES (#213)

📌 **Source:** Vol 1 Extraction #213

### What Makes a Gimmick Connect

| Source | Generates |
|--------|----------|
| **Catchphrase** | Pop recognition, merch potential |
| **Entrance** | Visual pop, atmosphere |
| **Mannerisms** | Character depth, heel heat |
| **Finish** | Match climax pop |
| **Promo Style** | Heat or pop depending on alignment |
| **Stable Affiliation** | Borrowed credibility/heat |
| **Music** | Pavlovian response, instant recognition |

**Stacking:** Multiple strong sources = more over gimmick.

---

## Connected Mechanics

- [[Buzz Decay]] - accelerates during stagnation/burnout
- [[Gimmick Management]] - tools to move between stages
- [[Iconic Lock]] - can freeze gimmick at Peak indefinitely

---

## Open Questions

- Exact duration for each stage (weeks? months?)
- Can a gimmick skip stages (debut straight to peak)?
- Multiple rebirth attempts: diminishing returns?

---

## Implementation Notes

```json
{
  "gimmick_id": "gim_001",
  "lifecycle_stage": "peak",
  "stage_entered": "2024-06-15",
  "weeks_in_stage": 24,
  "stage_history": [
    {"stage": "debut", "weeks": 6},
    {"stage": "climb", "weeks": 18},
    {"stage": "peak", "weeks": 24}
  ],
  "stagnation_risk": 0.35
}
```
