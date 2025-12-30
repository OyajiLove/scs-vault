# Chant Memory

📛 **MECHANIC:** Chant Memory
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** chant memory, chant persistence, weaponized chants, chant evolution, ritual chant
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

Chants can persist, evolve, and be weaponized. They're not just reactions; they're stored behaviors that the crowd remembers and can deploy strategically.

---

## Chant Storage Types

| Type | Description | Example |
|------|-------------|---------|
| **Stored Per Worker** | Auto-triggered by AI if conditions match | "Goldberg! Goldberg!" |
| **Region Locked** | Only used in certain regions | "This is awesome" (not in Japan) |
| **Era Locked** | Only used in certain time periods | "What?" (2000s+ US only) |
| **Reclaimed Over Time** | May return years after last appearance | Old catchphrase revival |
| **Weaponized by Crowd** | Used against booking intent | "We want [Other Worker]" |

---

## Chant Persistence

| Condition | Chant Behavior |
|-----------|----------------|
| **Worker active** | Chant regularly triggered |
| **Worker retired** | Chant fades unless [[Fan Memory Engine/_Fan Memory Index|memory]] strong |
| **Worker returns** | Chant instantly reactivates |
| **Long absence** | Chant may return distorted or nostalgic |

---

## Weaponized Chants

Fans can use chants to reject booking:

| Chant | Meaning |
|-------|---------|
| "We want [X]" | Reject current focus |
| "Boring!" | Reject match/segment |
| "[Worker] sucks!" | Reject push |
| Old gimmick name | Reject repackage |
| "You sold out!" | Reject face/company alignment |

---

## Chant Evolution

Chants can change over time:

| Evolution | Example |
|-----------|---------|
| **Tone shift** | Earnest → ironic |
| **Split chant** | "Let's go Cena / Cena sucks" |
| **Adoption by other worker** | Successor inherits chant |
| **Death/retirement** | Chant becomes tribute |

---

## Booker Response to Chants

| Response | Outcome |
|----------|---------|
| **Follow crowd will** | Give them what they want |
| **Ignore/override** | Risk push resistance |
| **Acknowledge in-story** | Worker references chants |
| **Punish crowd choice** | Book against fan favorite (nuclear heat) |

---

## Connected Mechanics

- [[Signal Types]] - chants are a signal type
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - chants tied to memory persistence
- [[Heat vs Hate]] - catchphrase adoption tracked as drift indicator
- [[Heel to Face Drift]] - weaponized chants can accelerate drift
- [[Region Era Profiles]] - determines chant availability

---

## Open Questions

- Chant inheritance mechanics (successor workers)
- Chant fatigue (overused chants lose power?)
- Cross-promotion chant transfer (AEW crowd chanting WWE catchphrase)

---

## Implementation Notes

```json
{
  "chant_record": {
    "chant_id": "ch_001",
    "text": "Goldberg! Goldberg!",
    "worker_id": "w_goldberg",
    "type": "ritual_chant",
    "region_lock": ["us_southeast", "us_northeast"],
    "era_lock": ["1997-2004", "2016-present"],
    "intensity": 18,
    "persistence": "high",
    "last_triggered": "show_nitro_1998_09_14",
    "weaponized": false,
    "evolution_history": [
      {"date": "1997-09-22", "state": "earnest"},
      {"date": "2003-03-30", "state": "nostalgic"}
    ]
  }
}
```
