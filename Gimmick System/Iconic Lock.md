# Iconic Lock

📛 **MECHANIC:** Iconic Lock
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** iconic lock, perma-over, protected gimmick, legendary status
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 1-4 | "Perma-over" concept discussed for legendary characters; no formal trigger system |
| v2.0 | Vol 6 | **LOCKED** - Iconic Lock formalized with trigger conditions (Legacy 80+, Buzz 15+ sustained, cultural penetration). Decay immunity, booking protection, and memory permanence effects specified |

---

## Overview

When a gimmick achieves such cultural penetration that it becomes permanently protected from normal decay mechanics. The character is "locked in" to the cultural consciousness.

---

## Trigger Conditions

A gimmick achieves Iconic Lock when:

| Condition | Threshold |
|-----------|-----------|
| [[Legacy Tracker/_Legacy Tracker Index|Legacy Score]] | 80+ |
| Sustained [[Buzz Scale|Buzz]] | 15+ for 6+ months |
| Cultural Penetration | Referenced outside wrestling context |
| Cross-generational | Recognized by non-fans |

All conditions must be met. Partial achievement = "Near-Iconic" status.

---

## Iconic Lock Effects

| Effect | Description |
|--------|-------------|
| **Decay immunity** | [[Buzz Decay]] no longer applies normally |
| **Return pop guaranteed** | Any return generates automatic Buzz spike |
| **Booking protection** | AI bookers won't bury the character |
| **Memory permanence** | [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] never fully forgets |
| **Merch immortality** | Continues selling even during absence |
| **Legacy ceiling raised** | Can reach [[Cultural Immortality]] tier |

---

## Real-World Examples

| Gimmick | Lock Trigger | Era |
|---------|--------------|-----|
| **Hulkamania** | WrestleMania III, cultural phenomenon | Mid-80s |
| **Stone Cold** | Austin 3:16, beer truck, Mr. McMahon feud | Late 90s |
| **The Undertaker** | Streak, supernatural mystique | Early 90s |
| **John Cena** | Make-A-Wish, mainstream crossover | Mid-2000s |
| **Great Muta** | International icon, green mist, paint | Late 80s Japan |

---

## Near-Iconic Status

Workers who approach but don't fully achieve lock:

- High legacy but limited cultural penetration
- Iconic within wrestling, unknown outside
- Regional icons (huge in Japan, unknown in US)

Near-Iconic workers:
- Get partial decay protection
- Can achieve full lock with right booking
- Risk falling back without maintenance

---

## Connected Mechanics

- [[Iconic Lock Decay]] - even locked gimmicks can fade
- [[Lock Break System]] - catastrophic events that shatter locks
- [[Cultural Immortality]] - tier above Iconic Lock
- [[Legacy Tracker/_Legacy Tracker Index|Legacy Tracker]] - feeds into lock calculation

---

## Open Questions

- Exact formula for lock calculation
- Regional Iconic Lock (locked in Japan but not US)?
- Tag team Iconic Lock (Road Warriors, Dudleys)?

---

## Implementation Notes

```json
{
  "gimmick_id": "gim_001",
  "iconic_lock": {
    "status": "locked",
    "lock_date": "1987-03-29",
    "trigger_event": "wrestlemania_iii",
    "legacy_at_lock": 85,
    "decay_immunity": true,
    "cultural_penetration": "mainstream",
    "near_iconic_history": [
      {"date": "1985-01-01", "status": "near_iconic"}
    ]
  }
}
```
