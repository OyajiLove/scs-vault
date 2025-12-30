# Tournament Wizard System

📛 **MECHANIC:** Tournament Wizard / G1-Style League Setup
🔗 **PARENT SYSTEM:** [[_Booking System Index|Booking System]]
🧭 **CATEGORY:** Event Booking / Special Event Management
🔑 **KEYWORDS:** tournament, G1, round robin, brackets, fatigue, seeding, knockout
📌 **ORIGIN:** Vol 1 Extraction #96
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

The Tournament Wizard provides a streamlined interface for booking tournaments of various formats. From G1-style round robin leagues to single-elimination brackets, the system handles scheduling, fatigue accumulation, and storyline integration automatically.

---

## G1-Style League Wizard Example (#96)

📌 **Source:** Vol 1 Extraction #96

### Setup Configuration

```
- Choose Tournament Name: [G1 Climax XXVI]
- Format: Blocked Round Robin (2 Blocks of 10)
- Match Style: 30-min Time Limit Matches
- Points System: Win = 2, Draw = 1, Loss = 0
- Fatigue: Moderate
- Injury Risk: Enabled (5%)
- Stakes: Winner challenges for World Heavyweight Title at Wrestle Kingdom
- Seeding: Top 5 Seeds / Random draw for rest
- Crowd Bias: Japan (pops more for Japanese workers, underdog foreigners)
- Optional Surprise: Draw limit chaos (fans get wild for time limit finishes)
```

---

## Tournament Formats

| Format | Description | Best For |
|--------|-------------|----------|
| **Round Robin (Blocked)** | All vs all within blocks, block winners meet in finals | G1, N1 Victory |
| **Round Robin (Single)** | All vs all, most points wins | Champion Carnival |
| **Single Elimination** | Lose and you're out | King of the Ring, BOSJ |
| **Double Elimination** | One loss moves to losers bracket | Longer tournaments |
| **Gauntlet** | Winner stays on | TV tournaments |
| **Tag League** | Tag team round robin | World Tag League |

---

## Dynamic Match Impacts

| Event | Effect |
|-------|--------|
| Worker A wins 5 matches straight in G1 | Slight fatigue (-5% stamina next matches) |
| Worker B wrestles 3 30-minute draws | Heavy fatigue (-15% stamina) |
| Worker C injures Worker D mid-tournament | Replacements, upset brackets, crowd pop |
| Worker D wins anyway, limping | Hero arc, MASSIVE fan love |

---

## Tournament Momentum Modifier

**Key Insight:** "Winning the crowd during tournaments = big boosts even without winning the tourney."

| Scenario | Momentum Effect |
|----------|-----------------|
| Upset early favorite | Major buzz for winner |
| Survive grueling schedule | "Iron man" reputation |
| Consistently great matches | Tournament MVP buzz |
| Fail despite strong run | Sympathetic underdog heat |

---

## Fatigue Accumulation

| Match Type | Fatigue Added |
|------------|---------------|
| Short match (<10 min) | +5% |
| Standard match (10-20 min) | +10% |
| Long match (20-30 min) | +15% |
| Time limit draw | +20% |
| Brutal match (blood, weapons) | +25% |

**Recovery:** 1-2 days between matches = -5% fatigue recovery

---

## Smart Booking Assistance

| Situation | AI Assistance |
|-----------|---------------|
| Need to rest a star? | Suggests logical match layouts (short matches, DQ finishes) |
| Feud heating up? | Suggests angle or grudge match |
| Tournament is too chalky? | Suggests pulling an upset to keep crowd hot |
| Worker getting injured? | Offers replacement options, story covers |

---

## Post-Tournament Fallout (Automatic)

| Outcome | System Effect |
|---------|---------------|
| Tournament winner | Earns automatic world title match at scheduled PPV |
| Tournament MVP | Gains popularity/momentum even if didn't win |
| Strong performer | Career trajectory boost |
| Disappointing run | Possible character reassessment needed |
| Tag tournaments | Strengthen or fracture tag divisions organically |

---

## Seeding Options

| Option | Description |
|--------|-------------|
| **Top Seeds** | Highest-ranked workers get favorable draws |
| **Random** | Complete random assignment |
| **Regional** | Balance regional representation per block |
| **Storyline** | Place rivals in same block for guaranteed clash |
| **Custom** | Player determines all placements |

---

## Injury Risk Settings

| Setting | Injury Chance Per Match |
|---------|------------------------|
| **Off** | 0% |
| **Low** | 2% |
| **Moderate** | 5% |
| **Realistic** | 8% |
| **Brutal** | 12% |

**Injury Severity:** When injury occurs, severity rolled separately (minor to career-threatening).

---

## Block Calculation Example

**Two Blocks of 10:**
- Each worker has 9 matches
- 45 matches per block
- 90 matches total before finals
- Tournament spans 3-4 weeks (typical G1 schedule)

---

## Connected Mechanics

- [[Skill Growth Mechanics]] - Tournament performance affects growth
- [[Buzz System/_Buzz System Index|Buzz System]] - Tournament buzz tracked
- [[Injury System]] - Injury risk per match
- [[Title System]] - Winner's title shot booking
- [[Fatigue Tracking]] - Stamina across tournament

---

## Open Questions

- Maximum tournament size?
- Cross-promotion tournament handling?
- Historical tournament recreation (data import)?
- Women's tournament specific rules?

---

## Implementation Notes

```json
{
  "tournament_id": "tourn_001",
  "name": "G1 Climax XXVI",
  "format": "blocked_round_robin",
  "blocks": 2,
  "participants_per_block": 10,
  "points_system": {
    "win": 2,
    "draw": 1,
    "loss": 0
  },
  "time_limit_minutes": 30,
  "fatigue_level": "moderate",
  "injury_risk": 0.05,
  "prize": "world_title_shot",
  "seeding": "top_5_seeded",
  "regional_bias": "japan",
  "schedule": [
    {
      "night": 1,
      "block": "A",
      "matches": [
        {"w1": "okada", "w2": "tanahashi"},
        {"w1": "naito", "w2": "ishii"}
      ]
    }
  ]
}
```

---

**Document Status:** Concept Locked
**Last Updated:** 2025-12-25
