# Shield Wear Down Over Time

📛 **MECHANIC:** Cumulative Shield Decay from Repeated Scandals  
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]  
🧭 **CATEGORY:** Long-Term Consequences / Organizational Health  
🔑 **KEYWORDS:** shield decay, cumulative rot, scandal accumulation, trust erosion  
📌 **ORIGIN:** Vol 2 Chunk 07 (Scandal System Polish)  
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 07 | 🔒 LOCKED |

---

## Overview

Even if a promotion successfully shields early scandals, every new scandal weakens the company's shielding ability over time.

**Core Truth:** First scandal? Maybe you survive clean. Second? Harder. Third? The cracks show. Fourth? The dam bursts.

---

## Core Mechanics

| Mechanic | Description |
|----------|-------------|
| **Shield Strength** | Starts high (100%); represents full ability to protect scandal figures |
| **Decay After Every Scandal** | Each major scandal (hidden OR exposed) permanently lowers Shield Strength |
| **Exponential Decay** | Damage worsens over time; each scandal wears down more than the one before |
| **Cultural/Era Sensitivity** | Modern eras (2020s+) = much faster decay due to social media, leaks, journalism |
| **Fan Hypocrisy Ties** | Even loyal fans eventually break after enough betrayals |

---

## Shield Decay Table

| Scandal # | Shield Strength (from 100%) | Description |
|-----------|----------------------------|-------------|
| **1st** | 85-90% | Small dent, easily survivable |
| **2nd** | 70-80% | Fan/media questions begin |
| **3rd** | 55-65% | Clear cracks in image, harder media pressure |
| **4th** | 35-50% | Major PR bleeding, sponsors pulling |
| **5th** | 15-30% | Death spiral danger zone |
| **6+** | 0-10% | Even small scandals become lethal |

---

## Shield Strength Formula

Shield Strength is determined by:

| Factor | Effect |
|--------|--------|
| **Company Size** | Bigger = stronger shield (more PR muscle, media influence) |
| **Company Prestige** | Respected companies get longer fan loyalty buffers |
| **Company Resources** | Money, legal departments, PR firms = shield enhancement |
| **Fan Loyalty Depth** | Rabid fanbases defend longer (until they don't) |
| **Scandal History** | Past scandals still rot shield invisibly ("brittle trust") |
| **Current Scandal Severity** | Major scandals cause burn-through regardless of starting strength |

---

## Scandal Severity and Immediate Shield Damage

Even at 100% Shield, severe scandals cause immediate damage:

| Scandal Type | Immediate Shield Hit |
|--------------|---------------------|
| **Minor** (DUI, Fight, Backstage Beef) | -5% to -10% |
| **Moderate** (Drug Abuse, Gambling, Minor Cheating) | -10% to -20% |
| **Serious** (Racism, Sexism - Speech Only) | -20% to -30% |
| **Severe** (Sexual Harassment, Assault Allegations) | -30% to -50% |
| **Career-Killer** (Grooming, Pedophilia, Violent Assaults) | -50% to -70% |
| **Catastrophic** (Murder, Death-Linked Scandals) | -70% to -90% |

---

## Decay Modifiers

### What Accelerates Decay

| Factor | Effect |
|--------|--------|
| **Deny At All Costs management** | Fastest shield collapse possible |
| **Dirty Cover-Up Artist tag** | Short-term gain, doubled long-term chain risk |
| **Modern Era (2020s+)** | Social media amplification; faster decay |
| **Multiple cover-ups exposed** | Each doubles decay rate |

### What Slows Decay

| Action | Effect |
|--------|--------|
| **Major Public Reform** | Recover 5-10% Shield Strength |
| **Crisis Reformer Leadership** | Stabilizes decay |
| **Whistleblower Friendly Culture** | Fewer chain events; slower decay |
| **Keeping Internal Culture Clean** | Natural slow recovery over time |
| **Hire Reformer Management** | Can rebuild shield over 1-2 years |

---

## When Shield Reaches 0%

When Shield collapses completely:

| Consequence | Description |
|-------------|-------------|
| **Total Sponsor Exodus** | Brands distance within weeks |
| **TV Deal At Risk** | Network demands immediate action or threatens cancellation |
| **Locker Room Fracture** | Star workers request releases; leaks to media increase |
| **Fan Loyalty Shatters** | Merch, gates, engagement crash |
| **Media Siege Mode** | Journalists hunt every skeleton; minor mistakes become headlines |
| **Rival Attacks** | Other feds market as "the clean alternative" |
| **Internal Coup Attempts** | Executives maneuver to oust leadership |
| **Talent Avoidance** | Future top stars refuse to sign ("toxic brand") |

---

## Connection to Cascading Scandals

When shield is weak, cascading scandals hit harder:

| If Shield < 50% | Then... |
|-----------------|---------|
| Minor locker room beefs | Explode into full media stories |
| Small unpaid paychecks | Cause lawsuits/leaks |
| Old scandals | Re-emerge from the past ("reopened wounds") |
| Workers | Begin airing dirty laundry publicly |
| Ex-workers | Sue for wrongful termination, discrimination |

**Real Example:** Vince McMahon's Ring Boy Scandal (1992) → Deaths of wrestlers → New sexual assault lawsuits → Corporate governance investigations (2022-23). One crack leads to a flood because suffering needs witnesses to be heard.

---

## Connected Systems

- [[Burnout Collapse States]] - Shield collapse triggers burnout
- [[Star Protection System]] - Initial shielding mechanics
- [[Scandal Chain Events]] - Weak shields accelerate chains
- [[Management Behaviour Tags]] - Tags modify decay rates
- [[Fan Loyalty Resistance]] - Fan trust is shield's foundation

---

## Implementation Notes

```json
{
  "promotion_shield": {
    "promotion_id": "promo_001",
    "base_shield_strength": 100,
    "current_shield_strength": 42,
    "scandal_count": 4,
    "decay_history": [
      {"scandal": "scandal_001", "decay": -12},
      {"scandal": "scandal_002", "decay": -18},
      {"scandal": "scandal_003", "decay": -15},
      {"scandal": "scandal_004", "decay": -13}
    ],
    "recovery_actions_taken": [],
    "cascade_risk_modifier": 1.8
  }
}
```

---

**Document Status:** Locked (Vol 2 Chunk 07)  
**Last Updated:** 2025-12-26  
**Next Review:** Connect to Economics System for financial cascade effects
