# Legacy Score

📛 **MECHANIC:** Calculating Historical Impact
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy
🔑 **KEYWORDS:** legacy, historical impact, career score, legend rating
📌 **ORIGIN:** Vol 1-4 (Legacy scoring, HOF eligibility)
✅ **STATUS:** Locked

---

## Overview

Legacy Score measures a worker's lasting historical impact, distinct from current popularity. A worker can have low current popularity but high legacy (retired legend), or high popularity but low legacy (flash in the pan). Legacy determines HOF eligibility, historical rankings, and how workers are remembered.

---

## Legacy Score Components

| Component | Weight | Description |
|-----------|--------|-------------|
| **Peak Achievement** | 25% | Highest career point |
| **Sustained Excellence** | 20% | Years at top level |
| **Championship History** | 15% | Title reigns, quality |
| **Match Quality** | 15% | Career workrate |
| **Cultural Impact** | 15% | Changed the business |
| **Drawing Power** | 10% | Proven money draw |

---

## Peak Achievement Factors

| Factor | Points |
|--------|--------|
| **World Champion** | 20-30 |
| **Multiple World Titles** | +5 per reign |
| **Dynasty Champion** | +15 |
| **Grand Slam** | +10 |
| **Major Event Main Event** | +5 per |
| **MOTY Winner** | +10 per |
| **5-Star Match** | +5 per |

---

## Sustained Excellence

| Duration at Top | Points |
|-----------------|--------|
| **1-2 years** | 10 |
| **3-5 years** | 20 |
| **6-10 years** | 35 |
| **10+ years** | 50 |
| **Multi-era relevance** | +15 |

---

## Championship History

| Achievement | Points |
|-------------|--------|
| **World Title Reign** | 10 per |
| **Long World Reign (1+ year)** | +5 |
| **Secondary Title** | 5 per |
| **Tag Title** | 3 per |
| **Grand Slam** | +10 |
| **Unified Titles** | +5 |

---

## Match Quality Legacy

| Achievement | Points |
|-------------|--------|
| **Career Average 80+** | 20 |
| **Career Average 70-79** | 10 |
| **5+ MOTY Candidates** | 15 |
| **Legendary Matches** | 5 per |
| **Carried Opponents** | +5 |
| **Style Innovation** | +10 |

---

## Cultural Impact

| Achievement | Points |
|-------------|--------|
| **Defined an Era** | 20 |
| **Created New Style** | 15 |
| **Mainstream Crossover** | 10 |
| **Trained Future Legends** | 10 |
| **Changed Business Practices** | 15 |
| **International Impact** | 10 |
| **Locker Room Leadership** | 5 |

---

## Drawing Power

| Achievement | Points |
|-------------|--------|
| **Proven Top Draw** | 15 |
| **Rating Mover** | 10 |
| **PPV Buy Rate Impact** | 10 |
| **Merchandise King** | 10 |
| **House Show Draw** | 5 |

---

## Legacy Modifiers

### Positive

| Factor | Bonus |
|--------|-------|
| **Clean career** | +5 |
| **Graceful exit** | +5 |
| **Respected by peers** | +5 |
| **Torch passing** | +5 |
| **Positive influence** | +5 |
| **Documentary subject** | +3 |

### Negative

| Factor | Penalty |
|--------|---------|
| **Major scandal** | -10 to -30 |
| **Burned bridges** | -5 to -15 |
| **Hurt others' careers** | -5 to -10 |
| **Bitter exit** | -5 |
| **Poor late career** | -5 |
| **Tarnished legacy** | -10 to -20 |

---

## Legacy Score Tiers

| Score | Tier | Description |
|-------|------|-------------|
| 90-100 | **All-Time Great** | Mount Rushmore level |
| 80-89 | **Legend** | Undisputed HOF |
| 70-79 | **Star** | Strong legacy |
| 60-69 | **Solid** | Remembered fondly |
| 50-59 | **Journeyman** | Modest legacy |
| Below 50 | **Forgotten** | Fading memory |

---

## Legacy vs. Popularity

| Scenario | Popularity | Legacy |
|----------|------------|--------|
| **Active hot star** | High | Building |
| **Retired legend** | Low-Moderate | High |
| **Flash in the pan** | Was High | Low |
| **Late bloomer** | Rising | Lower than deserved |
| **Consistent midcarder** | Moderate | Moderate |

---

## Legacy Growth and Decay

| Phase | Legacy Behavior |
|-------|-----------------|
| **Active Career** | Building based on achievements |
| **Recent Retirement** | Crystallizes at retirement |
| **Post-Retirement** | Slow growth if remembered |
| **Long Retirement** | Stable or slow decay |
| **Death** | Often spikes (nostalgia) |
| **Scandal Exposure** | Can decay sharply |

---

## Connected Mechanics

- [[HOF Eligibility]] - Legacy determines eligibility
- [[Crowd Memory]] - Memory anchors build legacy
- [[Retirement System]] - Retirement type affects legacy
- [[Scandal System]] - Scandal damages legacy

---

## Open Questions

- [ ] Exact point values for each factor
- [ ] How legacy compares across eras
- [ ] Regional legacy variations
- [ ] How legacy affects AI booking decisions
- [ ] Legacy inflation/deflation over time

---

## Implementation Notes

```json
{
  "legacy_score": {
    "worker_id": "worker_001",
    "total_score": 87,
    "tier": "legend",
    "components": {
      "peak_achievement": 28,
      "sustained_excellence": 18,
      "championship_history": 15,
      "match_quality": 12,
      "cultural_impact": 10,
      "drawing_power": 8
    },
    "modifiers": {
      "clean_career": 5,
      "peer_respect": 5,
      "scandal_penalty": -5
    },
    "growth_trend": "stable",
    "last_calculated": "1995-01-01"
  }
}
```
