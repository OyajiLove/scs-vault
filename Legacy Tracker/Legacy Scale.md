# Legacy Scale

📛 **MECHANIC:** Legacy Scale
🔗 **PARENT SYSTEM:** [[_Legacy Tracker Index|Legacy Tracker]]
🧭 **CATEGORY:** Career & Recognition
🔑 **KEYWORDS:** legacy score, 0-100, career tiers, historical status
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

The 0-100 scale measuring long-term historical impact. Legacy grows slowly over an entire career and represents how a worker will be remembered.

---

## The Scale

| Score | Tier | Description |
|-------|------|-------------|
| 0-19 | Forgettable | No lasting impact, quickly forgotten |
| 20-39 | Journeyman | Remembered by hardcore fans only |
| 40-59 | Solid Career | Respected professional, regional recognition |
| 60-79 | Notable | Remembered fondly, HOF consideration |
| 80-89 | Legendary | [[Hall of Fame/_Hall of Fame Index\|First Ballot HOF]], widely recognized |
| 90-100 | [[Cultural Immortality\|Immortal]] | Transcends wrestling, permanent cultural fixture |

---

## Tier Thresholds

| Threshold | Unlocks |
|-----------|---------|
| 50+ | HOF Veteran's Committee eligibility |
| 65+ | Standard HOF eligibility |
| 80+ | [[Iconic Lock]] potential |
| 85+ | First Ballot HOF |
| 95+ | [[Cultural Immortality]] potential |

---

## Score Examples

| Worker | Approximate Score | Reasoning |
|--------|-------------------|-----------|
| El Santo | 98 | Cultural icon, national hero |
| The Rock | 95 | Mainstream crossover, Hollywood |
| Steve Austin | 93 | Changed the industry, iconic |
| Bret Hart | 85 | Technical excellence, respected |
| Honky Tonk Man | 55 | Memorable run, limited scope |
| Random Jobber | 5 | No lasting impact |

---

## Connected Mechanics

- [[Legacy Builders]] - how to increase Legacy
- [[Legacy Modifiers]] - what affects growth rate
- [[Hall of Fame/HOF Eligibility|HOF Eligibility]] - Legacy is primary factor

---

## Open Questions

- Minimum career length to reach each tier?
- Regional Legacy variation?

---

## Implementation Notes

```json
{
  "worker_id": "w_001",
  "legacy": {
    "score": 78,
    "tier": "notable",
    "peak_score": 78,
    "hof_eligible": true,
    "iconic_lock_eligible": false,
    "score_history": [
      {"year": 2000, "score": 15},
      {"year": 2005, "score": 35},
      {"year": 2010, "score": 58},
      {"year": 2015, "score": 72},
      {"year": 2020, "score": 78}
    ]
  }
}
```
