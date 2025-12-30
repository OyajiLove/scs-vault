# Scandal Types

📛 **MECHANIC:** Scandal Classification System
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]
🧭 **CATEGORY:** Worker Simulation / Media
🔑 **KEYWORDS:** scandal types, substance abuse, legal, criminal, sexual, backstage, severity
📌 **ORIGIN:** Vol 4 (Scandal and Public Image Layer)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Not all scandals are equal. Different types carry different weights, recovery pathways, and era-dependent responses. The system categorizes scandals by type and severity to determine career and legacy impact.

---

## Scandal Categories

### Substance Abuse Issues

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Single failed wellness test, rumored use | Warning, brief media cycle |
| **Moderate** | Public intoxication, multiple failures | Suspension, rehab requirement |
| **Major** | DUI with injury, overdose incident | Extended suspension, potential firing |
| **Catastrophic** | Fatal overdose, dealer involvement | Career end, tragic legacy |

**Effects:**
- News leaks damage reputation
- Booking trust decays
- Fan memory taints legacy unless redemption arcs occur
- Triggers [[Addiction Risk System]] integration

---

### Legal Trouble

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Disorderly conduct, minor traffic violations | Brief embarrassment |
| **Moderate** | Bar fight arrests, domestic disputes (no conviction) | Suspension, PR damage |
| **Major** | Assault charges, restraining orders | Extended leave, firing risk |
| **Catastrophic** | Serious criminal conviction, prison time | Career likely over |

**Effects:**
- Arrests and lawsuits shift public perception sharply
- Booking trust erodes with legal uncertainty
- Promotion may distance itself for PR reasons

---

### Backstage Betrayal Leaks

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Gossip about colleagues, minor politicking | Locker room heat |
| **Moderate** | Conspiring against friends/factions | Trust damage, potential faction collapse |
| **Major** | Major scheme exposed (screwjob involvement, etc.) | Career-defining controversy |
| **Catastrophic** | Industry-wide betrayal exposed | Blackballing possible |

**Effects:**
- Betrayal memories leak to newsletters, fans (era-dependent)
- Can destroy faction loyalty and make group collapse inevitable
- Creates long-term grudges that affect future booking

---

### Sexual/Assault Scandals

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Inappropriate comments (unverified) | Quiet HR warning |
| **Moderate** | Credible harassment allegations | Suspension, investigation |
| **Major** | Sexual misconduct with evidence | Firing, PR crisis |
| **Catastrophic** | Assault conviction, multiple victims | Career destroyed, legacy erased |

**Effects:**
- Near-impossible to recover from unless handled perfectly
- Era's public morality stance dramatically affects response
- Some scandals in this category cannot be erased, only marginalized over decades

---

### Criminal Activity

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Petty theft, vandalism | Embarrassment, minor discipline |
| **Moderate** | Fraud, significant theft | Suspension, legal proceedings |
| **Major** | Major fraud, organized crime ties | Firing, blacklisting |
| **Catastrophic** | Murder, trafficking, child crimes | Career destroyed, erasure from history |

**Effects:**
- Serious crimes create permanent legacy damage
- Some categories (child abuse, murder) result in "Cancelled Immortal" status
- Industry-wide blacklisting likely for major crimes

---

### Public Meltdowns

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Heated interview, minor social media drama | Brief buzz |
| **Moderate** | Major podcast shoot, controversial statements | Heat from office, some fans |
| **Major** | Public breakdown, racist/sexist statements exposed | Suspension, PR disaster |
| **Catastrophic** | Complete public mental breakdown | Extended leave, career pivot needed |

**Effects:**
- Modern era amplifies through social media
- Can become defining moment (positive or negative)
- Territory era had more tolerance for volatile behavior

---

### Relationship Scandals

| Severity | Examples | Career Impact |
|----------|----------|---------------|
| **Minor** | Dating rumors, messy breakup | Tabloid fodder |
| **Moderate** | Public affair exposed, colleague's partner | Locker room tension, media cycle |
| **Major** | Affair + betrayal of close friend (Edge/Lita/Matt) | Major storyline potential, real heat |
| **Catastrophic** | Marriage destruction + violence + custody | Career secondary to personal crisis |

**Effects:**
- Affairs, divorces, cheating scandals can leak and create huge public blowups
- Era-dependent: more damaging in modern social media era
- Can be worked into storylines (but risks real heat)

---

## Severity Modifiers

What affects scandal severity:

| Factor | Effect |
|--------|--------|
| **Worker Popularity** | More popular = more media coverage = higher impact |
| **Era** | Modern era = faster spread, more permanent record |
| **Promotion Size** | Major promotion = national/international coverage |
| **Previous Scandals** | Pattern of behavior increases severity |
| **Evidence Level** | Proven vs. alleged affects response |
| **Victim Status** | Harming vulnerable people (children, etc.) = maximum severity |

---

## Scandal Trigger Factors

What increases scandal likelihood:

| Factor | Effect |
|--------|--------|
| **Low Morality Rating** | More likely to engage in scandal-worthy behavior |
| **Substance Abuse Tags** | Higher risk of related scandals |
| **Criminal Risk Tag** | Higher legal trouble probability |
| **Scandal Magnet Tag** | Attracts controversy consistently |
| **High Ego + Low Morality** | Dangerous combination for public meltdowns |
| **Relationship Status** | Active relationships = affair risk |

---

## Connected Mechanics

- [[Public Image Impact]] - How scandals affect reputation
- [[Scandal Flex System]] - Long-term legacy effects
- [[Redemption Arcs]] - Recovery pathways
- [[Era-Based Response]] - How different eras react
- [[Hidden Personality]] - Morality determines behavior
- [[Addiction Risk System]] - Substance scandals

---

## Open Questions

- [ ] Exact probability tables for each scandal type by morality level
- [ ] How multiple scandals compound (additive vs. multiplicative)
- [ ] Witness/accuser credibility mechanics
- [ ] Legal proceedings timeline and outcome variance
- [ ] How unproven allegations affect reputation vs. proven

---

## Implementation Notes

```json
{
  "scandal_type": {
    "id": "substance_abuse",
    "category": "personal",
    "severity_levels": ["minor", "moderate", "major", "catastrophic"],
    "recovery_difficulty": "moderate",
    "era_modifiers": {
      "territory": 0.5,
      "national_tv": 0.8,
      "monday_night_wars": 0.9,
      "modern": 1.5
    },
    "redemption_eligible": true,
    "memory_decay_rate": 0.05,
    "related_tags": ["Substance Abuse History", "Addiction Recovery", "Redemption Arc"]
  }
}
```
