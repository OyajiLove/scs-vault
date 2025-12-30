# Physical Decline

📛 **MECHANIC:** Stat Deterioration with Age
🔗 **PARENT SYSTEM:** [[_Aging System Index|Aging System]]
🧭 **CATEGORY:** Worker Lifecycle
🔑 **KEYWORDS:** decline, deterioration, aging, stats, physical, injury, wear
📌 **ORIGIN:** Vol 4 (decline concept), Worker Skills (decline rates)
✅ **STATUS:** Partially Locked (rates from Vol 4), Open (exact formulas)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4, Worker Skills | 🔒 LOCKED (rates) |

---

## Overview

Physical decline is the gradual deterioration of a worker's body over their career. Stats decrease at predictable rates after peak years, modified by style, injury history, and lifestyle factors. Understanding decline helps players manage rosters and plan for generational transitions.

---

## Base Decline Rates

### Post-Peak Decline (Age > Peak End)

| Stat Category | Annual Decline | Notes |
|---------------|----------------|-------|
| **Speed/Agility** | -1.5 | Declines fastest |
| **Stamina** | -1.0 | Cardio fades |
| **Strength** | -0.5 | Holds longer |
| **Durability** | -0.5 | Varies by injury history |
| **Aerial** | -1.5 | Correlates with speed |
| **Power** | -0.5 | Correlates with strength |
| **Technical** | -0.25 | Skill-based, minimal decline |
| **Striking** | -0.5 | Moderate |
| **Psychology** | +0.25 | Can IMPROVE with age |
| **Selling** | +0.25 | Can IMPROVE with age |
| **Composure** | +0.25 | Can IMPROVE with age |

**Formula:**
```
Stat at Age X = Peak Stat - (Age - Peak End) × Decline Rate × Style Modifier × Injury Modifier
```

---

## Style Modifiers to Decline

| Style | Modifier | Effect |
|-------|----------|--------|
| **High Flyer** | 1.5x | Accelerated decline |
| **Deathmatch** | 1.75x | Fastest decline |
| **Technical** | 0.75x | Slower decline |
| **Submission** | 0.5x | Slowest decline |
| **Psychology-Based** | 0.5x | Mind compensates |
| **Power** | 1.0x | Standard |
| **Brawler** | 1.25x | Accumulated damage |

---

## Injury Modifiers

Accumulated injuries accelerate decline:

| Injury History | Modifier | Notes |
|----------------|----------|-------|
| **Clean** (0-2 minor injuries) | 1.0x | No acceleration |
| **Light** (3-5 minor injuries) | 1.1x | Slight acceleration |
| **Moderate** (1-2 major injuries) | 1.25x | Noticeable |
| **Heavy** (3+ major injuries) | 1.5x | Significant |
| **Severe** (career-altering injury) | 2.0x+ | Rapid decline |

### Specific Injury Effects

| Injury Type | Stat Most Affected |
|-------------|-------------------|
| **Knee** | Speed, Aerial, Stamina |
| **Back** | Power, Durability, Aerial |
| **Neck** | All physical stats |
| **Shoulder** | Power, Striking |
| **Concussion (multiple)** | Psychology, Composure |
| **Hand/Wrist** | Technical, Submission |

---

## LIFESTYLE TRACKER (#45)

📌 **Source:** Vol 1 Extraction #45

### Core Concept

Lifestyle choices create visible wear on workers over time. Drinkers, smokers, and hard-living wrestlers show it in their faces and bodies.

### Lifestyle Categories

| Factor | Effect on Aging |
|--------|----------------|
| **Drinkers/Smokers** | Deeper lines, sunken eyes, rougher aging curves |
| **"Hard liver" personalities** | Faster overall decline |
| **Natural freaks** | Slower aging (genetic blessing) |
| **Wrestling Style** | Brawlers/deathmatch workers show more wear |
| **Clean living** | Preserved appearance and function |

### Genetics/Natural Resistance Stat

| Factor | Effect |
|--------|--------|
| Some workers scar easier | Funk bled buckets, face tells the story |
| Some barely scar | Baba looked the same for decades |
| Affects visual portrait evolution | AI-generated faces reflect lifestyle |

### Implementation Note

Lifestyle tracking feeds into both [[Physical Decline]] calculations AND visual portrait evolution system.

---

## Lifestyle Modifiers (Decline Rates)

Hidden Personality and lifestyle tags affect decline:

| Factor | Modifier | Notes |
|--------|----------|-------|
| **"Substance Abuse Risk"** | 1.5x | Accelerates all decline |
| **High Drive** | 0.9x | Training slows decline |
| **Low Drive** | 1.2x | Coasting accelerates decline |
| **Clean Living** | 0.8x | Healthy habits slow decline |
| **Party Lifestyle** | 1.3x | Burns out faster |

---

## Decline Thresholds

### Functional Thresholds

| Stat Level | Status |
|------------|--------|
| **15+** | Elite, main event capable |
| **12-14** | Good, upper-midcard viable |
| **9-11** | Functional, midcard |
| **6-8** | Limited, enhancement level |
| **3-5** | Barely functional |
| **1-2** | Cannot perform safely |

### Retirement Consideration Triggers

| Trigger | Effect |
|---------|--------|
| **3+ physical stats below 6** | Active retirement consideration |
| **Speed or Stamina below 5** | Cannot work full matches |
| **All physical stats below average** | Forced retirement likely |
| **Match quality consistently below 2 stars** | Performance-based retirement |

---

## Compensating for Decline

Workers can partially offset physical decline:

| Compensation | Effect | Requirements |
|--------------|--------|--------------|
| **Style Change** | Reduces relevant decline | Adaptability, training time |
| **Psychology Focus** | Mental stats compensate | High base psychology |
| **Part-Time Schedule** | Preserves body longer | Contract negotiation |
| **Protected Matches** | Hides limitations | Booking cooperation |
| **Manager/Mouthpiece** | Covers promo decline | Relationship available |
| **Tag Team** | Partner covers weaknesses | Chemistry required |

---

## Visual Decline Indicators

Players may notice decline through:

| Indicator | What It Means |
|-----------|---------------|
| **Slower match pace** | Stamina decline |
| **Fewer aerial moves** | Speed/Aerial decline |
| **More rest holds** | Stamina compensation |
| **Protected finishes** | Cannot take bumps |
| **Shorter matches** | Overall physical decline |
| **Better promos** | Mental stats compensating |
| **More psychology spots** | Skill compensating for athletics |

---

## Exceptional Cases

### Extended Peak (Rare)

Some workers defy normal decline:

| Worker | Age at High Performance | Explanation |
|--------|------------------------|-------------|
| **Ric Flair** | 55+ | Psychology mastery, protected style |
| **Terry Funk** | 50+ | Toughness, hardcore adaptation |
| **AJ Styles** | 45+ | Clean lifestyle, style adaptation |
| **Chris Jericho** | 50+ | Constant reinvention |

**Requirements:**
- Exceptional base talent
- Clean lifestyle or extreme toughness
- Successful style adaptation
- Promotional protection
- "Never Say Die" or equivalent tags

### Rapid Decline (More Common)

| Worker | Decline Trigger | Notes |
|--------|-----------------|-------|
| **Ultimate Warrior** | Limited skillset exposed | No adaptation possible |
| **Dynamite Kid** | Accumulated injuries | Style destroyed body |
| **Jeff Hardy** | Lifestyle + injuries | Multiple factors |

---

## Connected Mechanics

- [[Career Phases]] - Phase determines decline context
- [[Peak Years by Style]] - Style affects decline rate
- [[_Injury System Index|Injury System]] - Injuries accelerate decline
- [[_Retirement System Index|Retirement System]] - Decline triggers retirement

---

## Open Questions

- [ ] Exact formula coefficients for each stat
- [ ] How does training during decline slow it?
- [ ] Minimum stat floors (can stats hit 0?)
- [ ] Recovery from decline (temporary boosts)?

---

## Implementation Notes

```json
{
  "worker_decline": {
    "worker_id": "worker_001",
    "current_age": 38,
    "peak_ended_age": 35,
    "years_post_peak": 3,
    "style": "high_flyer",
    "style_modifier": 1.5,
    "injury_modifier": 1.25,
    "lifestyle_modifier": 1.0,
    "stat_changes": {
      "speed": {
        "peak_value": 16,
        "current_value": 12,
        "annual_decline": -1.5,
        "adjusted_decline": -2.8
      },
      "psychology": {
        "peak_value": 14,
        "current_value": 15,
        "annual_change": +0.25
      }
    }
  }
}
```

---

**Document Status:** Partially Locked (rates), Open (formulas)
**Last Updated:** 2025-12-21
**Next Review:** Design exact coefficient formulas
