# Merch Cut System

📛 **MECHANIC:** Merch Cut System
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** merchandise, royalties, revenue share, worker compensation, licensing
📌 **ORIGIN:** Vol 4 (locked with "Locked: MERCH SYSTEM" marker)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Merchandise cuts are more than passive income. They're a marker of worker leverage, a source of push justification, a trigger for backstage resentment, and sometimes a contract-breaking point. High sales with low cut equals morale and trust crisis.

---

## Base Merch Cut Types

| Type | Split | Description | Typical Use |
|------|-------|-------------|-------------|
| **Standard Cut** | 70/30 or 60/40 (promotion keeps majority) | Default for most workers | Roster standard |
| **Equal Split** | 50/50 | Mid-level stars with decent pull | Established workers |
| **Top Talent Clause** | 70/30 (worker keeps majority) | Rare; used to sign or retain big draws | Ace-level stars |
| **In-House Merch Only** | Cut only applies to promotion-run stores | Indie and touring feds | Small promotions |
| **Exclusive Branding** | Worker owns likeness; promotion pays licensing | Colt Cabana model, post-WWE name holders | Independent-minded stars |

---

## Merch Cut Dynamics

### Sales vs. Cut Tension
High merch sales + low cut percentage = major morale and trust issues

| Sales Level | Cut Type | Worker Reaction |
|-------------|----------|-----------------|
| High | Standard (30%) | Resentment builds; demands renegotiation |
| High | Equal (50%) | Satisfied; may still want more |
| High | Top Talent (70%) | Happy; strong loyalty |
| Low | Standard (30%) | No issue (low stakes) |
| Low | Top Talent (70%) | Promotion resentment (overpaying) |

### Morale Impact Formula
```
Merch Morale = (Worker Cut %) × (Sales Rank Modifier) × (Fairness Perception)

Where:
- Worker Cut %: 30, 50, 70, etc.
- Sales Rank Modifier: Top 5 = 1.5, Top 10 = 1.2, Mid = 1.0, Low = 0.8
- Fairness Perception: Based on push level vs. cut (pushed hard with low cut = unfair)
```

---

## Union Merch Protections

If a union is active, it may enforce:

| Protection | Effect |
|------------|--------|
| **Minimum Cut Floor** | No worker can receive less than 40% of their merch sales |
| **Transparency Clause** | Promotion must disclose actual sales figures to workers |
| **Audit Rights** | Union can audit promotion's merch accounting |
| **Collective Merch Pool** | Optional: portion of all merch goes to developmental/injured workers fund |

---

## Merch Types

Not all merch is equal. Worker involvement varies:

| Merch Type | Worker Input | Revenue Potential |
|------------|--------------|-------------------|
| T-Shirts | High (design approval) | Core revenue |
| Action Figures | Medium (likeness) | Collectible market |
| Posters/Photos | Low | Minor |
| Video Games | Low (likeness only) | High (flat fee typical) |
| NFTs/Digital | Variable | Modern era only |
| Replica Gear | High (signature items) | Niche but loyal buyers |

---

## Historical Context

Real-world merch disputes inform this system:

- **CM Punk/WWE:** Claimed underpayment on merch royalties
- **Colt Cabana Model:** Owns everything, licenses to promotions
- **WWE Standard:** Historically 70/30 promotion-heavy; recent improvements
- **AEW Approach:** Better cuts used as recruiting tool

---

## Renegotiation Triggers

Workers may demand merch renegotiation when:

| Trigger | Likelihood |
|---------|------------|
| Merch sales spike (new design, push, viral moment) | High |
| Discover another worker's better deal | Medium-High |
| Contract renewal period | Standard |
| Union formation | Automatic audit |
| After major championship win | Medium |

---

## Connected Mechanics

- [[Contract Types]] - Merch cut is a contract clause
- [[Negotiation Clauses]] - Can include exclusive branding
- [[Contract Morality Score]] - Unfair merch deals lower morality score
- [[Worker Resistance]] - Poor merch treatment triggers pushback
- [[Union System]] - Unions can mandate merch protections

---

## Open Questions

- [ ] Exact merch revenue formulas (units sold × price × cut %)
- [ ] How merch sales affect popularity independently
- [ ] Cross-promotion merch rules (who gets cut when worker appears elsewhere)
- [ ] Counterfeit/bootleg merch impact on official sales

---

## Implementation Notes

```json
{
  "merch_contract": {
    "cut_type": "standard",
    "worker_percentage": 30,
    "promotion_percentage": 70,
    "transparency_clause": false,
    "exclusive_branding": false,
    "in_house_only": false
  },
  "merch_performance": {
    "sales_rank": 7,
    "monthly_units": 2500,
    "monthly_revenue": 62500,
    "worker_earnings": 18750,
    "satisfaction_score": 45
  }
}
```
