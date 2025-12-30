# Manager System

📛 **SYSTEM:** Non-Wrestling Talent Management
🧭 **CATEGORY:** Booking / Roster
🔑 **KEYWORDS:** manager, valet, mouthpiece, package deal, promo, corner, loyalty
📝 **SUMMARY:** Manages the role of non-wrestling talent who accompany wrestlers to the ring. Managers provide promo support, match interference, stable leadership, and character enhancement. Manager loyalty matters: firing a manager fractures groups organically, and separating bonded pairs hurts morale.

⚙️ **LOGIC OVERVIEW:**
- Managers bring bonus momentum to their clients
- Manager loyalty tree tracks who they protect and sabotage
- Package deals link managers to specific wrestlers/teams
- Promo skills can cover for weak talkers
- Match interference affects outcomes and heat
- Firing managers has morale and stability consequences

🔬 **LLM INTEGRATION:** Minimal to Moderate
- Manager promo generation (optional)
- Mistranslation heat angles (optional)

📌 **ORIGIN:** Vol 1-4 (Manager Loyalty Tree, Package Deals, Manager Tags)

---

## VERSION HISTORY

**Version 1.0 (Vol 1-4) [CURRENT - LOCKED]**
- Manager System formalized
- Manager types and roles defined
- Manager-client relationship mechanics
- Loyalty tree tracking
- Package deal contracts
- Match interference effects
- Manager tags created
- Historical examples integrated

---

📎 **CONNECTED SYSTEMS:**
- [[Faction System/_Faction System Index|Faction System]] (Managers lead or support stables)
- [[Segment Promo System/_Segment Promo System Index|Promo System]] (Managers provide promo boost)
- [[Contract System/_Contract System Index|Contract System]] (Package deal contracts)
- [[Match Engine/_Match Engine Index|Match Engine]] (Interference affects matches)
- [[Morale System]] (Separation hurts morale)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Manager Types]] | Different manager roles and styles | ✅ Locked |
| [[Manager-Client Relationships]] | Loyalty, package deals, bonds | ✅ Locked |
| [[Manager Match Impact]] | Ringside presence and interference effects | ✅ Locked |

---

## Design Philosophy

Managers aren't just accessories: they're force multipliers who can make or break careers. A great manager elevates a limited talker, generates heat for a monster, or provides the mouthpiece a technical wrestler needs. The system captures how managers bond with clients, what happens when those bonds break, and how managers affect every aspect of presentation.

**Core truths:**
- Manager loyalty matters (Cornette, Heenan, Heyman examples)
- Firing a manager fractures the stable organically
- Where the Midnights went, so too did Cornette
- Managers bring bonus momentum to teams
- Morale penalties for separating bonded manager-wrestler combos
- Some managers sabotage as easily as they protect

---

## Manager Roles

| Role | Description | Example |
|------|-------------|---------|
| **Mouthpiece** | Speaks for wrestlers who can't talk | Jimmy Hart, Paul Ellering |
| **Heat Magnet** | Draws heel heat, takes bumps | Bobby Heenan, Jim Cornette |
| **Valet** | Adds glamour, distraction spots | Miss Elizabeth, Sunny |
| **Stable Leader** | Leads faction, strategic mind | Paul Heyman, Teddy Long |
| **Authority** | On-screen power figure managing | Mr. McMahon (active) |
| **Advocate** | Speaks for special attraction | Heyman for Lesnar |

---

## Manager Tags

| Tag | Description |
|-----|-------------|
| **Heat Magnet Manager** | Expert at drawing heel heat |
| **Nostalgia Manager** | Manages old stars, legends |
| **Passive Corner Man** | Minimal interference, presence only |
| **Mic Saver** | Saves weak talkers with promo ability |
| **Cult Builder** | Builds stables, creates followings |
| **Backstage Politician** | Uses position for political leverage |
| **Loyalty Maker** | Creates deep bonds with clients |

---

## Historical Examples

| Manager | Style | Notable Clients |
|---------|-------|-----------------|
| **Bobby Heenan** | Heat Magnet, Mouthpiece | André, Rude, Perfect |
| **Jim Cornette** | Heat Magnet, Package Deal | Midnight Express |
| **Paul Heyman** | Stable Leader, Advocate | ECW roster, Lesnar |
| **Jimmy Hart** | Mouthpiece, Prolific | Dozens across promotions |
| **Miss Elizabeth** | Valet | Macho Man |
| **Sensational Sherri** | Versatile (valet to heel) | Savage, Michaels |

---

## Manager Value Proposition

| Benefit | Description |
|---------|-------------|
| **Promo Coverage** | Speaks for non-talkers |
| **Heat Generation** | Draws crowd reactions |
| **Match Interference** | Alters outcomes believably |
| **Character Enhancement** | Adds depth to presentation |
| **Stable Cohesion** | Unifies faction identity |
| **Drawing Power** | Famous managers add star power |

---

## Open Questions

- [ ] Exact momentum bonus formulas
- [ ] How manager skill levels work
- [ ] Manager contract specifics
- [ ] Manager vs. manager feuds
- [ ] Retirement transition (Future Manager tag)

---

## Implementation Notes

```json
{
  "manager": {
    "manager_id": "manager_001",
    "name": "Jim Cornette",
    "role": "heat_magnet",
    "promo_skill": 95,
    "heat_generation": 90,
    "interference_skill": 75,
    "clients": ["worker_001", "worker_002"],
    "package_deals": ["midnight_express"],
    "loyalty_tree": {
      "protects": ["worker_001", "worker_002"],
      "sabotages": []
    },
    "tags": ["heat_magnet_manager", "loyalty_maker"],
    "stable_affiliation": "faction_001"
  }
}
```

---

**Document Status:** Locked (Vol 1-4)
**Last Updated:** 2025-12-21
**Next Review:** Integrate with Promo System for speaking roles
