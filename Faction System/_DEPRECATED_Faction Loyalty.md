# Faction Loyalty

📛 **MECHANIC:** Multi-Axis Worker Loyalty System
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** loyalty, promotion loyalty, faction loyalty, friend loyalty, drift, Scott Hall
📌 **ORIGIN:** Vol 4 (How Loyalty Systems Work in SCS, Scott Hall 1996 example)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Workers don't have a single loyalty value: they have multiple loyalty axes that can conflict and override each other. Loyalty drifts based on life events, booking decisions, and relationships. The game grows these organically; modders only need to set basic starting conditions.

---

## Loyalty Axes

Every worker tracks loyalty across multiple dimensions:

| Loyalty Type | Description |
|--------------|-------------|
| **Promotion Loyalty** | Emotional tie to current employer (not just contractual) |
| **Faction/Stable Loyalty** | Connection to current team, stable, alliance |
| **Mentor/Trainer Loyalty** | Early career emotional bonds |
| **Friend Loyalty** | Hidden loyalty to specific workers (strong friendships) |
| **Self Loyalty (Ego)** | Loyalty to oneself: career advancement prioritized |

---

## Loyalty Scale

| Range | Description |
|-------|-------------|
| 90-100 | **Absolute** | Would never betray under any circumstance |
| 70-89 | **Strong** | Very committed, only extreme events shake |
| 50-69 | **Moderate** | Committed but can be swayed |
| 30-49 | **Weak** | Staying but not deeply invested |
| 10-29 | **Minimal** | Ready to leave given opportunity |
| 0-9 | **None** | No emotional connection |

---

## Loyalty Defaults at Creation

Modders don't need to set every value:

| Loyalty Type | Default Behavior |
|--------------|------------------|
| **Promotion** | Medium-high to first employer unless personality conflicts |
| **Faction** | Initializes at formation; builds through booking |
| **Mentor** | Optional manual assignment; grows naturally if mentor relationship established |
| **Friend** | Formed in-simulation through tag runs, alliances, hardship |
| **Self** | Based on Ego rating from Hidden Personality |

---

## Promotion Loyalty Over Time

| Time with Promotion | Default Loyalty Level |
|---------------------|----------------------|
| **New Hire** | Neutral: only contractual, no deep bond |
| **1-2 Years** | Minor loyalty building if treated fairly |
| **3-5 Years** | Moderate loyalty if steady booking and push |
| **5-10 Years** | High loyalty potential unless betrayed |
| **10+ Years** | "Legacy Worker" potential: may stick through downturns |

### Grudging Stay vs. Real Loyalty

| Type | Description | Behavior |
|------|-------------|----------|
| **Grudging Stay** | Stays for money or friends, not emotional bond | Won't rise emotionally; flight risk if better offer |
| **Real Loyalty** | Treated well, given creative freedom, friendships grow | Strong, self-sustaining loyalty |

---

## Loyalty Drift Events

| Event Type | Effect |
|------------|--------|
| **Booking Support** | Raises promotion/faction loyalty if protected, pushed, trusted |
| **Burial/Betrayal** | Erodes loyalty sharply |
| **Mentorship Growth** | Loyalty to trainers/friends grows with positive experiences |
| **New Friends/Factions** | New bonds can override old faction loyalty |
| **Public/Private Scandals** | Backstabbing exposure destroys faction loyalty |
| **Personal Growth/Collapse** | Rehab, depression, ego inflation drift loyalty |

---

## Historical Example: Scott Hall 1996

| Loyalty Layer | Estimation at WWF→WCW Jump |
|---------------|---------------------------|
| **Promotion Loyalty (WWF)** | Moderate-Low: grateful for Razor platform but felt underpaid, creatively unfulfilled |
| **Faction Loyalty (Kliq)** | Very High: strong bond with Nash, Michaels, Waltman |
| **Mentor Loyalty** | Minimal: not especially tied to trainers by '96 |
| **Friend Loyalty (Nash)** | Extremely High: key reason he felt comfortable jumping |
| **Self Loyalty (Ego)** | Medium-High: wanted better pay, opportunities, stardom |

**Result:** When WCW offered money and Nash was already leaning, Hall felt justified betraying WWF with little guilt. His loyalty landscape made the choice almost inevitable.

---

## Loyalty Conflicts

When loyalties clash, higher values win:

| Scenario | Resolution |
|----------|------------|
| **Friend vs. Promotion** | May leave promotion for friend |
| **Faction vs. Self** | High ego may betray faction |
| **Mentor vs. Faction** | Old bonds may override new group |
| **Promotion vs. Self** | Frustration leads to departure |

---

## Relationship-Driven Loyalty

Editable relationships affect loyalty:

| Relationship | Loyalty Effect |
|--------------|----------------|
| **Tagged as Friend** | Raises initial Friend Loyalty |
| **Tagged as Mentor** | Raises initial Mentor Loyalty |
| **Tagged as Enemy** | Blocks alliance unless turned via storyline |
| **Tagged as Romantic** | Deep loyalty web, breakup risks |

---

## Connected Mechanics

- [[Faction Stability]] - Aggregate of member loyalties
- [[Betrayal and Breakup]] - What happens when loyalty breaks
- [[Hidden Personality]] - Base traits affect loyalty behavior
- [[Contract System]] - Loyalty affects contract negotiations

---

## Open Questions

- [ ] Exact loyalty drift formulas
- [ ] How injuries affect loyalty
- [ ] Loyalty inheritance (does joining faction affect promotion loyalty?)
- [ ] AI loyalty decision thresholds
- [ ] How retirement affects legacy loyalty

---

## Implementation Notes

```json
{
  "worker_loyalty": {
    "worker_id": "worker_001",
    "promotion_loyalty": {
      "promo_001": 65,
      "time_employed_months": 36,
      "type": "real_loyalty"
    },
    "faction_loyalty": {
      "faction_001": 82
    },
    "mentor_loyalty": {
      "worker_042": 55
    },
    "friend_loyalty": {
      "worker_002": 90,
      "worker_003": 75
    },
    "self_loyalty": 60,
    "loyalty_events": [
      { "date": "1985-03-15", "type": "booking_support", "effect": +5, "target": "promotion" }
    ]
  }
}
```
