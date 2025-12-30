# Era Values Matrix

📛 **MECHANIC:** Era Values Matrix / Era-Sensitive Fan Logic
🔗 **PARENT SYSTEM:** [[Territory System/_Territory System Index|Territory System]]
🧭 **CATEGORY:** Historical Context / Fan Behavior
🔑 **KEYWORDS:** era, time period, fan values, kayfabe, scandal impact, historical
📌 **ORIGIN:** Vol 1 Extraction #35, #199-201
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Different eras have fundamentally different fan expectations, values, and tolerances. What works in 1985 fails in 2025, and vice versa. The Era Values Matrix defines these differences for historically accurate simulation.

---

## Core Era Definitions

### Golden Age (1950s-1960s)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | CRITICAL |
| Authority Respect | Very High |
| Violence Appetite | Moderate |
| Workrate Expectation | Low-Moderate |
| Character Importance | High |
| Scandal Tolerance | Very High (swept under rug) |
| Fan Cynicism | Very Low |

**Characteristics:**
- Wrestling presented as legitimate sport
- Heroes are pure, villains are despicable
- Ethnic/foreign heel gimmicks common
- Television just emerging as platform
- Regional territories dominate

---

### Territory Era (1970s-1985)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | Very High |
| Authority Respect | High |
| Violence Appetite | Moderate-High |
| Workrate Expectation | Moderate |
| Character Importance | Very High |
| Scandal Tolerance | High |
| Fan Cynicism | Low |

**Characteristics:**
- Peak territorial system
- TV deal importance growing
- NWA governing body politics
- Southern/Memphis style storytelling
- First supercards emerge

---

### Expansion Era (1985-1995)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | Moderate (declining) |
| Authority Respect | Moderate |
| Violence Appetite | Moderate |
| Workrate Expectation | Moderate |
| Character Importance | CRITICAL |
| Scandal Tolerance | Moderate |
| Fan Cynicism | Moderate (growing) |

**Characteristics:**
- WWF national expansion
- Cartoon characters dominate
- Steroid scandals emerge
- Territory system collapses
- Pay-per-view becomes major revenue

---

### Attitude Era (1996-2002)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | Low |
| Authority Respect | Low (anti-authority is cool) |
| Violence Appetite | Very High |
| Workrate Expectation | Moderate |
| Character Importance | Very High |
| Scandal Tolerance | High |
| Fan Cynicism | High |

**Characteristics:**
- "Anything goes" mentality
- Edgy content celebrated
- Anti-heroes ascendant
- Monday Night Wars
- ECW influence mainstream
- Worked shoots popular

---

### Reality Era (2011-2019)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | Low |
| Authority Respect | Low |
| Violence Appetite | Moderate |
| Workrate Expectation | High |
| Character Importance | High |
| Scandal Tolerance | Moderate (declining) |
| Fan Cynicism | Very High |

**Characteristics:**
- Social media changes everything
- "Smart" fans mainstream
- Pipe Bomb moment
- Indie wrestlers valued
- NXT as "third brand"
- Fans chant wrestler's real names

---

### Social Media Era (2020+)

| Value | Weight |
|-------|--------|
| Kayfabe Respect | Very Low |
| Authority Respect | Very Low |
| Violence Appetite | Moderate |
| Workrate Expectation | Very High |
| Character Importance | High |
| Scandal Tolerance | VERY LOW |
| Fan Cynicism | Extreme |

**Characteristics:**
- Instant information spread
- Cancel culture affects booking
- Wrestlers have direct fan access
- Behind-the-scenes leaks constant
- AEW competition
- Streaming changes consumption

---

## Era Value Parameters

### Authority Respect

| Era | Level | Effect |
|-----|-------|--------|
| 1950s-60s | Very High | Fans accept booking decisions |
| 1970s-80s | High | Fans trust promoters mostly |
| 1990s | Moderate | Fans question some decisions |
| 2000s | Low | "We know it's fake" attitude |
| 2010s+ | Very Low | Fans think they can book better |

### Violence Appetite

| Era | Level | Effect |
|-----|-------|--------|
| Golden Age | Moderate | Blood rare, impactful |
| Territory | High | Blading common, accepted |
| Attitude | Very High | Hardcore mainstream |
| PG Era | Low | Blood restricted |
| Modern | Moderate | Selective violence acceptable |

### Scandal Impact by Era

| Era | Scandal Handling |
|-----|------------------|
| 1950s-1980s (Kayfabe) | Swept under rug, only kayfabe breaks matter |
| 1990s-2000s (Post-Kayfabe) | Affects alignment, momentum, crowd respect |
| 2010s-Now (Social Media) | Instant explosion, fans expect action |

---

## Era Adaptability (#35 Extension)

Workers dropped into unfamiliar eras need **Era Adaptability** checks:

### Example: Omega in 1984 Crockett

| Factor | Result |
|--------|--------|
| High spots | Crowd boos "phony wrestler" |
| Fast pace | Seen as "not selling" |
| V-Triggers | "What is that supposed to be?" |

**Options:**
- **Adapt:** Learn to sell more, work gritty, minimize flash
- **Refuse:** Get marginalized, leave territory
- **Hybrid:** Find balance (rare success)

### Example: Bruno in 2020 AEW

| Factor | Result |
|--------|--------|
| Simple movesets | "Boring, can't wrestle" |
| Long rests | "Slow, gassed" |
| Strong booking | Fans reject push |

---

## Implementation Notes

```json
{
  "era_id": "attitude_era",
  "date_range": ["1996-01-01", "2002-12-31"],
  "values": {
    "kayfabe_respect": 3,
    "authority_respect": 3,
    "violence_appetite": 9,
    "workrate_expectation": 5,
    "character_importance": 8,
    "scandal_tolerance": 7,
    "fan_cynicism": 7
  },
  "modifiers": {
    "hardcore_bonus": 1.5,
    "pure_technical_penalty": 0.8,
    "anti_hero_bonus": 1.3
  }
}
```

---

## Connected Mechanics

- [[Booking_Engine_P1-3]] - Era-Sensitive Fan Logic
- [[Territory System/_Territory System Index|Territory System]] - Regional era variations
- [[Crowd_Memory]] - Era affects what crowds remember
- [[Scandal System/_Scandal System Index|Scandal System]] - Era determines response

---

## Open Questions

- Granular year-by-year values or era brackets?
- Regional sub-eras (Japan vs US in same year)?
- Transition periods between eras?

---

**Document Status:** Concept Locked
**Last Updated:** 2024-12-23
