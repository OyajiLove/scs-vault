# Stipulation Matches

📛 **MECHANIC:** Stipulation Matches
🔗 **PARENT SYSTEM:** [[_Match Types Index|Match Types & Era Flavor]]
🧭 **CATEGORY:** Match Simulation / Booking Context
🔑 **KEYWORDS:** stipulation, gimmick match, cage, ladder, no DQ, hardcore, street fight, hell in a cell
📌 **ORIGIN:** Vol 3
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 | 🔒 LOCKED |

---

## Overview

Stipulations are gimmick modifiers added to base [[Match Type Categories|match types]]. A cage match is a singles match with the cage stipulation. Stipulations raise stakes, provide blowoff options, and have era/regional availability.

---

## Stipulation Categories

| Category | Purpose | Risk Level |
|----------|---------|------------|
| **Enclosure** | Prevent escape/interference | Medium |
| **Weapons** | Enable brutality | High |
| **Career stakes** | Maximum consequences | Maximum |
| **Special rules** | Change win conditions | Varies |
| **Time-based** | Test endurance | Medium |

---

## Enclosure Stipulations

| Stipulation | Description | Era Availability |
|-------------|-------------|------------------|
| **Steel Cage** | Escape or pin to win | All eras |
| **Hell in a Cell** | Larger cage, no escape | 1998+ |
| **Elimination Chamber** | Pods, timed releases | 2002+ |
| **WarGames** | Two rings, dual cages | 1987-2000, 2017+ |
| **Shark Cage** | Suspend manager above ring | Territory era |

---

## Weapons Stipulations

| Stipulation | Description | Era Availability |
|-------------|-------------|------------------|
| **No DQ** | Anything legal | All eras |
| **Street Fight** | Falls count anywhere, no DQ | All eras |
| **Hardcore** | Weapons encouraged | 1990s+ |
| **Tables Match** | Win by putting opponent through table | 1998+ |
| **Ladder Match** | Retrieve object above ring | 1992+ |
| **TLC** | Tables, ladders, chairs | 2000+ |
| **Barbed Wire** | Ring ropes replaced | Japan 1990s+, rare elsewhere |
| **Exploding Ring** | Pyro on ropes/corners | Japan, ultra-rare |

### Weapon Mechanics (#122)

📌 **Source:** Vol 1 Extraction #122

| Type | Effects |
|------|--------|
| **Tables** | Bump risk, visual drama, can end match |
| **Ladders** | High injury risk, spot potential, ladder climb drama |
| **Chairs** | Strike damage, heat, relatively safe |
| **Cage** | No interference, climb/escape finishes, blood |
| **Hell in Cell** | Maximum carnage, career-defining potential |
| **Barbed Wire** | Extreme damage, deathmatch credibility required |

### Worker Comfort Tags

| Tag | Effect |
|-----|--------|
| **Hardcore Specialist** | Bonus in weapon matches |
| **Deathmatch Sicko** | Massive bonus in extreme matches |
| **Clean Worker** | Penalty in weapon matches, prefers pure wrestling |

---

## Career Stakes Stipulations

| Stipulation | Description | Cultural Weight |
|-------------|-------------|-----------------|
| **Loser Leaves Town** | Loser must leave promotion | High |
| **Career vs Career** | Loser retires | Maximum |
| **Hair vs Hair** | Loser gets head shaved | High (cultural humiliation) |
| **Mask vs Mask** | Loser unmasks permanently | Sacred (lucha) |
| **Mask vs Hair** | Cross-stakes lucha variant | Sacred |
| **Title vs Career** | Champion risks career for shot | Maximum |

---

## Special Rules Stipulations

| Stipulation | Rule Change |
|-------------|-------------|
| **Submission Only** | No pins, must tap/pass out |
| **First Blood** | First to bleed loses |
| **I Quit** | Must verbally surrender |
| **Last Man Standing** | 10-count after knockdown |
| **Buried Alive** | Cover opponent in grave |
| **Inferno** | Set opponent on fire |
| **Kennel from Hell** | Cage + dogs (please don't) |

---

## Time-Based Stipulations

| Stipulation | Description |
|-------------|-------------|
| **Ironman** | Most falls in time limit |
| **30/60 Minute Draw** | Time limit emphasized |
| **Ultimate Submission** | Most submissions in time limit |

---

## Era Availability Matrix

| Stipulation | 1970s | 1980s | 1990s | 2000s | 2010s+ |
|-------------|-------|-------|-------|-------|--------|
| Steel Cage | ✓ | ✓ | ✓ | ✓ | ✓ |
| Ladder | - | - | ✓ | ✓ | ✓ |
| Hell in a Cell | - | - | ✓ | ✓ | ✓ |
| TLC | - | - | - | ✓ | ✓ |
| Mask vs Mask | ✓ | ✓ | ✓ | ✓ | ✓ |
| Barbed Wire | - | ✓ | ✓ | ✓ | ✓ |

**Note:** Full matrix TBD in implementation.

---

## Stipulation Selection Guidelines

| Consideration | Guidance |
|---------------|----------|
| **Feud intensity** | Higher stakes = bigger stipulation |
| **Worker skills** | Don't book ladder match with non-flyers |
| **Blowoff timing** | Save big stipulations for feud end |
| **Recent usage** | Overuse diminishes impact |
| **Era appropriateness** | Don't book 2020s stipulation in 1980s |

---

## Stakes and Stipulations

From [[Predictability_Stakes|Predictability & Stakes]]:

| Stakes Type | Multiplier |
|-------------|------------|
| Mask vs Mask | 3.5x |
| Career vs Career | 3.0x |
| Loser Leaves Town | 2.5x |
| Hair vs Hair | 2.0x |
| Cage/Cell | 1.5x |
| No DQ | 1.2x |

---

## Connected Mechanics

- [[Match Type Categories]] - stipulations modify base types
- [[Predictability_Stakes|Predictability & Stakes]] - stipulation affects stakes weight
- [[Era Booking Profiles]] - era determines availability
- [[Match Quality Factors]] - stipulation sets expectations

---

## Open Questions

- Complete era/region availability matrix
- Stipulation fatigue mechanics (overuse penalty)
- Custom stipulation creation rules

---

## Implementation Notes

```json
{
  "stipulation": {
    "stip_id": "stip_cage",
    "name": "Steel Cage",
    "category": "enclosure",
    "win_conditions": ["escape", "pin", "submission"],
    "stakes_multiplier": 1.5,
    "risk_level": "medium",
    "era_availability": {
      "1970s": true,
      "1980s": true,
      "1990s": true,
      "2000s": true,
      "2010s": true
    },
    "region_popularity": {
      "us": "high",
      "japan": "medium",
      "mexico": "low"
    },
    "worker_requirements": {
      "min_stamina": 12,
      "recommended_tags": ["brawler", "veteran"]
    }
  }
}
```
