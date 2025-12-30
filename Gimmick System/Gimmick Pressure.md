# Gimmick Pressure System

📛 **MECHANIC:** Gimmick Pressure / Worker Resistance
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker-Gimmick Dynamics
🔑 **KEYWORDS:** gimmick pressure, resistance, demands, creative control, unhappy worker
📌 **ORIGIN:** Vol 1 Extraction #118, #44
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Workers aren't passive about their characters. They have opinions about their gimmicks and will push back if unhappy. This creates organic tension between booking vision and worker autonomy.

---

## Core Concept

When a worker's gimmick fit is poor OR when they've been stuck in a bad gimmick too long, **Gimmick Pressure** builds:

```
Gimmick Pressure = (Time in Bad Gimmick × Ego) + (Failed Promos × 2) + (Losses While Gimmicked × 0.5)
```

When Gimmick Pressure exceeds threshold → Worker demands change.

---

## Resistance Mechanics

### Worker Refusal/Resistance (#44)

Workers can actively resist booking decisions:

| Resistance Type | Trigger | Worker Action |
|-----------------|---------|---------------|
| **Gimmick Refusal** | Hates current character | Demands meeting, threatens no-show |
| **Loss Refusal** | Ego too high for proposed job | Negotiates harder finish or refuses |
| **Turn Resistance** | Doesn't want alignment change | Sandbags heel/face work |
| **Push Resistance** | Being pushed down | Complains, considers leaving |
| **Creative Control** | Has negotiated control | Can veto booking decisions |

### The Austin Example (Locked)

> "Steve Austin hates Ringmaster, demands change."

Timeline:
1. Austin assigned Ringmaster gimmick
2. Gimmick Fit: ~45% (poor)
3. Promos feel forced, crowd indifferent
4. Austin's Gimmick Pressure builds over months
5. Austin demands meeting with bookers
6. Options: Grant change, compromise, or force compliance (risk morale)
7. Austin becomes Stone Cold, Gimmick Fit: 98%

---

## Pressure Thresholds

| Pressure Level | Worker Behavior |
|----------------|-----------------|
| 0-20 | Content, no complaints |
| 21-40 | Privately unhappy, hints to agents |
| 41-60 | Requests meeting with booker |
| 61-80 | Demands change, considers leaving |
| 81-100 | Refuses to work, potential walkout |

---

## Factors Affecting Pressure Build

| Factor | Effect on Pressure |
|--------|-------------------|
| **High Ego** | Pressure builds faster |
| **Low Loyalty** | More willing to walk |
| **Veteran Status** | Has more leverage |
| **Current Overness** | If still over despite gimmick, less pressure |
| **Gimmick Success** | Good match/promo ratings reduce pressure |

---

## Resolution Options

When worker demands gimmick change:

| Option | Effect |
|--------|--------|
| **Grant Full Change** | Worker happy, risk of "giving in" reputation |
| **Negotiate Tweak** | Partial change, moderate satisfaction |
| **Refuse** | Worker morale drops, may leave/sandbag |
| **Fire Them** | Lose talent, send message to locker room |
| **Creative Control Clause** | If they have it, you must comply |

---

## Creative Control

Top stars can negotiate **Creative Control** in contracts:

| Control Level | Rights |
|---------------|--------|
| **None** | Accept booking or leave |
| **Consultation** | Must be consulted, can't veto |
| **Approval** | Can veto major decisions |
| **Full Control** | They book themselves essentially |

**Warning:** Creative control can backfire (Hogan, Nash refusing to job).

---

## Connected Mechanics

- [[Gimmick Attributes]] - Gimmick Fit affects pressure
- [[Gimmick Lifecycle]] - Stagnation phase triggers pressure
- [[Hidden_Personality]] - Ego, Loyalty affect pressure dynamics
- [[Contract System/_Contract System Index|Contract System]] - Creative control negotiation

---

## Implementation Notes

```json
{
  "worker_id": "austin_1995",
  "current_gimmick": "ringmaster",
  "gimmick_fit": 0.45,
  "gimmick_pressure": 72,
  "pressure_history": [
    {"month": 1, "pressure": 15, "trigger": "gimmick_assigned"},
    {"month": 2, "pressure": 28, "trigger": "failed_promo"},
    {"month": 3, "pressure": 45, "trigger": "loss_streak"},
    {"month": 4, "pressure": 72, "trigger": "continued_failure"}
  ],
  "status": "demanding_meeting",
  "creative_control": false
}
```

---

## Open Questions

- Exact formula coefficients for pressure calculation?
- How does charisma affect pressure tolerance?
- Can workers be "broken" into accepting bad gimmicks long-term?

---

**Document Status:** Locked
**Last Updated:** 2024-12-23
