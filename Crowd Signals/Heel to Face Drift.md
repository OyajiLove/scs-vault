# Heel to Face Drift

📛 **MECHANIC:** Heel to Face Drift
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** heel drift, face drift, organic turn, crowd chemistry, double turn, alignment shift
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

When crowd chemistry turns villains into heroes without consent. Even if booking stays heel, crowd may turn the character face on their own. This mechanic tracks the organic erosion of heel status.

---

## Drift Detection Triggers

| Trigger | Effect |
|---------|--------|
| **Promo Sympathy Moment** | Heel shows trauma/truth; crowd connects |
| **Workrate Respect Spike** | Banger match triggers "That was awesome" chants |
| **Catchphrase Infection** | Fans adopt heel's insults with joy |
| **Babyface Shortage** | Fans latch onto heel because no viable faces |
| **Hero Targeting Fatigue** | Crowd turns when heel keeps burying beloved workers |
| **[[Fan Memory Engine/_Fan Memory Index|Legacy Memory]] Activation** | Heel reminds fans of respected older version |
| **Push Resistance Flip** | Face too corporate; heel becomes "realer" |

---

## Drift Phases

| Phase | Crowd Behavior |
|-------|----------------|
| **Denial** | Booed, but name chanted between matches |
| **Confusion** | "Let's go X / X sucks" splits |
| **Acceptance** | Full cheers in hot markets |
| **Reframing** | Commentary softens: "Love him or hate him..." |
| **Full Flip** | Double turn or face promo arc begins |

---

## Drift Rate Modifiers

| Modifier | Effect |
|----------|--------|
| **Era + Region** | Modern US/UK = likely; 80s NWA = less |
| **Fan Culture Index** | Smark-heavy = flip faster; Traditionalist = resist |
| **AI Booker Personality** | Chaos/Smark = embrace; Traditionalist = resist/bury |
| **Worker Morality/Drive** | High Morality = easier flip; high Ego = may resist |
| **[[Buzz System/_Buzz System Index|Buzz]] vs [[Popularity_System|Pop]] Gap** | If misaligned, drift risk rises |
| **Recent Snapshots** | If [[Fan Memory Engine/Memory Snapshots|Memory Moment]] landed emotionally, fans may reframe |

---

## Drift Response Options

| Option | Effect |
|--------|--------|
| **Lean Into It** | Shift promos/segments, slow-burn turn |
| **Snap Turn** | Face promo, big save, double turn at PPV |
| **Double Down on Heat** | Goes nuclear (attacks fan fave in home city) |
| **Ignore Crowd** | Push resistance risk grows, chants escalate |
| **Promo Gaslight** | Heel claims still hated even as cheers ring out |

---

## Integration Points

- May trigger [[Gimmick System/_Gimmick System Index|Gimmick]] evolution (not full change)
- Creates [[Fan Memory Engine/Memory Snapshots|Memory Snapshots]] during drift-triggered segments
- [[Push Resistance]] affected by drifted heels stealing support
- Commentary switches tone: "This isn't the man we saw a year ago..."
- [[Booking Trails/_Booking Trails Index|Booking Trails]] may fracture, start new Redemption/Reframing Arc

---

## Connected Mechanics

- [[Heat vs Hate]] - drift happens when Heat exists without Hate
- [[Region Era Profiles]] - drift susceptibility varies by region/era
- [[Turn_Engine|Turn Engine]] - processes alignment changes when drift completes
- [[Chant Memory]] - tracks catchphrase adoption that accelerates drift

---

## Open Questions

- Exact phase transition thresholds
- Can drift be fully reversed without a turn?
- Face to Heel Drift (reverse mechanic, less common)

---

## Implementation Notes

```json
{
  "drift_tracking": {
    "worker_id": "w_001",
    "current_alignment": "heel",
    "drift_phase": "confusion",
    "drift_rate": 0.08,
    "weeks_in_phase": 6,
    "triggers_active": ["workrate_respect", "babyface_shortage"],
    "response_selected": "lean_into_it",
    "projected_full_flip": "12_weeks"
  }
}
```
