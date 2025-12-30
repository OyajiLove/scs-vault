# Loyalty System

📛 **MECHANIC:** Loyalty System
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** loyalty, emotional bonds, formative fed, mentor, faction, promotion loyalty
📌 **ORIGIN:** Vol 4 (Worker Booking Decisions priority system, loyalty axes)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Loyalty isn't a single number. Workers have multiple loyalty axes: Promotion, Faction, Mentor, Friend, Self. These compete when booking decisions conflict. A worker might stay at a promotion they hate because their best friend is there, or leave a beloved home fed for a mentor's new venture.

---

## Loyalty Axes

| Axis | Description | Priority Weight |
|------|-------------|-----------------|
| **Promotion Loyalty** | Emotional bond to home/formative promotion | High |
| **Faction Loyalty** | Commitment to stable, clique, or alliance | Medium-High |
| **Mentor Loyalty** | Bond with teacher, trainer, or guide | High |
| **Friend Loyalty** | Personal relationships with peers | Medium |
| **Self Loyalty** | Career advancement, money, legacy | Variable |

---

## Loyalty Score Ranges

| Range | Description |
|-------|-------------|
| 1-5 | Mercenary (will leave for any better offer) |
| 6-10 | Low (easily swayed, needs incentive to stay) |
| 11-15 | Moderate (considers leaving but weighs factors) |
| 16-20 | High (strong emotional attachment, hard to poach) |

---

## Loyalty Formation

### Time-Based Defaults
| Time with Promotion | Baseline Loyalty (if treated fairly) |
|--------------------|-------------------------------------|
| 0-1 years | 5-8 (minor, transactional) |
| 1-2 years | 8-12 (developing emotional bond) |
| 3-5 years | 12-16 (moderate loyalty) |
| 5-10 years | 16-18 (high loyalty potential) |
| 10+ years | 18-20 (institutional loyalty) |

### Modifiers
| Factor | Loyalty Change |
|--------|----------------|
| Good booking treatment | +1 to +3 per year |
| Title reign(s) | +2 to +5 |
| Burial or mistreatment | -5 to -15 |
| Broken promises | -3 to -8 |
| Mentor relationship at promotion | +3 to +6 |
| Best friend at promotion | +2 to +4 |
| Personal scandal covered for | +5 to +10 |
| Publicly humiliated | -10 to -20 |

---

## Formative Fed Loyalty

Special loyalty bonus for the promotion where worker "came up":

| Condition | Effect |
|-----------|--------|
| Trained there | +5 permanent loyalty |
| First TV appearance | +3 |
| First title | +5 |
| Career-making moment | +5 to +10 |
| Stayed 5+ years early career | +10 |

**Formative Fed Priority:** Workers may turn down better offers to stay with formative promotion, or feel guilt when leaving.

---

## Grudging Stay vs. True Bond

Not all "staying" is equal:

| Stay Type | Description | Risk |
|-----------|-------------|------|
| **True Loyalty** | Genuine emotional attachment | Low flight risk |
| **Grudging Stay (Money)** | Only there for paycheck | Will leave for better offer |
| **Grudging Stay (Friends)** | Stays for colleagues, not promotion | Leaves when friends leave |
| **Grudging Stay (Fear)** | Afraid of blacklist or career damage | Resentful, may sabotage |

---

## Loyalty Conflicts

When axes compete:

### Example: Scott Hall, 1996
| Axis | Score | Factor |
|------|-------|--------|
| WWF Promotion Loyalty | Low (3) | Felt undervalued |
| Kliq Faction Loyalty | High (18) | Deep brotherhood |
| Nash Friend Loyalty | High (19) | Best friend |
| Self Loyalty | High (17) | Money, fresh start |

**Result:** Low promotion loyalty + high friend/self loyalty = jump to WCW inevitable when Nash moved.

### Decision Priority Layers
1. **Contractual Obligations** - Full-time contracts override if airtight
2. **Emotional Formative Loyalty** - Home promotion heavily biases workers
3. **Prestige/Pay Opportunity** - Bigger promotions may override if emotional ties weak
4. **Event Type and Stakes** - Major anniversaries, title defenses spike loyalty temporarily
5. **Mutually Negotiated Agreements** - Peaceful handling allows priority negotiation

---

## Loyalty Impact on Contracts

| Loyalty Level | Contract Behavior |
|---------------|-------------------|
| 1-5 | Shops around constantly, signs shortest deals |
| 6-10 | Open to offers, negotiates hard |
| 11-15 | Gives promotion first chance to match |
| 16-20 | Signs long-term, may accept less money |

---

## Loyalty Archetypes

| Archetype | Loyalty Pattern | Example |
|-----------|-----------------|---------|
| **Mercenary Soul** | 1-8 across all axes; jumps for money | Lex Luger |
| **Loyal Soldier** | 16-20 promotion; stays despite bad booking | Mark Henry |
| **Faction First** | Low promotion, high faction | nWo members |
| **Mentor's Shadow** | Follows mentor anywhere | Many dojo products |
| **Terminal Nomad** | No loyalty anywhere; drifts forever | Some journeymen |

---

## Connected Mechanics

- [[Hidden Personality]] - Base Loyalty rating (1-20)
- [[Worker Resistance]] - Low loyalty + mistreatment = resistance
- [[Contract Types]] - Loyalty affects signing behavior
- [[Faction System]] - Faction loyalty axis
- [[Turn Engine]] - Betrayals damage loyalty permanently

---

## Open Questions

- [ ] Exact formulas for loyalty axis priority calculations
- [ ] Loyalty decay over time if not reinforced
- [ ] Cross-promotion loyalty (can worker be loyal to two feds?)
- [ ] Redemption path for damaged loyalty
- [ ] How departures affect remaining workers' loyalty

---

## Implementation Notes

```json
{
  "worker_loyalty": {
    "worker_id": "worker_001",
    "promotion_loyalty": {
      "promotion_id": "promo_001",
      "score": 14,
      "is_formative": true,
      "years_tenure": 6
    },
    "faction_loyalty": {
      "faction_id": "faction_001",
      "score": 17
    },
    "mentor_loyalty": {
      "mentor_id": "worker_042",
      "score": 16
    },
    "friend_loyalty": [
      { "worker_id": "worker_015", "score": 18 },
      { "worker_id": "worker_023", "score": 12 }
    ],
    "self_loyalty": 13,
    "grudging_stay": false,
    "stay_reason": "true_bond"
  }
}
```
