# Buzz Spikes and Crashes

ðŸ“› **MECHANIC:** Buzz Spikes and Crashes
ðŸ”— **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
ðŸ§­ **CATEGORY:** Booking & Simulation / Momentum Tracking
ðŸ”‘ **KEYWORDS:** buzz spike, buzz crash, viral moment, momentum shift, extreme events
ðŸ“Œ **ORIGIN:** Vol 5, Vol 6
âœ… **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Rare but extreme momentum events that jolt the system beyond normal [[Buzz Inputs]]. Spikes can launch careers; crashes can derail them. Both create [[Fan Memory Engine/_Fan Memory Index|Memory Snapshots]].

---

## Buzz Spikes

Massive upward momentum shifts:

| Event | Effect |
|-------|--------|
| Viral promo shoot (pipebomb) | Massive +Controversy, +Speculative Buzz |
| Surprise return after years | +Emotional, +Live Buzz |
| Retirement match with perfect payoff | Long-term +Legacy Buzz |
| Shock title change | +Live, +Booking Momentum |
| Betrayal of beloved figure | +Emotional (positive or negative) |

### Spike Behavior

- Spikes are temporary unless followed up
- One-off viral moments fade within 4-6 weeks without reinforcement
- Well-timed spikes can launch careers or resurrect dead pushes
- Poorly timed spikes waste momentum

---

## Buzz Crashes

Massive downward momentum shifts:

| Event | Effect |
|-------|--------|
| Major botch in big match | -Live, -Momentum |
| Booking betrayal (screwjob done poorly) | +Controversy but possible -Emotional |
| No-sell or shoot fight | Chaos: fallout varies wildly |
| Public scandal | -All subtypes, possible career damage |
| "Go away" heat from overexposure | -Live, -Emotional |

### Crash Recovery

- Some crashes are recoverable (time off, repackage)
- Some crashes are permanent (scandal, trust violation)
- AI Bookers may panic-book after crashes
- Player can attempt damage control or lean into chaos

---

## Connected Mechanics

- [[Buzz Inputs]] - normal-range momentum changes
- [[Memory Snapshots]] - spikes/crashes create permanent memories
- [[Buzz Decay]] - what happens after a spike fades

---

## Open Questions

- Exact threshold for "spike" vs "large input"
- Crash recovery timeline formulas
- Interaction with [[Buzz System/Push Resistance|Push Resistance]]

---

## Implementation Notes

```json
{
  "buzz_spike": {
    "worker_id": "w_001",
    "event_type": "pipebomb_promo",
    "buzz_change": 8,
    "creates_snapshot": true,
    "decay_rate": "accelerated",
    "followup_required": true
  }
}
```
