# Lucha Booking Culture

📛 **MECHANIC:** Lucha Booking Culture / Lucha Politics System
🔗 **PARENT SYSTEM:** [[Booking_Engine_P1-3|Booking Engine]]
🧭 **CATEGORY:** Regional Booking / Cultural Mechanics
🔑 **KEYWORDS:** lucha libre, CMLL, AAA, mask match, family protection, no yob, booking negotiation
📌 **ORIGIN:** Vol 1 Extraction #30, #241
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Lucha libre operates under different cultural rules than American or Japanese wrestling. The booking engine must account for unique Mexican wrestling traditions, family dynasties, mask significance, and worker negotiation expectations.

---

## Special Mechanics

### Family Protection Tag (#241)

**Effect:** Workers with strong family legacies (dynasties like Casas, Guerrero, Santo) are harder to book jobbing.

| Situation | Modifier |
|-----------|----------|
| Clean jobber loss | Strong resistance |
| Competitive loss | Mild resistance |
| Title loss (respected) | Acceptable |
| Mask loss | Requires major negotiation |

**Examples:** 
- La Dinastía Muñoz (Casas family)
- Los Guerreros
- Santo/Blue Demon dynasties

---

### No Yob Clause (Refusal to Job)

**Definition:** Some workers have contractual or personality-based refusal to lose cleanly.

| Clause Level | Effect |
|--------------|--------|
| **Soft No Yob** | Will lose, but only to top stars |
| **Hard No Yob** | Refuses to lose clean except in special circumstances |
| **Absolute No Yob** | Will walk before jobbing (rare, legends only) |

**Negotiation Required:** Must offer compensation (money, future push, title shot) to get clean loss.

---

### Regional Loyalty

**Effect:** Workers may refuse to work in rival territories or for rival promotions.

| Factor | Impact |
|--------|--------|
| CMLL vs AAA feud | Workers may refuse to appear for "enemy" |
| Family ties | Loyalty to family's traditional promotion |
| Personal grudges | Historical issues affect booking availability |

---

### Mask Loss Sensitivity

**Mechanism:** Mask matches are the most sacred stipulation in lucha.

| Scenario | Requirement |
|----------|-------------|
| Proposing mask match | Worker must be consulted |
| Mask loss decision | Major negotiation, often career-altering |
| Mask recovery | Generally impossible (kayfabe) |
| Unmasking without match | FORBIDDEN, nuclear heat |

**Booking Negotiation Screen:** Special interface for proposing mask matches with top masked workers.

---

## Lucha Politics System (#241)

### Booking Negotiation Engine

For major matches involving top luchadors:

```
Negotiation Factors:
- Worker's Ego stat
- Worker's Family Protection tag
- No Yob clause level
- Current push status
- Historical relationship with opponent
- Mask/hair stakes
- Financial compensation offered
- Promise of future booking
```

### Negotiation Outcomes

| Result | Description |
|--------|-------------|
| **Accepted** | Worker agrees to booking |
| **Conditional** | Worker wants changes (finish, time, protection) |
| **Refused** | Worker declines, must rebook |
| **Walkout** | Relationship damaged, may leave promotion |

---

## Era Sensitivity

### Traditional Era (Pre-2000)

- Mask matches extremely rare and protected
- Family dynasties respected absolutely
- CMLL monopoly = stable politics
- Worker movement rare

### Modern Era (2000+)

- AAA emergence creates talent wars
- Mask matches more frequent (some say devalued)
- Indie scene creates alternative paths
- Social media affects negotiations

---

## Implementation Notes

```json
{
  "worker_id": "negro_casas",
  "lucha_politics": {
    "family_protection": true,
    "family_name": "Casas",
    "no_yob_level": "soft",
    "regional_loyalty": "CMLL",
    "mask_status": "unmasked",
    "negotiation_difficulty": 0.7,
    "traditional_values": 0.9
  }
}
```

---

## Connected Mechanics

- [[Booking_Engine_P1-3]] - Core booking systems
- [[Contract System/_Contract System Index|Contract System]] - Negotiation mechanics
- [[Hidden_Personality]] - Ego and loyalty traits
- [[Archetypes/Lucha_Archetypes|Lucha Archetypes]] - Técnico/Rudo dynamics

---

## Open Questions

- How does mask value depreciate with frequent mask matches?
- Inter-generational feuds: how long do dynasty grudges last?
- Talent sharing between CMLL/AAA in modern era?

---

**Document Status:** Concept Locked
**Last Updated:** 2024-12-23
