# Star Protection and Cover-Up System

📛 **MECHANIC:** Scandal Management Based on Star Power
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]
🧭 **CATEGORY:** Worker Simulation / Business
🔑 **KEYWORDS:** cover-up, star protection, scandal management, promoter personality, PR, sponsor
📌 **ORIGIN:** Vol 1 Extraction #109, #110
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Not all workers are treated equally when scandal strikes. The bigger the star, the more desperate promoters become to protect them. This system governs how scandals are managed based on worker value, era context, and promoter personality.

**Core Law (User-Locked):** "The bigger the star = the more desperate promoters will be to cover up, excuse, or bury scandals. Small fry = immediately sacrificed."

---

## Star Protection Logic (#109)

### Response by Star Level

| Star Level | Response Pattern |
|------------|------------------|
| **Megastar (Hogan-tier)** | Will move mountains to protect, cover up at any cost |
| **Main Eventer** | Strong cover-up attempts, high-risk PR plays |
| **Midcarder** | May protect if politically connected, otherwise expendable |
| **Low-card / Nobody** | Immediately thrown under the bus |

### Protection Mechanics

| Factor | Effect on Protection |
|--------|---------------------|
| **Draw Value** | Higher draw = more protection |
| **Contract Value** | Major investment = protect investment |
| **Political Connections** | Friends in high places = shielded |
| **Replacement Availability** | Unique talents = more protected |
| **Scandal Severity** | Even megastars have limits |

---

## Cover-Up System

### Player Options When Scandal Breaks

| Option | Description | Outcome Factors |
|--------|-------------|-----------------|
| **Cover It Up Quietly** | Suppress information, deny, deflect | Success depends on era, star power, media savvy |
| **Publicly Punish** | Fire, suspend, make example | Fast resolution, lower backlash, may lose talent |
| **Defend the Worker** | Stand by them publicly | Bad PR risk, but keeps star, loyalty boost |

### Cover-Up Success Factors

| Factor | Effect |
|--------|--------|
| **Era** | Pre-90s = easier; Post-Internet = much harder |
| **Star Power** | Ironically HARDER to cover for bigger names (more scrutiny) |
| **Scandal Severity** | Minor issues = easy; major crimes = nearly impossible |
| **Media Relationships** | Good press connections = better suppression |
| **Witness Control** | More witnesses = harder to contain |

### Era Difficulty Table

| Era | Cover-Up Difficulty |
|-----|---------------------|
| 1970s Amarillo | Easy to squash |
| 1990s WWF | Hard to contain |
| 2020s AEW/NJPW | Instant social media bomb |

---

## PR Fallout System (#110)

### Fan Reaction Based on Scandal + Management

| Scenario | Result |
|----------|--------|
| Minor scandal handled transparently | Minor damage, quick healing |
| Major scandal covered up (and exposed) | Long-term fan desertion, sponsor loss, worker morale collapse |
| Promotion backs known creeps | Lose massive sections of fanbase (especially women, younger fans) |

### Sponsor Reactions

| Era | Sponsor Behavior |
|-----|------------------|
| **Pre-90s** | Sponsors largely uninvolved, local deals easily replaced |
| **1990s-2000s** | Growing awareness, will pull money if scandals taint brand |
| **Modern** | Immediate pressure, social media campaigns against sponsors |

**Key Mechanic:** Regional promotions who tolerate problematic workers might still pull decent gates locally, but lose national expansion chance permanently.

### Worker Fallout

| Scenario | Effect |
|----------|--------|
| Workers associated with scandal-tainted companies | Gain "stigma" debuff (hurts value if they move) |
| Workers wrongly accused but exonerated | Can become cult heroes if managed right |
| Workers protected despite serious accusations | Become ticking PR time bombs |

---

## Promoter Personality Impacts

How promoter type affects scandal management:

| Promoter Type | Scandal Response Pattern |
|---------------|-------------------------|
| **Ruthless** | Cover up and threaten victims (Vince/Snuka model) |
| **Pragmatic** | Cut ties quickly to protect brand |
| **Cowardly** | Freeze and let it fester |
| **Idealistic** | Run full internal investigations, no tolerance |

### Long-Term Effects of Management Style

| Style | Short-Term | Long-Term |
|-------|------------|-----------|
| **Ruthless** | Keeps stars, suppresses truth | Eventually exposed, catastrophic fallout |
| **Pragmatic** | Loses talent, manages PR | Stable reputation, attracts sponsors |
| **Cowardly** | Neither protects nor releases | Festering resentment, unpredictable crises |
| **Idealistic** | May lose stars, high turnover | Clean reputation, attracts certain talent |

---

## Historical Examples

### Cover-Up Successes (Temporary)

| Case | Method | Duration | Eventual Fallout |
|------|--------|----------|------------------|
| Hogan steroid use | Denial, legal maneuvering | Years | Trial, public knowledge |
| Snuka murder case | Suppression, influence | Decades | Documentary exposure, legal action |
| Various territory-era crimes | Local media control | Indefinite | Some never surfaced |

### Cover-Up Failures

| Case | What Went Wrong | Consequence |
|------|-----------------|-------------|
| SpeakingOut movement | Social media bypassed gatekeepers | Industry-wide reckoning |
| Benoit case | Scale too large to suppress | Complete erasure, policy changes |
| Modern leaks | Screenshots, recordings exist | Instant exposure |

---

## The Money vs. Morality Equation

**Final Law:** "Promoters love money. They will burn morality on the altar of box office... or burn so many bridges you die isolated. (Just like real life.)"

### Cost-Benefit Calculation

| Consideration | Weight |
|---------------|--------|
| Gate revenue lost if star released | High |
| Sponsor revenue lost if star kept | Variable by era |
| Fan trust long-term | Undervalued by most |
| Worker morale if creeps protected | Often ignored |
| Legal liability | Growing concern |

---

## Connected Mechanics

- [[Era-Based Response]] - Era dramatically affects options
- [[Public Image Impact]] - Scandal management affects reputation
- [[Scandal Types]] - Different scandals have different containment difficulty
- [[Redemption Arcs]] - Management style affects redemption possibility
- [[Contract System/_Contract System Index|Contract System]] - Morality clauses, firing decisions

---

## Open Questions

- [ ] Exact cover-up success probability formulas
- [ ] Media relationship mechanics
- [ ] Cross-promotion information sharing
- [ ] Whistleblower/leak mechanics
- [ ] Legal consequence simulation

---

## Implementation Notes

```json
{
  "scandal_management": {
    "scandal_id": "scan_001",
    "worker_id": "worker_megastar",
    "star_level": "megastar",
    "promoter_type": "pragmatic",
    "player_decision": "cover_up",
    "cover_up_attempt": {
      "success_probability": 0.45,
      "era_modifier": 0.7,
      "star_power_modifier": 0.6,
      "final_roll": 0.38,
      "outcome": "failed"
    },
    "fallout": {
      "fan_reaction": "hostile",
      "sponsor_pressure": "high",
      "morale_impact": -25,
      "long_term_reputation": -40
    }
  }
}
```

---

**Document Status:** Locked (Vol 1)
**Last Updated:** 2025-12-24
**Next Review:** Design cover-up probability formulas
