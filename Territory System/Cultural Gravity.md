# Cultural Gravity

📛 **MECHANIC:** Cultural Gravity / Style Drift Resistance
🔗 **PARENT SYSTEM:** [[_Territory System Index|Territory System]]
🧭 **CATEGORY:** Promotion Identity
🔑 **KEYWORDS:** cultural gravity, style drift, promotion identity, brand inertia, style change
📌 **ORIGIN:** Vol 1 Extraction #115, HB-10
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Promotions can't change their style overnight. A strong-style company trying to become a comedy federation faces massive resistance from fans, workers, and its own identity. This is **Cultural Gravity**: the accumulated expectations and traditions that define a promotion.

---

## Core Concept

Every promotion has a **Style DNA** that defines its cultural gravity:

```
Style Change Difficulty = Cultural Gravity × (Style Distance) × (Time Factor)
```

The longer a promotion has existed with a certain style, the harder it is to change.

---

## Style DNA Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Primary Style** | Dominant wrestling approach | Strong Style, Lucha, Sports Entertainment |
| **Secondary Style** | Supporting approach | Technical, Hardcore, Comedy |
| **Production Values** | Presentation level | Big budget, indie, underground |
| **Kayfabe Level** | How seriously treated | Strict, loose, ironic |
| **Violence Tolerance** | Blood/hardcore acceptance | Family-friendly, adult, deathmatch |
| **Workrate Expectation** | Match quality standards | High, moderate, spectacle-focused |

---

## Cultural Gravity Levels

| Level | Change Difficulty | Examples |
|-------|-------------------|----------|
| **Extreme (90+)** | Near impossible | NJPW Strong Style, CMLL Lucha Tradition |
| **High (70-89)** | Very difficult, takes years | AJPW King's Road, Mid-South grit |
| **Moderate (40-69)** | Possible with effort | Most regional promotions |
| **Low (20-39)** | Flexible identity | New promotions, experimental indies |
| **Minimal (0-19)** | No established identity | Startups |

---

## Style Drift Example

**NJPW trying to become GCW:**

1. NJPW Cultural Gravity: 95 (Strong Style locked in)
2. Target: Deathmatch/Outlaw style
3. Style Distance: Massive (different worlds)

**What happens:**
- Fans rebel: "This isn't New Japan"
- Veterans refuse: "I didn't sign up for this"
- Critics pile on: "They've lost their identity"
- Attendance drops
- Takes 5-10 years minimum, if possible at all

**Realistic NJPW style drift:**
- Adding more gaijin workers: Low resistance
- Slightly more comedy: Moderate resistance
- Full deathmatch focus: Near-impossible

---

## Drift Mechanics

### Gradual Drift (Successful)

Small changes over time are more acceptable:

| Change Size | Time Required | Resistance |
|-------------|---------------|------------|
| Subtle tweak | 3-6 months | Low |
| Moderate shift | 1-2 years | Medium |
| Major change | 3-5 years | High |
| Complete reinvention | 5-10 years | Extreme |

### Forced Drift (Risky)

Rapid style changes trigger:
- Fan exodus
- Worker morale collapse
- Critical backlash
- Identity crisis

### Exception: Crisis Events

Major events can enable faster drift:
- Company sale/new ownership
- Exodus of key talent
- Near-bankruptcy
- Cultural moment (Montreal Screwjob → Attitude Era)

---

## Formula Components

### Style Distance

How different is the target style from current style?

| Shift Type | Distance |
|------------|----------|
| Strong Style → More Strikes | 0.1 (minimal) |
| Technical → Lucha influence | 0.3 (moderate) |
| Sports Entertainment → Workrate | 0.5 (significant) |
| Family-friendly → Hardcore | 0.8 (major) |
| Strong Style → Comedy | 1.0 (complete opposite) |

### Time Factor

How long has promotion held current identity?

| Years | Modifier |
|-------|----------|
| 0-2 | 0.5x (still forming) |
| 3-5 | 1.0x (established) |
| 6-10 | 1.5x (entrenched) |
| 11-20 | 2.0x (deep tradition) |
| 20+ | 3.0x (cultural institution) |

---

## Fan Expectations by Style

| Style | Fans Expect |
|-------|-------------|
| **Strong Style** | Hard strikes, fighting spirit, grueling matches |
| **Lucha Libre** | High flying, mask tradition, técnico/rudo morality |
| **Sports Entertainment** | Characters, promos, spectacle over workrate |
| **Shoot Style** | Realism, submissions, legitimacy |
| **Hardcore** | Blood, weapons, pain tolerance |
| **Comedy** | Laughs, absurdity, not taking itself seriously |
| **Technical** | Chain wrestling, mat work, in-ring excellence |

---

## Connected Mechanics

- [[Regional Identity]] - Geographic style traditions
- [[Regional Crowd Behavior]] - How crowds respond to style
- [[Gimmick System/_Gimmick System Index|Gimmick System]] - Character fit within style
- [[Booking_Engine_P1-3]] - Era-Sensitive Fan Logic

---

## Implementation Notes

```json
{
  "promotion_id": "njpw",
  "style_dna": {
    "primary": "strong_style",
    "secondary": "puroresu_tradition",
    "production": "high_budget",
    "kayfabe": "moderate",
    "violence": "stiff_not_bloody",
    "workrate": "elite"
  },
  "cultural_gravity": 95,
  "years_established": 52,
  "drift_attempts": [
    {
      "year": 2016,
      "target": "more_western_appeal",
      "distance": 0.2,
      "success": "moderate",
      "time_taken": 3
    }
  ]
}
```

---

## Open Questions

- Can new ownership reset cultural gravity?
- How do worker rosters affect style expectations?
- Does TV deal type affect style flexibility?

---

**Document Status:** Concept Locked, Details Open
**Last Updated:** 2024-12-23
