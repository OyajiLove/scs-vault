# Scandal Flex System

📛 **MECHANIC:** Scandal Memory and Legacy Interaction
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]
🧭 **CATEGORY:** Worker Simulation / Legacy
🔑 **KEYWORDS:** scandal flex, legacy, memory drift, fan reappraisal, documentary, cancelled immortal
📌 **ORIGIN:** Vol 4 (Anti-Propaganda & Fan Memory Resistance Engine)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Scandal impact isn't static. Over time, fan perception drifts based on morality, promotion bias, time passed, and cultural shifts. Some disgraced workers are partially re-evaluated later; others stay buried forever. The Scandal Flex System determines how scandals interact with legacy memory over decades.

---

## Scandal Flex Curve

Based on three factors:
- **Morality of Scandal:** How severe/unforgivable the act was
- **Promotion Bias:** How hard the promotion pushes narrative either way
- **Time Passed:** Distance softens or hardens memory

```
Scandal Flex = (Base Severity) × (Time Decay) × (Era Modifier) × (Narrative Push)

Where:
- Base Severity: 1-100 based on scandal type
- Time Decay: Reduces over years (slower for severe scandals)
- Era Modifier: Modern era = slower decay (permanent record)
- Narrative Push: Promotion/media effort to rehabilitate or suppress
```

---

## Memory Decay by Scandal Type

| Scandal Type | Decay Rate | Floor (Minimum Impact) |
|--------------|------------|------------------------|
| **Substance Abuse** | Fast (3-5 years) | Low (can fully recover) |
| **Legal Trouble (Minor)** | Fast (2-3 years) | Low |
| **Backstage Betrayal** | Moderate (5-10 years) | Low-Medium |
| **Public Meltdown** | Moderate (3-7 years) | Low |
| **Relationship Scandal** | Fast (2-4 years) | Very Low |
| **Sexual Misconduct** | Very Slow (10-20+ years) | High |
| **Criminal (Major)** | Very Slow (15-25+ years) | High |
| **Criminal (Catastrophic)** | Near-Zero | Maximum (never fades) |

---

## Scandal Flex Categories

### Forgettable Scandals
- Minor substance, minor legal, relationship drama
- Fade from memory within 3-5 years
- Full career recovery possible
- Legacy unaffected long-term

### Complicated Legacies
- Moderate scandals that become part of the story
- Neither fully erased nor fully defining
- Context-dependent discussion
- Examples: Jeff Hardy's struggles, Ric Flair's controversies

### Cancelled but Remembered
- Severe scandals that prevent celebration but don't erase memory
- Can't be canonized (Hall of Fame, tributes) but can't be forgotten
- "Cancelled Immortal" status
- Example: Chris Benoit

### Fully Erased
- Catastrophic scandals leading to complete industry removal
- Name not mentioned, footage removed, history rewritten
- Extremely rare; requires industry consensus
- Example: Some child abuse/trafficking cases

---

## Fan Reappraisal Mechanics

Every 10-15 in-game years, the younger fanbase has a chance to rediscover and reframe workers:

| Trigger | Effect |
|---------|--------|
| **Documentary Release** | Spike in visibility, narrative reframing |
| **Shoot Interview** | Can elevate buried workers or tear down canonized figures |
| **Death/Tragedy** | Martyr effect possible, or reinforces cautionary tale |
| **Generational Shift** | New fans discover old controversies with fresh perspective |
| **Cultural Change** | Society's moral standards shift, changing scandal weight |

### Documentary Influence
Third-party documentaries can challenge official narratives:
- Dark Side of the Ring effect
- Rise & Fall retrospectives
- Fan-made content and podcasts
- Deadlock/wrestling podcast culture

---

## Underground Legacy Score

Hidden secondary memory tracker:
- Based on shoot discourse, rare replays, community lore
- Exists separately from official promotion narrative
- Cult figures maintain underground legacy even when officially erased
- Internet era makes underground memory more powerful

---

## Scandal-Related Legacy Tags

| Tag | Description | Legacy Effect |
|-----|-------------|---------------|
| **Scandal Magnet** | Pattern of controversies | Remembered for drama |
| **Cancelled Immortal** | Erased from canon but unforgettable | Complex, uncomfortable legacy |
| **Redemption Arc** | Overcame scandal through work | Inspirational narrative |
| **Controversial Truth-Teller** | Scandal was exposing truth | May be vindicated later |
| **Forgotten Because Scandal** | Career overshadowed by one event | Tragic legacy |

---

## Era Impact on Scandal Flex

| Era | Scandal Decay | Permanence |
|-----|---------------|------------|
| **Territory** | Fast (limited documentation) | Low (word of mouth fades) |
| **National TV** | Moderate (magazines, newsletters) | Medium |
| **Monday Night Wars** | Slower (early internet, tape trading) | Medium-High |
| **Modern** | Very Slow (social media, permanent record) | Very High |

### Modern Era Specifics
- Screenshots last forever
- Video evidence widely distributed
- Cancel culture dynamics (rapid, sometimes reversible)
- Sponsor pressure creates faster initial response
- But also: faster redemption cycles for minor scandals

---

## Promotion Narrative Control

Promotions can attempt to control scandal memory:

| Strategy | Effect | Limitations |
|----------|--------|-------------|
| **Erasure** | Remove from all media | Only works short-term; fans remember |
| **Rehabilitation Push** | Positive booking, comeback stories | Requires genuine behavior change |
| **Narrative Spin** | Reframe scandal in favorable light | Depends on fan trust in promotion |
| **Ignore** | Hope it fades naturally | Works for minor scandals only |
| **Lean Into It** | Make scandal part of character | Works for heel turns, edgy gimmicks |

### Tension with Fan Memory
Internal friction between company narrative and underground truth alters:
- Match legacy
- Hall of Fame discussions
- Documentary weight
- Historical rankings

---

## Connected Mechanics

- [[Scandal Types]] - Base severity determines flex parameters
- [[Public Image Impact]] - Short-term effects feed into flex
- [[Redemption Arcs]] - Active rehabilitation changes flex curve
- [[Crowd Memory]] - Fan memory integrates with scandal flex
- [[Hall of Fame System]] - Scandal flex affects eligibility

---

## Open Questions

- [ ] Exact formulas for scandal decay over time
- [ ] Documentary event trigger mechanics
- [ ] How cultural shift events affect scandal reappraisal
- [ ] Underground legacy score calculation
- [ ] Promotion narrative control effectiveness

---

## Implementation Notes

```json
{
  "scandal_flex": {
    "worker_id": "worker_001",
    "scandal_id": "scan_001",
    "base_severity": 65,
    "current_severity": 42,
    "years_since_scandal": 8,
    "decay_rate": 0.05,
    "floor": 20,
    "era_modifier": 1.2,
    "narrative_push": {
      "direction": "rehabilitation",
      "strength": 0.3
    },
    "underground_legacy": {
      "score": 55,
      "sentiment": "complicated"
    },
    "reappraisal_events": [
      { "type": "documentary", "date": "1993-01-01", "effect": -10 }
    ],
    "legacy_tag": "Redemption Arc"
  }
}
```
