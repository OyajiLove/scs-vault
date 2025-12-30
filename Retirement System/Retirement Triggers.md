# Retirement Triggers

📛 **MECHANIC:** What Causes Workers to Retire
🔗 **PARENT SYSTEM:** [[_Retirement System Index|Retirement System]]
🧭 **CATEGORY:** Worker Lifecycle
🔑 **KEYWORDS:** retirement trigger, forced retirement, voluntary retirement, injury, burnout
📌 **ORIGIN:** Vol 1-4 (Career Arc Templates, Injury System, Worker Tags)
✅ **STATUS:** Locked

---

## Overview

Retirement happens for many reasons: some workers choose to leave at their peak, others are forced out by broken bodies, and some simply lose the passion. The system tracks multiple trigger types and their likelihood based on worker traits, physical condition, and career circumstances.

---

## Trigger Categories

### Physical Triggers

| Trigger | Description | Examples |
|---------|-------------|----------|
| **Career-Ending Injury** | Injury too severe to continue | Edge (neck), Paige (neck) |
| **Accumulated Damage** | Body worn down over time | Austin (neck + knees) |
| **Chronic Condition** | Ongoing issue makes wrestling unsafe | Daniel Bryan (concussions) |
| **Age Decline** | Physical skills no longer competitive | Natural career end |
| **Medical Advice** | Doctors recommend stopping | Concussion protocols |

### Mental/Emotional Triggers

| Trigger | Description | Examples |
|---------|-------------|----------|
| **Burnout** | Mental exhaustion from the road | Many 2020s wrestlers |
| **Lost Passion** | No longer loves wrestling | Punk (first retirement) |
| **Achieved Goals** | Nothing left to prove | Rare, but exists |
| **Family Priority** | Family becomes more important | Many women after children |
| **Mental Health** | Depression, anxiety make continuing harmful | Various |

### External Triggers

| Trigger | Description | Examples |
|---------|-------------|----------|
| **Scandal Force-Out** | Scandal makes continuing impossible | Various |
| **Legal Issues** | Legal troubles end career | Criminal convictions |
| **Financial Security** | Earned enough, no need to continue | Smart investors |
| **Better Opportunity** | Other career beckons | Rock (acting) |
| **Promotion Closure** | Home company dies, no desire to continue | Territory era |

---

## Personality Factors

| Trait | Effect on Retirement |
|-------|---------------------|
| **Desperado** | Won't retire until very old unless forced |
| **Heart's Not In It** | Retires younger than expected |
| **Wrestling In The Blood** | Never truly leaves the business |
| **Health First** | Retires early to protect body |
| **Outside Interests** | More likely to leave if career stalls |
| **Lifer Mentality** | Intends to stay regardless of success |

---

## Drive Rating Impact

| Drive Level | Retirement Behavior |
|-------------|---------------------|
| **Very High** | Fights through pain, resists retirement |
| **High** | Standard career length, retires when appropriate |
| **Moderate** | May retire earlier if not pushed |
| **Low** | Coasts, may retire once comfortable |
| **Very Low** | Quick to quit when things get hard |

---

## Age-Based Triggers

| Age Range | Natural Retirement Chance |
|-----------|--------------------------|
| **Under 30** | Very low (unless injury) |
| **30-35** | Low |
| **36-40** | Moderate |
| **41-45** | High |
| **46-50** | Very High |
| **50+** | Extremely High (Desperado exception) |

### Modifiers

| Factor | Effect |
|--------|--------|
| **High Popularity** | Delays retirement (still drawing) |
| **Title Holder** | Delays retirement (obligation) |
| **Injury History** | Accelerates retirement |
| **Financial Need** | Delays retirement |
| **Outside Income** | Accelerates retirement |

---

## Injury Severity Thresholds

| Injury Status | Retirement Risk |
|---------------|-----------------|
| **Minor Accumulated** | Low |
| **Moderate Chronic** | Moderate |
| **Severe Single** | High |
| **Career-Threatening** | Very High |
| **Catastrophic** | Forced retirement |

---

## Warning Signs

System can alert player:

| Warning | Meaning |
|---------|---------|
| "[Worker] showing signs of physical decline" | Age/injury catching up |
| "[Worker] seems burned out" | Mental trigger building |
| "[Worker] has been discussing retirement" | Considering voluntary exit |
| "[Worker] medically advised to stop" | Serious health concern |
| "[Worker] has outside opportunities" | May leave for other career |

---

## Connected Mechanics

- [[Injury System]] - Physical triggers
- [[Scandal System]] - External force-out triggers
- [[Hidden Personality]] - Drive, passion affect timing
- [[Contract System]] - Contract status affects retirement timing

---

## Open Questions

- [ ] Exact probability formulas for each trigger
- [ ] How multiple triggers compound
- [ ] Player intervention options
- [ ] AI booking around imminent retirement
- [ ] How to handle "worked" retirement angles

---

## Implementation Notes

```json
{
  "retirement_triggers": {
    "worker_id": "worker_001",
    "active_triggers": [
      { "type": "age_decline", "severity": 60 },
      { "type": "accumulated_damage", "severity": 45 }
    ],
    "personality_modifiers": {
      "desperado": false,
      "health_first": true,
      "drive_level": "moderate"
    },
    "retirement_probability": 35,
    "warning_flags": ["physical_decline", "discussing_retirement"],
    "estimated_career_remaining_months": 18
  }
}
```
