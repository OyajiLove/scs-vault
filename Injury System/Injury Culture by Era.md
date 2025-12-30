# Injury Culture by Era

📛 **MECHANIC:** Era-Based Injury Treatment and Attitudes
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** World Simulation / Era Flavor
🔑 **KEYWORDS:** injury culture, era, working hurt, rehab, medical
📌 **ORIGIN:** Vol 1 Extraction #46
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Wrestling's relationship with injuries has evolved dramatically across eras. What was expected in the 1970s (work through it, hide it) is unacceptable in 2020s (wellness policies, concussion protocols). This system defines how each era treats worker health.

---

## Era Profiles (#46)

| Era | Injury Culture | Notes |
|-----|----------------|-------|
| **1970s** | Everyone works hurt, injuries hidden | "You're not hurt, you can still walk" |
| **1980s** | Toughing it out expected, minimal downtime | Territory economics: no work = no pay |
| **1990s** | Car crash TV, lots of long-term injuries | Extreme style causes extreme damage |
| **2000s** | Awareness growing, still macho culture | Benoit aftermath began changes |
| **2010s** | Better rehab, but more delicate bodies | Wellness policies, concussion awareness |
| **2020s** | Protocols in place, careers protected | Long-term health prioritized |

---

## Era-Specific Injury Behaviors

### 1970s-1980s Territory Era

| Aspect | Behavior |
|--------|----------|
| **Disclosure** | Injuries hidden from promoters if possible |
| **Working Hurt** | Expected, refusing = losing your spot |
| **Medical Care** | Basic, often self-administered |
| **Recovery Time** | Minimal, return ASAP |
| **Long-term Damage** | Ignored until career-ending |
| **Painkiller Use** | Rampant, unmonitored |

### 1990s Extreme Era

| Aspect | Behavior |
|--------|----------|
| **Disclosure** | Still hidden, "tough guy" culture |
| **Working Hurt** | Expected, especially in hardcore |
| **Medical Care** | Improving but inconsistent |
| **Recovery Time** | Pressure to return early |
| **Long-term Damage** | Accumulating visibly |
| **Painkiller Use** | Peak abuse, multiple deaths |

### 2000s Transition Era

| Aspect | Behavior |
|--------|----------|
| **Disclosure** | Wellness policies force some transparency |
| **Working Hurt** | Still common, beginning to change |
| **Medical Care** | Professional staff in major promotions |
| **Recovery Time** | More realistic timelines |
| **Long-term Damage** | Awareness increasing (Benoit effect) |
| **Painkiller Use** | Monitored (theoretically) |

### 2010s-2020s Modern Era

| Aspect | Behavior |
|--------|----------|
| **Disclosure** | Required by most major promotions |
| **Working Hurt** | Discouraged, protocols exist |
| **Medical Care** | High quality in major promotions |
| **Recovery Time** | Proper timelines enforced |
| **Long-term Damage** | Career management prioritized |
| **Painkiller Use** | Strict policies, testing |

---

## Gameplay Effects

| Era | Player Options | Consequences |
|-----|---------------|--------------|
| **Territory** | Can push workers through injuries | Higher long-term damage, accepted |
| **Extreme** | Extreme matches = extreme injuries | Expected cost of business |
| **Transition** | Must balance old/new attitudes | Workers have varying expectations |
| **Modern** | Must follow protocols | Penalties for ignoring medical advice |

---

## Worker Expectations by Era

| Era | Worker Attitude |
|-----|-----------------|
| **1970s** | "If I can walk, I can work" |
| **1980s** | "Spot machine won't let me rest" |
| **1990s** | "The bump is the job" |
| **2000s** | "Starting to question this" |
| **2010s** | "My body has value" |
| **2020s** | "Career longevity matters" |

---

## Connected Mechanics

- [[Wear and Tear System]] - Era affects accumulation rate
- [[Medical Exam System]] - Era affects exam options
- [[Addiction Risk System]] - Era affects painkiller access
- [[_Injury System Index]] - Parent system

---

## Implementation Notes

```json
{
  "era_injury_culture": {
    "era": "1980s_territory",
    "work_hurt_expectation": 0.9,
    "medical_quality": 0.4,
    "disclosure_requirement": 0.1,
    "painkiller_access": 0.95,
    "protocol_enforcement": 0.1,
    "long_term_awareness": 0.2
  }
}
```

---

**Document Status:** Locked
**Last Updated:** 2025-12-25
