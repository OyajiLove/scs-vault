# Package Deal System

📛 **MECHANIC:** Inseparable Pair Mechanics
🔗 **PARENT SYSTEM:** [[_Tag Team System Index|Tag Team System]]
🧭 **CATEGORY:** Worker Relationships / Booking
🔑 **KEYWORDS:** package deal, tag team, partnership, splitting, loyalty, morale
📌 **ORIGIN:** Vol 1 Extraction #52
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Some partnerships are more than booking convenience: they're inseparable packages. Road Warriors, Rock 'n' Roll Express, Steiners, Outsiders are coded as package deals by default. Splitting them has real consequences beyond storyline drama.

---

## Core Rules (#52)

### Default Package Deal Teams

Certain iconic teams have built-in package deal status:

| Team | Package Integrity |
|------|-------------------|
| Road Warriors | 95% |
| Rock 'n' Roll Express | 90% |
| Steiner Brothers | 85% |
| Outsiders (Hall/Nash) | 80% |
| Midnight Express | 90% |
| British Bulldogs | 75% |
| Hart Foundation | 70% |
| Smoking Gunns | 60% |

**Package Integrity:** How strongly bonded the team is (affects split consequences).

---

## Splitting Consequences

When you break a package deal team:

| Consequence | Description |
|-------------|-------------|
| **Contract Demands Change** | Both workers may demand new terms |
| **Morale Hits** | "Hawk furious he's being booked solo!" |
| **Booking Penalties** | Reduced performance from misused workers |
| **Fan Backlash** | Fans boo singles push for wrong team member |
| **Potential Departure** | Workers may leave if unhappy enough |

### Consequence Severity by Integrity

| Integrity Level | Split Impact |
|-----------------|--------------|
| 90-100% | Catastrophic (major morale crash, likely departures) |
| 75-89% | Severe (significant morale hit, contract issues) |
| 60-74% | Moderate (manageable with proper handling) |
| Below 60% | Minimal (team was already loosely bonded) |

---

## Manager/Wrestler Bonds

Same mechanics apply to iconic manager-wrestler pairings:

| Pairing | Bond Strength |
|---------|---------------|
| Cornette + Midnight Express | 95% |
| Paul Ellering + Road Warriors | 85% |
| Bobby Heenan + Andre | 75% |
| Jimmy Hart + Various | 50% (rotates) |

**Key Rule:** "Where the Midnights went, so too did Cornette."

### Manager Split Consequences

| Action | Effect |
|--------|--------|
| Fire manager but keep talent | Talent morale drop, may follow manager out |
| Keep manager but release talent | Manager may refuse to manage others |
| Split iconic pairing | Faction stability collapse |
| Attempt reconciliation | May repair if not too much damage done |

---

## Package Deal Contract Considerations

| Factor | Effect |
|--------|--------|
| **Joint Contracts** | Must sign/release together |
| **Salary Linkage** | One's raise affects other's expectations |
| **Booking Requirements** | Must appear together or morale hit |
| **Travel Together** | Natural chemistry bonus from proximity |

---

## Singles Push from Tag Team

When pushing one half of a package deal team:

| Scenario | Fan Response |
|----------|--------------|
| Push wrong half solo | Confusion, muted reaction |
| Push right half solo | Can work if partner involved |
| Push while ignoring partner | Partner resentment, team friction |
| Push with partner blessing | Smooth transition possible |

**Example:** "Fans boo singles push for Morton without Gibson" because Morton was the babyface-in-peril, not the hot tag guy.

---

## Repairing Split Package Deals

If a split goes badly, reconciliation is possible:

| Time Since Split | Reconciliation Difficulty |
|------------------|--------------------------|
| 1-3 months | Easy (minor resentment) |
| 4-12 months | Moderate (needs storyline reason) |
| 1-3 years | Hard (trust damaged) |
| 3+ years | Very hard (may never fully repair) |

---

## Connected Mechanics

- [[Manager System/Manager-Client Relationships|Manager-Client Relationships]] - Manager bond mechanics
- [[Relationship System]] - Underlying relationship tracking
- [[Morale System]] - Split consequences affect morale
- [[Contract System/_Contract System Index|Contract System]] - Joint contract handling

---

## Implementation Notes

```json
{
  "package_deal": {
    "team_id": "road_warriors",
    "members": ["hawk", "animal"],
    "package_integrity": 95,
    "manager_bond": {
      "manager_id": "paul_ellering",
      "bond_strength": 85
    },
    "split_history": [],
    "current_status": "intact",
    "morale_linkage": true,
    "contract_linkage": true
  }
}
```

---

## Open Questions

- [ ] How does package integrity decay over time apart?
- [ ] Can new package deals form organically?
- [ ] Cross-promotion package deals (one in WWF, one in WCW)?
- [ ] Family package deals (Hart brothers, Guerreros)?

---

**Document Status:** Locked
**Last Updated:** 2025-12-25
