# Legend Status Effects

📛 **MECHANIC:** Ongoing Effects of HOF Induction
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy
🔑 **KEYWORDS:** legend, return pop, legend morale, nostalgia, booking
📌 **ORIGIN:** Vol 1-4 (Legend Morale, Return boosts, Sustained Legacy)
✅ **STATUS:** Locked

---

## Overview

Hall of Fame induction isn't just an endpoint: it creates ongoing effects that influence how legends interact with the game world. HOF inductees get return pop boosts, special booking opportunities, enhanced memory effects, and ongoing morale considerations. Legends retain popularity even after retirement.

---

## Return Pop Bonuses

HOF inductees get amplified pops when returning:

| Legend Tier | Base Pop Bonus |
|-------------|----------------|
| **All-Time Great** | +75% to +100% |
| **Legend** | +50% to +75% |
| **Star** | +30% to +50% |
| **Solid** | +15% to +30% |

### Modifiers to Return Pop

| Factor | Effect |
|--------|--------|
| **Time since last appearance** | Longer = bigger pop |
| **Surprise return** | +25% to +50% |
| **Announced return** | Baseline |
| **Meaningful story** | +20% |
| **Dream match context** | +30% |
| **Home territory** | +15% |

---

## Legend Morale

Post-induction emotional state:

| Morale Level | Description |
|--------------|-------------|
| **Honored** | Feels respected, cooperative |
| **Content** | Satisfied with legacy |
| **Restless** | Wants more involvement |
| **Bitter** | Feels underutilized |
| **Forgotten** | Ignored post-induction |

### What Affects Legend Morale

| Factor | Effect |
|--------|--------|
| **Used for returns** | +15 to +25 |
| **Ignored post-HOF** | -10 per year |
| **Legacy acknowledged** | +10 |
| **Feuds with current stars** | +20 |
| **Disrespected by booking** | -20 |
| **Young stars pay tribute** | +15 |
| **Documentary/retrospective** | +10 |

---

## Booking Opportunities

Exclusive to HOF inductees:

| Opportunity | Description |
|-------------|-------------|
| **HOF Segment** | Induction ceremony booking |
| **Legend vs. Legend** | Dream match possibilities |
| **Torch Passing** | Put over rising star |
| **Authority Figure** | GM, commissioner role |
| **Special Enforcer** | Big match addition |
| **Nostalgia Run** | Limited return program |
| **Cameo Appearances** | One-off surprises |
| **Commentary** | Announce team guest |

---

## Memory Effects

HOF status enhances memory anchors:

| Effect | Description |
|--------|-------------|
| **Permanent Recognition** | Name never forgotten |
| **Match Memory Boost** | Past matches remembered stronger |
| **Feud Memory Boost** | Rivalries become legendary |
| **Catchphrase Immortality** | Lines become permanent |
| **Tribute Matches** | Future workers reference style |

---

## Merchandise and Value

| Factor | Effect |
|--------|--------|
| **Nostalgia Merch** | Retro items sell |
| **Appearance Fees** | Command premium |
| **Promotional Value** | PR asset for company |
| **Cross-Promotion Draw** | Other companies want them |
| **Media Opportunities** | Interviews, documentaries |

---

## Legend Contracts

Special contract types for HOF inductees:

| Contract Type | Description |
|---------------|-------------|
| **Legends Contract** | Minimal dates, high per-appearance |
| **Ambassador Role** | PR duties, minimal wrestling |
| **Part-Time Legend** | Sporadic appearances |
| **One-Night-Only** | Single appearance deals |
| **Commentary Deal** | Announce team role |
| **Training Role** | Development involvement |

---

## Negative Possibilities

HOF status doesn't prevent problems:

| Issue | Effect |
|-------|--------|
| **Post-HOF scandal** | Damages legacy score |
| **Poor return match** | Tarnishes memory |
| **Overstaying welcome** | Diminishing returns |
| **Bitter public comments** | Damages relationship |
| **Health decline visible** | Uncomfortable |

---

## Historical Examples

| Legend | Post-HOF Status | Notes |
|--------|-----------------|-------|
| **Ric Flair** | Highly active | Continued appearing, managing |
| **Shawn Michaels** | Respected elder | NXT involvement |
| **Undertaker** | Limited appearances | Protects mystique |
| **Hulk Hogan** | Controversial | Multiple returns, scandal issues |
| **Bret Hart** | Reconciled | Returned after long absence |

---

## Era Differences

| Era | Legend Treatment |
|-----|------------------|
| **Territory** | Legends kept wrestling |
| **80s National** | Some HOF concept emerging |
| **Attitude Era** | Legends used for pops |
| **Modern** | Formal HOF, nostalgia booking |

---

## Connected Mechanics

- [[Comeback Mechanics]] - Return dynamics for legends
- [[Legacy Score]] - Determines legend tier
- [[Contract System]] - Legend contract types
- [[Crowd Memory]] - Enhanced memory effects

---

## Open Questions

- [ ] How legend morale affects willingness to appear
- [ ] Multi-promotion legend handling
- [ ] Legend vs. legend booking priority
- [ ] How death affects legend status
- [ ] Legend involvement in storylines

---

## Implementation Notes

```json
{
  "legend_status": {
    "worker_id": "worker_001",
    "hof_inducted": true,
    "legend_tier": "legend",
    "legend_morale": 78,
    "return_pop_bonus": 1.55,
    "last_appearance": "1994-06-15",
    "current_contract": "legends_contract",
    "booking_opportunities": ["authority_figure", "special_enforcer", "torch_passing"],
    "merch_value": "high",
    "media_value": "very_high",
    "health_status": "limited",
    "availability": "occasional"
  }
}
```
