# Buzz Inputs

ðŸ“› **MECHANIC:** Buzz Inputs
ðŸ”— **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
ðŸ§­ **CATEGORY:** Booking & Simulation / Momentum Tracking
ðŸ”‘ **KEYWORDS:** buzz modifiers, momentum change, booking effects, match impact
ðŸ“Œ **ORIGIN:** Vol 5, Vol 6
âœ… **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Buzz Inputs are events and booking decisions that raise or lower a worker's [[Buzz Scale|Buzz]] rating. Every appearance, match, and segment has the potential to shift momentum positively or negatively.

---

## Positive Buzz Events

| Action/Event | Buzz Effect |
|--------------|-------------|
| Key win in a hot feud | +2 to +3 |
| Memorable promo or segment | +1 to +2 |
| Banger match with high crowd heat | +1 to +2 |
| Surprise return / swerve | +2 to +4 |
| Title win (well built) | +2 to +4 |
| Pull-apart brawl | +1 to +2 |
| Shock betrayal | +2 to +3 |
| Viral promo moment | +2 to +4 |

---

## Negative Buzz Events

| Action/Event | Buzz Effect |
|--------------|-------------|
| Cold loss or flat promo | -1 to -2 |
| Overexposure / burnout | -2 to -3 |
| Predictable booking | -1 to -2 |
| Cold crowd response | -1 to -2 |
| Phoned-in match performance | -1 to -2 |
| "Forced" push despite low fan interest | Buzz stagnates or dips |

---

## Context Modifiers

| Context | Effect |
|---------|--------|
| Main event position | Buzz changes amplified |
| Title involvement | Buzz gains convert faster to [[Popularity_System|Pop]] |
| Regional saturation | Buzz only changes where seen |
| Promotion size | Larger reach = bigger swings |

---

## Connected Mechanics

- [[Buzz Scale]] - the rating being modified
- [[Buzz Spikes and Crashes]] - extreme versions of inputs
- [[Buzz Decay]] - what happens without positive inputs

---

## Open Questions

- Exact modifier values for context effects not specified
- Stacking rules for multiple events in one show
- Diminishing returns on repeated positive inputs?

---

## Implementation Notes

```json
{
  "buzz_event": {
    "type": "match_win",
    "context": "feud_blowoff",
    "base_change": 2,
    "modifiers": {
      "main_event": 1.5,
      "title_match": 1.25
    },
    "final_change": 3.75
  }
}
```
