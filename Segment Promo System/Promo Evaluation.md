# Promo Evaluation

📛 **MECHANIC:** Promo Evaluation
🔗 **PARENT SYSTEM:** [[_Segment Promo Index|Segment & Promo System]]
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** promo quality, mic skills, character work, believability, catchphrase, heat generation
📌 **ORIGIN:** Vol 2-3 (Booking Engine Phase 3)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2-3 | 🔒 LOCKED |

---

## Overview

What makes a promo succeed or fail. Promo quality is a function of worker skills, booking context, and crowd response. Great promos create memory anchors; bad promos damage momentum.

---

## Promo Evaluation Factors

| Factor | Weight | Description |
|--------|--------|-------------|
| **Mic Skills** | High | Worker's verbal ability, delivery, timing |
| **Character Work** | High | Staying in gimmick, facial expressions, personality |
| **Crowd Response** | High | Heat generation, engagement level |
| **Believability** | Medium | Does it feel real? Authentic emotion? |
| **Advancement** | Medium | Does it move story forward? |
| **Catchphrase/Moment** | Medium | Quotability, potential viral moment |

---

## Worker Skills Impact

From [[Worker_Skills|Worker Skills]]:

| Skill | Promo Impact |
|-------|--------------|
| **Mic Skills/Promos** | Direct multiplier on promo quality |
| **Character Work** | Determines gimmick consistency |
| **Crowd Connection** | Affects live response regardless of content |
| **Entrance/Presentation** | Pre-promo aura affects reception |

---

## Promo Quality Tiers

| Tier | Description | Effect |
|------|-------------|--------|
| **Promo Kills** | Iconic, career-defining | Massive Buzz spike, memory anchor created |
| **Great Promo** | Highly effective, memorable | Strong Buzz boost, advances feud significantly |
| **Solid Promo** | Advances story, maintains interest | Modest Buzz, story progression |
| **Weak Promo** | Crowd loses interest | Momentum stalls, no advancement |
| **Bombed Promo** | Crowd turns on speaker | Negative Buzz, damages worker |
| **Derailed Promo** | Crowd hijacks segment | See [[Promo Response]] for recovery |

---

## Context Modifiers

| Context | Effect |
|---------|--------|
| **Hot crowd** | Easier to succeed, reactions amplified |
| **Dead crowd** | Harder to succeed, reactions muted |
| **Post-hot match** | Energy carries over |
| **Cold open** | Must generate own heat |
| **Heel city** | Face promos harder, heel promos easier |
| **Hometown** | Automatic sympathy/heat bonus |

---

## Believability Factors

| Factor | Effect on Believability |
|--------|-------------------------|
| **Emotion matches stakes** | High if proportional |
| **Worker history supports claims** | High if consistent |
| **Shoot elements** | Risky but can boost if done right |
| **Over-scripted feel** | Reduces believability |
| **Genuine emotion bleeding through** | Major boost |

---

## Catchphrase/Moment Creation

Conditions for quotable moment:

| Condition | Likelihood |
|-----------|------------|
| **Simple, punchy line** | High |
| **Crowd can repeat it** | High |
| **Tied to character identity** | High |
| **Organic delivery** | Medium-High |
| **Forced insertion** | Low |
| **Overly complex** | Very Low |

Catchphrases that land become [[Crowd Signals/Chant Memory|Chant Memory]] entries.

---

## Promo Archetypes

| Archetype | Strengths | Weaknesses |
|-----------|-----------|------------|
| **Fiery Babyface** | Passion, crowd connection | Can become predictable |
| **Cerebral Heel** | Mind games, quotable insults | May go over casual heads |
| **Shoot Talker** | Authenticity, edge | Risk of breaking kayfabe too hard |
| **Intense Silent Type** | Aura, mystique | Limited promo opportunities |
| **Comedy Promo** | Crowd relief, quotability | Hard to transition to serious |
| **Manager Mouthpiece** | Elevates non-talker | Dependency, manager stealing heat |

---

## Territory-Style Promo Reference: Eric Embry (#245)

📌 **Source:** Vol 1 Extraction #245

### Calibration Purpose

Example of territory-style emotional promo for AI generation reference. Demonstrates that promo excellence doesn't require polish; raw emotional transmission trumps technical smoothness.

### Eric Embry Calibration

| Attribute | Rating | Notes |
|-----------|--------|-------|
| **Mic Fluency** | 10 | Not smooth, stumbles occasionally |
| **Emotional Resonance** | 18 | Makes you FEEL everything |
| **Memorable Moments** | 16 | Creates tension, real hatred |

### Style Markers

- **Emotional over technical:** The feeling matters more than word choice
- **Genuine anger/pain:** Sounds like it's coming from a real place
- **Simple language:** Speaks to the crowd, not above them
- **Stakes feel real:** You believe consequences matter
- **Territory storytelling:** Long-form investment, weekly callbacks

### LLM Generation Reference

When generating territory-era promos, use Embry-style as a calibration point:
- Prioritize emotional authenticity over verbal polish
- Allow imperfect delivery if the feeling lands
- Simple, direct language that working-class crowd connects to
- Real stakes communicated through tone, not just words

---

## Manager/Mouthpiece Delegation

When worker has low Mic Skills:

| Option | Effect |
|--------|--------|
| **Manager talks** | Uses manager's skills, worker stays silent |
| **Brief worker lines** | Worker delivers key moments only |
| **Wordless intensity** | Worker uses physicality/expression |
| **Avoiding promos** | Protect weakness, find other story tools |

---

## Connected Mechanics

- [[Promo Response]] - how crowd reacts
- [[Segment Outcomes]] - what happens after
- [[Worker_Skills|Worker Skills]] - skill inputs
- [[Buzz System/_Buzz System Index|Buzz]] - promo affects Buzz

---

## Open Questions

- Exact quality calculation formula
- Scripted vs improvised promo mechanics
- Tag team promo dynamics

---

## Implementation Notes

```json
{
  "promo_evaluation": {
    "segment_id": "seg_001",
    "worker_id": "w_001",
    "mic_skills": 16,
    "character_work": 14,
    "crowd_connection": 15,
    "context_modifiers": {
      "crowd_heat": "hot",
      "placement": "show_open",
      "hometown": false
    },
    "quality_score": 82,
    "quality_tier": "great_promo",
    "catchphrase_created": true,
    "catchphrase_text": "And that's the bottom line!",
    "buzz_change": 12,
    "memory_anchor": true
  }
}
```
