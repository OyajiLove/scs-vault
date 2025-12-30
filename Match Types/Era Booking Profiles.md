# Era Booking Profiles

📛 **MECHANIC:** Era Booking Profiles
🔗 **PARENT SYSTEM:** [[_Match Types Index|Match Types & Era Flavor]]
🧭 **CATEGORY:** Match Simulation / Booking Context
🔑 **KEYWORDS:** era booking, booking flavor, promotion history, AJPW, WCW, NOAH, time period
📌 **ORIGIN:** Vol 3 (locked)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 | 🔒 LOCKED |

---

## Overview

Promotions have evolving booking philosophies by era. The same promotion in different years books completely differently. Era profiles define these norms so match quality and booking decisions can be evaluated in proper context.

---

## Canonical Era Profiles

### AJPW 1990-1992

| Element | Norm |
|---------|------|
| **Card structure** | Heavy 6/8-man tags |
| **Violence curve** | Escalating through show |
| **Battle royals** | Light-hearted, for fun |
| **Singles focus** | Reserved for top feuds |
| **Tag importance** | Primary storytelling vehicle |

**Booking flavor:** Tag-centric, violence builds, battle royals as breathers

---

### AJPW 1994-1998

| Element | Norm |
|---------|------|
| **Card structure** | Serious singles and tags |
| **Match quality** | King's Road at peak |
| **Main events** | Extended dramatic epics |
| **Juniors** | Respected but secondary |
| **Finishes** | Fighting spirit, head drops |

**Booking flavor:** Peak King's Road, every main event is a war

---

### WCW 1997

| Element | Norm |
|---------|------|
| **Openers** | Hot, hook the channel-flippers |
| **Finishes** | Bait-and-switch, screwy |
| **Swerves** | Weekly, unpredictable |
| **nWo presence** | Dominates all storylines |
| **Cruiserweight** | Workrate showcase mid-card |

**Booking flavor:** Swerve-heavy, hot openers, interference finishes

---

### NOAH 2000-2005

| Element | Norm |
|---------|------|
| **Special matches** | Captain's Fall featured |
| **Tone** | Respect emphasis |
| **Tournament** | Central booking structure |
| **Pacing** | Deliberate, meaningful |
| **Betrayals** | Rare, devastating when happen |

**Booking flavor:** Tournament-driven, respect culture, meaningful matches

---

### WWF 1998-2001 (Attitude Era)

| Element | Norm |
|---------|------|
| **Promos** | Long, character-driven |
| **Matches** | Shorter, angle-heavy |
| **Interference** | Common, faction warfare |
| **Swerves** | Weekly turns and betrayals |
| **Main event style** | Brawling, weapons |

**Booking flavor:** Storyline over workrate, chaotic, edgy

---

### ECW 1995-1999

| Element | Norm |
|---------|------|
| **Violence** | Extreme, blood common |
| **Promos** | Shoot-style, fourth-wall |
| **Workrate** | High for undercard |
| **Crowd** | Participatory, chanting |
| **Finishes** | Brutal, decisive |

**Booking flavor:** Hardcore spectacle, smart crowd, workrate + violence

---

### 1980s NWA Territories

| Element | Norm |
|---------|------|
| **Heel heat** | Real, dangerous |
| **Face chases** | Long, earned payoffs |
| **TV matches** | Short, angle setup |
| **House shows** | Where real matches happen |
| **Blood** | Reserved for blowoffs |

**Booking flavor:** Slow builds, territory protection, earned moments

---

## Using Era Profiles

| Application | How It Works |
|-------------|--------------|
| **Match evaluation** | Quality judged against era norms |
| **AI booking** | Suggests era-appropriate decisions |
| **Crowd expectations** | Fans expect era-appropriate booking |
| **Commentary** | Flavored by era context |

---

## Era Transitions

Promotions drift between eras:

| Transition Type | Example |
|-----------------|---------|
| **Gradual shift** | AJPW 1992 → 1994 (tag focus → singles) |
| **Sudden change** | WWF 1997 (new era declaration) |
| **Personnel-driven** | NOAH 2000 (exodus creates new culture) |
| **Market pressure** | WCW 1996 (nWo changes everything) |

---

## Connected Mechanics

- [[House Styles]] - era profiles include style expectations
- [[Match Quality Factors]] - era context affects judging
- [[Crowd Signals/Region Era Profiles|Region Era Profiles]] - crowd behavior by era
- [[Booking Trails/_Booking Trails Index|Booking Trails]] - era affects trail structure

---

## Open Questions

- Complete era profile database (all major promotions)
- Era transition mechanics (how does profile change?)
- Custom era creation for fictional promotions

---

## Implementation Notes

```json
{
  "era_profile": {
    "promotion": "ajpw",
    "era": "1994-1998",
    "name": "Peak King's Road",
    "house_style": "kings_road",
    "booking_norms": {
      "tag_focus": 0.6,
      "singles_focus": 0.8,
      "tournament_structure": 0.7,
      "swerve_frequency": 0.2,
      "violence_level": 0.9,
      "workrate_priority": 0.95
    },
    "match_type_weights": {
      "singles": 1.0,
      "tag": 0.9,
      "six_man": 0.7,
      "battle_royal": 0.3
    },
    "finish_expectations": {
      "clean": 0.7,
      "screwy": 0.1,
      "time_limit": 0.2
    }
  }
}
```
