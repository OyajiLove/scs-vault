# Iconic Lock Decay

📛 **MECHANIC:** Iconic Lock Decay
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** iconic decay, lock erosion, legacy fade, overexposure
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Volume | Changes |
|---------|--------|--------|
| v1.0 | Vol 6 | **LOCKED** - Decay triggers defined (overexposure, bad booking, cultural irrelevance, scandal, diminished performance). Speed modifiers and response options specified. Hulkamania case study provided as canonical example |

**Note:** This mechanic was introduced alongside Iconic Lock in Vol 6 as a balancing mechanism. No earlier version exists.

---

## Overview

Even [[Iconic Lock|Iconic Locks]] aren't truly permanent. Sustained misuse, overexposure, or cultural shifts can erode protected status. The lock doesn't break suddenly; it decays over time.

---

## Decay Triggers

| Trigger | Effect |
|---------|--------|
| **Overexposure** | Too many returns dilute nostalgia pop |
| **Bad booking** | Embarrassing losses, burial by lesser workers |
| **Cultural irrelevance** | Audience generational shift, gimmick feels dated |
| **Real-world scandal** | Out-of-character behavior damages perception |
| **Diminished performance** | Ring work no longer matches legend status |

---

## Hulkamania Case Study (1984-1996)

| Period | Status | Notes |
|--------|--------|-------|
| 1984-1988 | **Peak Lock** | Untouchable, mainstream icon |
| 1989-1991 | **Stable Lock** | Still protected, slight staleness |
| 1992-1993 | **Decay Beginning** | Steroid trial, cultural shift to edgier content |
| 1994-1995 | **Accelerated Decay** | WCW move, crowds cooling |
| 1996 | **Lock Broken → Rebuilt** | nWo heel turn creates NEW lock (Hollywood Hogan) |

Key insight: The heel turn didn't just save the gimmick; it created an entirely new Iconic Lock.

---

## Detailed Hulkamania Decay Triggers (Vol 6)

| Trigger | Example | Effect |
|---------|---------|--------|
| **Cultural Turn** | Early 90s fans shift to edgy realism (Bret, Shawn, ECW) | Legacy stays, buzz plummets |
| **Style Disconnect** | Hogan's WWF routine didn't match WCW in-ring trends | Booking memory devalues current matches |
| **Promotion Repetition** | Same catchphrases, posing, no evolution | AI fans begin tagging segments as "stale" |
| **Mismatch Booking** | Feuds with Dungeon of Doom, no emotional stakes | Fan Memory doesn't refresh, no new fuel |
| **Workrate Gap** | Surrounded by Pillman, Benoit, Eddy, Savage | Buzz cap lowers in workrate-heavy environments |
| **Fan Rejection** | Havoc '95 (booed out of building), steroids whispers | Pop begins active decline, crowd betrayal triggers |

---

## Simulation Response to Decay

As triggers pile up:
- Buzz begins decaying even while Pop stays high
- Fan chants turn ironic or hostile
- AI bookers split:
  - **Traditionalists** double down ("We owe him...")
  - **Chaos bookers** experiment (heel turn, torch pass)
- Locker room heat begins building

---

## Decay Speed Modifiers

| Factor | Decay Speed |
|--------|-------------|
| Active wrestling (good booking) | Very slow |
| Active wrestling (bad booking) | Moderate |
| Retired but occasional returns | Slow |
| Retired, no appearances | Minimal (nostalgia preserved) |
| Scandal/controversy | Fast |
| Death | Decay stops (legacy frozen) |

---

## Response Options

| Option | When to Use |
|--------|-------------|
| **Reduce appearances** | Overexposure decay |
| **Quality over quantity** | Performance decay |
| **Reinvention** | Cultural irrelevance decay |
| **Retirement** | Preserve what remains |
| **Heel turn** | Nuclear option, high risk/reward |

---

## Connected Mechanics

- [[Iconic Lock]] - what's being eroded
- [[Lock Break System]] - when decay becomes catastrophic
- [[Gimmick Lifecycle]] - decay can push to Stagnation/Burnout
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - decay affects how gimmick is remembered

---

## Open Questions

- Decay rate formula (% per appearance? per month?)
- Recovery mechanics (can decay be reversed?)
- Regional decay variation

---

## Implementation Notes

```json
{
  "gimmick_id": "gim_001",
  "iconic_lock": {
    "status": "decaying",
    "lock_strength": 72,
    "peak_strength": 95,
    "decay_rate": 0.5,
    "decay_triggers_active": ["overexposure", "diminished_performance"],
    "months_decaying": 18
  }
}
```
