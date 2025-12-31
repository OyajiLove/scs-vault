# Hall of Fame System

📛 **SYSTEM:** Hall of Fame System v1.0
🔗 **PARENT:** [[_Legacy System Index|Legacy System]]
🧭 **CATEGORY:** Career & Long-Term Simulation
🔑 **KEYWORDS:** hall of fame, hof, induction, voting, retirement, legacy
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

A meaningful, memory-based Hall of Fame that reflects fan emotion, career arcs, political grudges, and cultural footprint, not just stats.

> It's not about who won the most matches.
> It's about who **mattered**.

---

## Voting Cycle

Happens annually (or on player-triggered retirement cards).

Each cycle includes:
1. **Eligible Candidates Pool**
2. **Voter Block** (AI + optional player influence)
3. **Public Buzz / Debate**
4. **Induction Ceremony Segment(s)**

---

## Eligibility Rules

| Requirement | Notes |
|-------------|-------|
| Worker must be **retired** (or semi-retired for 1+ year) | Can return later but risks credibility |
| **Legacy ≥ 50** (minimum) | Exceptions possible for cult icons or tragedy |
| No active major **scandal or suspension** | HOF freezes if reputation is toxic |
| Optional: **Regional vs Global HOF** | Some promotions run their own (e.g., Memphis HOF, Joshi Legends Shrine) |

---

## Core Voting Factors

| Factor | Description |
|--------|-------------|
| **Legacy Score** | Main baseline. Higher = more likely |
| **Fan Memory Strength** | Snapshot moments still remembered? |
| **Cultural Weight** | Did they define an era, style, or division? |
| **Promotion Impact** | Home promotion may lobby hard |
| **Emotional Arcs** | Redemption, perseverance, tragedy = huge voter bias |
| **Retirement Execution** | Was the farewell fitting or forgettable? |
| **Scandal Modifier** | Hurts chances based on timing & severity |
| **AI Booker Grudges / Alliances** | Political sabotage or championing |

---

## Voter Personality Types (AI-Driven)

| Voter Type | Bias Toward... |
|------------|----------------|
| **Traditionalist** | Title reigns, company loyalty, face roles |
| **Historian** | Emotional arcs, forgotten cult legends |
| **Smark** | Match quality, workrate, backstage reputation |
| **Pop Chaser** | Buzz runs, late-career heat |
| **Purist** | Style loyalty (e.g., lucha icons, joshi warriors) |
| **Political Crony** | Faction mates, promotion darlings |
| **Chaos Merchant** | Controversy, reformers, shoot legends |

These shape which candidates make it through controversial years.

---

## Individual Induction Effects

| If Inducted... | Effect |
|----------------|--------|
| **Pop Spike** (retirement angle) | Temporary resurgence, fans cheer again |
| **Locker Room Morale Bump** | Especially for allies, protégés |
| **Media Memory Reboot** | Promos start referencing legacy again |
| **Historical Status Locked In** | Legacy can no longer fall (unless scandal emerges) |
| **Return Push Opportunity** | Some stars parlay it into one last run, if healthy |

---

## HOF Segments & Events

- **Ceremony Cards** (with matches or not)
- **Video packages** using memory snapshots
- **Commentary lines** permanently updated ("HOFer X is watching this one closely...")
- **Year-end recap lists** shift to reflect class
- **Player can veto or override** inductions (with political fallout)

---

## Special Categories & Edge Cases

| Category | Rules |
|----------|-------|
| **Tragic Inductees** | Passed before legacy peak? Boosted by emotion, but may split voters |
| **Tag Team Inductions** | Legacy average + shared memory anchors |
| **Promotion-Specific Classes** | Smaller feds honor homegrown icons, even if unknown elsewhere |
| **Reevaluated Veterans** | Rediscovered via documentaries, fan campaigns, or myth runs |

---

## Meltzer HOF as Canonical Source (Vol 6)

For real-world historical databases, **Dave Meltzer's Wrestling Observer Hall of Fame** is the primary benchmark for:
- Worker HOF eligibility
- Real-world legacy calibration  
- Cultural context by region, style, and era
- Categorization: Japan, Mexico, Modern US/Canada, Historical, etc.

Used to:
- Seed Legacy Scores at world gen
- Flag HOF status for historical workers
- Create "Controversial Omissions" stories where fans push for overlooked stars
- Simulate alternate HOF paths in fictional promotions ("If WCW had its own...")

---

## Connected Systems

- [[Legacy Tracker]] - Source score for eligibility
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory Engine]] - Memory strength affects voting
- [[AI Booker System]] - Booker grudges/alliances affect votes
- [[Scandal System]] - Active scandals freeze eligibility
- [[Media System]] - Documentary releases can trigger reevaluation

---

## Open Questions

- Exact voting algorithm weights
- How many inductees per year (cap?)
- Player influence mechanics (lobby, veto costs)
- Posthumous induction special rules
- Cross-promotion HOF recognition

---

## Implementation Notes

```json
{
  "hof_candidate": {
    "worker_id": "w_001",
    "eligible": true,
    "legacy_score": 72,
    "memory_strength": 65,
    "cultural_weight": "high",
    "emotional_arcs": ["redemption"],
    "scandal_modifier": 0,
    "voter_support": {
      "traditionalist": 0.7,
      "historian": 0.9,
      "smark": 0.6,
      "pop_chaser": 0.5,
      "purist": 0.8,
      "political_crony": 0.4,
      "chaos_merchant": 0.3
    },
    "induction_probability": 0.68
  }
}
```
