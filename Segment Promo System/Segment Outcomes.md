# Segment Outcomes

📛 **MECHANIC:** Segment Outcomes
🔗 **PARENT SYSTEM:** [[_Segment Promo Index|Segment & Promo System]]
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** segment outcomes, buzz change, feud memory, morale, promo success, promo failure
📌 **ORIGIN:** Vol 2-3 (Booking Engine Phase 3)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2-3 | 🔒 LOCKED |

---

## Overview

What happens after a segment completes. Outcomes affect [[Buzz System/_Buzz System Index|Buzz]], [[Feud_Memory|Feud Memory]], worker morale, and crowd investment. Good segments build momentum; bad segments damage it.

---

## Outcome Categories

| Outcome | Description | Frequency |
|---------|-------------|-----------|
| **Promo Kills** | Career-defining, iconic | Rare |
| **Great Segment** | Highly effective | Uncommon |
| **Solid Segment** | Advances story, works | Common |
| **Weak Segment** | Crowd disengaged | Common |
| **Bombed Segment** | Active rejection | Uncommon |
| **Derailed Segment** | Crowd hijacked | Variable |

---

## Buzz Effects

| Outcome | Buzz Change | Duration |
|---------|-------------|----------|
| **Promo Kills** | +15 to +25 | Sustained (weeks) |
| **Great Segment** | +8 to +15 | Moderate (1-2 weeks) |
| **Solid Segment** | +3 to +7 | Short (days) |
| **Weak Segment** | 0 to -3 | Immediate |
| **Bombed Segment** | -5 to -15 | Moderate (1-2 weeks) |
| **Derailed Segment** | -10 to -20 | Sustained (depends on recovery) |

---

## Feud Memory Effects

| Outcome | Memory Impact |
|---------|---------------|
| **Promo Kills** | Permanent memory anchor created |
| **Great Segment** | Long-term memory entry |
| **Solid Segment** | Medium-term memory entry |
| **Weak Segment** | Quickly forgotten |
| **Bombed Segment** | Negative memory entry |
| **Derailed Segment** | Meta-memory ("that time crowd hijacked") |

---

## Morale Effects

| Outcome | Worker Morale | Others' Morale |
|---------|---------------|----------------|
| **Promo Kills** | Major boost | Positive (inspiration) |
| **Great Segment** | Boost | Neutral/Positive |
| **Solid Segment** | Minor boost | Neutral |
| **Weak Segment** | Minor hit | Neutral |
| **Bombed Segment** | Major hit | Potential schadenfreude (rivals) |
| **Derailed Segment** | Significant hit | Sympathy or distance |

---

## Crowd Investment Effects

| Outcome | Investment Change |
|---------|-------------------|
| **Promo Kills** | Major increase in workers involved |
| **Great Segment** | Moderate increase |
| **Solid Segment** | Maintains current level |
| **Weak Segment** | Minor decrease |
| **Bombed Segment** | Significant decrease |
| **Derailed Segment** | Complex (may increase meta-investment) |

---

## Feud Advancement

| Outcome | Story Progress |
|---------|----------------|
| **Promo Kills** | Major escalation, new feud phase |
| **Great Segment** | Clear advancement |
| **Solid Segment** | Incremental progress |
| **Weak Segment** | Stalled |
| **Bombed Segment** | May damage feud credibility |
| **Derailed Segment** | Forced pivot may be needed |

---

## Secondary Effects

| Effect | Trigger |
|--------|---------|
| **Catchphrase created** | Quotable line lands |
| **New [[Crowd Signals/Chant Memory\|chant]] born** | Crowd adopts line |
| **[[Turn_Engine\|Turn]] foreshadowed** | Tension planted |
| **[[Booking Trails/_Booking Trails Index\|Trail]] milestone hit** | Planned beat achieved |
| **Heat transferred** | One worker gets other's heat |
| **Viral moment** | Modern era, social media buzz |

---

## Segment Chain Effects

When multiple segments form a story across a show:

| Chain Quality | Effect |
|---------------|--------|
| **Building properly** | Each segment amplifies next |
| **Flat chain** | No escalation, energy dissipates |
| **Contradictory chain** | Confuses crowd, damages story |
| **Payoff chain** | Final segment gets cumulative boost |

---

## Connected Mechanics

- [[Buzz System/_Buzz System Index|Buzz System]] - primary output
- [[Feud_Memory|Feud Memory]] - memory creation
- [[Promo Evaluation]] - determines outcome tier
- [[Promo Response]] - crowd response feeds outcome
- [[Emotional_Show_Flow|Emotional Show Flow]] - segment emotional tags

---

## Open Questions

- Exact Buzz change formulas
- Long-term career effects of repeated bombs
- Viral moment mechanics in modern era

---

## Implementation Notes

```json
{
  "segment_outcome": {
    "segment_id": "seg_001",
    "outcome_tier": "great_segment",
    "effects": {
      "buzz_change": {
        "w_001": 12,
        "w_002": 8
      },
      "feud_memory": {
        "feud_id": "fd_001",
        "memory_added": true,
        "memory_intensity": "high"
      },
      "morale_change": {
        "w_001": 5,
        "w_002": 3
      },
      "catchphrase_created": false,
      "trail_milestone_hit": true
    },
    "crowd_investment_after": 72
  }
}
```
