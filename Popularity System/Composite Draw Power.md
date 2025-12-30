# Composite Draw Power

📛 **MECHANIC:** Composite Draw Power (Replaces Star Quality)
🔗 **PARENT SYSTEM:** [[Popularity_System]]
🧭 **CATEGORY:** Worker Evaluation / Business Impact
🔑 **KEYWORDS:** draw, star power, gates, merchandise, marketability, composite
📌 **ORIGIN:** Vol 1 Extraction #43
✅ **STATUS:** Concept (Half-Baked, needs formalization)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 📝 Concept |

---

## Overview

"Star Quality" as a single stat is insufficient. A worker's ability to draw money comes from multiple factors that combine differently depending on promotion context.

---

## User Critique (Locked)

> "Star Quality is a dog shit stat that really should be covered by momentum, one of the looks ratings (sex/menace), charisma, and promo ability."

The insight: Draw Power is **composite**, not singular.

---

## Proposed Formula

```
Draw Power = Momentum + Appearance Factor + Charisma + Promo Ability + Reputation
```

### Component Breakdown

| Component | Description |
|-----------|-------------|
| **Momentum** | Current booking trajectory (hot/cold) |
| **Appearance Factor** | Higher of Sex Appeal or Menace |
| **Charisma** | Natural magnetism |
| **Promo Ability** | Mic work effectiveness |
| **Reputation** | Long-term perception (overness baseline) |

---

## Context-Sensitive Weighting

Different promotions value components differently:

### Workrate-Focused Promotions

| Component | Weight |
|-----------|--------|
| Momentum | 25% |
| Appearance | 10% |
| Charisma | 15% |
| Promo | 10% |
| In-Ring Reputation | 40% |

### Sports Entertainment Promotions

| Component | Weight |
|-----------|--------|
| Momentum | 20% |
| Appearance | 25% |
| Charisma | 25% |
| Promo | 20% |
| Reputation | 10% |

### Traditional Territory

| Component | Weight |
|-----------|--------|
| Momentum | 20% |
| Appearance | 15% |
| Charisma | 20% |
| Promo | 15% |
| Reputation | 30% |

### Puroresu

| Component | Weight |
|-----------|--------|
| Momentum | 30% |
| Appearance | 10% |
| Charisma | 15% |
| Promo | 5% |
| Reputation | 40% |

---

## Draw Power Effects

| System | Effect |
|--------|--------|
| **Gate Revenue** | Higher draw = more tickets sold |
| **PPV Buys** | Main event draw affects total buys |
| **TV Ratings** | Advertised stars boost viewership |
| **Merchandise** | Draw affects merch sales (separate from character merch appeal) |
| **Contract Value** | Higher draw = higher salary demands |

---

## Calculating Match Draw

For tag/multi-person matches:

```
Match Draw = (Highest Draw × 0.6) + (Second Highest × 0.3) + (Others Average × 0.1)
```

For feuds:

```
Feud Draw = (Face Draw + Heel Draw) × Chemistry Modifier × Heat Multiplier
```

---

## Implementation Notes

```json
{
  "worker_id": "austin_1998",
  "draw_components": {
    "momentum": 95,
    "appearance_factor": 17,
    "charisma": 20,
    "promo_ability": 18,
    "reputation": 90
  },
  "context_draws": {
    "wwf_1998": 98,
    "wcw_1998": 85,
    "ecw_1998": 75,
    "njpw_1998": 60
  }
}
```

---

## Open Questions

- Should "match quality" factor into draw?
- How does international draw work (separate by region)?
- Draw decay rate when not featured?
- Can low draw workers become draws through booking?

---

## Related Mechanics

- [[Popularity_System]] - Overness/Reputation
- [[Booking_Engine_P1-3]] - Momentum tracking
- [[Worker_Skills]] - Charisma, Promo, Sex Appeal, Menace
- [[Buzz System/_Buzz System Index|Buzz System]] - Media amplification

---

**Document Status:** Concept (needs formalization)
**Last Updated:** 2024-12-23
