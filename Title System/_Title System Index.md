# Title System

📛 **SYSTEM:** Championship and Title Logic
🧭 **CATEGORY:** Booking / Promotion
🔑 **KEYWORDS:** title, championship, belt, prestige, lineage, hot potato, reign, chase, world title, tag titles
📝 **SUMMARY:** Comprehensive system governing championship prestige, title run dynamics, lineage memory, and the political/emotional weight of title decisions. Titles aren't just belts: they're battlegrounds, proof of worth, or the knife in your back.

⚙️ **LOGIC OVERVIEW:**
- Title prestige is dynamic, affected by booking quality, champion caliber, and match importance
- Chase is always easier than the reign: natural decay unless fresh challengers emerge
- Hot potato booking (frequent changes) tanks prestige rapidly
- Titles affect match ratings: hot titles boost, dead titles drag
- Shared titles and governing bodies create political warfare
- Lineage memory tracks all reigns for historical context

🔬 **LLM INTEGRATION:** Minimal
- Title history narration (optional)
- Prestige trend analysis reports (optional)
- Championship booking suggestions (optional)

📌 **ORIGIN:** Vol 1-4 (Title Logic sections, Travelling Heel Champion, Championship System overview)

---

## VERSION HISTORY

**Version 1.0 (Vol 1-2)**
- Title concept introduced
- Basic prestige tracking proposed
- Champion vs. chase dynamics noted

**Version 2.0 (Vol 3-4) [CURRENT - LOCKED]**
- Title prestige dynamic system formalized
- Hot potato risk mechanics
- Title run decay curves
- Governing body politics (NWA-style)
- Title lineage memory tracking
- Match rating modifiers by title status
- Title types categorized

---

📎 **CONNECTED SYSTEMS:**
- [[Booking_Engine_P1-3|Booking Engine]] (Title stakes affect match ratings)
- [[Crowd Memory]] (Title moments become anchor memories)
- [[Contract System]] (Title clauses, creative control)
- [[Worker Skills]] (Psychology, Charisma for champion runs)
- [[Hidden Personality]] (Ego, Drive affect title hunger)
- [[Faction System]] (Stable title reigns, Freebird rule)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Title Prestige]] | How prestige is earned, maintained, and decayed | Locked |
| [[Title Run Dynamics]] | Chase vs. reign, decay curves, champion maintenance | Locked |
| [[Hot Potato Risk]] | Dangers of frequent title changes | Locked |
| [[Title Types]] | World, secondary, specialty, tag, junior titles | Locked |
| [[Shared Titles and Governing Bodies]] | NWA-style politics, board votes, political capital | Locked |
| [[Title Lineage Memory]] | Historical tracking, reign significance | Locked |

---

## Design Philosophy

Titles aren't just prizes: they're emotional investments, political weapons, and historical anchors. The system captures:

**Core truths:**
- The chase is always easier than the reign
- Hot titles massively boost match prestige; dead titles actively drag
- Heel champions dominate because they're easier to hate (different decay curve)
- Winning a title for your guy should feel like a revolution, not just a booking note
- Title prestige and feud momentum need to be dynamic systems

**The weight of the crown:**
- Champion runs grind workers down unless managed
- Babyface champions struggle to stay hot without fresh challengers
- Overprotection creates fan resentment
- Hot potato booking destroys prestige instantly

---

## Title Impact on Match Ratings

Titles directly affect match quality perception:

| Title Status | Match Rating Modifier |
|--------------|----------------------|
| **Hot Title** (high prestige, recent great defenses) | +10% to +15% |
| **Warm Title** (stable prestige, competent booking) | +5% |
| **Neutral Title** | No modifier |
| **Cold Title** (declining prestige, weak booking) | -5% to -10% |
| **Dead Title** (24/7 style, joke booking) | -15% or worse |

---

## Historical Examples

| Title Moment | Impact |
|--------------|--------|
| **WWF Title 2000** | Peak prestige: every defense felt massive |
| **NWA World Title (territory era)** | Political battlefield across promotions |
| **WWE 24/7 Title** | Dead on arrival, joke prestige |
| **IWGP Title (Okada era)** | Dynasty that fought decay through classic defenses |
| **ECW World Title** | Cult prestige despite small promotion |

---

## Open Questions

- [ ] Exact prestige decay formulas over time
- [ ] How vacated titles are handled (tournament, appointment, etc.)
- [ ] Interim championship mechanics
- [ ] Cross-promotion title unification effects
- [ ] Belt design/visual prestige impact

---

## Implementation Notes

```json
{
  "title": {
    "title_id": "title_001",
    "name": "World Heavyweight Championship",
    "promotion_id": "promo_001",
    "type": "world",
    "prestige": {
      "current": 85,
      "peak": 95,
      "floor": 40,
      "trend": "stable"
    },
    "current_champion": {
      "worker_id": "worker_001",
      "reign_start": "1985-03-15",
      "defenses": 8,
      "reign_quality": "excellent"
    },
    "lineage": [],
    "hot_potato_counter": 0,
    "last_change_date": "1985-03-15",
    "governing_body": null
  }
}
```

---

**Document Status:** Locked (Vol 1-4)
**Last Updated:** 2025-12-21
**Next Review:** Integrate with Booking Engine for match rating modifiers
