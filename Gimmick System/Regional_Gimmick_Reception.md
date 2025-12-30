# Regional Gimmick Reception System

📛 **NAME:** Regional Gimmick Reception System
🧭 **CATEGORY:** Gimmick System / World Builder
🔑 **KEYWORDS:** context-sensitive gimmicks, face/heel by region, cultural alignment, variable reception, Bret Hart 97
📝 **SUMMARY:** Some gimmicks aren't globally face or heel; they're loved by some audiences and hated by others, sometimes on the same night in the same match. Gimmick reception is calculated by comparing gimmick type tags against regional/era fan DNA.

⚙️ **LOGIC OVERVIEW:**
- Workers carry gimmick tags defining ideological/cultural stance
- Regions have DNA profiles with political, cultural, and value preferences
- Era modifiers adjust baseline reception (nationalism hot in 80s, stale in late 90s)
- Same character can be face in Canada, heel in US, mixed in Europe
- Booking system reads crowd type and adjusts or warns

🔬 **LLM INTEGRATION:** Minimal (tag comparison calculations)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Fanbase Region DNA]] (cultural alignment check)
- [[Gimmick System]] (gimmick type tags)
- [[Era System]] (era modifiers)
- [[Booking System]] (crowd reaction prediction)
- [[Language Compatibility]] (presentation alignment)

❓ **OPEN QUESTIONS:**
- How to handle gimmick "drift" when touring extensively?
- Should crowd reactions mid-match shift gimmick perception?
- How granular should regional reception tracking be?

✅ **STATUS:** Locked

---

## Core Principle

**Gimmick Reception = Gimmick Type Tags + Regional Fan DNA Compatibility + Era Modifier**

The same promo, gear, music, and attitude land totally differently depending on where you're standing.

---

## Gimmick Tags That Trigger Variable Reception

| Tag | Description |
|-----|-------------|
| **Anti-Nationalist** | Slams nationalism of one region while uplifting another (Bret Hart '97) |
| **Nationalist Hero** | Celebrates local pride; hero at home, heel elsewhere |
| **Culture Clash Artist** | Brings foreign values/culture to unsettle audience |
| **Globalist Diplomat** | Tries to connect all cultures; may bore some, beloved by others |
| **Regional Patriot** | Plays directly to local fans ("Texas Forever"); alienates everyone else |
| **Political Provocateur** | Pushes divisive political stances |
| **Regional Antihero** | Flawed/bitter regional star; defended at home, booed elsewhere |
| **Iconoclast** | Attacks industry legends/sacred traditions |
| **Cultural Traditionalist** | Respects "old values," slams modern changes |
| **Honor-Based Character** | Personal/professional honor above cheap victories |
| **Moral Superiority Complex** | Thinks they're better than modern society |
| **Family Loyalty Focus** | Constantly references family ties |
| **Foreign Monster Heel** | Large foreigner positioned as threat to local champions |

---

## Case Study: Bret Hart 1997

### Gimmick Tags

| Tag | Explanation |
|-----|-------------|
| Cultural Traditionalist | Respects dignity, family, sportsmanship; slams modern edginess |
| Anti-American Critic | Specific hostility toward American greed, selfishness, violence |
| Internationalist Hero | Embraces Canada, Europe, Japan as counterweight to US |
| Honor-Based Character | Personal honor above cheap victories |
| Moral Superiority Complex | Thinks he's better than modern society |
| Family Loyalty Focus | Hart Foundation ties constantly referenced |

### Regional Reception

| Region | Reaction | Why |
|--------|----------|-----|
| Canada (Quebec, Ontario, Alberta) | Huge Face | Traditionalism + Internationalist Hero + Family Loyalty = Maximum loyalty |
| UK/Germany/France | Face-leaning | Anti-Americanism plays sympathetically among 90s Europeans |
| US South/Midwest (conservative 90s) | Heel | Anti-Americanism + Moral Superiority = betrayal |
| US Northeast (smart/progressive) | Mixed | Some respect, some jeering; depends on sophistication |
| Mexico | Face-leaning | Family + International Respect connects emotionally |
| Japan | Neutral/Respectful | Technical skill respected; political content doesn't resonate |

---

## Era Evolution: "America First" Gimmicks (US)

| Era | Crowd Reaction |
|-----|----------------|
| 1980s (Reagan Era) | Massive face pops everywhere except smart progressive pockets |
| Early 1990s (Pre-Attitude) | Starting to stale; Gulf War nationalism still hot but cracks showing |
| Late 1990s (Attitude Era) | Super stale among youth; edginess and rebellion valued over flag-waving |
| Early 2000s (Post-9/11 spike) | Temporary revival; fans rally emotionally |
| Mid-2000s onward | Quickly declines; fans want complex characters |
| 2020s | Hyper-polarized; depends entirely on urban/rural split, dangerous to touch |

---

## Reception Calculation

```
FOR each gimmick_tag:
    alignment_score = compare(tag, region.values, region.politics)
    era_modifier = era_reception_table[tag][current_era]
    
    final_score += (alignment_score * era_modifier)

IF final_score > threshold_face:
    reception = "face"
ELIF final_score < threshold_heel:
    reception = "heel"
ELSE:
    reception = "mixed" or "volatile"
```

### Reaction Types

| Type | Description |
|------|-------------|
| Face | Cheered consistently |
| Heel | Booed consistently |
| Mixed | Split reactions, unpredictable |
| Volatile | Reactions can flip mid-match based on spots/promos |
| Indifferent | Crowd doesn't care either way |

---

## Example Booking Scenarios

| Match | Location | Year | Likely Reaction |
|-------|----------|------|-----------------|
| Bret Hart vs Steve Austin | Calgary, Alberta | 1997 | Thunderous Bret face pop; Austin booed |
| Bret Hart vs Steve Austin | Houston, Texas | 1997 | Strong anti-Bret boos; Austin massive face |
| Bret Hart vs Steve Austin | Berlin, Germany | 1997 | Bret more dignified; Austin respected but Bret cleaner face |
| Bret Hart vs Steve Austin | Chicago, Illinois | 1997 | Smart crowd; Austin pop bigger, Bret respected but not loved |
| Bret Hart vs Steve Austin | Tokyo, Japan | 1997 | Bret deeply respected; Austin edginess appreciated but less emotional |

---

## Optional Gameplay Tools

| Tool | Function |
|------|----------|
| Gimmick Regional Alignment Tracker | Shows where gimmick plays as face/heel/volatile |
| Smart Booking Suggestion | "Crowd likely to boo [worker] in [region], consider turn" |
| AI Promo Modifier | Adjusts promo tone depending on territory expectations |
| Commentary Customization | Commentary reacts differently by region |

---

## Implementation Notes

### Gimmick Tag Data

```json
{
  "gimmick_id": "bret_hart_1997",
  "tags": [
    "cultural_traditionalist",
    "anti_american_critic", 
    "internationalist_hero",
    "honor_based",
    "moral_superiority_mild",
    "family_loyalty"
  ],
  "default_alignment": "heel_us_face_international"
}
```

### Regional Reception Check

```json
{
  "region_id": "alberta_canada",
  "gimmick_id": "bret_hart_1997",
  "calculated_reception": "strong_face",
  "key_factors": [
    "family_loyalty_high_match",
    "anti_american_positive_in_canada",
    "traditionalism_respected"
  ]
}
```

---

## RELATED SYSTEMS

- **[[Fanbase Region DNA]]:** Cultural values to compare against
- **[[Gimmick System]]:** Gimmick tag definitions
- **[[Era System]]:** Era modifiers for gimmick reception
- **[[Booking System]]:** Prediction and warnings
- **[[Language Compatibility]]:** Promo delivery alignment

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Build comprehensive gimmick tag database, era reception tables
