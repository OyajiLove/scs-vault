# Title Prestige

📛 **MECHANIC:** Title Prestige System
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Promotion
🔑 **KEYWORDS:** prestige, belt value, championship importance, title heat, credibility
📌 **ORIGIN:** Vol 1-4 (Title prestige decay, hot/cold titles)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Title prestige is a dynamic rating that reflects how much fans care about a championship. Hot titles massively boost match importance; dead titles actively drag matches down even if the workers perform well. Prestige must be actively maintained through quality booking.

---

## Prestige Scale

| Range | Status | Description |
|-------|--------|-------------|
| 90-100 | **Legendary** | Every defense is must-see; title defines promotion |
| 75-89 | **Hot** | Fans deeply invested; strong match boost |
| 60-74 | **Warm** | Solid credibility; moderate positive effect |
| 40-59 | **Neutral** | Exists but doesn't excite; no modifier |
| 20-39 | **Cold** | Fans losing interest; slight negative |
| 0-19 | **Dead** | Joke title; actively hurts matches |

---

## Prestige Factors

### What Builds Prestige

| Factor | Effect |
|--------|--------|
| **Quality Defenses** | Great matches boost prestige |
| **Credible Champions** | Popular, skilled champions add value |
| **Clean Finishes** | Decisive victories build legitimacy |
| **Long, Meaningful Reigns** | Dynasty runs create prestige (if maintained) |
| **Hot Feuds** | Emotional stakes elevate title importance |
| **Major Show Defenses** | PPV/big event matches add weight |
| **Historic Lineage** | Prestigious history carries forward |

### What Damages Prestige

| Factor | Effect |
|--------|--------|
| **Hot Potato Booking** | Frequent changes tank credibility |
| **Weak Champions** | Unbelievable holders devalue title |
| **Dusty Finishes** | DQ/countout endings erode faith |
| **Cold Feuds** | Uninteresting programs drag title down |
| **Overexposure** | Too many defenses without stakes |
| **Comedy Booking** | Joke segments, gimmick matches |
| **Vacancy** | Extended periods without champion |

---

## Prestige Decay Over Time

Titles naturally lose prestige without active maintenance:

| Scenario | Monthly Decay |
|----------|---------------|
| **No defenses, no storyline** | -3 to -5 |
| **Weak defenses (bad matches)** | -2 to -4 |
| **Champion absent (injury, etc.)** | -2 |
| **Hot potato period** | -5 to -10 per extra change |
| **Strong defense (great match)** | +2 to +5 |
| **Classic defense (MOTY candidate)** | +5 to +10 |

---

## Champion Quality Impact

Who holds the title matters:

| Champion Type | Prestige Effect |
|---------------|-----------------|
| **Legendary Draw** | +10 to +20 base boost |
| **Established Star** | +5 to +10 |
| **Rising Star (earned)** | Neutral to +5 |
| **Unproven Push** | -5 to -10 (until proven) |
| **Transitional Champion** | -5 (short-term) |
| **Joke/Comedy Champion** | -10 to -20 |

---

## Title Prestige by Type

Different title types have different prestige ceilings:

| Title Type | Prestige Ceiling | Notes |
|------------|------------------|-------|
| **World Title** | 100 | Promotion's crown jewel |
| **Secondary Title** | 85 | IC/US tier, workhorse belt |
| **Tag Team Title** | 80 | Depends on tag division strength |
| **Women's Title** | 85-100 | Era-dependent ceiling |
| **Junior/Cruiserweight** | 75 | Style showcase belt |
| **TV/Midcard Title** | 70 | Frequent defense format |
| **Specialty (Hardcore, etc.)** | 60 | Niche appeal |
| **Comedy Title** | 30 | Intentionally low |

---

## Prestige Recovery

Rebuilding damaged prestige:

| Method | Effect | Time Required |
|--------|--------|---------------|
| **Tournament for vacant title** | +10 to +15 | Immediate |
| **Credible new champion** | +5 to +10 | 1-2 months |
| **Classic defense** | +5 to +10 | Per match |
| **Hot feud program** | +10 to +20 | 2-4 months |
| **Rebranding/new belt design** | +5 (temporary) | Immediate, fades |

---

## Era Impact on Prestige

| Era | Prestige Dynamics |
|-----|-------------------|
| **Territory** | Titles meant everything; slow changes |
| **National TV** | Prestige spread wider; more eyes |
| **Monday Night Wars** | Hot potato periods damaged prestige |
| **Modern** | Oversaturation of titles; harder to maintain |

---

## Connected Mechanics

- [[Title Run Dynamics]] - How reigns affect prestige
- [[Hot Potato Risk]] - Frequent changes destroy prestige
- [[Crowd Memory]] - Fans remember title moments
- [[Match Rating]] - Prestige modifies match perception

---

## Open Questions

- [ ] Exact formula for prestige calculation
- [ ] How prestige transfers during unification
- [ ] Lineage prestige inheritance (new titles from old)
- [ ] Cross-promotion prestige recognition

---

## Implementation Notes

```json
{
  "title_prestige": {
    "title_id": "title_001",
    "current_prestige": 82,
    "prestige_history": [
      { "date": "1985-01-01", "value": 75 },
      { "date": "1985-06-01", "value": 82 }
    ],
    "factors": {
      "champion_quality": +8,
      "defense_quality": +5,
      "feud_heat": +3,
      "time_decay": -2,
      "hot_potato_penalty": 0
    },
    "trend": "rising",
    "ceiling": 100,
    "floor": 40
  }
}
```
