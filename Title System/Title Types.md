# Title Types

📛 **MECHANIC:** Championship Classification System
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Promotion
🔑 **KEYWORDS:** world title, secondary title, tag titles, junior title, specialty belt, TV title
📌 **ORIGIN:** Vol 1-4 (Specialty title traits, title hierarchy)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Different title types serve different purposes in a promotion's ecosystem. World titles anchor the main event scene, secondary titles showcase workhorses, tag titles drive team divisions, and specialty titles create unique opportunities. Each type has different prestige ceilings, booking expectations, and fan engagement patterns.

---

## Title Hierarchy

| Tier | Title Types | Purpose |
|------|-------------|---------|
| **Tier 1** | World Heavyweight, Universal | Promotion's crown jewel; main event anchor |
| **Tier 2** | Secondary (IC, US, National) | Workhorse belt; upper midcard |
| **Tier 3** | Tag Team, Women's, Junior | Division flagships |
| **Tier 4** | TV, Hardcore, Specialty | Niche appeal; frequent defenses |
| **Tier 5** | Comedy, 24/7, Internet | Low stakes; entertainment focused |

---

## Title Type Details

### World Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Defines the promotion's top star |
| **Prestige Ceiling** | 100 |
| **Defense Frequency** | Monthly at major shows |
| **Champion Profile** | Top stars, draws, ace-level workers |
| **Match Expectations** | Main event, long matches, clean-ish finishes |
| **Reign Expectations** | 3-12 months typical; dynasties possible |

### Secondary Championship (IC/US Tier)

| Aspect | Details |
|--------|---------|
| **Purpose** | Workhorse belt; elevates upper midcard |
| **Prestige Ceiling** | 85 |
| **Defense Frequency** | 2-4 times per month |
| **Champion Profile** | Workers with great matches; future main eventers |
| **Match Expectations** | Strong work; can be MOTN |
| **Reign Expectations** | 2-6 months typical |
| **Historic Examples** | WWF IC Title under Perfect, Steamboat; US Title under Cena |

### Tag Team Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Anchor tag division; showcase teamwork |
| **Prestige Ceiling** | 80 (depends on division strength) |
| **Defense Frequency** | 1-3 times per month |
| **Champion Profile** | Established teams with chemistry |
| **Match Expectations** | Team storytelling; hot tags; drama |
| **Reign Expectations** | 2-6 months typical |
| **Special Rules** | Freebird Rule option for stables |

### Women's Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Top of women's division |
| **Prestige Ceiling** | 85-100 (era-dependent) |
| **Defense Frequency** | Monthly at major shows |
| **Champion Profile** | Best women's workers available |
| **Match Expectations** | Varies by era; modern = main event caliber |
| **Reign Expectations** | Similar to men's equivalent tier |
| **Era Notes** | Pre-2015: often comedy/eye candy; Post-2015: serious competition |

### Junior/Cruiserweight Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Showcase high-flying, technical wrestling |
| **Prestige Ceiling** | 75 |
| **Defense Frequency** | 2-3 times per month |
| **Champion Profile** | Smaller, athletic workers; style specialists |
| **Match Expectations** | Fast-paced, athletic showcases |
| **Reign Expectations** | 1-4 months typical |
| **Weight Limit** | Often 220 lbs or similar |

### TV Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Guaranteed weekly defenses; workhorse belt |
| **Prestige Ceiling** | 70 |
| **Defense Frequency** | Weekly or bi-weekly |
| **Champion Profile** | Reliable workers who can go every week |
| **Match Expectations** | Shorter, tighter TV matches |
| **Reign Expectations** | 1-3 months typical; high defense count |
| **Time Limit** | Often 10-15 minute limit |

### Hardcore/Specialty Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Violence showcase; niche appeal |
| **Prestige Ceiling** | 60 |
| **Defense Frequency** | Variable; often chaotic |
| **Champion Profile** | Brawlers, deathmatch workers, pain specialists |
| **Match Expectations** | Weapons, blood, spectacle |
| **Reign Expectations** | Short to medium; hot potato acceptable |
| **Special Rules** | Falls Count Anywhere, 24/7 variants |

### Trios Championship

| Aspect | Details |
|--------|---------|
| **Purpose** | Showcase stable warfare; lucha tradition |
| **Prestige Ceiling** | 70-80 |
| **Defense Frequency** | 1-2 times per month |
| **Champion Profile** | Established trios with chemistry |
| **Match Expectations** | Six-man tag storytelling |
| **Reign Expectations** | 2-4 months typical |
| **Freebird Rule** | Common; any three from stable |

---

## Regional Title Traditions

| Region | Title Preferences |
|--------|-------------------|
| **US (Territory)** | World, TV, Tag; regional prestige |
| **US (National)** | World, Secondary, Tag, Women's, specialty |
| **Japan** | Heavyweight, Junior, Tag; strict hierarchy |
| **Mexico** | Trios central; masks > belts sometimes |
| **UK** | World of Sport tradition; technical focus |

---

## Title Traits (Special Modifiers)

Some titles have special characteristics:

| Trait | Effect |
|-------|--------|
| **Travelling Champion** | Defends across multiple promotions |
| **Defended Weekly** | TV title style; high frequency |
| **Weight Limit** | Junior/cruiserweight restrictions |
| **Freebird Eligible** | Stable members can rotate |
| **Falls Count Anywhere** | Hardcore/24/7 style |
| **Time Limit Draw Risk** | TV title or strong style format |
| **Mask vs. Title** | Lucha tradition; apuestas eligible |

---

## Creating New Titles

When promotions create new championships:

| Factor | Effect |
|--------|--------|
| **Tournament** | +10 to +15 initial prestige |
| **Inaugural Champion** | Quality of first holder sets tone |
| **Belt Design** | Visual prestige matters |
| **Booking Consistency** | Early treatment determines trajectory |
| **Division Strength** | Weak division = weak title |

---

## Connected Mechanics

- [[Title Prestige]] - Each type has different ceiling
- [[Title Run Dynamics]] - Different expectations by type
- [[Faction System]] - Freebird rule for stables
- [[Worker Skills]] - Different types favor different skills

---

## Open Questions

- [ ] Weight limit enforcement mechanics
- [ ] Title unification procedures
- [ ] Inter-promotional title recognition
- [ ] Creating custom title types
- [ ] Title retirement/deactivation

---

## Implementation Notes

```json
{
  "title_type_config": {
    "type": "secondary",
    "prestige_ceiling": 85,
    "defense_frequency_expected": "bi-weekly",
    "champion_tier_expected": "upper_midcard",
    "reign_length_expected": {
      "min_months": 2,
      "max_months": 6
    },
    "traits": ["workhorse_belt"],
    "special_rules": [],
    "weight_limit": null,
    "freebird_eligible": false
  }
}
```
