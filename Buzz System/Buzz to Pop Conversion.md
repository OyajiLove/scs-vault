# Buzz to Pop Conversion

ðŸ“› **MECHANIC:** Buzz to Pop Conversion
ðŸ”— **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
ðŸ§­ **CATEGORY:** Booking & Simulation / Momentum Tracking
ðŸ”‘ **KEYWORDS:** buzz conversion, popularity growth, sustained momentum, trailing average
ðŸ“Œ **ORIGIN:** Vol 5, Vol 6
âœ… **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

If a worker sustains high [[Buzz Scale|Buzz]] over time, fans start to see them as a star. One bright moment that fades means nothing for long-term overness. This mechanic governs how short-term momentum becomes lasting [[Popularity_System|Popularity]].

---

## Conversion Formula (Per Region)

```
If: Current Buzz â‰¥ 13
And: Trailing Buzz Average (past 4-6 appearances) â‰¥ 12
Then: Small Popularity Gain (+0.5 to +1.5 depending on exposure)
```

---

## Conversion Patterns

| Buzz Pattern | Pop Result |
|--------------|------------|
| Hot streak over 6 shows | +1.0 to +2.0 Pop (per region) |
| Up/down inconsistency | +0.0 to +0.5 or stagnant |
| Cold or unused | Pop decay triggers (slow erosion) |
| Sudden viral buzz spike | Temporary +Pop (may fade if not sustained) |

---

## Modifiers

| Factor | Effect on Buzzâ†’Pop |
|--------|-------------------|
| Promotion Size | Larger reach = more Pop gain per Buzz |
| Match Position | Main event buzz matters more |
| Title Involvement | Buzz in title feuds converts faster |
| Regional Saturation | Buzz converts only where the match was seen |
| Worker Gimmick Tags | "Cult Follower Favorite" may convert slower but stronger |
| AI Booker Respect | If booker buries you despite high Buzz, conversion is slower |

---

## Connected Mechanics

- [[Buzz Scale]] - the input being converted
- [[Popularity_System]] - the output being gained
- [[Buzz Decay]] - competing force against conversion

---

## Open Questions

- Exact trailing average window (4 or 6 appearances?)
- Regional conversion rate differences
- Tag team Buzz â†’ individual Pop split rules

---

## Implementation Notes

```json
{
  "conversion_check": {
    "worker_id": "w_001",
    "region": "northeast_us",
    "current_buzz": 15,
    "trailing_average": 13.5,
    "appearances_in_window": 5,
    "eligible": true,
    "pop_gain": 1.2
  }
}
```
