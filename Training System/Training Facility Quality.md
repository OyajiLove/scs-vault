# Training Facility Quality

📛 **MECHANIC:** Impact of School/Dojo Prestige on Development
🔗 **PARENT SYSTEM:** [[_Training System Index|Training System]]
🧭 **CATEGORY:** Infrastructure, Development
🔑 **KEYWORDS:** facility, dojo, school, training center, equipment, prestige, development speed
📌 **ORIGIN:** Vol 4 (dojo concepts), Ringstate Atlas (promotion facilities)
✅ **STATUS:** Exploratory (concepts documented, formulas TBD)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4, Ringstate Atlas | 📐 EXPLORATORY |

---

## Overview

Not all training facilities are equal. Elite dojos with legendary trainers produce better workers faster than backyard rings with amateur coaches. Facility quality affects growth rate, injury prevention, tag acquisition speed, and the caliber of training partners available.

---

## Facility Quality Scale

| Rating | Description | Examples | Growth Modifier |
|--------|-------------|----------|-----------------|
| **Elite (5)** | World-class, legendary trainers, full equipment | NJPW Dojo, WWE PC, Miss Mitsuko's NSP | +30-40% |
| **Excellent (4)** | Professional grade, experienced coaches | Major territory schools, established feds | +15-25% |
| **Good (3)** | Solid fundamentals, adequate equipment | Regional schools, mid-tier promotions | +5-10% |
| **Basic (2)** | Minimal equipment, part-time training | Small indie schools, side operations | 0% (baseline) |
| **Poor (1)** | Backyard level, inexperienced trainers | Garage gyms, self-taught environments | -10-20% |

---

## Facility Components

### Physical Infrastructure

| Component | Impact |
|-----------|--------|
| **Ring Quality** | Affects bump safety, technique development |
| **Mat Space** | Multiple rings = more training time |
| **Gym Equipment** | Physical conditioning, strength training |
| **Video System** | Match review, technique analysis |
| **Medical Staff** | Injury prevention, recovery support |

### Human Resources

| Component | Impact |
|-----------|--------|
| **Head Trainer Prestige** | Overall quality multiplier |
| **Assistant Trainers** | Individual attention capacity |
| **Guest Coaches** | Specialty style instruction |
| **Training Partners** | Quality of sparring, match practice |
| **Psychology Coach** | Mental/entertainment development |

### Support Systems

| Component | Impact |
|-----------|--------|
| **Nutrition Program** | Physical development, recovery |
| **Travel Support** | Excursion quality, logistics |
| **Contract Pipeline** | Path to professional work |
| **Alumni Network** | Post-training opportunities |

---

## Facility Effects

### Growth Rate Modification

| Facility Rating | Stat Growth | Tag Acquisition | Injury Risk |
|-----------------|-------------|-----------------|-------------|
| **Elite (5)** | +35% | +40% faster | -25% |
| **Excellent (4)** | +20% | +25% faster | -15% |
| **Good (3)** | +10% | +10% faster | -5% |
| **Basic (2)** | Baseline | Baseline | Baseline |
| **Poor (1)** | -15% | -20% slower | +15% |

### Available Training Focus

| Facility Rating | Focus Options |
|-----------------|---------------|
| **Elite** | All styles, all specializations |
| **Excellent** | Most styles, core specializations |
| **Good** | Home style focus, limited specializations |
| **Basic** | Fundamentals only |
| **Poor** | Self-directed, gaps in training |

---

## Notable Facilities (Ringstate Canon)

### Elite Tier

**NJPW Dojo (Tokyo)**
- Philosophy: Traditional dojo
- Specialty: Strong style, psychology, toughness
- Notable Alumni: Generation of main eventers
- Quality: 5/5

**WWE Performance Center (Orlando)**
- Philosophy: Corporate pipeline
- Specialty: Entertainment, character, promos
- Notable Alumni: Modern main roster
- Quality: 5/5

**Miss Mitsuko's NSP Women's Division (Tokyo)**
- Philosophy: Traditional dojo with idol presentation
- Specialty: Joshi fundamentals, pop presentation
- Notable Alumni: NSP women's roster
- Quality: 5/5 (brutal but effective)

### Excellent Tier

**Starlight Wrestling Association Men's (Tokyo)**
- Philosophy: Hybrid (corporate with Japanese rigor)
- Specialty: Junior heavyweight, athletic presentation
- Quality: 4/5

**Various CCA Territory Schools**
- Philosophy: Traditional wrestling
- Specialty: Varies by territory
- Quality: 3-4/5 (varies)

### Specialized Tier

**Frontier Real Fight Dojo (Kyoto)**
- Philosophy: Shootstyle combat
- Specialty: Legitimate fighting, minimal performance
- Quality: 4/5 (for shootstyle)
- Note: Produces specialists, not all-rounders

---

## Facility Improvement

### Promotion Investment
- Facilities can be upgraded over time
- Requires financial investment
- Hiring better trainers raises quality
- Equipment upgrades provide incremental gains

### Reputation Building
- Successful alumni raise facility prestige
- Failed students damage reputation
- Guest trainers temporarily boost quality
- Alumni returning to teach elevates status

---

## Facility Selection Impact

### Worker Generation
- Workers generated from elite facilities start with higher floors
- Facility tags applied: "NJPW Dojo Product", "WWE PC Graduate"
- Facility philosophy shapes initial Hidden Personality

### Career Development
- Workers training at better facilities during career improve faster
- Changing facilities (via promotion move) affects growth
- Elite facility access may be contract perk

---

## Connected Mechanics

- [[Training Philosophy Types]] - Facility embodies philosophy
- [[Skill Growth Mechanics]] - Facility modifies growth rate
- [[Mentor System]] - Facility provides mentor pool
- [[Tag Acquisition Through Training]] - Facility determines available tags

---

## Open Questions

- [ ] Exact formula for facility quality calculation
- [ ] How does facility quality affect potential ceiling?
- [ ] Cross-training at multiple facilities?
- [ ] Facility rivalry mechanics (graduates clash)?

---

## Implementation Notes

```json
{
  "training_facility": {
    "facility_id": "FAC_001",
    "name": "NJPW Dojo",
    "location": "Tokyo, Japan",
    "quality_rating": 5,
    "philosophy": "traditional_dojo",
    "specialty_styles": ["Strong Style", "Puroresu", "Psychology"],
    "head_trainer": {
      "worker_id": "WORK_TRAINER",
      "prestige": 18
    },
    "effects": {
      "growth_modifier": 0.35,
      "tag_acquisition_modifier": 0.40,
      "injury_risk_modifier": -0.25
    },
    "available_focuses": [
      "technical",
      "striking",
      "psychology",
      "strong_style",
      "selling"
    ],
    "current_trainees": 12,
    "capacity": 20,
    "notable_alumni": ["WORK_ALUMNI_1", "WORK_ALUMNI_2"]
  }
}
```

---

**Document Status:** Exploratory (concepts documented, formulas TBD)
**Last Updated:** 2025-12-21
