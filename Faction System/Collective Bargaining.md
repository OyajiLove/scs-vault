# Collective Bargaining

📛 **MECHANIC:** Package Deal Contracts
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Contracts / Relationships
🔑 **KEYWORDS:** package deal, collective bargaining, joint contract, Road Warriors, Bucks
📌 **ORIGIN:** Vol 4 (Contract and Negotiation Personality Layers)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Some teams and factions negotiate contracts together as a unit. Road Warriors and the Young Bucks absolutely collectively bargain and won't sign without each other. Less cohesive teams (two singles thrown together) won't be so rigid. The system tracks contract binding between workers.

---

## Contract Binding Types

| Type | Description | Separation Difficulty |
|------|-------------|----------------------|
| **Package Deal** | Won't sign without partner(s) | Very High |
| **Preferred Partners** | Want to stay together, but negotiable | Moderate |
| **Loose Alliance** | Happy to negotiate separately | Low |
| **Forced Together** | Would prefer to separate | None |

---

## Package Deal Characteristics

When workers are package deal bound:

| Behavior | Description |
|----------|-------------|
| **Joint Negotiation** | Single contract covers all members |
| **Synchronized Terms** | Same start/end dates, similar pay ratios |
| **Mutual Exit Clauses** | If one leaves, others may follow |
| **Veto Power** | Can block deals that exclude partner |
| **Shared Creative** | Booking decisions affect all |

---

## What Creates Package Deals

| Factor | Binding Strength |
|--------|------------------|
| **Family/Blood** | Very Strong |
| **Long-term Tag Team** | Strong |
| **High Friend Loyalty** | Strong |
| **Shared History** | Moderate |
| **Manager Representation** | Moderate |
| **Strategic Alliance** | Weak |

### Package Deal Formation

```
Package_Deal_Likelihood = 
  (Friend_Loyalty × 0.4) +
  (Time_Together_Years × 5) +
  (Shared_Success_Bonus × 0.3) +
  (Family_Bonus if applicable)
```

---

## Road Warriors Example

| Factor | Status |
|--------|--------|
| **Years Together** | 10+ years |
| **Friend Loyalty** | Maximum |
| **Brand Identity** | Inseparable |
| **Contract Type** | Absolute package deal |
| **Separation Event** | Only injury (Animal 1993) |

When Animal was injured, Hawk didn't negotiate for solo WWF deal: he went to Japan and formed spiritual successor team while waiting.

---

## Young Bucks Example

| Factor | Status |
|--------|--------|
| **Family Bond** | Brothers |
| **Years Together** | Career-long |
| **Brand Identity** | Inseparable |
| **Contract Type** | Absolute package deal |
| **Leverage** | Major: promotions must take both |

---

## Negotiation Dynamics

### For Package Deals

| Promotion Behavior | Effect |
|--------------------|--------|
| **Wants Both** | Normal negotiation |
| **Wants One Only** | Rejected; must take both |
| **Tries to Split** | Loyalty tested; usually fails |
| **Offers Imbalanced Pay** | May cause internal tension |

### Breaking Package Deals

What can separate package deal teams:

| Trigger | Likelihood |
|---------|------------|
| **Major Betrayal** | High (emotional break) |
| **Money Disparity** | Moderate (ego conflicts) |
| **Career Divergence** | Moderate (one outgrows other) |
| **Injury (Long-term)** | Low (usually wait) |
| **Death/Retirement** | Forced separation |

---

## Loose Team Contracts

Less cohesive teams negotiate separately:

| Scenario | Behavior |
|----------|----------|
| **Singles Thrown Together** | Separate contracts, may not renew together |
| **Faction Members** | Individual deals unless core duo |
| **Manager's Clients** | Manager may bundle, but workers separate |

---

## Faction Collective Bargaining

Larger groups may have tiered binding:

| Tier | Members | Binding |
|------|---------|---------|
| **Core** | Leader + right-hand | Package deal |
| **Inner Circle** | Key members | Preferred partners |
| **Outer Members** | Associates | Loose alliance |

---

## Contract Loyalty Effects

How package deals affect loyalty:

| Scenario | Effect |
|----------|--------|
| **Partner Signs First** | Pressure to follow |
| **Partner Gets Better Deal** | Ego friction possible |
| **Promotion Wants Split** | Tests friendship loyalty |
| **One Partner Unhappy** | May drag other into conflict |

---

## Historical Package Deal Failures

| Team | What Happened |
|------|---------------|
| **Rockers** | Michaels outgrew Jannetty; package dissolved |
| **Mega Powers** | Ego conflicts shattered alliance |
| **Hart Foundation** | Injury + creative differences |

---

## Connected Mechanics

- [[Contract System]] - Contract structure and negotiation
- [[Faction Loyalty System]] - Friend loyalty determines binding
- [[Tag Team Mechanics]] - Partnership basis for deals
- [[Faction Formation]] - How teams form affects contracts

---

## Open Questions

- [ ] Exact package deal negotiation flow
- [ ] How promotions handle package deal salary splitting
- [ ] Cross-promotion package deals (same team, different feds)
- [ ] Manager's role in collective bargaining
- [ ] Package deal breach penalties

---

## Implementation Notes

```json
{
  "package_deal": {
    "deal_id": "pkg_001",
    "members": ["worker_001", "worker_002"],
    "binding_type": "package_deal",
    "binding_strength": 95,
    "formation_date": "1983-06-15",
    "current_contract": {
      "promotion_id": "promo_001",
      "start_date": "1985-01-01",
      "end_date": "1987-12-31",
      "total_value": 500000,
      "split_ratio": [0.5, 0.5]
    },
    "binding_factors": {
      "friend_loyalty": 98,
      "years_together": 12,
      "family_bond": false,
      "shared_success": "high"
    },
    "separation_risk": "very_low"
  }
}
```
