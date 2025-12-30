# Draft War Room System

📛 **MECHANIC:** Draft War Room / All-Time Peak Draft Mode
🔗 **PARENT SYSTEM:** [[Booking System/Three-Tier Booking Assistance|Booking Assistance]]
🧭 **CATEGORY:** Game Mode / Roster Construction
🔑 **KEYWORDS:** draft, war room, roster building, all-time peak, fantasy booking
📌 **ORIGIN:** Vol 1 Extraction #228-229
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

The Draft War Room provides a strategic interface for roster construction, whether for fantasy scenarios, new promotions, or "what if" games. The All-Time Peak Draft Mode allows players to draft historical wrestlers at their career peaks.

---

## Draft War Room Features (#228)

### AI Assistant Suggestions

During draft, the AI assistant provides:

| Feature | Description |
|---------|-------------|
| **Pick Suggestions** | "Based on your roster needs, consider..." |
| **Fit Analysis** | How well a worker fits your promotion style |
| **Chemistry Flags** | Known good/bad combinations |
| **Gap Identification** | "You lack a monster heel" |
| **Value Assessment** | Over/undervalued workers |

### Handicap System

For competitive drafts between human players:

| Handicap Level | Effect |
|----------------|--------|
| **None** | Standard draft order |
| **Mild** | Weaker player gets extra late pick |
| **Moderate** | Weaker player drafts 1st and 3rd |
| **Heavy** | Weaker player gets 2 picks per round |
| **Extreme** | Strong player drafts from limited pool |

### Draft Formats

| Format | Description |
|--------|-------------|
| **Snake** | 1-2-2-1 order reversal |
| **Auction** | Budget bidding for workers |
| **Territorial** | Geographic restrictions |
| **Era-Locked** | Only workers from specific era |
| **Style-Themed** | Only workers matching style (puroresu, lucha, etc.) |

---

## All-Time Peak Draft Mode (#229)

### Concept

Draft historical wrestlers at their absolute career peak, regardless of when that peak occurred.

### Peak Year Examples

| Worker | Peak Year | Peak Version |
|--------|-----------|--------------|
| Ric Flair | 1985 | NWA Champion, 60-minute king |
| Stone Cold | 1998 | Attitude Era megastar |
| Mitsuharu Misawa | 1994 | Four Pillars peak |
| Rey Mysterio | 2006 | World Champion run |
| The Rock | 2000 | People's Champion era |
| Bret Hart | 1997 | Pre-screwjob excellence |
| Hulk Hogan | 1985 | Hulkamania peak |
| Shawn Michaels | 1996 | Pre-injury HBK |
| Kurt Angle | 2001 | Wrestling machine |
| AJ Styles | 2016 | NJPW/WWE transition |

### Multi-Era Versions

Some workers have multiple draftable versions:

| Worker | Version 1 | Version 2 | Version 3 |
|--------|-----------|-----------|-----------|
| Undertaker | 1991 (Dead Man) | 1998 (Ministry) | 2007 (Streak) |
| Ric Flair | 1985 (NWA) | 1992 (WWF) | 2003 (Evolution) |
| Shawn Michaels | 1996 (Pre-injury) | 2002 (Comeback) | 2008 (HBK/Taker) |
| Terry Funk | 1977 (NWA) | 1989 (Hardcore) | 1997 (ECW) |
| Mick Foley | 1995 (Cactus Jack) | 1998 (Mankind) | 1999 (Commissioner) |

### Era Interaction Rules

When drafting cross-era:

| Scenario | Rule |
|----------|------|
| 1985 worker in 2020 | Era Adaptability check required |
| 2020 worker in 1985 | Style may not translate |
| Same era interaction | Normal chemistry rules |
| Peak vs Peak | Fair matchup, best versions |

---

## Draft Strategy AI

The AI assistant considers:

| Factor | Weight |
|--------|--------|
| **Roster Balance** | Need variety of styles |
| **Main Event Depth** | Multiple credible champions |
| **Heel/Face Balance** | Proper alignment mix |
| **Tag Teams** | Established teams vs. thrown together |
| **Manager Coverage** | Promo support for weak talkers |
| **Regional Appeal** | Market-specific stars |

### Sample AI Suggestion

> "With your 3rd pick, I recommend Toshiaki Kawada (1995 peak). Your roster lacks a Strong Style top star, and Kawada's selling/psychology would contrast well with your existing technical workers. He'd be a natural foil for Bret Hart in a dream feud scenario."

---

## Implementation Notes

```json
{
  "draft_id": "draft_001",
  "mode": "all_time_peak",
  "participants": ["player_1", "player_2"],
  "format": "snake",
  "rounds": 15,
  "picks": [
    {
      "round": 1,
      "pick": 1,
      "player": "player_1",
      "worker": "austin_1998",
      "ai_suggestion": "flair_1985",
      "ai_reasoning": "Flair provides more versatility as heel or face"
    }
  ],
  "roster_analysis": {
    "player_1": {
      "main_eventers": 2,
      "heel_face_ratio": 0.6,
      "style_coverage": ["brawler", "entertainer"],
      "gaps": ["technician", "high_flyer"]
    }
  }
}
```

---

## Connected Mechanics

- [[Worker_Skills]] - Peak stats for each era version
- [[Era Values Matrix]] - Era interaction rules
- [[Hidden_Personality]] - Chemistry calculations
- [[Booking System/Three-Tier Booking Assistance|Three-Tier Booking]] - AI suggestions

---

## Open Questions

- How many "versions" per worker maximum?
- Peak year determination criteria?
- Handling career-overlapping workers (Austin vs Rock)?
- Fantasy booking restrictions?

---

**Document Status:** Concept Locked
**Last Updated:** 2024-12-23
