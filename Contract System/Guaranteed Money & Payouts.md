# Guaranteed Money & Payouts

📛 **MECHANIC:** Guaranteed Money & Payouts
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** guaranteed contracts, buyouts, settlements, payout liability, WCW, financial risk
📌 **ORIGIN:** Vol 4 (locked with "Locked: Advanced Contract Dynamics" marker)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Guaranteed contracts mean workers get paid whether booked or not. This creates the 90s WCW disaster potential: a bloated roster of highly paid workers sitting at home while the promotion hemorrhages money. Every guaranteed deal is a financial bet on the worker's value.

---

## Payout Liability Rules

| Event | Outcome |
|-------|---------|
| **Worker is fired or released early** | Promotion owes full remainder of contract (or negotiated settlement) |
| **Promotion reduces push or usage** | Worker may protest and still gets paid |
| **Promotion buries worker creatively** | Could lead to grievance or fan/media backlash |
| **Worker leaves voluntarily** | May lose payout (depends on contract language) |

---

## Settlement Negotiation

When terminating a guaranteed contract early, promotions can negotiate:

| Settlement Type | Description | Worker Acceptance Factors |
|-----------------|-------------|---------------------------|
| **Full Payout** | Pay entire remaining contract value | Always accepted (worker's right) |
| **Negotiated Reduction** | Pay percentage of remaining value | Depends on market options, loyalty, age |
| **Deferred Payment** | Pay over time rather than lump sum | Worker needs money now vs. security |
| **Trade to Another Promotion** | Transfer contract obligation | Worker willingness + destination quality |
| **Mutual Release** | Both parties walk away clean | Worker has better opportunity elsewhere |

### Settlement Factors

| Factor | Effect on Settlement |
|--------|---------------------|
| **Worker Age** | Older = more likely to accept reduced settlement |
| **Market Demand** | High demand = worker wants full payout to leverage next deal |
| **Loyalty Score** | High loyalty = may accept less to help promotion |
| **Backstage Relations** | Poor relations = wants maximum payout as revenge |
| **Financial Health** | Worker's personal finances affect urgency |

---

## Guaranteed Contract Risks

### For Promotions:
- **Overpaying idle talent:** Paying millions for workers not being used
- **Locker room resentment:** Active workers see benched stars earning more
- **Financial death spiral:** WCW 2000 scenario (too many guarantees, can't release anyone)
- **Creative stagnation:** Afraid to push new talent over expensive signed stars

### For Workers:
- **Career stall:** Getting paid but not building legacy
- **Skill atrophy:** Not working regularly hurts in-ring ability
- **Reputation damage:** "Coasting on guaranteed money" perception
- **Post-contract market:** No recent work makes next deal harder to get

---

## Historical Models

| Promotion | Guaranteed Contract Culture | Outcome |
|-----------|----------------------------|---------|
| **WCW (1996-2001)** | Widespread, massive deals | Financial collapse |
| **WWE (Modern)** | Selective, usually justified | Sustainable but worker resentment |
| **AEW (2019-Present)** | Common, competitive tool | Recruiting advantage, financial risk |
| **NJPW** | Rare; mostly base + bonus structure | Lean operation |

---

## Buyout Calculations

When terminating early:

```
Buyout Amount = (Remaining Months × Monthly Salary) × Settlement Modifier

Where:
- Remaining Months: Time left on contract
- Monthly Salary: Base guaranteed pay
- Settlement Modifier: 1.0 (full), 0.75 (negotiated), 0.5 (mutual), etc.
```

### Example:
- Worker has 18 months remaining at $250,000/month
- Full buyout: 18 × $250,000 = $4,500,000
- Negotiated (75%): $3,375,000
- Mutual release (50%): $2,250,000

---

## Renegotiation Mechanics

Workers may demand raises if:
- Performance exceeds contract tier
- Merch sales spike significantly
- Championship wins elevate status
- Discovery of lower-paid workers getting similar push
- Market value increases (other promotions bidding)

Promotions may request restructure if:
- Worker underperforms expectations
- Financial crisis requires cost-cutting
- Worker agrees to reduced role for security
- Union CBA mandates adjustments

---

## Connected Mechanics

- [[Contract Types]] - Guaranteed is a base contract type
- [[Firing System]] - Guaranteed contracts complicate termination
- [[Contract Morality Score]] - Buyout handling affects morality
- [[Financial System]] - Guaranteed obligations affect promotion budget
- [[Morale System]] - Idle guaranteed workers may have morale issues

---

## Open Questions

- [ ] Exact settlement negotiation success rate formulas
- [ ] Insurance/loan options for guaranteeing contracts
- [ ] Partial guarantee structures (50% guaranteed, 50% bonus)
- [ ] Multi-year guarantee cap rules

---

## Implementation Notes

```json
{
  "guaranteed_contract": {
    "worker_id": "worker_001",
    "total_value": 3000000,
    "monthly_salary": 250000,
    "remaining_months": 12,
    "remaining_value": 3000000,
    "termination_options": {
      "full_buyout": 3000000,
      "negotiated_70": 2100000,
      "mutual_50": 1500000
    },
    "status": "active"
  }
}
```
