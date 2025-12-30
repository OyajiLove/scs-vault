# Wear and Tear System

📛 **MECHANIC:** Wear and Tear Memory
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** bumps, accumulated damage, style wear, recovery, silent deterioration
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Not every injury shows on TV. Wear and tear accumulates silently over careers, degrading performance before visible injuries occur. Workers can seem "fine" but lose half-steps: slower movement, sloppier execution, lower stamina, hidden chronic pain.

---

## Core Mechanics

### Accumulated Bumps Counter
Tracks rough estimate of hard bumps, falls, dangerous moves over career.

| Counter Type | What It Tracks |
|--------------|----------------|
| **Total Bumps** | All bumps taken across career |
| **High-Impact Bumps** | Particularly dangerous bumps (powerbombs, piledrivers, table spots) |
| **Style-Specific Counters** | Body part wear based on wrestling style |

### Style-Specific Wear Counters

Different styles destroy different body parts:

| Style | Primary Wear Zones | Examples |
|-------|-------------------|----------|
| **High-Flyer** | Knees, hips, lower back | Hayabusa, Sabu |
| **Deathmatch** | Blood loss, scarring, infection risk | Mick Foley, Nick Gage |
| **Strong Style** | Neck, spine, brain trauma | Misawa, Kobashi, Shibata |
| **Power/Hoss** | Lower back, shoulders, knees | Vader, Hansen |
| **Technical/Mat** | Shoulders, elbows, neck | Bret Hart, Angle |
| **Old School/Brawler** | Shoulders, hands, forehead | Flair, Dusty |

---

## Recovery Efficiency

Workers with high Athleticism + Drive + Durability recover faster between matches. Others degrade.

```
Recovery Efficiency = (Athleticism + Durability + Age Modifier) / 3

Where:
- Athleticism: 1-20 worker stat
- Durability: 1-20 worker stat
- Age Modifier: 
  - 20s = +5
  - 30s = 0
  - 40s = -5
  - 50s = -10
```

---

## Silent Deterioration

Workers can seem "fine" but suffer hidden degradation:

| Symptom | Effect |
|---------|--------|
| **Slower Movement** | Reduced speed in matches |
| **Sloppier Execution** | Higher botch chance |
| **Lower Stamina** | Match quality drops in longer matches |
| **Hidden Chronic Pain** | Morale penalty, painkiller usage temptation |

### Deterioration Threshold
```
If Style-Specific Wear > 70% of body part threshold:
  → Silent Deterioration begins
  → Worker loses half-steps
  → Not visible to player until match quality drops noticed
```

---

## Wear Curve by Age

| Age Range | Recovery Speed | Healing Quality | Notes |
|-----------|----------------|-----------------|-------|
| **20s** | Fast | Full recovery common | Peak physical years |
| **Early 30s** | Moderate | Minor permanent damage possible | Prime years but wear showing |
| **Late 30s** | Slow | Permanent damage likely | Style adaptation critical |
| **40s** | Very slow | Always some permanent loss | Survival mode |
| **50s** | Minimal | Every bump costs | Legend status or tragic shell |

---

## Bump Types and Weight

| Bump Type | Wear Points | Notes |
|-----------|-------------|-------|
| **Standard Bump** | 1 | Basic flat back |
| **Turnbuckle Bump** | 2 | Corner impact |
| **Apron Bump** | 3 | "Hardest part of the ring" |
| **Floor Bump** | 4 | Outside concrete/mats |
| **Table Spot** | 5-8 | Depending on height/break |
| **Ladder/Cage Fall** | 8-15 | Extreme height, extreme cost |
| **Piledriver/Powerbomb** | 3-6 | Neck/spine compression |
| **Headbutt (Taken)** | 4-7 | Brain trauma risk |

---

## Match Volume Impact

High match counts accelerate wear:

| Monthly Match Count | Wear Multiplier |
|--------------------|-----------------|
| 1-4 matches | 1.0x (baseline) |
| 5-10 matches | 1.2x |
| 11-20 matches | 1.5x |
| 20+ matches | 2.0x (tour schedule, territory pace) |

---

## Rest Recovery (Vol 1 Merge)

Time off allows wear reduction:

| Rest Duration | Recovery Rate |
|---------------|---------------|
| 1 week | -2 to -5 wear per region |
| 1 month | -10 to -20 wear per region |
| 3 months | -30 to -50 wear per region |

Recovery modified by:
- Age (younger = faster)
- Recovery Efficiency stat
- Lifestyle choices (clean living vs. partying)

---

## Permanent Damage Thresholds (Vol 1 Merge)

Some wear cannot be fully repaired:

| Threshold | Permanent Effect |
|-----------|------------------|
| Region hit 90+ | Minimum 30 wear permanently |
| Region hit 100 | Minimum 50 wear permanently |
| Multiple surgeries | Diminishing returns on each repair |

### Surgery Wear Reset

| Surgery Type | Wear Reset | Recovery Time |
|--------------|------------|---------------|
| Minor (scope) | Reset to 40 wear | 2-3 months |
| Major (reconstruction) | Reset to 20 wear | 6-12 months |
| Experimental | Variable results | Variable |

---

## Connected Mechanics

- [[Injury Types]] - Wear thresholds trigger chronic injuries
- [[Style Adaptation]] - Smart workers shift before breakdown
- [[Addiction Risk System]] - Pain management for accumulated wear
- [[Worker Skills]] - Durability, Athleticism affect recovery

---

## Open Questions

- [ ] Exact threshold values for body part deterioration
- [ ] How wear visibility works for player (hints vs. hidden)
- [ ] Match type modifiers (hardcore match = 2x wear?)
- [ ] Training/conditioning mechanics that slow wear

---

## Implementation Notes

```json
{
  "wear_and_tear": {
    "worker_id": "worker_001",
    "total_bumps": 4500,
    "high_impact_bumps": 890,
    "monthly_match_average": 12,
    "style_wear_counters": {
      "neck": { "current": 45, "threshold": 100 },
      "back": { "current": 62, "threshold": 100 },
      "knees": { "current": 78, "threshold": 100 },
      "shoulders": { "current": 35, "threshold": 100 },
      "head": { "current": 28, "threshold": 80 }
    },
    "recovery_efficiency": 0.72,
    "silent_deterioration": {
      "active": true,
      "affected_areas": ["knees"],
      "performance_penalty": -8
    }
  }
}
```
