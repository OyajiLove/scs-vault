# Faction and Stable System

📛 **SYSTEM:** Faction Logic and Alliance Evolution
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** faction, stable, alliance, betrayal, loyalty, formation, breakup, Freebird, collective bargaining
📝 **SUMMARY:** Dynamic system for team building, faction evolution, betrayal arcs, and loyalty warfare. Factions don't just form and break: they bleed, evolve, betray, immortalize, or vanish. Workers have multiple loyalty axes (promotion, faction, mentor, friends, self) that drift based on life events.

⚙️ **LOGIC OVERVIEW:**
- Faction stability score tracks internal health
- Internal friction meter (jealousy, momentum imbalance, uneven push)
- Stable leader traits affect group dynamics (benevolent, tyrannical, absent)
- Event triggers: mutiny, coup, splinter cell, exile, unification
- Freebird Rule allows title defense rotation among 3+ members
- Collective bargaining for bonded teams (Road Warriors, Bucks)
- Betrayals fester over time, don't come from nowhere

🔬 **LLM INTEGRATION:** Minimal
- Faction dynamic storyline suggestions (optional)
- Internal conflict narration (optional)

📌 **ORIGIN:** Vol 1-4 (Faction Logic & Alliance Evolution), Vol 4 (Tag Team and Faction Expanded Systems v2.0)

---

## VERSION HISTORY

**Version 1.0 (Vol 1-2)**
- Faction concept introduced
- Basic formation and breakup mechanics
- Loyalty concept proposed

**Version 2.0 (Vol 3-4) [CURRENT - LOCKED]**
- Tag Team and Faction Expanded Systems v2.0
- Faction stability score and friction meter
- Multi-axis loyalty system formalized
- Leader type traits defined
- Freebird Rule mechanics
- Collective bargaining for bonded teams
- Faction Identity Evolution on member changes
- Faction goal types categorized

---

📎 **CONNECTED SYSTEMS:**
- [[Hidden_Personality|Hidden Personality]] (Ego, Loyalty, Paranoia affect faction dynamics)
- [[Contract System/_Contract System Index|Contract System]] (Collective bargaining, package deals)
- [[Title System/_Title System Index|Title System]] (Freebird Rule, faction title reigns)
- [[Crowd_Memory|Crowd Memory]] (Faction moments become anchors)
- [[Turn_Engine|Turn Engine]] (Faction betrayals are major turns)
- [[Morale System]] (Faction health affects worker morale)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Faction_System_Overview]] | Comprehensive overview: roles, evolution, AutoBooker logic (Vol 5) | 🔒 Locked |
| [[Faction Formation]] | How factions form, worker lobbying, chemistry | Locked |
| [[Faction Stability]] | Internal health, friction, goal tracking | Locked |
| [[Faction Loyalty System]] | Multi-axis loyalty, drift mechanics | Locked |
| [[Betrayal and Breakup]] | How factions collapse, split types | Locked |
| [[Freebird Rule]] | Title defense rotation for stables | Locked |
| [[Faction Identity Evolution]] | How groups change when members leave | Locked |
| [[Faction Collapse and Evolution]] | 6 evolution types, fracture triggers | Locked |
| [[Collective Bargaining]] | Package deals, negotiation leverage | Locked |
| [[Tag Team Mechanics]] | Duo-specific mechanics | Locked |

---

## Design Philosophy

Factions aren't just roster groupings: they're living organisms with internal politics, goals, and emotional bonds that grow, decay, and explode.

**Core truths:**
- Betrayals don't come from nowhere; they fester over time like real-life grudges
- Workers have multiple loyalty axes that can conflict
- Formation attempts can fail or be reluctantly accepted, causing tension later
- Breakups are emotional detonations that fuel feuds for decades
- Faction identity shifts when lynchpins leave

**What makes factions work:**
- Shared goals (dominate titles, protect the boss, prove loyalty to a cause)
- Strong leader with clear traits
- Balanced push across members
- Success in achieving objectives
- Chemistry from tag runs and backstage bonding

---

## Faction Goals

Every faction has implicit or explicit goals:

| Goal Type | Description | Example |
|-----------|-------------|---------|
| **Title Domination** | Control all/most championships | NWO, Bullet Club |
| **Leader Protection** | Shield a vulnerable or hated leader | Corporation, Bloodline |
| **Ideology** | Prove a philosophy or worldview | Straight Edge Society |
| **Territory Control** | Dominate a division or region | Los Ingobernables |
| **Family/Loyalty** | Protect family or close bonds | Hart Foundation, Anoa'i |
| **Revolution** | Overthrow establishment | nWo, DX, AEW Elite |
| **Survival** | Band together against common threat | Shield (early) |

---

## Leader Traits

Stable leaders shape group dynamics:

| Leader Type | Behavior | Effect on Members |
|-------------|----------|-------------------|
| **Benevolent** | Shares spotlight, elevates members | High loyalty, low friction |
| **Tyrannical** | Demands obedience, buries members | High friction, betrayal risk |
| **Absent** | Hands-off, lets members self-govern | Variable; can drift |
| **Charismatic** | Personal magnetism holds group | Loyalty to leader, not faction |
| **Strategic** | Plans long-term, uses members tactically | Moderate loyalty if successful |

---

## Historical Examples

| Faction | Key Dynamics |
|---------|--------------|
| **nWo** | Started revolutionary, bloated with membership, collapsed from ego |
| **Bullet Club** | Multiple leadership changes, identity shifts, constant reinvention |
| **Shield** | Tight bond, triple threat breakup, multiple reunions |
| **Hart Foundation** | Family loyalty core, US vs. Canada storyline peak |
| **Four Horsemen** | Rotating membership, prestige badge, Flair as constant |
| **House of Black** | Lost leader (Malakai), identity shifted to new direction |

---

## Faction-Related Tags

| Tag | Description |
|-----|-------------|
| **Faction Loyalist** | Deeply committed to stable over self |
| **Faction General** | Natural leader of groups |
| **Push Killer** | Curses whatever faction they join |
| **Bad Influence** | Corrupts locker rooms, encourages faction splits |
| **Collective Bargainer** | Negotiates as package deal |
| **Golden Rat** | Betrays others for personal gain |

---

## Open Questions

- [ ] Exact faction stability score calculation
- [ ] How faction size affects dynamics
- [ ] AI faction formation logic
- [ ] Cross-promotion faction branches
- [ ] Faction merchandise split mechanics

---

## Implementation Notes

```json
{
  "faction": {
    "faction_id": "faction_001",
    "name": "The Elite",
    "promotion_id": "promo_001",
    "formation_date": "1985-01-15",
    "leader_id": "worker_001",
    "members": ["worker_001", "worker_002", "worker_003", "worker_004"],
    "goals": ["title_domination", "revolution"],
    "stability_score": 72,
    "friction_meter": 15,
    "chemistry_rating": 85,
    "leader_type": "charismatic",
    "collective_bargaining": true,
    "freebird_eligible": true,
    "active": true
  }
}
```

---

**Document Status:** Locked (Vol 1-4)
**Last Updated:** 2025-12-21
**Next Review:** Integrate with Turn Engine for betrayal triggers
