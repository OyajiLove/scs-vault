# Faction Formation

📛 **MECHANIC:** Faction Creation and Worker Lobbying
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** formation, lobbying, chemistry, alliance, team building
📌 **ORIGIN:** Vol 4 (Worker-Led Formation Lobbying)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Factions form through worker initiative, booker decision, or organic chemistry development. Workers can lobby to form teams or factions, but success depends on personality compatibility, booking momentum, and promotion willingness. Formation attempts can fail or be reluctantly accepted, causing tension down the road.

---

## Formation Types

| Type | Description | Examples |
|------|-------------|----------|
| **Booker-Created** | Promotion assigns workers to group | Nation of Domination, Nexus |
| **Worker-Initiated** | Workers lobby to team up | Kliq, Elite |
| **Organic Chemistry** | Natural bonds from tag runs, feuds | Shield, Golden Lovers |
| **Family/Bloodline** | Pre-existing family connections | Hart Foundation, Anoa'i |
| **Ideology-Driven** | Shared philosophy/worldview | Straight Edge Society |
| **Emergency Alliance** | Temporary against common threat | Unlikely allies storylines |

---

## Worker-Led Formation Lobbying

Workers can request faction formation:

| Factor | Effect on Success |
|--------|-------------------|
| **Strong Backstage Loyalty** | Higher chance: promotion sees natural chemistry |
| **High Booking Momentum** | Promotion more willing if workers are hot |
| **Existing Friendships** | Pre-tagged friendships boost approval |
| **Singles Ambitions** | Workers with high solo drive may resist |
| **High Ego** | May want to lead, not follow |
| **Low Loyalty** | May not commit fully to faction |

### Lobbying Outcomes

| Outcome | Effect |
|---------|--------|
| **Approved Enthusiastically** | Full support, booking investment |
| **Approved Reluctantly** | Minimal support, may be tested first |
| **Denied** | Workers may resent, lobby again later |
| **Partial Approval** | Some members approved, others not |

---

## Faction Expansion

Existing factions can add members:

| Scenario | Consideration |
|----------|---------------|
| **Junior Partner Addition** | Adds depth, fresh matchups |
| **Muscle Addition** | Protection, intimidation factor |
| **Charisma Piece** | Promo/entertainment boost |
| **Legacy Addition** | Family member, trainee joins |

### Expansion Risks

| Risk | Description |
|------|-------------|
| **Bloat** | Too many members dilutes identity (nWo syndrome) |
| **Chemistry Mismatch** | New member doesn't fit |
| **Jealousy** | Existing members resent new addition |
| **Power Struggle** | New member challenges leadership |

---

## Resistance to Forced Teams

Not all workers accept faction assignment:

| Worker Type | Resistance Level |
|-------------|------------------|
| **High Ego** | Resists unless leader position |
| **Strong Singles Ambition** | Resists team assignment |
| **Low Loyalty** | May accept but not commit |
| **High Paranoia** | Suspicious of teammates |
| **Independent Spirit** | Prefers solo career |

### Forced Formation Consequences

| Outcome | Description |
|---------|-------------|
| **Reluctant Cooperation** | Works but no chemistry bonus |
| **Passive Sabotage** | Underperforms in faction matches |
| **Early Exit** | Leaves faction quickly |
| **Betrayal Setup** | Resentment builds to explosion |

---

## Chemistry Development

How faction bonds strengthen:

| Activity | Chemistry Boost |
|----------|-----------------|
| **Tag Team Matches** | +2 to +5 per quality match |
| **Successful Feuds** | +5 to +10 per feud win |
| **Title Reign** | +10 if defended together |
| **Shared Hardship** | +5 to +15 (injuries, losses overcome) |
| **Backstage Bonding** | +1 to +3 over time |
| **Promo Segments Together** | +1 to +2 per segment |

### Chemistry Degradation

| Event | Chemistry Loss |
|-------|----------------|
| **Uneven Push** | -3 to -5 per month |
| **Failed Goals** | -5 to -10 per failure |
| **Backstage Conflict** | -5 to -15 |
| **Public Disagreement** | -3 to -8 |
| **Injury Absence** | -2 per month absent |

---

## Promotion Response to Formation

How promotions react:

| Action | Effect |
|--------|--------|
| **Support Organic Alliances** | Boosts booking memory, strengthens roster connections |
| **Ignore Worker Chemistry** | Risks backfiring: lost momentum, fan rejection |
| **Force Incompatible Groups** | High failure rate, resentment |
| **Poach Successful Factions** | Target established groups to destabilize rivals |

---

## Connected Mechanics

- [[Faction Stability]] - How well the group holds together
- [[Faction Loyalty]] - Individual member commitment
- [[Hidden Personality]] - Ego, Loyalty affect formation success
- [[Contract System]] - Package deal negotiations

---

## Open Questions

- [ ] Exact lobbying success probability formulas
- [ ] How long chemistry takes to develop
- [ ] AI faction formation triggers
- [ ] Cross-faction membership (worker in multiple groups)
- [ ] Manager role in faction formation

---

## Implementation Notes

```json
{
  "formation_attempt": {
    "requesting_workers": ["worker_001", "worker_002"],
    "proposed_name": "The Alliance",
    "proposed_leader": "worker_001",
    "lobbying_strength": 72,
    "chemistry_baseline": 65,
    "compatibility_score": 78,
    "promotion_response": "approved_enthusiastically",
    "resistance_flags": [],
    "formation_date": "1985-06-01"
  }
}
```
