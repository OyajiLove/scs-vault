# Buzz Decay

ðŸ“› **MECHANIC:** Buzz Decay
ðŸ”— **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
ðŸ§­ **CATEGORY:** Booking & Simulation / Momentum Tracking
ðŸ”‘ **KEYWORDS:** buzz decay, momentum fade, overexposure, fatigue, stale feuds
ðŸ“Œ **ORIGIN:** Vol 5, Vol 6
âœ… **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Buzz isn't permanent. Without regular appearances and emotional evolution, momentum fades. This mechanic ensures that workers need continuous investment to maintain their heat.

---

## Natural Decay

- Inactive workers lose Buzz over time
- Rate: approximately -1 per 2-3 weeks of inactivity (exact formula TBD)
- Floor: Buzz doesn't drop below 1

---

## Buzz Fatigue

Overexposure causes accelerated decay:

| Condition | Effect |
|-----------|--------|
| Appears every show without story evolution | Fatigue builds |
| Same promo beats repeated | Audience tunes out |
| Feuds that don't escalate emotionally | White noise effect |
| Fast-burn company style | Entire roster risks fatigue |

---

## Stale Feuds

A feud with high Buzz but no emotional evolution becomes white noise:

- Initial Buzz spike from confrontation
- Buzz plateaus if matches repeat without stakes change
- Eventually crowd stops caring
- "We've seen this before" effect

---

## Reinvigoration Methods

| Method | Effect |
|--------|--------|
| Fresh angles | Resets fatigue counter |
| Surprise twists | Spike + fatigue reset |
| Rest periods (cooldowns) | Allows natural hunger to rebuild |
| [[Gimmick System/_Gimmick System Index|Gimmick]] evolution | New presentation resets perception |
| New opponent | Fresh matchup can revive stale worker |

---

## Connected Mechanics

- [[Buzz Inputs]] - positive inputs counteract decay
- [[Buzz to Pop Conversion]] - decay competes with conversion
- [[Gimmick Lifecycle]] - stagnation stage accelerates buzz decay

---

## Open Questions

- Exact decay curve formula not specified
- Per-region decay rates (does Japan decay slower?)
- Interaction between fatigue and fan type distribution

---

## Implementation Notes

```json
{
  "decay_check": {
    "worker_id": "w_001",
    "weeks_since_appearance": 3,
    "base_decay": -1,
    "fatigue_modifier": 0,
    "final_decay": -1,
    "new_buzz": 13
  }
}
```
