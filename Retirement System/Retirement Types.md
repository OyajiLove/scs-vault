# Retirement Types

📛 **MECHANIC:** Categories of Career Endings
🔗 **PARENT SYSTEM:** [[_Retirement System Index|Retirement System]]
🧭 **CATEGORY:** Worker Lifecycle
🔑 **KEYWORDS:** voluntary, forced, gradual, sudden, ceremonial, quiet
📌 **ORIGIN:** Vol 1-4 (Career Arc Templates, Retirement Patterns)
✅ **STATUS:** Locked

---

## Overview

Not all retirements are equal. Some workers get grand ceremonial farewells, others are forced out by injury, and some simply fade away. The type of retirement affects legacy, comeback potential, and fan memory.

---

## Retirement Type Classifications

### By Choice

| Type | Description | Legacy Impact |
|------|-------------|---------------|
| **Voluntary Peak** | Retires at or near peak | High: "went out on top" |
| **Voluntary Decline** | Chooses to stop as skills fade | Moderate: respectful exit |
| **Forced Injury** | Body gives out | Variable: tragic or inspiring |
| **Forced Scandal** | Scandal makes continuing impossible | Low to Negative |
| **Forced Firing** | Released and can't find work | Low: career ended badly |

### By Ceremony

| Type | Description | Memory Impact |
|------|-------------|---------------|
| **Grand Farewell** | Major retirement ceremony/match | Very High |
| **Quiet Exit** | Leaves without fanfare | Low |
| **Gradual Fade** | Reduces schedule until gone | Moderate |
| **Abrupt Disappearance** | Suddenly stops appearing | Variable |
| **Death in Harness** | Dies while still active | Very High (tragic) |

### By Finality

| Type | Description | Comeback Potential |
|------|-------------|-------------------|
| **Clean Break** | Truly done, no returns | Low |
| **Open Door** | Leaves door open for returns | High |
| **Forever Retiree** | Retires/unretires repeatedly | Very High |
| **Unable to Return** | Physically cannot wrestle again | None |

---

## Retirement Type Details

### Voluntary Peak Retirement

- Worker chooses to leave while still excellent
- Rare and respected
- Creates "what if" legacy
- High memory anchor
- Examples: Very rare (most can't resist)

### Voluntary Decline Retirement

- Worker recognizes diminishing skills
- Leaves before embarrassing themselves
- Dignified exit
- Moderate legacy boost
- Examples: Most "good" retirements

### Forced Injury Retirement

- Career-ending injury forces exit
- Can be tragic or inspiring depending on framing
- Often creates comeback narrative potential
- Legacy depends on career before injury
- Examples: Edge (first), Paige, Tyson Kidd

### Forced Scandal Retirement

- Scandal makes continuing impossible
- Negative legacy impact (usually)
- Low comeback potential (era-dependent)
- May be "quiet" to avoid attention
- Examples: Various throughout history

### Gradual Fade

- Reduces schedule over years
- Part-time, then special appearances, then gone
- Comfortable transition
- Moderate memory impact
- Examples: Undertaker's final years

### Grand Farewell

- Full retirement ceremony
- Retirement match (often loss)
- Speeches, tributes, emotion
- Very high memory anchor
- Examples: Flair (2008), Michaels (2010), Undertaker (2020)

---

## Legacy Impact by Type

| Retirement Type | Base Legacy Modifier |
|-----------------|---------------------|
| Voluntary Peak | +20% |
| Grand Farewell | +15% |
| Voluntary Decline | +5% |
| Gradual Fade | Neutral |
| Forced Injury (inspiring) | +10% |
| Forced Injury (tragic) | Neutral to -5% |
| Quiet Exit | -5% |
| Abrupt Disappearance | -10% |
| Forced Scandal | -20% to -50% |

---

## Comeback Potential by Type

| Retirement Type | Comeback Likelihood |
|-----------------|---------------------|
| Open Door | 70-90% |
| Forever Retiree | 95%+ |
| Voluntary Decline | 40-60% |
| Forced Injury | 20-40% (if healed) |
| Grand Farewell | 30-50% |
| Clean Break | 10-20% |
| Unable to Return | 0% |
| Forced Scandal | 10-30% (era-dependent) |

---

## Worker Personality Effects

| Personality | Retirement Type Tendency |
|-------------|-------------------------|
| **High Ego** | Resists retirement, wants grand farewell |
| **Low Ego** | May accept quiet exit |
| **High Drive** | Fights to continue, forced retirement |
| **Low Drive** | Voluntary decline more likely |
| **Can't Stay Away** | Forever Retiree pattern |
| **Health First** | Clean break, voluntary |

---

## Era Differences

| Era | Typical Retirement Pattern |
|-----|---------------------------|
| **Territory** | Quiet fades, move to managing |
| **80s National** | Some ceremonies, mostly fades |
| **Attitude Era** | Dramatic retirements, many returns |
| **Modern** | Grand farewells expected for stars |

---

## Connected Mechanics

- [[Retirement Triggers]] - What causes each type
- [[Comeback Mechanics]] - Return potential by type
- [[Retirement Matches]] - Ceremonial booking
- [[Hall of Fame System]] - Eligibility affected by type
- [[Crowd Memory]] - Memory anchor strength varies

---

## Open Questions

- [ ] How "worked" retirements are distinguished
- [ ] Multiple retirement type (starts voluntary, becomes forced)
- [ ] Posthumous retirement handling
- [ ] How promotions frame different types publicly
- [ ] Fan reaction variance by type

---

## Implementation Notes

```json
{
  "retirement_record": {
    "worker_id": "worker_001",
    "retirement_type": {
      "by_choice": "voluntary_decline",
      "by_ceremony": "grand_farewell",
      "by_finality": "open_door"
    },
    "legacy_modifier": 0.18,
    "comeback_potential": 55,
    "retirement_date": "1990-04-01",
    "farewell_event": "event_001",
    "public_framing": "emotional_tribute"
  }
}
```
