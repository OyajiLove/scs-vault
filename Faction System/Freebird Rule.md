# Freebird Rule

📛 **MECHANIC:** Stable Title Defense Rotation
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Titles
🔑 **KEYWORDS:** Freebird, title rotation, stable, tag titles, trios, championship defense
📌 **ORIGIN:** Vol 4 (Freebird Rule Stable Booking)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

The Freebird Rule allows stables of 3+ members to rotate which members defend tag team or trios championships. Named after the Fabulous Freebirds, this system creates booking flexibility while adding chemistry considerations: well-oiled groups perform consistently across combinations while dysfunctional stables show inconsistent quality.

---

## Eligibility Requirements

| Requirement | Details |
|-------------|---------|
| **Minimum Members** | 3+ active members (configurable by player) |
| **Title Type** | Tag Team, Trios, or 8-person titles |
| **Promotion Approval** | Some promotions may not allow Freebird defenses |
| **All Members Eligible** | Each defending member must be contracted and healthy |

---

## Defense Rotation Mechanics

| Aspect | Description |
|--------|-------------|
| **Any Two/Three** | Any eligible members can defend |
| **No Fixed Pair** | Champion record applies to stable, not individuals |
| **Booking Flexibility** | Rotate based on storyline, availability, or matchups |
| **Fresh Matchups** | Different combinations create variety |

---

## Chemistry Impact

Not all combinations perform equally:

| Combination Type | Effect |
|------------------|--------|
| **Primary Pair** | Highest chemistry, best match quality |
| **Secondary Pair** | Good chemistry, slightly lower ceiling |
| **Weak Pair** | Lower chemistry, inconsistent matches |
| **Forced Pair** | Members with tension: chemistry penalty |

### Chemistry Development

| Activity | Chemistry Boost |
|----------|-----------------|
| **Defending Together** | +3 to +5 per successful defense |
| **Training Together** | +1 to +2 per month |
| **Winning Feuds** | +5 per feud victory |
| **Tag Match Practice** | +2 per quality match |

---

## Freebird Stables Performance

| Stable Type | Performance Pattern |
|-------------|---------------------|
| **Well-Oiled** (Shield, Elite) | Consistent across all combinations |
| **Leader-Dependent** | Strong with leader, weaker without |
| **Dysfunctional** | Wildly inconsistent, surprise factor |
| **Specialist Pairs** | Certain combos excel, others struggle |

---

## Legacy Bonus

Freebird Rule stables can achieve special legacy status:

| Achievement | Legacy Effect |
|-------------|---------------|
| **Multiple Successful Combos** | "Versatile Champions" recognition |
| **Long Combined Reign** | Stable remembered as dominant |
| **Innovative Defenses** | Creative use of rotation noted |
| **Dynasty** | Freebird reign becomes historic |

---

## Booking Considerations

| Consideration | Description |
|---------------|-------------|
| **Workload Distribution** | Rotate to manage fatigue |
| **Storyline Matching** | Use specific members vs. specific challengers |
| **Build Weaker Pairs** | Develop underused combinations |
| **Protect Injuries** | Rotate around injured members |
| **Heat Management** | Fresh faces prevent staleness |

---

## Historical Examples

| Stable | Freebird Usage |
|--------|----------------|
| **Fabulous Freebirds** | Original: Hayes, Gordy, Roberts rotated |
| **New Day** | Modern example: Kofi, Big E, Woods |
| **Shield** | Could have used but typically fixed pairs |
| **Undisputed Era** | Four-man stable, tag rotation |
| **House of Torture** | NJPW dysfunction example |

---

## Restrictions

| Restriction | Description |
|-------------|-------------|
| **Injury** | Injured members can't defend |
| **Suspension** | Suspended members ineligible |
| **Contract Issues** | Must be contracted to defending promotion |
| **Title Rules** | Some titles may prohibit Freebird |
| **Weight Class** | Junior titles may require eligible weights |

---

## Connected Mechanics

- [[Title System]] - Freebird affects title prestige tracking
- [[Faction Stability]] - Successful rotation builds stability
- [[Faction Loyalty]] - Equal rotation prevents jealousy
- [[Match Rating]] - Chemistry affects match quality

---

## Open Questions

- [ ] How individual vs. stable title records are tracked
- [ ] Freebird rule for singles titles (unlikely but edge case)
- [ ] Maximum stable size for Freebird eligibility
- [ ] How departing members affect title status
- [ ] Cross-promotion Freebird complications

---

## Implementation Notes

```json
{
  "freebird_title": {
    "title_id": "title_tag_001",
    "holding_faction": "faction_001",
    "eligible_members": ["worker_001", "worker_002", "worker_003"],
    "freebird_enabled": true,
    "defense_history": [
      { "date": "1985-06-01", "defenders": ["worker_001", "worker_002"], "result": "retained" },
      { "date": "1985-07-15", "defenders": ["worker_001", "worker_003"], "result": "retained" },
      { "date": "1985-08-20", "defenders": ["worker_002", "worker_003"], "result": "retained" }
    ],
    "chemistry_matrix": {
      "worker_001_worker_002": 88,
      "worker_001_worker_003": 75,
      "worker_002_worker_003": 70
    },
    "combined_reign_days": 120,
    "total_defenses": 3
  }
}
```
