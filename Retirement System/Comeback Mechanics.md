# Comeback Mechanics

📛 **MECHANIC:** How Retired Workers Return
🔗 **PARENT SYSTEM:** [[_Retirement System Index|Retirement System]]
🧭 **CATEGORY:** Worker Lifecycle
🔑 **KEYWORDS:** comeback, return, unretire, one more match, return pop
📌 **ORIGIN:** Vol 1-4 (Can't Stay Away tag, One More Match, Forever Retiree, Comeback Arcs)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Retirement isn't always permanent. Many workers return after "final" farewells, drawn back by the spotlight, money, or unfinished business. Comebacks generate massive pops but must contend with physical decline and the risk of tarnishing legacy. The system tracks comeback potential, return conditions, and the inevitable decay that follows.

---

## Comeback Potential Factors

| Factor | Effect on Comeback Chance |
|--------|--------------------------|
| **Can't Stay Away Tag** | +30% comeback likelihood |
| **One More Match Tag** | Very easy to talk back |
| **Forever Retiree Tag** | 95%+ will return eventually |
| **Unable To Wrestle Again** | 0% chance (physically impossible) |
| **High Ego** | Misses spotlight, more likely |
| **High Drive** | Restless, wants competition |
| **Financial Need** | Money talks |
| **Unfinished Business** | Story hook for return |

---

## Comeback Types

| Type | Description | Example |
|------|-------------|---------|
| **One More Match** | Single appearance, truly final | Terry Funk (repeatedly) |
| **Limited Run** | Short program, few months | Goldberg returns |
| **Part-Time Legend** | Sporadic appearances | Undertaker (2010s) |
| **Full Return** | Back on regular schedule | Edge (2020) |
| **Desperation Return** | Needs money, has to work | Various |
| **Dream Match** | Returns for specific opponent | Many |
| **Revenge/Unfinished** | Returns to settle score | Story-driven |

---

## Physical Reality on Return

Retired workers don't return at peak:

| Time Retired | Physical Decline |
|--------------|------------------|
| **Under 1 year** | Minimal: -5% to -10% |
| **1-2 years** | Moderate: -10% to -20% |
| **3-5 years** | Significant: -20% to -35% |
| **5-10 years** | Major: -35% to -50% |
| **10+ years** | Severe: -50%+ |

### Decline Modifiers

| Factor | Effect |
|--------|--------|
| **Stayed in shape** | Reduces decline |
| **Injury that caused retirement** | May not heal |
| **Age at return** | Older = more decline |
| **Good Genetics tag** | Slower decline |
| **Bad Genetics tag** | Faster decline |

---

## Return Pop Dynamics

Comebacks generate huge initial reactions:

| Return Type | Initial Pop Bonus |
|-------------|-------------------|
| **Surprise Return** | +50% to +100% |
| **Announced Return** | +25% to +50% |
| **Long-Awaited** | +75% to +150% |
| **Dream Match Context** | +50% |
| **Revenge Story** | +40% |

### Pop Decay

| Time Since Return | Pop Retention |
|-------------------|---------------|
| **First Night** | 100% (peak) |
| **First Month** | 80-90% |
| **3 Months** | 60-75% |
| **6 Months** | 40-60% |
| **1 Year** | 25-40% (normalized) |

---

## Comeback Booking Considerations

| Consideration | Risk |
|---------------|------|
| **Overexposure** | Return pop burns out fast |
| **Physical Limitations** | Can't do old spots safely |
| **Nostalgia vs. Reality** | Fans remember peak, not current |
| **Booking Around Decline** | Shorter matches, protection needed |
| **Legacy Risk** | Bad return can tarnish memory |

---

## Talking Workers Out of Retirement

| Factor | Persuasion Modifier |
|--------|---------------------|
| **One More Match tag** | Very easy |
| **Can't Stay Away tag** | Easy |
| **High Ego** | Moderate (appeals to pride) |
| **Financial Offer** | Scales with need |
| **Dream Match** | Strong motivator |
| **Revenge Angle** | Strong motivator |
| **Health First tag** | Very difficult |
| **Clean Break retirement** | Difficult |

---

## Multiple Comebacks

Some workers return repeatedly:

| Pattern | Description |
|---------|-------------|
| **Forever Retiree** | Retires 3+ times, always returns |
| **Periodic Legend** | Returns every few years |
| **Failed Retirements** | Can't make it stick |
| **Genuine Final** | Actually stays retired (rare) |

### Diminishing Returns

| Comeback Number | Pop Modifier |
|-----------------|--------------|
| **First Return** | 100% (full pop) |
| **Second Return** | 75-85% |
| **Third Return** | 50-70% |
| **Fourth+ Return** | 30-50% (cynicism sets in) |

---

## Return Failure Scenarios

| Scenario | Legacy Impact |
|----------|---------------|
| **Terrible Match** | -10% to -20% legacy |
| **Obvious Physical Decline** | -5% to -15% |
| **Injured During Return** | Variable |
| **Failed Story** | -5% to -10% |
| **Embarrassing Performance** | -15% to -25% |

---

## Historical Examples

| Worker | Comeback Pattern | Success |
|--------|------------------|---------|
| **Terry Funk** | Forever Retiree | Mixed (legendary for trying) |
| **Shawn Michaels** | 4-year absence, full return | Legendary |
| **Edge** | 9-year absence, full return | Very successful |
| **Goldberg** | Multiple returns | Diminishing |
| **Sting** | Multiple promotion returns | Generally successful |
| **Hulk Hogan** | Constant returns | Varying success |

---

## Connected Mechanics

- [[Retirement Types]] - Type affects comeback potential
- [[Retirement Triggers]] - Original cause affects return viability
- [[Injury System]] - Physical capability on return
- [[Crowd Memory]] - Return becomes memory anchor
- [[Popularity System]] - Return pop dynamics

---

## Open Questions

- [ ] Exact comeback pop formulas
- [ ] How to handle "worked" retirements for storylines
- [ ] Multiple promotion comeback coordination
- [ ] How comebacks affect HOF eligibility timing
- [ ] Ring rust mechanics

---

## Implementation Notes

```json
{
  "comeback_state": {
    "worker_id": "worker_001",
    "currently_retired": true,
    "comeback_potential": 72,
    "times_retired": 2,
    "times_returned": 1,
    "years_since_retirement": 3,
    "physical_capability_estimate": 55,
    "persuasion_factors": {
      "financial_need": 30,
      "ego_appeal": 70,
      "dream_match_available": true,
      "revenge_story_hook": false
    },
    "return_pop_modifier": 0.75,
    "tags": ["cant_stay_away", "one_more_match"]
  }
}
```
