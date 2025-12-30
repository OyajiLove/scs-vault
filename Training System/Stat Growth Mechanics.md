# Stat Growth Mechanics

📛 **MECHANIC:** Skill Improvement Over Time
🔗 **PARENT SYSTEM:** [[_Training System Index|Training System]]
🧭 **CATEGORY:** Worker Development
🔑 **KEYWORDS:** growth, improvement, experience, age, peak, decline, stat increase
📌 **ORIGIN:** Vol 4 (Worker Skills System), confirmed in Bible extraction
✅ **STATUS:** Locked (growth/decline rates), Open (exact formulas)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED (rates) |

---

## Overview

Worker skills change over time through natural development, match experience, focused training, and age-related decline. Growth is not linear: young workers improve quickly, peak-years workers plateau, and veterans decline physically while potentially gaining mental/experience stats.

---

## Base Growth Rates by Age

### Young Workers (18-27)

| Category | Annual Growth Rate | Notes |
|----------|-------------------|-------|
| **Physical Stats** | +1 to +3 | Fastest improvement period |
| **Bell-to-Bell** | +1 to +2 | Match experience accelerates this |
| **Entertainment** | +1 to +2 | Character work develops |
| **Mental** | +1 to +2 | Psychology grows with exposure |

**Modifiers:**
- Active match schedule: +1 bonus to growth
- Focused training: +1 to targeted skill
- Mentor relationship: +1 to mentor's specialty
- Low Drive trait: -1 to all growth
- High Drive trait: +1 to all growth

### Peak Years (28-35)

| Category | Annual Growth Rate | Notes |
|----------|-------------------|-------|
| **Physical Stats** | +0 to +1 | Maintenance mode, decline begins late |
| **Bell-to-Bell** | +0 to +1 | Refinement, not revolution |
| **Entertainment** | +0 to +1 | Can still improve character |
| **Mental** | +0 to +2 | Psychology, Composure can still grow |

**Special Note:** Psychology and Composure can increase during peak years as experience compounds. A 32-year-old can have higher psychology than they did at 26.

### Veteran Years (36+)

| Category | Annual Growth Rate | Notes |
|----------|-------------------|-------|
| **Physical Stats** | -1 per year | Accelerated by injuries |
| **Bell-to-Bell** | -0 to -1 | Technique may hold |
| **Entertainment** | +0 | Can maintain |
| **Mental** | +0 to +1 | Experience still counts |

**Decline Modifiers:**
- Major injuries: Additional -1 to relevant stats
- Accumulated wear: Compounds physical decline
- Low Durability: Faster decline
- High Durability: Slower decline

---

## Peak Age Variations by Style

Different wrestling styles have different peak windows:

| Style | Peak Start | Peak End | Notes |
|-------|------------|----------|-------|
| **High Flyer** | 24 | 32 | Early peak, speed-dependent |
| **Technical** | 26 | 38 | Longer peak, skill-based |
| **Power/Brawler** | 27 | 36 | Strength holds longer |
| **Striker/Strong Style** | 26 | 35 | Balance of physical demands |
| **Submission/Grappling** | 28 | 40 | Longest peak, technique over athletics |
| **Psychology Monster** | 30 | 45 | Mind over body, peaks late |
| **Deathmatch** | 25 | 33 | Short peak, body accumulates damage |

**Tag Implications:**
- "High Flyer" tag may convert to "Grounded Veteran" after peak
- "Innovator" workers may extend peak through adaptation
- "Never Say Die" workers resist decline longer

---

## Match Experience Contribution

Every match contributes to organic skill growth:

| Match Quality | Experience Points | Notes |
|---------------|-------------------|-------|
| **1-2 Star** | 1 XP | Basic execution |
| **3 Star** | 2 XP | Solid work |
| **4 Star** | 3 XP | Excellent performance |
| **5 Star** | 5 XP | Career-defining |
| **Botch-Heavy** | 0 XP | No learning, possible injury |

**XP Thresholds (Conceptual):**
- 10 XP in a stat category: +1 improvement chance
- XP resets after improvement or at year-end

**Match Type Bonuses:**
- Long matches (20+ min): +1 XP to Stamina
- Hardcore matches: +1 XP to Durability (but injury risk)
- Technical showcases: +1 XP to Technical/Submission
- High-spot matches: +1 XP to Aerial (but injury risk)

---

## Skill Ceilings

Workers have natural talent ceilings for each stat:

| Ceiling Level | Range | Description |
|---------------|-------|-------------|
| **Low Potential** | 10-12 | Limited natural ability |
| **Average Potential** | 13-15 | Typical worker ceiling |
| **High Potential** | 16-17 | Above average talent |
| **Elite Potential** | 18-20 | Rare natural gifts |

**Ceiling Modification:**
- Training may raise ceiling by +1 over career (rare, requires years)
- Injury may permanently lower ceiling
- Style change can unlock different ceiling (brawler→technical)

---

## Green Worker Development

Workers with the "Green" tag are inexperienced rookies:

### Green Tag Removal Conditions (Conceptual)

| Requirement | Threshold | Notes |
|-------------|-----------|-------|
| **Match Count** | 50+ matches | Minimum ring time |
| **Time in Wrestling** | 2+ years | Calendar requirement |
| **No Major Botches** | 6-month window | Must demonstrate consistency |
| **Skill Minimum** | 10+ in 3 categories | Basic competency |

**Green Tag Effects:**
- -10% match quality contribution
- Higher botch probability
- Lower crowd tolerance for mistakes
- Mentor relationship more impactful

---

## Connected Mechanics

- [[Training Focus]] - Deliberate practice targeting specific skills
- [[Mentor System]] - Veteran guidance accelerates growth
- [[Dojo System]] - Japanese training school model
- [[_Aging System Index|Aging System]] - Career arc context

---

## Open Questions

- [ ] Exact XP formula for stat improvement
- [ ] How much can training raise natural ceilings?
- [ ] Do mental stats have different ceilings than physical?
- [ ] How quickly can a focused training regimen improve a stat?
- [ ] Diminishing returns as stats approach ceiling?

---

## Implementation Notes

```json
{
  "worker_development": {
    "worker_id": "worker_001",
    "age": 24,
    "career_phase": "young",
    "skills": {
      "technical": {
        "current": 12,
        "ceiling": 16,
        "xp_accumulated": 7
      },
      "aerial": {
        "current": 14,
        "ceiling": 17,
        "xp_accumulated": 3
      }
    },
    "training_focus": "submission",
    "mentor_id": "mentor_veteran_001",
    "green_tag": true,
    "match_count": 35,
    "years_active": 1.5
  }
}
```

---

**Document Status:** Locked (base rates), Open (formulas)
**Last Updated:** 2025-12-21
**Next Review:** Design XP formulas and ceiling modification rules
