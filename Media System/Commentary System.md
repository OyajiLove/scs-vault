# COMMENTARY SYSTEM

📛 **NAME:** Commentary System
🧭 **CATEGORY:** Presentation / Atmosphere
🔑 **KEYWORDS:** commentary, announcers, play-by-play, color, broadcast, call, reaction
📝 **SUMMARY:**

The Commentary System governs how matches and segments are presented through announcer voices. Commentary teams have distinct roles (play-by-play, color), skill ratings, chemistry, and era-appropriate styles. Quality commentary enhances the viewing experience and conveys important storyline information.

⚙️ **LOGIC OVERVIEW:**

- Commentary teams have defined roles and skills
- Team chemistry affects broadcast quality
- Era-appropriate commentary styles
- Commentary reflects feuds, history, and psychology
- LLM generates contextual commentary text

🔬 **LLM INTEGRATION:** High (commentary generation, historical callbacks)

📌 **ORIGIN:** Vol 1 Extraction #143

📎 **CONNECTED SYSTEMS:**
- [[Match Engine/_Match Engine Index|Match Engine]] - Commentary on match action
- [[Crowd_Memory]] - Commentary references history
- [[Era System]] - Era affects commentary style
- [[Promo System/_Promo System Index|Promo System]] - Commentary on promos

❓ **OPEN QUESTIONS:**
- Commentary skill rating scale
- Chemistry calculation formulas
- Audio vs. text presentation

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #143 | 🔒 LOCKED (concept) |

---

## COMMENTARY TEAM ROLES (#143)

### Core Roles

| Role | Function | Examples |
|------|----------|----------|
| **Play-by-Play** | Call action, set stakes, guide viewer | Jim Ross, Tony Schiavone |
| **Color** | Add personality, explain psychology, react | Jesse Ventura, Bobby Heenan |
| **Special Guest** | One-off appearances, storyline integration | Manager at ringside, legend cameo |

### Role Responsibilities

| Role | Primary Tasks |
|------|---------------|
| **Play-by-Play** | Move identification, match flow, stakes reminder, time management |
| **Color** | Psychology explanation, character perspective, emotional reaction, heel/face bias |
| **Special Guest** | Storyline advancement, personal stakes, limited duration |

---

## COMMENTARY QUALITY FACTORS

### Announcer Skills

| Skill | Effect |
|-------|--------|
| **Call Quality** | Accuracy and timing of move calls |
| **Storytelling** | Ability to weave narrative into broadcast |
| **Knowledge** | Depth of wrestling history awareness |
| **Chemistry** | How well they work with partners |
| **Adaptability** | Handle unexpected moments |
| **Character Work** | Maintain consistent persona |

### Team Chemistry

| Chemistry Level | Effect |
|-----------------|--------|
| **Legendary** | Elevates entire broadcast, memorable calls |
| **Strong** | Smooth flow, natural interactions |
| **Professional** | Competent but unremarkable |
| **Awkward** | Noticeable tension, poor timing |
| **Disaster** | Actively hurts broadcast |

### Chemistry Factors

| Factor | Effect |
|--------|--------|
| **Time Together** | Longer = better chemistry |
| **Personal Relationship** | Real friendship helps |
| **Style Complementary** | Straight man + character works |
| **Ego Compatibility** | Two big egos = problems |

---

## ERA-APPROPRIATE STYLES

### Commentary Evolution by Era

| Era | Style Characteristics |
|-----|----------------------|
| **Territory (70s-80s)** | Kayfabe strict, sports presentation, local focus |
| **National Expansion** | Character-driven, catch phrases, spectacle emphasis |
| **Attitude Era** | Edgy, fourth-wall teasing, personality clashes |
| **Modern** | Workrate appreciation, social media references, self-aware |

### Regional Variations

| Region | Commentary Style |
|--------|------------------|
| **Japan** | Respectful, move-focused, emotional climax calls |
| **Mexico** | Rapid-fire, dramatic, family audience |
| **US South** | Storytelling emphasis, blood feud history |
| **UK** | Technical appreciation, understatement |

---

## BROADCAST ELEMENTS

### Show Components

| Element | Description |
|---------|-------------|
| **Pre-Show Panels** | Preview, predictions, hype |
| **Match Commentary** | Live match calls |
| **Backstage Interviews** | Promo setup, post-match reactions |
| **Replay Packages** | History recaps, feud summaries |
| **Post-Show Analysis** | Results, implications, next steps |

### Commentary Triggers

| Trigger | Commentary Type |
|---------|-----------------|
| **Signature Move** | Name call, history reference |
| **Near Fall** | Excitement escalation |
| **Callback Spot** | Historical reference |
| **Heel Tactics** | Bias expression |
| **Injury Angle** | Concern, story advancement |
| **Debut/Return** | Major moment call |

---

## IMPLEMENTATION NOTES

### Announcer Data Structure

```json
{
  "announcer_id": "ann_001",
  "name": "Jim Ross",
  "role": "play_by_play",
  "skills": {
    "call_quality": 95,
    "storytelling": 98,
    "knowledge": 99,
    "chemistry_base": 85,
    "adaptability": 90,
    "character_work": 80
  },
  "era_fit": {
    "territory": 70,
    "national_expansion": 90,
    "attitude": 100,
    "modern": 85
  },
  "signature_calls": ["BAH GAWD", "STONE COLD", "AS GOD AS MY WITNESS"],
  "bias": "neutral",
  "active_years": [1974, 2024]
}
```

### Commentary Team Structure

```json
{
  "team_id": "team_001",
  "members": [
    {"announcer_id": "ann_001", "role": "play_by_play"},
    {"announcer_id": "ann_002", "role": "color"}
  ],
  "chemistry": 0.92,
  "time_together_months": 48,
  "show_assignment": "main_event",
  "era": "attitude"
}
```

---

## CONNECTED MECHANICS

- [[Match Engine/_Match Engine Index|Match Engine]] - Provides action to call
- [[Crowd_Memory]] - Historical references
- [[Era System]] - Era-appropriate style
- [[Feud_Memory]] - Feud history callbacks

---

## OPEN QUESTIONS

- [ ] Audio generation vs. text display
- [ ] Commentary archives for replay
- [ ] Player-customizable commentary teams
- [ ] Foreign language commentary options

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define commentary generation prompts
