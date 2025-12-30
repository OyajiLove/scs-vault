# Legacy Uses

📛 **MECHANIC:** Legacy Uses
🔗 **PARENT SYSTEM:** [[_Legacy Tracker Index|Legacy Tracker]]
🧭 **CATEGORY:** Career & Recognition
🔑 **KEYWORDS:** legacy applications, HOF, booking value, return pop
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

How Legacy Score affects other game systems. Legacy isn't just a number; it unlocks privileges, affects booking, and determines post-career options.

---

## Hall of Fame Integration

| Legacy Score | HOF Status |
|--------------|------------|
| 50+ | Veteran's Committee eligible |
| 65+ | Standard ballot eligible |
| 85+ | First Ballot lock |
| 90+ | Headliner/Main Event induction |

See [[Hall of Fame/_Hall of Fame Index|Hall of Fame System]] for full details.

---

## Booking Value

| Legacy Tier | Effect |
|-------------|--------|
| Legendary (80+) | Premium appearance fee, automatic main event |
| Notable (60-79) | Enhanced return pop, credibility transfer |
| Solid (40-59) | Standard legend treatment |
| Journeyman (20-39) | Nostalgia act, limited value |
| Forgettable (<20) | No legend privileges |

---

## Return Pop Calculation

When a retired/semi-retired worker returns:

```
Return Pop = Base Pop + (Legacy Score × 0.3) + Absence Modifier
```

High Legacy = bigger return pops, regardless of how long they've been gone.

---

## Credibility Transfer

Feuding with or losing to high-Legacy workers transfers credibility:

| Action | Credibility Transfer |
|--------|---------------------|
| Clean win over legend | +5 to +10 [[Buzz Scale\|Buzz]] |
| Competitive loss to legend | +2 to +3 Buzz |
| Being chosen by legend | +3 to +5 Buzz |
| Legend endorsement | +3 to +5 Buzz |

---

## Retirement Arc Options

Legacy unlocks retirement storyline options:

| Legacy Score | Available Arcs |
|--------------|----------------|
| 80+ | Grand farewell tour, choose opponent |
| 60-79 | Retirement match, ceremony |
| 40-59 | Quiet exit, possible one-off return |
| <40 | No special treatment |

---

## Post-Career Roles

| Legacy Score | Available Roles |
|--------------|-----------------|
| 70+ | On-screen authority figure |
| 60+ | Commentary, manager |
| 50+ | Trainer, backstage agent |
| 40+ | Occasional cameos |
| <40 | Limited to fan events |

---

## Connected Mechanics

- [[Legacy Scale]] - the score driving these uses
- [[Hall of Fame/_Hall of Fame Index|Hall of Fame]] - primary Legacy use
- [[Buzz System/_Buzz System Index|Buzz System]] - return pop calculations
- [[Immortal Feud Templates]] - high Legacy booking patterns

---

## Open Questions

- Legacy licensing (using name/likeness after retirement)
- Legacy inheritance (passing the torch mechanically)
- Negative Legacy uses (cautionary tales, "what not to do")

---

## Implementation Notes

```json
{
  "legacy_uses": {
    "worker_id": "w_001",
    "legacy_score": 82,
    "unlocked_privileges": {
      "hof_eligible": true,
      "hof_tier": "first_ballot",
      "booking_tier": "legendary",
      "return_pop_bonus": 24.6,
      "retirement_arcs": ["grand_farewell", "choose_opponent"],
      "post_career_roles": ["authority_figure", "commentary", "trainer"]
    }
  }
}
```
