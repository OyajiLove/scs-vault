# Match Quality Factors

📛 **MECHANIC:** Match Quality Factors
🔗 **PARENT SYSTEM:** [[_Match Types Index|Match Types & Era Flavor]]
🧭 **CATEGORY:** Match Simulation / Booking Context
🔑 **KEYWORDS:** match quality, match rating, psychology, chemistry, expectations, finish
📌 **ORIGIN:** Vol 3
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 | 🔒 LOCKED |

---

## Overview

What determines match quality in context. Quality is not universal; it's evaluated against [[Era Booking Profiles|era expectations]], [[House Styles|house style norms]], and crowd context.

---

## Core Quality Factors

| Factor | Weight | Description |
|--------|--------|-------------|
| **Psychology** | Highest | Story told through action, selling, timing |
| **Worker Skill Compatibility** | High | Do their styles mesh? |
| **Crowd Expectations vs Reality** | High | Did the match deliver what was promised? |
| **Emotional Stakes** | High | Investment from [[Feud_Memory|feud history]] |
| **Match Type Appropriateness** | Medium | Right format for feud stage? |
| **Finish Believability** | Medium | Did ending make sense? |
| **Era/Regional Style Alignment** | Medium | Does it fit the context? |

---

## Psychology as Primary Multiplier

Psychology is the most important factor. A technically perfect match with no story is worse than a sloppy match with perfect psychology.

| Psychology Element | Effect |
|--------------------|--------|
| **Selling** | Makes moves matter |
| **Timing** | Creates drama and tension |
| **Callbacks** | Rewards fan memory |
| **Escalation** | Builds to climax |
| **Character work** | Face/heel dynamics in-match |

---

## Skill Compatibility

| Scenario | Result |
|----------|--------|
| **Complementary styles** | Natural flow, easy chemistry |
| **Same style** | Can be great or boring |
| **Clashing styles** | Requires adjustment, risk of trainwreck |
| **Carry job needed** | One worker compensates for other |

Compatibility affected by:
- Wrestling style tags
- Experience level
- Communication skills
- Ego/professionalism

---

## Expectations vs Reality

| Scenario | Effect |
|----------|--------|
| **Exceeded expectations** | Major positive bump |
| **Met expectations** | Neutral to positive |
| **Underdelivered** | Negative, damages workers |
| **Completely wrong** | Disaster, crowd rejects |

Expectations set by:
- Feud intensity
- Worker reputations
- Match type selection
- Promotional hype

---

## Emotional Stakes

Matches with high emotional investment are more forgiving of technical issues:

| Stakes Level | Quality Floor |
|--------------|---------------|
| **Blood feud** | Technical issues forgiven if story delivers |
| **Title match** | Higher expectations, less forgiveness |
| **Random match** | Must deliver on work alone |
| **Debut/return** | Crowd goodwill provides buffer |

---

## Era/Regional Alignment

A match judged as excellent in one context may be mediocre in another:

| Context | What's Valued |
|---------|---------------|
| **1990s AJPW** | Escalation, head drops, fighting spirit |
| **2020s US** | Spots, near-falls, dramatic sequences |
| **1980s Territory** | Heat, storytelling, protected finishes |
| **Lucha** | Flow, innovation, tradition respect |

---

## Finish Quality

| Finish Type | Quality Impact |
|-------------|----------------|
| **Clean, decisive** | Positive, builds winner |
| **Protected loss** | Loser preserved |
| **Screwy/interference** | Depends on story needs |
| **Botched** | Damages both workers |
| **Anti-climactic** | Crowd disappointment |

---

## Quality Calculation (Conceptual)

### Match Quality Component Weights (#191)

📌 **Source:** Vol 1 Extraction #191

| Component | Weight | Factors |
|-----------|--------|--------|
| **Storytelling** | 30% | Psychology, selling, build |
| **Technical Execution** | 25% | Skills, safety, consistency |
| **Crowd Engagement** | 25% | Pops, heat, investment |
| **Stakes/Context** | 20% | Title, feud heat, show importance |

### Modifier Stack

- Chemistry bonus/penalty
- Gimmick fit adjustment
- Fatigue penalty
- Crowd energy state
- Stakes multiplier

### Formula (Conceptual)

```
Base Quality = (Worker A Skill + Worker B Skill) / 2
Psychology Multiplier = 0.5 to 2.0
Chemistry Modifier = -20 to +20
Stakes Modifier = -10 to +30
Era Alignment = 0.8 to 1.2
Finish Quality = -15 to +15

Final Quality = (Base × Psychology × Era) + Chemistry + Stakes + Finish
```

**Note:** Exact formula TBD in implementation.

---

## Connected Mechanics

- [[House Styles]] - style determines judging criteria
- [[Era Booking Profiles]] - era sets expectations
- [[Predictability_Stakes|Predictability & Stakes]] - stakes affect quality perception
- [[Worker_Skills|Worker Skills]] - base inputs for calculation
- [[Buzz System/_Buzz System Index|Buzz System]] - quality affects Buzz change

---

## Open Questions

- Exact formula weights and values
- Chemistry calculation between specific workers
- Crowd type effects on quality perception (smark vs casual)

---

## Implementation Notes

```json
{
  "match_quality_calc": {
    "match_id": "m_001",
    "workers": ["w_001", "w_002"],
    "base_quality": 72,
    "psychology_multiplier": 1.4,
    "chemistry_modifier": 8,
    "stakes_modifier": 15,
    "era_alignment": 1.1,
    "finish_quality": 5,
    "final_quality": 88,
    "context": {
      "era_profile": "ajpw_1994_1998",
      "house_style": "kings_road",
      "match_type": "singles",
      "stakes": "title_match"
    }
  }
}
```
