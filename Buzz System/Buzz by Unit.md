# Buzz by Unit

ðŸ“› **MECHANIC:** Buzz by Unit
ðŸ”— **PARENT SYSTEM:** [[_Buzz System Index|Buzz System]]
ðŸ§­ **CATEGORY:** Booking & Simulation / Momentum Tracking
ðŸ”‘ **KEYWORDS:** worker buzz, feud buzz, show buzz, title buzz, promotion buzz
ðŸ“Œ **ORIGIN:** Vol 5, Vol 6
âœ… **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

[[Buzz Scale|Buzz]] applies to multiple units in the simulation, not just workers. Feuds, shows, titles, and entire promotions can be "hot" or "cold" independent of individual worker momentum.

---

## Trackable Units

| Unit | Notes |
|------|-------|
| **Worker** | Primary tracking unit. Cumulative across appearances. Can decay or spike. |
| **Match** | Can be remembered as a "Buzz Match" (e.g., Ospreay vs Omega). Feeds into worker Buzz. |
| **Segment** | Promos, brawls, betrayals tracked for buzz contribution. |
| **Show** | Overall "Buzz Rating" based on high/low points across card. |
| **Feud** | Tracks multi-week storylines and long-term engagement between participants. |
| **Championship** | Title matches can gain or lose prestige based on Buzz. Distinct from Title Prestige. |
| **Promotion** | Tracks how "hot" the company is overall. Affects contracts, poaching, talent interest. |

---

## Worker Buzz (Primary)

The core Buzz tracking:

- Individual 1-20 score per worker
- Regional variation (hot in Japan, cold in US)
- History tracked for trailing average calculations
- Flags for special states (hot streak, title contender, etc.)

---

## Feud Buzz

Feuds have their own Buzz score separate from workers involved:

- Two cold workers can have a hot feud (chemistry, stakes)
- Two hot workers can have a cold feud (bad booking, no evolution)
- Feud Buzz affects segment ratings and crowd investment
- Feud Buzz has no "Popularity" equivalent; feuds are temporary

---

## Promotion Buzz

Aggregate measure of company momentum:

- Affects talent attraction (hot company = easier signings)
- Affects TV negotiations
- Affects cross-promotion leverage
- Can spike or crash based on major events

---

## Connected Mechanics

- [[Buzz Scale]] - the rating system used across all units
- [[Feud_Memory]] - long-term tracking of feud emotional investment
- Title Prestige - separate from title Buzz

---

## Open Questions

- Promotion Buzz calculation formula (average of roster? weighted by card position?)
- Show Buzz persistence (does it affect next week's expectations?)
- Championship Buzz vs Prestige distinction needs formal definition

---

## Implementation Notes

```json
{
  "worker_buzz": {
    "worker_id": "w_001",
    "current_buzz": 14,
    "buzz_history": [12, 13, 14, 15, 14],
    "trailing_average": 13.6,
    "last_appearance": "2025-03-15",
    "buzz_by_region": {
      "northeast_us": 14,
      "southeast_us": 12,
      "japan_kanto": 16
    },
    "buzz_flags": ["hot_streak", "title_contender"]
  }
}
```
