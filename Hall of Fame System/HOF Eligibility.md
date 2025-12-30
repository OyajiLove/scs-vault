# HOF Eligibility

📛 **MECHANIC:** Qualification for Hall of Fame Induction
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy
🔑 **KEYWORDS:** eligibility, qualification, career achievement, milestone
📌 **ORIGIN:** Vol 1-4 (HOF voting/eligibility, Legacy scoring)
✅ **STATUS:** Locked

---

## Overview

Hall of Fame eligibility is earned through career achievements, sustained popularity, and industry influence. Not everyone qualifies, and some who qualify never get inducted due to politics or scandal. The system tracks eligibility separately from actual induction.

---

## Eligibility Factors

### Career Achievements

| Factor | Weight | Description |
|--------|--------|-------------|
| **World Title Reigns** | High | Top championship history |
| **Secondary Titles** | Moderate | IC, US, tag titles |
| **Match Quality Average** | High | Career workrate |
| **Legendary Matches** | Very High | MOTY, 5-star matches |
| **Main Event History** | High | PPV/major show main events |
| **Longevity** | Moderate | Career length |
| **Era Representation** | Moderate | Defined an era |

### Popularity Metrics

| Factor | Weight | Description |
|--------|--------|-------------|
| **Peak Popularity** | High | Highest popularity reached |
| **Sustained Popularity** | High | Years at top level |
| **Drawing Power** | Very High | Gate, ratings impact |
| **Merchandise** | Moderate | Merch sales history |
| **Crossover Appeal** | Moderate | Mainstream recognition |

### Industry Influence

| Factor | Weight | Description |
|--------|--------|-------------|
| **Innovator Status** | High | Created moves, styles |
| **Mentored Legends** | Moderate | Trained future stars |
| **Changed Business** | Very High | Transformed industry |
| **International Impact** | Moderate | Global influence |
| **Locker Room Leadership** | Moderate | Backstage respect |

---

## Eligibility Thresholds

| Tier | Score Range | Description |
|------|-------------|-------------|
| **Certain** | 90-100 | First ballot, no debate |
| **Strong** | 75-89 | Eventually inducted |
| **Borderline** | 60-74 | Depends on politics |
| **Unlikely** | 40-59 | Needs special circumstance |
| **Ineligible** | Below 40 | Not HOF caliber |

---

## Eligibility Modifiers

### Positive Modifiers

| Factor | Bonus |
|--------|-------|
| **Clean retirement** | +5 |
| **Graceful exit** | +5 |
| **Torch passing** | +5 |
| **Locker room respected** | +5 |
| **Company loyalty** | +3 to +10 |
| **PR friendly** | +3 |
| **Fan favorite** | +5 |

### Negative Modifiers

| Factor | Penalty |
|--------|---------|
| **Active scandal** | -10 to -30 |
| **Criminal conviction** | -20 to -50 |
| **Public dispute with company** | -10 to -20 |
| **Burned bridges** | -5 to -15 |
| **Short career** | -5 to -10 |
| **Locker room cancer** | -10 |
| **Unable to reconcile** | -15 |

---

## Scandal Impact on Eligibility

| Scandal Severity | Eligibility Effect |
|------------------|-------------------|
| **Minor** | Delayed 1-3 years |
| **Moderate** | Delayed 5-10 years |
| **Severe** | Indefinite delay |
| **Criminal** | Likely permanent block |
| **Unforgivable** | Permanent blacklist |

### Rehabilitation Path

| Action | Effect |
|--------|--------|
| **Time passage** | Scandal memory fades |
| **Public apology** | Reduces penalty |
| **Charity work** | Positive PR |
| **Reconciliation** | Removes company grudge |
| **Death** | Often clears path (posthumous) |

---

## Special Eligibility Categories

### Legacy/Builder

Non-wrestlers (announcers, managers, executives):

| Criteria | Description |
|----------|-------------|
| **Years of service** | Long tenure |
| **Industry impact** | Changed the business |
| **Name recognition** | Public awareness |
| **Company relationship** | In good standing |

### Celebrity Wing

Non-wrestling celebrities:

| Criteria | Description |
|----------|-------------|
| **Crossover impact** | Brought mainstream attention |
| **Memorable appearance** | Iconic moment |
| **Company PR value** | Useful for publicity |

### Tag Team/Faction

Group inductions:

| Criteria | Description |
|----------|-------------|
| **Team legacy** | Defined tag division |
| **Combined achievements** | Titles, matches |
| **Cultural impact** | Remembered as unit |

---

## Waiting Period

| Circumstance | Minimum Wait |
|--------------|--------------|
| **Active wrestler** | Cannot be inducted |
| **Semi-retired** | Variable (some inducted) |
| **Retired (clean)** | 1-3 years typical |
| **Retired (scandal)** | 5+ years |
| **Deceased** | Can be immediate |

---

## Connected Mechanics

- [[Legacy Score]] - Calculates overall eligibility
- [[HOF Voting and Selection]] - How eligible workers get chosen
- [[Scandal System/_Scandal System Index|Scandal System]] - Scandal blocks or delays
- [[Retirement System/_Retirement System Index|Retirement System]] - Retirement type affects eligibility

---

## Open Questions

- [ ] Exact point values for each factor
- [ ] How multi-promotion careers aggregate
- [ ] Minimum career length requirements
- [ ] How style/era affects evaluation
- [ ] Fan voting impact on eligibility vs. selection

---

## Implementation Notes

```json
{
  "hof_eligibility": {
    "worker_id": "worker_001",
    "eligibility_score": 87,
    "tier": "strong",
    "factors": {
      "world_titles": 25,
      "match_quality": 18,
      "peak_popularity": 15,
      "longevity": 12,
      "influence": 10,
      "drawing_power": 7
    },
    "modifiers": {
      "clean_retirement": 5,
      "company_loyalty": 8,
      "scandal_penalty": -5
    },
    "waiting_period_complete": true,
    "scandal_blocks": [],
    "eligible_since": "1992-01-01"
  }
}
```
