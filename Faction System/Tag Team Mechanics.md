# Tag Team Mechanics

📛 **MECHANIC:** Partnership Dynamics
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** tag team, partnership, split, reunion, chemistry, emotional memory
📌 **ORIGIN:** Vol 4 (Tag Team and Faction Expanded Systems v2.0, Tag Split Emotional Memory)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Tag teams are living partnerships with chemistry, emotional memory, and evolution potential. Breakups are emotional detonations that can fuel feuds, character growth, and fan legacy for decades. Teams that reunite after injury or betrayal can recapture part (but never all) of the original magic.

---

## Tag Team Types

| Type | Description | Chemistry Baseline |
|------|-------------|-------------------|
| **Natural Partners** | Formed organically, similar styles | High |
| **Package Deal** | Signed together, won't separate | Very High |
| **Mentor/Protégé** | Veteran guides younger talent | Moderate |
| **Odd Couple** | Contrasting styles forced together | Variable |
| **Singles Thrown Together** | Two solos paired by booker | Low |
| **Sibling/Family** | Blood relation | High (but volatile) |
| **Spiritual Successor** | New partner carries old team's spirit | Moderate |

---

## Chemistry System

Chemistry determines tag team effectiveness:

### Chemistry Components

| Factor | Weight |
|--------|--------|
| **Friendship Loyalty** | 30% |
| **Style Compatibility** | 25% |
| **Shared Goals** | 15% |
| **Time Together** | 15% |
| **Recent Success** | 10% |
| **Ego Balance** | 5% |

### Chemistry Effects

| Level | Match Bonus | Stability |
|-------|-------------|-----------|
| **Excellent (90-100)** | +15% to tag matches | Very stable |
| **Good (70-89)** | +10% | Stable |
| **Adequate (50-69)** | +5% | Some tension |
| **Poor (30-49)** | No bonus | Visible cracks |
| **Toxic (0-29)** | -10% | Imminent collapse |

---

## Tag Split Categories

| Split Type | Memory Type | Feud Heat | Example |
|------------|-------------|-----------|---------|
| **Mentor Jealousy Betrayal** | Deep, violent, permanent scars | Maximum | Magnum/Mr. Wrestling II |
| **Ego Explosion** | One partner outgrows other | High | Michaels/Jannetty |
| **Cold Contract Split** | One leaves for money, no arc | Low (decays fast) | Generic departures |
| **Injury Hiatus** | Forced apart, may reunite | Moderate | Road Warriors 1993 |
| **Storyline Heel Turn** | Planned betrayal for angle | High if executed well | Rollins/Shield |
| **Amicable Split** | Both pursue singles | Low | Respectful partings |

---

## Tag Split Emotional Memory

Breakups create lasting impact:

| Split Severity | Memory Duration | Legacy Effect |
|----------------|-----------------|---------------|
| **Violent Betrayal** | Permanent | Defines both careers |
| **Heated Breakup** | 5-10 years | Major career chapter |
| **Cold Departure** | 1-3 years | Minor footnote |
| **Amicable Split** | 6-12 months | Reunion always possible |

---

## Road Warriors 1993 Case Study

| Event | What Happened | System Simulation |
|-------|---------------|-------------------|
| **Injury + Insurance** | Animal collected Lloyd's of London policy | Injury + Insurance: can't wrestle while claiming |
| **Tag Splintering** | Hawk wanted to keep working | Career continuation desperation |
| **New Alliance** | Hawk + Kensuke as "Hell Raisers" | Spiritual successor formation |
| **Identity Drift** | Road Warrior aura continued in Japan | Team spirit survives geographically |
| **Eventual Reunion** | Reunited mid-90s, not at same peak | Redemption/Reunion layer: partial magic |

---

## Reunion Mechanics

When split teams reunite:

| Factor | Effect |
|--------|--------|
| **Time Apart** | Longer = more nostalgia potential |
| **How They Split** | Amicable = easier; betrayal = harder |
| **Both Still Active** | Required for full reunion |
| **Fan Memory** | Strong original memory = bigger pop |
| **Changed Dynamics** | One may have surpassed other |

### Reunion Chemistry

```
Reunion_Chemistry = Original_Chemistry × 0.7 + Nostalgia_Bonus - Grudge_Penalty
```

Reunited teams rarely reach original peak but can create new legacy.

---

## Tag Team Overstaying

Teams that refuse to split past expiration risk:

| Risk | Description |
|------|-------------|
| **Career Stagnation** | "What if they had gone solo?" memory |
| **Diminishing Returns** | Fan interest declines |
| **Booking Difficulty** | Hard to keep fresh |
| **Singles Skills Atrophy** | Workers lose solo capability |

---

## Spiritual Successor Teams

When partners form new teams carrying old spirit:

| Scenario | Example |
|----------|---------|
| **Injury replacement** | Hawk + Kensuke while Animal recovers |
| **Death/retirement** | New partner honors legacy |
| **Regional branch** | Same gimmick, different territory |

Spiritual successors inherit partial chemistry and fan memory.

---

## Connected Mechanics

- [[Faction Formation]] - How teams initially form
- [[Faction Loyalty System]] - Partnership loyalty
- [[Freebird Rule]] - Stable tag mechanics
- [[Crowd Memory]] - Split moments become anchors
- [[Contract System]] - Package deal negotiations

---

## Open Questions

- [ ] Exact chemistry calculation formulas
- [ ] How long until team feels "stale"
- [ ] Reunion chemistry restoration over time
- [ ] Three-way team dynamics (one leaves, two remain)
- [ ] Manager attachment to tag teams

---

## Implementation Notes

```json
{
  "tag_team": {
    "team_id": "team_001",
    "name": "The Road Warriors",
    "members": ["worker_hawk", "worker_animal"],
    "type": "package_deal",
    "formation_date": "1983-06-15",
    "chemistry": 95,
    "status": "active",
    "titles_won": 12,
    "signature_moves": ["Doomsday Device"],
    "split_history": [
      {
        "date": "1993-01-01",
        "type": "injury_hiatus",
        "initiator": null,
        "reason": "Animal back injury",
        "reunion_date": "1996-01-01"
      }
    ],
    "current_chemistry_factors": {
      "friendship": 95,
      "style_compatibility": 90,
      "shared_goals": 85,
      "time_together": 100,
      "recent_success": 80,
      "ego_balance": 85
    }
  }
}
```
