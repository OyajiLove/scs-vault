# House Styles

📛 **MECHANIC:** House Styles
🔗 **PARENT SYSTEM:** [[_Match Types Index|Match Types & Era Flavor]]
🧭 **CATEGORY:** Match Simulation / Booking Context
🔑 **KEYWORDS:** house style, King's Road, Strong Style, lucha libre, American style, puroresu, booking philosophy
📌 **ORIGIN:** Vol 3 (critical distinction locked: styles ≠ match types)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 | 🔒 LOCKED |

---

## Overview

House styles are promotion philosophies that flavor how matches are worked, judged, and perceived. **Critical insight:** Strong Style, King's Road, etc. are NOT match types. They're aesthetic and philosophical frameworks that can apply to any match type.

---

## The Core Distinction

| Concept | What It Is | Example |
|---------|------------|---------|
| **Match Type** | Structural format | Singles, Tag, Gauntlet |
| **House Style** | How matches are worked | King's Road, Strong Style |
| **Stipulation** | Added gimmick rules | Cage, Ladder, No DQ |

A King's Road singles match and a Strong Style singles match are both singles matches, but they feel completely different.

---

## Major House Styles

### King's Road (AJPW)

| Element | Characteristic |
|---------|----------------|
| **Pace** | Slow build, dramatic escalation |
| **Selling** | Long-term, cumulative damage |
| **Finishes** | Fighting spirit kickouts, head drops |
| **Psychology** | Story through exhaustion and will |
| **Signature spots** | Lariat wars, dangerous suplexes |

**Era peak:** 1990-1999 AJPW

---

### Strong Style (NJPW)

| Element | Characteristic |
|---------|----------------|
| **Pace** | Stiff, intense, shoot-influenced |
| **Selling** | Immediate impact, fighting through |
| **Finishes** | Strikes, submissions, quick pins |
| **Psychology** | Combat legitimacy, martial arts base |
| **Signature spots** | Stiff kicks, forearm exchanges |

**Era peak:** 1970s-1980s Inoki-era, 2010s revival

---

### Lucha Libre

| Element | Characteristic |
|---------|----------------|
| **Pace** | Fast, acrobatic, continuous motion |
| **Selling** | Quick recovery, resilience |
| **Finishes** | Pins from high-flying, submissions |
| **Psychology** | Honor, mask/hair stakes, family legacy |
| **Signature spots** | Dives, armdrags, rapid exchanges |

**Era peak:** Continuous tradition, peaks in 1980s CMLL/UWA

---

### American Main Event Style

| Element | Characteristic |
|---------|----------------|
| **Pace** | Heat segment → hope spots → comeback |
| **Selling** | Face-in-peril extended sequences |
| **Finishes** | Protected finishers, signature moves |
| **Psychology** | Babyface triumph over adversity |
| **Signature spots** | Hot tags, Hulk-up comebacks |

**Era peak:** 1980s WWF, 1980s NWA

---

### Southern Brawl Style

| Element | Characteristic |
|---------|----------------|
| **Pace** | Slow, violent, personal |
| **Selling** | Pain, blood, exhaustion |
| **Finishes** | Often screwjob or brutal climax |
| **Psychology** | Grudge, hatred, revenge |
| **Signature spots** | Blade jobs, brawling outside ring |

**Era peak:** 1970s-1980s territories (Memphis, Mid-South)

---

### Deathmatch/Garbage Style

| Element | Characteristic |
|---------|----------------|
| **Pace** | Chaotic, spot-based |
| **Selling** | Visual damage (blood, scars) |
| **Finishes** | Extreme spots, weapon use |
| **Psychology** | Survival, pain threshold |
| **Signature spots** | Glass, fire, barbed wire |

**Era peak:** 1990s FMW/ECW, ongoing underground

---

### Joshi Puroresu

| Element | Characteristic |
|---------|----------------|
| **Pace** | Fast, athletic, high-impact |
| **Selling** | Intense, emotional, dramatic |
| **Finishes** | Crisp pins, devastating moves |
| **Psychology** | Rivalry, respect, generational passing |
| **Signature spots** | Dangerous drops, chain wrestling |

**Era peak:** 1990s AJW

---

## Style Interactions

| Scenario | Result |
|----------|--------|
| **Same style vs same style** | Pure expression of that style |
| **Style clash** | Tension, adjustment period, or trainwreck |
| **Worker adapts to promotion style** | Integration, may lose original flavor |
| **Promotion imports foreign style** | Novelty pop, potential rejection |

---

## Style and Match Quality

Match quality is judged relative to house style expectations:

- King's Road match judged on escalation and drama
- Strong Style match judged on stiffness and intensity
- Lucha match judged on flow and innovation

A "bad" King's Road match might be a "good" American TV match, and vice versa.

---

## Connected Mechanics

- [[Match Type Categories]] - styles apply to any type
- [[Era Booking Profiles]] - styles have era peaks
- [[Match Quality Factors]] - style affects judging criteria
- [[Region Era Profiles]] - regional style expectations

---

## Open Questions

- Style fusion mechanics (King's Road + Strong Style hybrids)
- Worker style tags (personal style vs promotion style)
- Style drift over time within promotions

---

## Implementation Notes

```json
{
  "house_style": {
    "style_id": "hs_kings_road",
    "name": "King's Road",
    "region": "japan",
    "era_peak": "1990-1999",
    "associated_promotions": ["ajpw"],
    "judging_criteria": {
      "escalation": 1.5,
      "selling": 1.3,
      "drama": 1.4,
      "stiffness": 1.0,
      "highflying": 0.8
    },
    "signature_elements": ["lariat_war", "head_drop", "fighting_spirit"]
  }
}
```
