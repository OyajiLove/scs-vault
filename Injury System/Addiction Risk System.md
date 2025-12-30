# Addiction Risk System

📛 **MECHANIC:** Painkiller and Drug Addiction Risk
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** painkiller, addiction, substance abuse, overdose, recovery, rehab, drug spiral
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Pain management is not free. Wrestling eats lives quietly through pills before fans even notice. Workers who work through injuries without recovery accrue hidden painkiller usage, which can cross addiction thresholds and spiral into health crises, career collapses, or early deaths.

---

## Painkiller Usage Tracker

Workers who work hurt accumulate painkiller usage points:

| Trigger | Usage Points |
|---------|--------------|
| Working through minor injury | +1 per match |
| Working through moderate injury | +2 per match |
| Working through major injury | +3-5 per match |
| Post-surgery early return | +3 per week |
| Heavy touring schedule while hurt | +1-2 per week |
| Chronic pain management | +1 per month |

---

## Addiction Thresholds

| Usage Level | Status | Effects |
|-------------|--------|---------|
| 0-5 | Clean | No effect |
| 6-10 | Elevated | Hidden concern, no visible impact |
| 11-15 | At Risk | Focus and Consistency start dropping |
| 16-20 | Addicted | Major stat penalties, behavior changes |
| 21+ | Crisis | Overdose risk, collapse risk, intervention needed |

---

## Addiction Effects

### Performance Impact
| Stat | Effect |
|------|--------|
| **Focus** | Decreases (-2 to -8 depending on severity) |
| **Consistency** | Decreases (-2 to -8) |
| **Recovery Efficiency** | Decreases (body can't heal properly) |
| **Promo Coherence** | May become erratic, slurred |

### Behavioral Changes
| Behavior | Description |
|----------|-------------|
| **Paranoia Rises** | Hidden personality shift toward distrust |
| **Relationship Sabotage** | Damages friendships, faction loyalty |
| **Erratic Booking Reliability** | No-shows, late arrivals, unpredictable |
| **Public Image Damage** | Visible decline noticed by fans, media |

### Example: Jeff Hardy Arcs
- Initial: Working through injuries, painkiller use rises
- Escalation: Visible performance decline, erratic promos
- Crisis: Public incidents, interventions required
- Recovery attempt: Time off, rehabilitation
- Potential relapse: Threshold resets but vulnerability remains

---

## Overdose and Collapse Risk

At crisis levels (21+):

| Risk | Probability | Outcome |
|------|-------------|---------|
| **Collapse at Show** | Low-Moderate | Career crisis, forced time off |
| **Medical Emergency** | Low | Hospitalization, potential career end |
| **Overdose (Non-Fatal)** | Rare | Major scandal, rehabilitation mandatory |
| **Overdose (Fatal)** | Very Rare | Death, legacy impact, industry ripple |

### Overdose Probability
```
Overdose Risk = (Usage Level - 20) × 2% per month

At Usage Level 25: 10% monthly risk of medical emergency
At Usage Level 30: 20% monthly risk
```

---

## Character Shift from Addiction

Addiction changes who workers are:

| Shift | Description |
|-------|-------------|
| **Paranoia Increase** | +5 to +15 hidden personality modifier |
| **Loyalty Decrease** | Trust erodes, may lash out at allies |
| **Ego Inflation** | Defensive, unable to accept help |
| **Drive Disruption** | May give up on career or desperately cling |
| **Morality Shift** | May do things they'd never do sober |

---

## Recovery and Rehabilitation

### Rehab Path
Workers can seek rehabilitation (voluntary or forced):

| Rehab Type | Trigger | Duration | Success Rate |
|------------|---------|----------|--------------|
| **Voluntary (Early)** | Worker or booker chooses | 1-3 months | High |
| **Voluntary (Crisis)** | After incident but self-initiated | 3-6 months | Moderate |
| **Forced (Intervention)** | Promotion or family forces | 3-6 months | Moderate-Low |
| **Forced (Legal/Medical)** | After arrest or emergency | 6-12 months | Variable |

### Recovery Success Factors
| Factor | Effect |
|--------|--------|
| **High Drive** | Better recovery odds |
| **High Morality** | More likely to accept help |
| **Strong Support Network** | Friends, family increase success |
| **Fan Forgiveness Trait** | Easier comeback if recovery works |
| **Previous Relapses** | Each relapse lowers future success rate |

### Post-Rehab Status
- Usage counter resets to 0
- Addiction vulnerability remains elevated
- Relapse risk: +2 usage per trigger (faster accumulation)
- Some permanent stat loss possible (brain fog, diminished reflexes)

---

## Era Differences

| Era | Substance Culture | Detection/Response |
|-----|-------------------|-------------------|
| **Territory** | Rampant, normalized | Almost none |
| **National TV (80s-90s)** | Still prevalent, hidden | Minimal unless public incident |
| **Attitude Era** | Common, some awareness | Occasional wellness concerns |
| **Modern** | Wellness policies, testing | Active monitoring, suspensions |
| **Unionized (Hypothetical)** | Support systems, benefits | Treatment coverage, job protection |

---

## Tough Guy Mythology

Some workers are remembered for working through pain:

| Legacy Type | Description |
|-------------|-------------|
| **Legendary** | Powered through, became icon (Austin's neck) |
| **Tragic** | Destroyed themselves for the business (Benoit, Dynamite) |
| **Cautionary Tale** | Career shortened, health ruined, used as warning |
| **Redemption Story** | Fell, recovered, came back stronger |

---

## Connected Mechanics

- [[Wear and Tear System]] - Pain from accumulated damage triggers usage
- [[Surgery and Recovery]] - Delayed surgery increases painkiller need
- [[Hidden Personality]] - Morality, Drive affect recovery chances
- [[Scandal System]] - Addiction can become public scandal
- [[Morale System]] - Addiction devastates morale
- [[Contract System]] - May affect employability

---

## Open Questions

- [ ] Exact threshold values for addiction stages
- [ ] Relapse probability formulas
- [ ] Era-specific substance types (pills vs. steroids vs. other)
- [ ] Promotion wellness policy enforcement mechanics
- [ ] How addiction affects contract negotiations

---

## Implementation Notes

```json
{
  "addiction_status": {
    "worker_id": "worker_001",
    "usage_level": 14,
    "status": "at_risk",
    "primary_substance": "painkillers",
    "addiction_history": {
      "previous_rehab": true,
      "rehab_count": 1,
      "last_rehab_date": "1984-03-15",
      "vulnerability_modifier": 1.5
    },
    "current_effects": {
      "focus_penalty": -3,
      "consistency_penalty": -2,
      "paranoia_modifier": +5
    },
    "triggers": [
      { "type": "chronic_pain", "contribution": 1, "frequency": "monthly" },
      { "type": "working_hurt", "contribution": 2, "recent_matches": 4 }
    ]
  }
}
```
