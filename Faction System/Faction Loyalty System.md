# Faction Loyalty System

📛 **MECHANIC:** Multi-Axis Loyalty Tracking
🔗 **PARENT SYSTEM:** [[Faction System/_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** loyalty, betrayal, faction decay, friend loyalty, promotion loyalty, Scott Hall, drift
📌 **ORIGIN:** Vol 4 (Faction Loyalty Decay and Betrayal Arcs, How Loyalty Systems Work, Scott Hall 1996 example)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

**Note:** This file consolidates "Faction Loyalty.md" and "Faction Loyalty System.md" which contained overlapping content.

---

## Overview

Loyalty isn't uniform: it's personal, political, and emotional. Workers track multiple loyalty axes that drift based on life events, booking, backstage politics, scandals, triumphs, and tragedies. Betrayals don't come from nowhere; they fester over time like real grudges.

The game grows loyalty organically; modders only need to set basic starting conditions.

---

## Loyalty Axes (Per Worker)

Every worker tracks loyalty across multiple dimensions:

| Loyalty Type | Description | Drift Speed |
|--------------|-------------|-------------|
| **Promotion Loyalty** | Emotional tie to current employer (not just contractual) | Slow |
| **Faction/Stable Loyalty** | Connection to current team, stable, alliance | Moderate |
| **Mentor/Trainer Loyalty** | Early career emotional bonds | Very Slow |
| **Friend Loyalty** | Hidden loyalty to specific workers (strong friendships) | Moderate |
| **Self Loyalty (Ego)** | Loyalty to oneself: career advancement prioritized | Personality-based |

---

## Loyalty Scale (1-20)

| Range | Level | Behavior |
|-------|-------|----------|
| 17-20 | **Absolute** | Unwavering; legendary bond; would never betray under any circumstance |
| 13-16 | **Strong** | Committed; resists temptation; only extreme events shake |
| 9-12 | **Moderate** | Functional but not ride-or-die; can be swayed |
| 5-8 | **Weak** | Easily tempted; unreliable; staying but not deeply invested |
| 1-4 | **Minimal** | Will leave/betray at first opportunity; no emotional connection |

---

## Loyalty Defaults at Creation

Modders don't need to set every value:

| Loyalty Type | Default Behavior |
|--------------|------------------|
| **Promotion** | Medium-high to first employer unless personality conflicts |
| **Faction** | Initializes at formation; builds through booking |
| **Mentor** | Optional manual assignment; grows naturally if mentor relationship established |
| **Friend** | Formed in-simulation through tag runs, alliances, hardship |
| **Self** | Based on Ego rating from [[Hidden_Personality|Hidden Personality]] |

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

### What Raises Loyalty

| Event | Loyalty Effect |
|-------|----------------|
| **Protected push** | +Promotion, +Faction if group benefits |
| **Successful title reign** | +Promotion |
| **Positive mentorship** | +Mentor, +Friend to mentor |
| **Shared hardship** | +Faction, +Friend |
| **Financial fairness** | +Promotion |
| **Creative freedom** | +Promotion |
| **Group success** | +Faction |

### What Lowers Loyalty

| Event | Loyalty Effect |
|-------|----------------|
| **Burial/Screwjob** | -Promotion sharply |
| **Broken promises** | -Promotion, -Faction if group involved |
| **Betrayal by friend** | -Friend to specific worker |
| **Public scandal exposure** | -Faction if leaked by member |
| **Faction failure** | -Faction if repeated losses |
| **Ego inflation** | -Faction (leader outgrows group) |
| **Outside offers** | Temptation tests loyalty |

---

## Faction Loyalty Decay Triggers

Specific situations that erode faction bonds:

| Trigger | Outcome |
|---------|---------|
| **Leader Ego Outgrows Group** | Followers lose loyalty; betrayal arcs ignite |
| **Suppressed Members** | Midcarders buried inside faction turn jealous, splinter off |
| **Failed Title Quests** | Repeated failure to achieve goals decays internal loyalty |
| **Outside Offers** | Workers may jump factions if tempted enough |

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

## Betrayal Threshold

Betrayal becomes possible when:

```
Faction_Loyalty < 8 AND (Self_Loyalty > Faction_Loyalty + 5)
OR
Friend_Loyalty to outside worker > Faction_Loyalty
OR
Promotion_Loyalty < 5 AND better offer exists
```

---

## Historical Example: Scott Hall 1996

How loyalty landscape predicted the NWO jump:

| Loyalty Axis | Hall's 1996 Level | Explanation |
|--------------|-------------------|-------------|
| **Promotion (WWF)** | Moderate-Low (~8) | Grateful for Razor platform but underpaid, unfulfilled |
| **Faction (Clique)** | Very High (~17) | Strong bonds to Nash, Michaels, Waltman |
| **Mentor** | Minimal (~4) | No deep trainer bonds by '96 |
| **Friend (Nash)** | Extremely High (~19) | Key reason for comfortable jump |
| **Self (Ego)** | Medium-High (~13) | Wanted better pay, opportunity |

**Result:** When WCW offered money and Nash was already leaning, Hall felt justified betraying WWF with little guilt. His loyalty landscape made the choice almost inevitable.

---

## Grudge Memory

Betrayals create lasting memory:

| Grudge Level | Duration | Effect |
|--------------|----------|--------|
| **Minor** | 1-2 years | -2 to future loyalty with betrayer |
| **Moderate** | 3-5 years | -5 to future loyalty; affects booking |
| **Major** | 10+ years | -8 or permanent; blood feud potential |

---

## Loyalty Visibility

| What Player Sees | What's Hidden |
|------------------|---------------|
| General morale indicators | Exact loyalty numbers |
| Obvious tension signs | Precise betrayal threshold |
| Backstage reports (vague) | Specific loyalty drift |
| Agent warnings | Complete loyalty picture |

Players learn workers' true natures over time through observation.

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

- [[Faction Formation]] - Loyalty initializes at formation
- [[Faction Stability]] - Aggregate of member loyalties
- [[Faction Collapse and Evolution]] - Low loyalty triggers collapse
- [[Betrayal and Breakup]] - What happens when loyalty breaks
- [[Hidden_Personality|Hidden Personality]] - Ego, Paranoia affect loyalty behavior
- [[Contract System/_Contract System Index|Contract System]] - Loyalty affects negotiation
- [[Scandal System/_Scandal System Index|Scandal System]] - Scandals damage faction loyalty

---

## Open Questions

- [ ] Exact loyalty drift formulas per event
- [ ] How long grudges persist by severity
- [ ] Multiple loyalties conflict resolution
- [ ] Loyalty to deceased/retired workers
- [ ] Cross-promotion loyalty (same faction, different feds)
- [ ] How injuries affect loyalty
- [ ] AI loyalty decision thresholds

---

## Implementation Notes

```json
{
  "worker_loyalty": {
    "worker_id": "worker_001",
    "promotion_loyalty": {
      "promo_001": 15,
      "time_employed_months": 36,
      "type": "real_loyalty"
    },
    "faction_loyalty": {
      "fac_001": 18
    },
    "mentor_loyalty": {
      "worker_042": 12
    },
    "friend_loyalty": {
      "worker_002": 19,
      "worker_003": 14
    },
    "self_loyalty": 11,
    "grudges": [
      { "target_id": "worker_055", "severity": "major", "date": "1984-06-15" }
    ],
    "betrayal_risk": "low",
    "loyalty_events": [
      { "date": "1985-03-15", "type": "booking_support", "effect": +2, "target": "promotion" }
    ]
  }
}
```

---

**Document Status:** Locked (Vol 4) - Consolidated from duplicate files
**Last Updated:** 2025-12-22
**Next Review:** Formalize loyalty drift formulas
