# Lifestyle Tracker

📛 **MECHANIC:** Lifestyle Tracker / Aging Modifier
🔗 **PARENT SYSTEM:** [[_Health System Index|Health System]]
🧭 **CATEGORY:** Career Longevity / Character Simulation
🔑 **KEYWORDS:** lifestyle, aging, drugs, alcohol, genetics, wear, longevity
📌 **ORIGIN:** Vol 1 Extraction #45
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Workers don't age uniformly. Their lifestyle choices, genetic makeup, and wrestling style all affect how quickly they break down. The Lifestyle Tracker models these factors for realistic career arcs.

---

## Lifestyle Factors

### Negative Factors (Accelerate Decline)

| Factor | Effect | Visual Impact |
|--------|--------|---------------|
| **Heavy Drinker** | Faster decline, worse recovery | Deeper lines, bloated face |
| **Smoker** | Reduced stamina ceiling | Sunken eyes, rough skin |
| **Drug Use (Recreational)** | Erratic decline, health scares | Unpredictable aging |
| **Drug Use (PEDs)** | Initial boost, then crash | Heart issues, joint problems |
| **Hard Lifestyle** | General wear acceleration | "Looks older than age" |
| **Deathmatch Style** | Massive cumulative damage | Visible scarring |
| **Stiff Worker** | Joint/head trauma buildup | Movement issues |

### Positive Factors (Slow Decline)

| Factor | Effect | Visual Impact |
|--------|--------|---------------|
| **Clean Living** | Slower decline curve | Ages gracefully |
| **Good Genetics** | Higher stat ceilings longer | "Natural freak" |
| **Technical Style** | Less bump damage | Longevity |
| **Smart Worker** | Protects self in matches | Fewer injuries |
| **Cross-Training** | Maintains athleticism | Stays in shape |

---

## Genetics/Natural Resistance

**Scar Tissue Variance:**

| Type | Description | Examples |
|------|-------------|----------|
| **Easy Bleeder** | Scars easily, hardway common | Terry Funk |
| **Average** | Normal scarring | Most workers |
| **Resistant** | Rarely scars, heals clean | Giant Baba |

**Physical Durability Variance:**

| Type | Description |
|------|-------------|
| **Ironman** | Recovers faster, works hurt effectively |
| **Average** | Normal injury patterns |
| **Fragile** | Injury prone, longer recovery |

---

## Career Arc Impact

### Young Worker (Under 28)

- Lifestyle effects minimal
- Recovery is fast
- Bad habits accumulating invisibly

### Prime Worker (28-35)

- Lifestyle effects emerging
- Hard living starts showing
- Recovery slowing

### Veteran Worker (35-42)

- Lifestyle effects dominant
- Clean livers vs hard livers diverge dramatically
- Recovery becomes major factor

### Aging Worker (42+)

- Lifestyle is destiny
- Clean livers can still go
- Hard livers broken or dead

---

## Visual Portrait Evolution

Lifestyle factors affect AI-generated portraits over career:

| Factor | Visual Change |
|--------|---------------|
| Drinking | Bloated face, red nose |
| Smoking | Weathered skin, lines |
| Drugs | Erratic weight, sunken features |
| Deathmatches | Forehead scars, missing teeth |
| Clean Living | Maintained appearance |
| Genetics (Good) | "Doesn't age" look |

---

## Implementation Notes

```json
{
  "worker_id": "terry_funk",
  "lifestyle": {
    "drinking": "heavy",
    "smoking": false,
    "drug_use": "none",
    "ped_use": "none",
    "wrestling_style": "hardcore",
    "living_clean": false,
    "genetics": {
      "durability": "ironman",
      "scar_tissue": "easy_bleeder",
      "natural_athlete": false
    }
  },
  "aging_modifier": 1.3,
  "recovery_modifier": 0.7
}
```

---

## Connected Mechanics

- [[Wear and Tear System]] - Cumulative damage
- [[Recovery System]] - Healing rates
- Aging System - Career decline curves
- [[Worker_Skills]] - Stat degradation

---

## Examples

### Terry Funk (Hard Living, Ironman Genetics)

- Heavy lifestyle damage
- But ironman genetics kept him going
- Working into his 70s despite broken body
- Visual: Scarred, weathered, but still moves

### Diamond Dallas Page (Clean Living, Late Bloomer)

- Started late, protected body
- Clean lifestyle extended career
- Developed yoga for recovery
- Visual: Maintained physique into 60s

### Dynamite Kid (Hard Living, Fragile)

- Brutal style + hard living
- Early physical collapse
- Wheelchair by 50s
- Cautionary tale

---

**Document Status:** Concept Locked
**Last Updated:** 2024-12-23
