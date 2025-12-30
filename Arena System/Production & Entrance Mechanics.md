# Production & Entrance Mechanics

📛 **MECHANIC:** Show Production and Entrance Presentation
🔗 **PARENT SYSTEM:** [[_Arena System Index|Arena System]]
🧭 **CATEGORY:** Show Presentation / Budget
🔑 **KEYWORDS:** production, entrance, pyro, stage, LED, budget, atmosphere, ring apron
📌 **ORIGIN:** Vol 1 Extraction #127
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #127 | 🔒 LOCKED (concept) |

---

## Overview

Production quality affects show atmosphere, fan expectations, and worker presentation. From pyro to LED stages to custom ring aprons, every element costs money and shapes perception. Fans notice when big feds cheap out, and forgive indie promotions for sparse setups.

---

## Core Concept

"Big entrance pyros only if you pay for it in production budget."

Production isn't just cosmetic: it affects how seriously fans take your promotion and how impactful worker entrances feel.

---

## Production Elements

| Element | Cost Level | Effect |
|---------|------------|--------|
| **Pyro** | High | Spectacular entrances, main event feel |
| **LED Screens** | High | Modern presentation, video packages |
| **Custom Stage** | Medium-High | Unique identity, memorable set |
| **Entrance Ramp** | Medium | Professional presentation |
| **Ring Aprons** | Low | Branding, customization |
| **Entrance Music** | Low | Identity, crowd reaction triggers |
| **Lighting Rig** | Medium | Atmosphere, dramatic moments |
| **Sound System** | Medium | Audio quality, crowd engagement |

---

## Budget Tiers

### Low-Budget Federation

| Characteristic | Effect |
|----------------|--------|
| **Fan Expectations** | Low, they don't punish sparse setups |
| **Production Quality** | Basic lighting, simple stage |
| **Pyro** | None or sparklers |
| **Media Perception** | "Indie charm" or "bush league" depending on execution |

### Mid-Budget Federation

| Characteristic | Effect |
|----------------|--------|
| **Fan Expectations** | Moderate, want decent presentation |
| **Production Quality** | Professional but not spectacular |
| **Pyro** | Special occasions only |
| **Media Perception** | Respectable, growing operation |

### Big Federation (Cheaping Out)

| Characteristic | Effect |
|----------------|--------|
| **Fan Expectations** | High, they notice cuts |
| **Production Quality** | Below expected standards |
| **Pyro** | Missing or reduced |
| **Media Perception** | "They're cutting corners" articles, fan complaints |

### Premium Production

| Characteristic | Effect |
|----------------|--------|
| **Fan Expectations** | Very high, this is the standard |
| **Production Quality** | Industry-leading |
| **Pyro** | Prominent, signature entrances |
| **Media Perception** | "Big league" presentation |

---

## Budget Impact on Perception

| Budget Level | Meets Expectations | Below Expectations |
|--------------|-------------------|-------------------|
| **Indie** | Neutral | Minor negative |
| **Regional** | Positive | Moderate negative |
| **National** | Expected | Major negative |
| **Premium** | Very positive | Catastrophic negative |

---

## Venue Atmosphere

AI-generated or preset arena visuals by tier:

| Venue Size | Visual Characteristics |
|------------|----------------------|
| **Small** (Armories, Bingo Halls) | Intimate, raw, underground feel |
| **Medium** (Civic Centers) | Professional, regional TV quality |
| **Big** (Arenas) | Polished, network presentation |
| **Stadium** | Spectacle, blockbuster production |

---

## Customization Options

Players can customize:

| Element | Options |
|---------|---------|
| **Stage Design** | Templates or custom layouts |
| **Ring Aprons** | Fed logo, event branding, sponsor logos |
| **Entrance Sets** | Titantron style, LED configuration |
| **Worker Entrances** | Pyro type, lighting cues, special effects |
| **Event Themes** | PPV-specific designs, seasonal variations |

---

## Production Budget Allocation

| Category | Typical % of Show Budget |
|----------|-------------------------|
| **Venue Rental** | 30-40% |
| **Staging/Set** | 15-25% |
| **Pyro/Effects** | 5-15% |
| **Audio/Video** | 10-15% |
| **Lighting** | 5-10% |
| **Miscellaneous** | 5-10% |

---

## Implementation Notes

```json
{
  "show_id": "show_001",
  "production_budget": 50000,
  "production_tier": "mid_budget",
  "elements": {
    "pyro": {
      "enabled": true,
      "cost": 8000,
      "workers_with_pyro": ["worker_001", "worker_015"]
    },
    "stage": {
      "type": "standard_led",
      "cost": 12000
    },
    "lighting": {
      "quality": "professional",
      "cost": 5000
    }
  },
  "fan_expectation_met": true,
  "perception_modifier": 1.0
}
```

---

## Connected Mechanics

- [[Arena Prestige]] - Venue quality affects production expectations
- [[Financial System]] - Production costs affect profit
- [[_Popularity System Index|Popularity]] - Entrance spectacle affects worker presentation
- [[_Gimmick System Index|Gimmick]] - Some gimmicks require production support

---

## Open Questions

- [ ] Exact cost formulas for production elements
- [ ] Worker-specific entrance customization depth
- [ ] Era-appropriate production (no LED in 1985)
- [ ] Production failures (pyro malfunction, audio issues)
- [ ] Sponsor logo placement value

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Design cost formulas, era restrictions
