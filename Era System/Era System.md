# ERA SYSTEM

📛 **NAME:** Era System
🧭 **CATEGORY:** World Simulation / Time Context
🔑 **KEYWORDS:** era, decade, time period, historical, fan expectations, style preferences, era adaptability
📝 **SUMMARY:**

The Era System governs how the game world changes across different time periods. Fan expectations, acceptable content, booking styles, production values, and worker style preferences all shift based on the in-game year. Workers have an Era Adaptability rating determining how well they fit different periods.

⚙️ **LOGIC OVERVIEW:**

- Game world operates within defined eras with distinct characteristics
- Fan expectations and preferences shift by era
- Workers have Era Adaptability ratings affecting cross-era performance
- Era affects AI booking behavior, production standards, and acceptable content
- Cultural expectations vary by region AND era

🔬 **LLM INTEGRATION:** Medium (era-appropriate flavor text, booking suggestions)

📌 **ORIGIN:** Vol 1 Extraction #81, #113, #140

📎 **CONNECTED SYSTEMS:**
- [[Era_UI_System]] - Visual presentation by era
- [[Territory System/_Territory System Index|Territory System]] - Regional variation within eras
- [[Popularity_System]] - Era affects what makes workers popular
- [[Crowd_Memory]] - Memory persistence across era boundaries

❓ **OPEN QUESTIONS:**
- Exact year breakpoints for each era
- How do workers transition between eras?
- Era-specific tag unlocks/locks?
- Mid-era shifts (e.g., Attitude Era within 90s)

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #81, #113, #140 | 🔒 LOCKED (concept) |

---

## ERA DEFINITIONS (#140)

| Era | Years | Key Features |
|-----|-------|--------------|
| **Territory** | 1950-1983 | Regional focus, kayfabe strong, slow builds, blood feuds |
| **National Expansion** | 1984-1992 | WWF dominance, cable TV, cartoonish characters, rock & wrestling |
| **Monday Night Wars** | 1995-2001 | Competition, edgy content, swerves, star-making pushes |
| **Ruthless Aggression** | 2002-2008 | Edgy content, brand split, OVW talent pipeline |
| **PG Era** | 2008-2014 | Family friendly, long reigns, brand splits, social media rise |
| **Reality Era** | 2014-2019 | Social media integration, worked shoots, "universe" branding |
| **Modern** | 2019+ | Workrate focus, AEW competition, part-timer events |

---

## ERA EFFECTS

Each era modifies multiple game systems:

| System | Era Effect |
|--------|------------|
| **Fan Expectations** | What fans want to see changes |
| **Acceptable Content** | Violence, language, sexuality thresholds |
| **Booking Style Preferences** | Long builds vs. hot-shot, clean vs. dusty finishes |
| **Production Values Expected** | Pyro budget, stage complexity |
| **Worker Style Preferences** | What in-ring styles get over |
| **Information Spread** | Kayfabe protection, dirt sheet influence |
| **Media Landscape** | TV importance, PPV model, streaming |

---

## ERA ADAPTABILITY SYSTEM (#81)

### Core Concept

For scenarios where workers appear outside their natural era (fantasy drafts, time-travel scenarios, alternate history).

**Era Adaptability Rating:** Measures how well a worker's style fits different eras and whether they can adjust.

| Adaptability Level | Effect |
|-------------------|--------|
| **High** (Vader, Jericho) | Can adapt to any era, learns to adjust style |
| **Medium** | Struggles initially but can learn |
| **Low** (Omega in 1984) | Disaster unless they fundamentally shift style |

### In Practice: Kenny Omega in 1985 Mid-South

```
Omega drops into 1985 Mid-South Wrestling:
- Tries his usual high spot sequences
- Crowd confused or booing "phony wrestler" vibes

Omega can:
1. Shift style (learn to sell more, work gritty, minimize motion) → Crowd accepts
2. Refuse to adapt → Die on the vine, never gets over
```

### Era-Appropriate Psychology Meter

Certain styles score differently by era:

| Style | 1980s NWA | 1990s Japan | 2020s US |
|-------|-----------|-------------|----------|
| High spot sequences | Low | Medium | High |
| Gritty selling | High | High | Medium |
| Character work | High | Medium | High |
| Workrate | Medium | Very High | High |
| Comedy | Medium | Low | High |

### Fanbase Cultural Expectations by Era/Region

| Era/Region | What Fans Want |
|------------|----------------|
| '80s Southern US | Realism, blood, clear good/evil |
| '90s Japan | Pure workrate, fighting spirit |
| '90s US (Attitude) | Edgy content, stars, storylines |
| 2020s US | Storytelling + workrate + meme moments |
| 2020s Japan | Tradition + modern pacing |

### Era Correction Factor

Adjust how fans perceive certain traits based on year and region:

**Example:** Hulk Hogan
- 1985 WWF: Maximum believable babyface (Era fit: Perfect)
- 2020 AEW: Nostalgia act at best (Era fit: Poor for active role)

---

## ERA-SPECIFIC AI BOOKING BEHAVIOR (#113)

CPU bookers behave differently based on era settings:

| Era | AI Booking Tendencies |
|-----|----------------------|
| **Territory (70s-80s)** | Protect top guys, long builds, regional focus, blood feuds |
| **National Expansion (80s-90s)** | Aggressive talent raids, TV focus, character-first |
| **Monday Night Wars** | Hot-shot booking, swerves, star-making pushes, counter-programming |
| **Ruthless Aggression** | Edgy content, rapid title changes, brand competition |
| **PG Era** | Safe booking, long reigns, brand splits, kid-friendly |
| **Modern (2020s)** | Workrate focus, social media awareness, part-timer reliance |

**AI Personality Overlay:** Era tendencies are modified by individual booker personality. A cutthroat booker in the Territory era still protects kayfabe, but raids talent more aggressively.

---

## ERA TRANSITION MECHANICS

When the game year crosses an era boundary:

| Event | Effect |
|-------|--------|
| **Fan Expectation Shift** | Gradual change in what pops crowds |
| **Style Relevance Shift** | Some workers gain/lose relevance |
| **Production Standard Shift** | Expectations for show quality change |
| **Content Threshold Shift** | What's acceptable changes |

### Transition Speed

Era changes don't happen overnight:

| Transition Type | Duration |
|-----------------|----------|
| **Gradual** | 2-3 years of blending |
| **Catalyst Event** | Single event accelerates change (e.g., Montreal Screwjob) |
| **Cultural Lag** | Some regions transition slower |

---

## REGIONAL ERA VARIATION

Not all regions are in the same "era" simultaneously:

| Region | May Lag Behind | May Lead |
|--------|----------------|----------|
| **Japan** | Character trends | Workrate trends |
| **Mexico** | Rarely changes core style | Mask/hair traditions timeless |
| **US South** | Often trails national trends | Blood feud traditions persist |
| **UK** | Follows US trends | Catch wrestling traditions persist |

---

## IMPLEMENTATION NOTES

### Era Data Structure

```json
{
  "era_id": "monday_night_wars",
  "name": "Monday Night Wars",
  "year_range": {
    "start": 1995,
    "end": 2001
  },
  "characteristics": {
    "kayfabe_strength": 0.4,
    "violence_tolerance": 0.8,
    "workrate_appreciation": 0.6,
    "character_importance": 0.9,
    "hot_shot_tendency": 0.7,
    "swerve_frequency": 0.8
  },
  "fan_preferences": {
    "style_weights": {
      "brawling": 0.7,
      "technical": 0.5,
      "high_flying": 0.7,
      "comedy": 0.6,
      "hardcore": 0.8
    }
  },
  "ai_booking_modifiers": {
    "title_change_frequency": 1.3,
    "build_length_modifier": 0.7,
    "swerve_probability": 0.25
  }
}
```

### Worker Era Adaptability Structure

```json
{
  "worker_id": "worker_001",
  "era_adaptability": {
    "base_rating": 65,
    "era_fits": {
      "territory": 40,
      "national_expansion": 55,
      "monday_night_wars": 70,
      "ruthless_aggression": 80,
      "pg_era": 75,
      "modern": 95
    },
    "style_flexibility": 0.7,
    "can_learn": true
  }
}
```

---

## CONNECTED MECHANICS

- [[Era_UI_System]] - Visual presentation changes by era
- [[Territory System/Territory Personality Types|Territory Personality Types]] - AI booker era behavior
- [[Scouting System]] - Era affects information availability
- [[Media System/_Media System Index|Media System]] - Era affects news presentation

---

## OPEN QUESTIONS

- [ ] Exact formulas for era adaptability penalties
- [ ] Can workers permanently change their era fit through training?
- [ ] How do era transitions affect ongoing storylines?
- [ ] Sub-eras within major eras (early vs. late Attitude)?

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define exact era transition year boundaries
