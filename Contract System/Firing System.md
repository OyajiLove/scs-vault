# Firing System

📛 **MECHANIC:** Firing System
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** termination, firing, release, just cause, buyout, consequences
📌 **ORIGIN:** Vol 4 (locked at line 70402 with "LOCKED: CONTRACTS + FIRING SYSTEM")
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Firing has massive consequences under every contract type, especially unionization. Everything you do is remembered, and sometimes leaked. You're not a fantasy GM; you're a labour boss in a volatile ecosystem. Handle terminations poorly and watch your reputation, morale, and finances collapse.

---

## Termination Rules by Contract Type

| Contract Type | Termination Ease | Financial Obligation | Worker Recourse |
|---------------|------------------|---------------------|-----------------|
| **Handshake** | Immediate, no notice | None | None (worker can also leave instantly) |
| **Per-Appearance** | Stop booking | None | None |
| **Written (Time-Locked)** | Breach clause or buyout | Buyout if early | Potential lawsuit |
| **Guaranteed** | Full payout required | Remainder of contract | Strong legal position |
| **Sliding Scale** | Stop booking | Owe only work completed | Limited |
| **Unionized** | Just cause + grievance review | CBA-determined | Full union protection |

---

## Just Cause Requirements (Union Contracts)

Under unionization, firings require documented just cause:

| Valid Just Cause | Examples |
|------------------|----------|
| **Gross Misconduct** | Violence, criminal charges, substance abuse |
| **Contract Breach** | No-shows, refusing to perform |
| **Insubordination** | Refusing direct booking orders (with limitations) |
| **Poor Performance** | Documented decline with warnings |

| NOT Just Cause | Examples |
|----------------|----------|
| **Creative Differences** | Not grounds for termination |
| **Political Disagreement** | Worker's opinions protected |
| **Union Activity** | Organizing is protected |
| **Popularity Decline** | Unless documented performance issues |

---

## Firing Archetypes

Based on booker/owner personality:

| Archetype | Firing Style | Historical Model |
|-----------|--------------|------------------|
| **Hard-Ass** | Fire first, negotiate never | Bill Watts, Ole Anderson |
| **Politician** | Quiet phase-out, never confronts | Eric Bischoff (early) |
| **Emotional Reactor** | Fires in anger, regrets later | Vince McMahon (volatile) |
| **Cold Calculator** | Fires by spreadsheet only | Modern WWE HR approach |
| **Family Protector** | Almost never fires, enables dysfunction | SMW, some territories |

---

## Firing Consequences

### Immediate Effects

| Effect | Description |
|--------|-------------|
| **Buyout Payment** | If guaranteed, owe remaining value |
| **Locker Room Reaction** | Workers watch how colleagues are treated |
| **Agent Whispers** | Word spreads about your firing style |
| **Media Coverage** | Era-dependent (modern = instant social media) |

### Long-Term Effects

| Effect | Description |
|--------|-------------|
| **Reputation Score** | Accumulates across all firings |
| **Recruiting Difficulty** | Bad reputation = harder to sign talent |
| **Union Mobilization** | Unfair firings accelerate union organizing |
| **Talent Pipeline** | Developmental workers may refuse contracts |

---

## Vindictive Firing Patterns

Some promotions fire workers associated with problem talent:

| Pattern | Description |
|---------|-------------|
| **Guilt by Association** | Friend of fired worker also released |
| **Faction Purge** | Entire stable released after leader's scandal |
| **Message Sending** | Fire one to scare others into compliance |
| **Clique Warfare** | Political faction gets rivals fired |

These patterns:
- Damage locker room trust severely
- Create enemies who may work for competitors
- Generate media coverage and fan backlash
- May trigger union organizing

---

## Response Options After Termination Decision

| Option | Description | Consequences |
|--------|-------------|--------------|
| **Clean Release** | Mutual, professional separation | Minimal damage |
| **Quiet Firing** | Phase out without announcement | Worker may leak |
| **Public Firing** | On-air or press release | Can be storyline or PR disaster |
| **Punitive Firing** | Make example of worker | Maximum locker room damage |
| **Negotiated Exit** | Settlement for clean departure | Costs money, buys silence |

---

## Era-Based Firing Norms

| Era | Firing Culture | Worker Protection |
|-----|----------------|-------------------|
| **Territory (1950s-1980s)** | At-will, handshake culture | None |
| **National TV (1980s-1990s)** | Contracts matter, but loose enforcement | Minimal |
| **Monday Night Wars (1996-2001)** | Competitive; workers have options | High (can jump ship) |
| **Modern (2010s-Present)** | HR involvement, social media scrutiny | Medium-High |
| **Unionized (Hypothetical)** | Just cause required, grievance process | Maximum |

---

## Connected Mechanics

- [[Contract Types]] - Termination rules vary by type
- [[Guaranteed Money & Payouts]] - Buyout obligations
- [[Contract Morality Score]] - Firing handling affects score
- [[Worker Resistance]] - Poor treatment leads to pushback
- [[Scandal System]] - Firings can become scandals
- [[Union System]] - Union protects against unjust firing

---

## Open Questions

- [ ] Exact reputation point system for firing patterns
- [ ] Severance package negotiation mechanics
- [ ] Non-compete clause enforcement rules
- [ ] Media leak probability calculations
- [ ] Worker "blacklist" mechanics across promotions

---

## Implementation Notes

```json
{
  "termination": {
    "worker_id": "worker_001",
    "contract_id": "contract_001",
    "termination_type": "mutual_release",
    "reason": "creative_differences",
    "just_cause_met": false,
    "buyout_paid": 750000,
    "public_announcement": true,
    "worker_statement": "grateful_for_opportunity",
    "locker_room_reaction": "neutral",
    "media_coverage": "moderate",
    "reputation_impact": -5
  }
}
```
