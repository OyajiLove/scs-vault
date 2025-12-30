# Legacy Modifiers

📛 **MECHANIC:** Legacy Modifiers
🔗 **PARENT SYSTEM:** [[_Legacy Tracker Index|Legacy Tracker]]
🧭 **CATEGORY:** Career & Recognition
🔑 **KEYWORDS:** legacy modifiers, growth rate, era factors, promotion prestige
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

Factors that affect how quickly Legacy accumulates. The same achievement in different contexts yields different Legacy gains.

---

## Promotion Prestige Modifier

| Promotion Tier | Modifier |
|----------------|----------|
| Global (WWE, NJPW) | 1.5x |
| Major (AEW, NOAH) | 1.25x |
| Regional (NWA territories) | 1.0x |
| Indie (ROH, PWG) | 0.75x |
| Local | 0.5x |

Achievements in bigger promotions build more Legacy.

---

## Era Modifier

| Era | Modifier | Notes |
|-----|----------|-------|
| Territory Era | 1.0x | Baseline |
| National Expansion | 1.25x | Larger audiences |
| Attitude Era | 1.5x | Cultural peak |
| Modern Era | 1.25x | Global but fragmented |
| Streaming Era | 1.0x | Diluted attention |

Peak cultural moments in wrestling history amplify Legacy building.

---

## Role Modifier

| Role | Modifier |
|------|----------|
| World Champion | 1.5x |
| Main Eventer | 1.25x |
| Upper Midcard | 1.0x |
| Midcard | 0.75x |
| Enhancement | 0.5x |

Card position affects how much Legacy events generate.

---

## Negative Modifiers

| Event | Effect |
|-------|--------|
| Scandal | -10 to -30 Legacy |
| Criminal conviction | -20 to -50 Legacy |
| Unprofessional behavior | -5 to -15 Legacy |
| Backstage politics (exposed) | -5 to -10 Legacy |
| Public meltdown | -10 to -20 Legacy |

Negative events are rare but devastating to Legacy.

---

## Recovery Modifiers

| Factor | Effect |
|--------|--------|
| Time passed | Negative impact fades (slowly) |
| Redemption arc | Can rebuild some lost Legacy |
| Death | Legacy often frozen at last good point |
| Selective memory | Fans focus on peak, ignore fall |

---

## Connected Mechanics

- [[Legacy Builders]] - what's being modified
- [[Legacy Scale]] - the score being affected
- [[Gimmick System/Lock Break System|Lock Break]] - major negative modifiers

---

## Open Questions

- Exact modifier stacking rules
- Regional Legacy variation modifiers
- Posthumous modifier changes

---

## Implementation Notes

```json
{
  "legacy_calculation": {
    "worker_id": "w_001",
    "event": "world_title_win",
    "base_gain": 8,
    "modifiers": {
      "promotion_prestige": 1.5,
      "era": 1.25,
      "role": 1.5
    },
    "modifier_product": 2.81,
    "final_gain": 22.5,
    "capped_gain": 20
  }
}
```
