# Post-Career Roles

📛 **MECHANIC:** Transitions After Active Competition
🔗 **PARENT SYSTEM:** [[_Retirement System Index|Retirement System]]
🧭 **CATEGORY:** Worker Lifecycle
🔑 **KEYWORDS:** manager, road agent, trainer, commentator, authority figure, post-career
📌 **ORIGIN:** Vol 1-4 (Future Referee, Future Manager, Future Road Agent tags)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Retirement doesn't mean leaving wrestling entirely. Many workers transition to backstage or on-screen roles that keep them connected to the business. These roles are influenced by worker skills, personality, and the "Future [Role]" tags that indicate natural inclinations.

---

## Available Post-Career Roles

| Role | Description | Key Requirements |
|------|-------------|------------------|
| **Manager** | Guides active workers, cuts promos | Charisma, Promo ability |
| **Road Agent** | Plans matches, works with talent | Psychology, Experience |
| **Head Trainer** | Runs developmental/dojo | Technical skill, Patience |
| **Play-by-Play** | Calls action | Knowledge, Voice |
| **Color Commentator** | Provides analysis/entertainment | Charisma, Knowledge |
| **Referee** | Officiates matches | Fitness, Respect |
| **Authority Figure** | On-screen power role | Charisma, Heat potential |
| **Personality** | Talk show host, interviewer | Charisma, Promo ability |
| **Scout** | Finds new talent | Eye for potential |
| **Booker/Creative** | Plans storylines | Psychology, Creativity |
| **Owner/Executive** | Runs promotion | Business sense, Capital |

---

## Future Role Tags

These tags indicate natural inclinations:

| Tag | Post-Career Tendency |
|-----|---------------------|
| **Future Referee** | Will be available as referee |
| **Future Play By Play** | Will be available as PBP |
| **Future Colour Commentator** | Will be available as color |
| **Future Manager** | Will be available as manager |
| **Future Personality** | Will be available as personality |
| **Future Road Agent** | Will be available as agent |
| **Natural Trainer** | Higher chance of running dojo |

---

## Role Transition Requirements

### Manager

| Requirement | Minimum Level |
|-------------|---------------|
| Charisma | 70+ |
| Microphone | 65+ |
| Psychology | 50+ |
| Physical Condition | Not required |

**Best Fit:** Talkers who can still generate heat or sympathy

### Road Agent

| Requirement | Minimum Level |
|-------------|---------------|
| Psychology | 75+ |
| Experience | 10+ years active |
| Respect | Moderate+ locker room standing |
| Creativity | 50+ |

**Best Fit:** Ring generals, technical masters, respected veterans

### Head Trainer

| Requirement | Minimum Level |
|-------------|---------------|
| Technical | 70+ |
| Psychology | 65+ |
| Patience | Moderate+ |
| Teaching Ability | Natural Trainer tag helps |

**Best Fit:** Fundamentally sound workers who can teach

### Commentator (Play-by-Play)

| Requirement | Minimum Level |
|-------------|---------------|
| Microphone | 70+ |
| Knowledge | Extensive |
| Voice Quality | Broadcast-ready |
| Stamina | Can work long shows |

**Best Fit:** Articulate workers with broadcast presence

### Commentator (Color)

| Requirement | Minimum Level |
|-------------|---------------|
| Charisma | 70+ |
| Microphone | 60+ |
| Personality | Entertaining |
| Knowledge | Solid |

**Best Fit:** Charismatic personalities, former heels often excel

### Authority Figure

| Requirement | Minimum Level |
|-------------|---------------|
| Charisma | 75+ |
| Microphone | 70+ |
| Heat Potential | Can draw reactions |
| Star Power | Recognized name |

**Best Fit:** Former main eventers, legendary figures

---

## Role Combinations

Workers can hold multiple roles:

| Combination | Viability |
|-------------|-----------|
| Manager + Commentator | Common |
| Road Agent + Trainer | Common |
| Authority Figure + Commentator | Possible |
| Scout + Road Agent | Common |
| Owner + Authority Figure | Common |

---

## Role Success Factors

| Factor | Effect |
|--------|--------|
| **Natural Inclination** | Future [Role] tag = +20% success |
| **Skill Match** | Right abilities = smooth transition |
| **Personality Fit** | Patient trainers, charismatic managers |
| **Locker Room Respect** | Affects agent/trainer effectiveness |
| **Physical Condition** | Some roles need mobility |

---

## Historical Examples

| Worker | Post-Career Role | Success Level |
|--------|------------------|---------------|
| **Pat Patterson** | Road Agent | Legendary |
| **Arn Anderson** | Road Agent | Very High |
| **Paul Heyman** | Manager | Legendary |
| **Bobby Heenan** | Manager → Commentator | Legendary both |
| **Jerry Lawler** | Commentator | Very High |
| **Booker T** | Commentator | High |
| **William Regal** | Trainer | Very High |
| **Fit Finlay** | Road Agent | Very High |

---

## Role Availability Timeline

| Post-Retirement Period | Role Availability |
|------------------------|-------------------|
| **Immediate** | Manager, Authority Figure |
| **6-12 months** | Commentator, Personality |
| **1-2 years** | Road Agent, Trainer |
| **2+ years** | Scout, Booker/Creative |

---

## Promotion Considerations

| Factor | Effect on Hiring |
|--------|------------------|
| **Former Employee** | Preference for familiar faces |
| **Competitor History** | May create friction |
| **Scandal History** | Reduces opportunities |
| **Star Power** | Opens more doors |
| **Skill Match** | Primary consideration |

---

## Connected Mechanics

- [[Retirement Types]] - Type affects role options
- [[Hidden Personality]] - Traits affect role success
- [[Contract System]] - Post-career contracts
- [[Hall of Fame System]] - Roles affect legacy

---

## Open Questions

- [ ] How roles affect ongoing storylines
- [ ] Role salary/compensation
- [ ] Role performance ratings
- [ ] Transitioning between post-career roles
- [ ] How roles affect comeback potential

---

## Implementation Notes

```json
{
  "post_career": {
    "worker_id": "worker_001",
    "active_roles": ["road_agent", "trainer"],
    "available_roles": ["manager", "commentator_color"],
    "role_performance": {
      "road_agent": 85,
      "trainer": 78
    },
    "natural_inclinations": ["future_road_agent", "natural_trainer"],
    "role_history": [
      { "role": "manager", "promotion": "promo_001", "years": "1990-1995" }
    ]
  }
}
```
