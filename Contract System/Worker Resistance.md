# Worker Resistance

📛 **MECHANIC:** Worker Resistance
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** pushback, refusal, leverage, booking resistance, ego, politics
📌 **ORIGIN:** Vol 4 (Phase 4 System 3: Worker Resistance & Pushback Logic)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Workers don't always play ball. This system adds tension to booking: workers can refuse finishes, demand changes, sandbag performances, or outright rebel. The key mechanic is Ego vs. Loyalty, modified by backstage leverage (contracts, merch numbers, fan support).

---

## Resistance Triggers

| Trigger | Description | Likelihood |
|---------|-------------|------------|
| **Asked to lose in hometown** | Pride and kayfabe protection | High (for high Ego) |
| **Refused title push after earning it** | Promise broken | High |
| **Assigned bad gimmick** | Creative dignity | Medium-High |
| **Drafted to rival fed** | Loyalty violation | Medium |
| **Booked to lose after big win** | Momentum kill | Medium |
| **Worked hard without payoff** | Trust erosion | Medium |
| **Used in shoot angle without consent** | Boundary violation | High |
| **Merch cut too low vs. sales** | Financial exploitation | Medium |
| **Favored worker gets better treatment** | Jealousy/fairness | Medium |
| **Friend fired unjustly** | Solidarity | Variable |

---

## Resistance Calculation

```
Resistance Score = (Ego × Trigger Severity) - (Loyalty × Relationship Quality)

Where:
- Ego: 1-20 hidden rating
- Trigger Severity: 1-10 based on offense type
- Loyalty: 1-20 hidden rating
- Relationship Quality: Booker trust, past treatment, 1-10

If Resistance Score > Threshold → Worker resists
```

### Threshold by Worker Type
| Worker Type | Resistance Threshold |
|-------------|---------------------|
| Loyal Soldier | 80+ |
| Neutral Worker | 50+ |
| Ego-Driven Star | 30+ |
| Political Operator | 40+ (but resistance is calculated, not emotional) |

---

## Resistance Forms

| Form | Description | Visibility |
|------|-------------|------------|
| **Quiet Protest** | Does the job but morale tanks | Hidden |
| **Negotiation Demand** | Asks for compromise before performing | Direct |
| **Sandbag Performance** | Goes through motions, match quality suffers | Visible in match |
| **Public Complaint** | Social media, interviews | Public |
| **No-Show** | Simply doesn't appear | Critical |
| **Shoot in Match** | Goes off-script, potentially dangerous | Visible, dramatic |
| **Walkout** | Leaves mid-show or mid-contract | Crisis |

---

## Backstage Leverage

Workers with more leverage can resist more boldly:

| Leverage Factor | Effect |
|-----------------|--------|
| **Guaranteed Contract** | Can resist without fear of firing |
| **High Merch Sales** | Financially valuable to promotion |
| **Fan Favorite Status** | Firing causes backlash |
| **Faction/Clique Support** | Others back them up |
| **Media Access** | Can go public easily |
| **Other Promotion Interest** | Has options if fired |

### Leverage Score
```
Leverage = Contract Security + Popularity + Merch Value + Faction Support + External Options

High Leverage (80+) = Can resist almost anything
Medium Leverage (40-79) = Selective resistance, picks battles
Low Leverage (0-39) = Risks career if resisting
```

---

## Booker Response Options

When worker resists:

| Response | Description | Consequences |
|----------|-------------|--------------|
| **Give In** | Accept worker's demands | Preserves morale, may shift power |
| **Compromise** | Meet halfway | Both sides save face |
| **Punish Quietly** | Reduce push, matches | Worker simmers, fans may notice |
| **Shoot Response** | On-air retaliation | Risks blowback, could be story gold |
| **Firing/Suspension** | Terminate or bench | Can restore control or trigger revolt |
| **Scapegoating** | Punish others to send message | Fractures cliques, creates enemies |

---

## Worker Memory

Workers remember:
- Every slight, burial, broken promise
- Who stood up for them and who didn't
- How colleagues were treated
- Whether resistance worked or backfired

This creates grudge networks that affect:
- Future negotiations
- Faction loyalty
- Retirement interviews
- Reunion possibilities

---

## Faction Resistance

Groups can resist collectively:

| Type | Description |
|------|-------------|
| **Solidarity Refusal** | Entire faction refuses to perform |
| **Slowdown** | Group does minimum effort |
| **Collective Bargaining** | Faction negotiates as unit |
| **Leadership Resistance** | Leader refuses, others follow |
| **Splinter Resistance** | One member breaks from faction to resist |

---

## Era-Based Resistance Norms

| Era | Resistance Culture |
|-----|-------------------|
| **Territory** | Rare public resistance; workers just leave |
| **National TV** | More resistance; workers have more visibility |
| **Monday Night Wars** | Maximum leverage; workers can jump ship |
| **Modern** | Social media amplifies resistance |
| **Unionized** | Formal grievance channels |

---

## Connected Mechanics

- [[Hidden Personality]] - Ego, Loyalty drive resistance
- [[Contract Types]] - Security affects willingness to resist
- [[Contract Morality Score]] - Poor treatment triggers resistance
- [[Faction System]] - Groups can resist together
- [[Firing System]] - Resistance may lead to termination
- [[Morale System]] - Resistance is symptom of low morale

---

## Open Questions

- [ ] Exact resistance threshold formulas
- [ ] Contagion effect (one resister inspiring others)
- [ ] Media leak probability when resisting
- [ ] Recovery path after resistance resolved
- [ ] Long-term relationship damage calculations

---

## Implementation Notes

```json
{
  "resistance_event": {
    "worker_id": "worker_001",
    "trigger": "refused_title_push",
    "resistance_score": 72,
    "threshold": 50,
    "resistance_form": "negotiation_demand",
    "worker_demands": [
      "title_match_within_60_days",
      "main_event_slot_at_next_ppv"
    ],
    "booker_response": "compromise",
    "outcome": {
      "demand_met": "partial",
      "morale_change": +8,
      "relationship_change": -3,
      "precedent_set": true
    }
  }
}
```
