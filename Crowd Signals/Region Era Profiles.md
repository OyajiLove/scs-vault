# Region Era Profiles

📛 **MECHANIC:** Region Era Profiles
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** region profiles, era profiles, crowd culture, Japan crowds, Mexico crowds, territory crowds
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

How crowds behave by location and time period. Chant styles, emotional expressions, and acceptable behaviors vary dramatically. This mechanic gates which [[Signal Types]] are available in any given context.

---

## US/Canada

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **1980s** | Loud boo/cheer waves, name chants ("Hogan! Hogan!") | Unironic, tribal, patriotic |
| **1990s** | "You screwed Bret," "ECW," anti-heel eruptions | Emotional, grudge-driven |
| **2000s** | "Let's go Cena / Cena sucks," "This is awesome" emerges | Split loyalty, crowd identity rising |
| **2010s-Now** | "You deserve it," ironic chants, troll noise | Hyper-aware, attention-seeking |

---

## Japan

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **1980s-2000s** | Silence, isolated first-name chants, claps | Deep respect, only major stars get chants |
| **2010s-Now** | Slight increase in callouts (Tanahashi, Ibushi) | Still restrained, rarely sarcastic |

---

## Mexico

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **Any** | Chant duels, "Santo! Santo!", region-based calls | Passionate, familial, tradition-rooted |

---

## UK/Europe

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **2010s-Now** | Football-style chants, singalongs | Communal, cheeky, genre-aware |

---

## Joshi Puro

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **1980s-Now** | Full-name chants, crying kids, ritual applause | Fierce loyalty, rarely ironic, emotional edge |

---

## Territory (US)

| Era | Chant Style | Personality |
|-----|-------------|-------------|
| **1970s-80s** | "Kick his ass," "Don't take no shit" | Bluster, aggression, working-class catharsis |

---

## Tone Enforcement

| Tone | Description | Era/Region Lock |
|------|-------------|-----------------|
| **Earnest** | Loyal, direct, not mocking | 1980s US, Territory |
| **Tribal** | Identity, face-heel allegiance | All eras, strongest in Mexico |
| **Ironic** | Booing good guy, chanting nonsense | 2000s+ US/UK |
| **Ritualized** | Stylized respect, not pop | Japan, Joshi |
| **Mocking** | "What?" chants derailing promos | 2000s+ US/UK |

---

## Hard Rules

- "This is awesome" won't happen in 80s Crockett or 90s AJPW
- Modern lucha may chant "rudo" but not ironic pop-fests
- Joshi at Korakuen = full-name chant or total silence unless legend involved
- Modern US = 50/50 crowds, "You deserve it," "Fight forever," "We want [someone else]"

---

## Connected Mechanics

- [[Signal Types]] - profiles determine which signals fire
- [[Ceremony Responses]] - regional ceremony expectations
- [[Garbage Throwing]] - region/era gated behavior
- [[Heat vs Hate]] - modern paradox most relevant in US/UK

---

## Open Questions

- Hybrid region handling (US show with heavy Japanese fanbase)
- Era transition periods (when does 90s become 2000s for crowd behavior?)
- Touring promotion adaptation (NJPW in US uses which profile?)

---

## Implementation Notes

```json
{
  "region_era_profile": {
    "region": "us_northeast",
    "era": "2010s",
    "tone_primary": "ironic",
    "tone_secondary": "tribal",
    "available_signals": ["unprompted_chant", "ritual_chant", "angry_chant", "this_is_awesome", "thank_you"],
    "blocked_signals": ["honor_clap", "silent_reverence"],
    "garbage_throwing_enabled": false,
    "heel_drift_susceptibility": 0.75
  }
}
```
