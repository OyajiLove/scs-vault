# Gimmick Attributes

📛 **MECHANIC:** Gimmick Attributes
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** gimmick attributes, ring name, alignment, presentation, emotional tags
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 1-3 | Gimmick concepts mentioned in context of character presentation, not formally systematized |
| v2.0 | Vol 6 | **LOCKED** - Full attribute set defined: Ring Name, Style, Alignment, Presentation, Emotional Tags, Intensity, Risk Profile, Legacy Potential, Merch Appeal |

---

## Overview

Every gimmick is defined by a set of attributes that shape how the character is perceived, booked, and remembered. These are distinct from [[Worker_Skills|Skills]] (what they can do) and [[Tags_System|Tags]] (who they are underneath).

---

## Core Attributes

| Attribute | Description |
|-----------|-------------|
| **Ring Name** | The performed identity (can differ from shoot name) |
| **Style** | Wrestling approach: Technical, Brawler, High-Flyer, Powerhouse, etc. |
| **Alignment** | Face / Heel / Tweener |
| **Presentation** | Visual identity: gear, entrance, mannerisms |
| **Emotional Tags** | Core feelings the gimmick evokes: Fear, Sympathy, Rage, Comedy, etc. |
| **Intensity** | How "turned up" the character is (subtle vs over-the-top) |
| **Risk Profile** | How much the gimmick relies on dangerous spots |
| **Legacy Potential** | Ceiling for long-term cultural impact |
| **Merch Appeal** | Commercial viability of the character |

---

## Ring Name

The performed identity:

- Can match shoot name (John Cena)
- Can be completely separate (Glenn Jacobs → Kane)
- Can evolve (Ringmaster → Stone Cold)
- Multiple workers can inherit a name (Tiger Mask lineage)

---

## Alignment

| Alignment | Description |
|-----------|-------------|
| **Face** | Hero, crowd favorite, plays by rules |
| **Heel** | Villain, generates heat, cheats/manipulates |
| **Tweener** | Morally ambiguous, can work either side |

Alignment affects:
- Promo tone and content
- Match finish options
- Crowd response calculations
- Feud dynamics

---

## Emotional Tags

The feelings a gimmick evokes in the crowd:

| Tag | Examples |
|-----|----------|
| **Fear** | Undertaker, Kane, Muta |
| **Sympathy** | Daniel Bryan, Hangman |
| **Rage** | Stone Cold, Moxley |
| **Comedy** | Orange Cassidy, Santino |
| **Awe** | Okada, early Goldberg |
| **Nostalgia** | Returning legends |
| **Cool** | nWo, Bullet Club |

Multiple emotional tags can coexist. Dominant tag affects booking suggestions.

---

## Connected Mechanics

- [[Gimmick Lifecycle]] - how attributes evolve over time
- [[Gimmick Management]] - changing attributes via repackage
- [[Iconic Lock]] - exceptional attributes can lock in

---

## Gimmick Fit Formula (#36)

📌 **Source:** Vol 1 Extraction #36

**Core Concept:** How well a gimmick matches a worker's natural abilities dramatically affects their performance.

### Effective Believability in Promos

```
Effective Believability = (Base Believability × Gimmick Fit Modifier) + (Small Random Emotion Surge if Stakes High)
```

### Gimmick Fit Thresholds

| Fit Range | Effect on Believability |
|-----------|-------------------------|
| 85%+ (Perfect) | +15% Believability during promos |
| 60%-84% (Good) | No bonus or penalty |
| 40%-59% (Poor) | -10% Believability during promos |
| <40% (Disaster) | -20% Believability + risk of audience ridicule |

### Design Calibration (User-Locked)

| Worker | Gimmick | Fit | Notes |
|--------|---------|-----|-------|
| Scott Steiner | White Meat Babyface 1990 | 40% | Believability suffers, feels forced |
| Scott Steiner | Big Poppa Pump | 95% | Everything feels rawly real |
| Steve Austin | Ringmaster | 45% | Million dollar smile doesn't fit |
| Steve Austin | Stone Cold | 98% | Perfect fusion of man and character |

### Important Balance Note (Locked)

"Gimmick Fit should matter, but mostly reinforce or erode performance by degrees, not completely redefine most workers."

- **80% of workers:** Mild boost or erosion from gimmick fit
- **20% (edge cases):** Major impact (Steiner, Ringmaster Austin, Glenn Jacobs → Kane)

### Factors Determining Fit

| Factor | Weight |
|--------|--------|
| Alignment match to personality | High |
| Style match to physical abilities | Medium |
| Intensity match to natural charisma | Medium |
| Presentation comfort level | Medium |
| Era appropriateness | Low-Medium |

---

## Open Questions

- Maximum emotional tags per gimmick?
- Intensity scaling formula for crowd response?
- Exact formula for calculating base Gimmick Fit %?

---

## Implementation Notes

```json
{
  "gimmick_id": "gim_001",
  "worker_id": "w_001",
  "ring_name": "The Undertaker",
  "style": "brawler_powerhouse",
  "alignment": "tweener",
  "presentation": {
    "entrance": "elaborate",
    "gear": "iconic",
    "mannerisms": "supernatural"
  },
  "emotional_tags": ["fear", "awe", "nostalgia"],
  "intensity": 9,
  "risk_profile": "medium",
  "legacy_potential": 95,
  "merch_appeal": 90
}
```
