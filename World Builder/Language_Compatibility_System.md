# Language Compatibility System

📛 **NAME:** Language Compatibility System
🧭 **CATEGORY:** World Builder / Fan Behavior / Promo System
🔑 **KEYWORDS:** multilingual promos, translation, regional language, cultural identity, presentation strategy
📝 **SUMMARY:** Language isn't just communication; it's identity, pride, memory, and sometimes resentment. This system tracks how promos in different languages land based on regional demographics and how promotions choose to present multilingual content.

⚙️ **LOGIC OVERVIEW:**
- Regions have primary/secondary language profiles
- Workers have language fluency tags
- How language is presented (raw, subtitled, translated) affects reception
- Fanbase type (smart/progressive vs traditional) modifies tolerance
- Mismatches create confusion, backlash, or opportunity for heel heat

🔬 **LLM INTEGRATION:** Minimal (lookup and comparison)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Fanbase Region DNA]] (language profile)
- [[Promo System]] (delivery effectiveness)
- [[Worker Tags]] (language fluency)
- [[Regional Gimmick Reception]] (cultural alignment)

❓ **OPEN QUESTIONS:**
- Should workers gain language fluency over time if booked in foreign territories?
- How to model accent/dialect reception?
- Exact percentage modifiers for presentation strategies

✅ **STATUS:** Locked

---

## Regional Language Profiles

| Attribute | Description |
|-----------|-------------|
| Primary Language(s) | Main language(s) spoken by majority |
| Secondary Languages | Minority/immigrant languages with cultural weight |
| Tolerance for Foreign Language Use | How receptive to promos in non-majority language |
| Language Pride/Sensitivity | How touchy about language identity |

### Example Profiles

| Region | Primary | Secondary | Foreign Tolerance | Sensitivity |
|--------|---------|-----------|-------------------|-------------|
| Los Angeles Metro | English, Spanish | Korean, Tagalog | Very High | Low |
| Quebec (Montreal) | French | English, Arabic | Low (if French ignored) | Very High |
| Texas Border Cities | English, Spanish | — | High | Moderate |
| Tokyo | Japanese | English (education) | Moderate (subtitles preferred) | Moderate |
| Vancouver Metro | English | Punjabi, Cantonese, Mandarin | High for communities | Low |
| Deep South Rural | English | — | Very Low | High |

---

## Presentation Strategies

How promotions handle multilingual content affects fan reception:

| Method | Effect on Fan Reaction |
|--------|------------------------|
| **Untranslated Foreign Promo (Live)** | Risky: progressive/smart fans may love authenticity; traditional fans may react with boredom, hostility, or heckling |
| **Pre-Taped, Subtitled Promos** | Strong option: preserves authenticity, informs audience; smart fans appreciate, traditional fans tolerate better |
| **Manager/Interpreter Translation** | Safe route: gives audience a bridge; can be serious (sports-style) or sleazy (heel managers lying about translation) |
| **Bilingual Worker (switching mid-promo)** | Highly effective if worker is charismatic and fluent; especially successful with Mexican-American, Japanese-American, Quebecois bilingual stars |
| **In-Character Mock Translation** | Heel managers mistranslating to insult crowd; risky but huge heat if done right, disaster if wrong |

---

## Promotion Type and Language Reception

| Promotion Type | Multilingual Promo Reaction |
|----------------|----------------------------|
| Sports-Based Realism (UFC-esque) | Serious translator use boosts credibility |
| Wild Sports-Entertainment (90s WWF) | Flashy, silly translations, mocking translations accepted for heat |
| Indie "Smart Mark" (PWG, AEW) | Subtitles, authentic multilingual promos welcomed |
| Traditional Family Entertainment | Safer to translate immediately; untranslated loses connection fast |
| Regional Outlaw Promotions | Very low tolerance unless framed heelishly ("outsiders stealing our sport!") |

---

## Gameplay Effects

| Situation | Outcome |
|-----------|---------|
| Spanish promos in San Diego/Houston | Boosts local fan loyalty |
| Spanish promos in Oklahoma City (no translation) | Confusion, weakened connection |
| English-only heel gimmick in Mexico City | Instantly hated (great heat if intentional, disastrous face turn if not) |
| French promos in Quebec (no English subtitles) | Deep fan loyalty through cultural identity |
| Cool Japanese/English hybrid in Tokyo 2020s | Tolerated; younger fans like it, older prefer pure Japanese |

---

## Worker Language Tags

| Tag | Description |
|-----|-------------|
| **Language Chameleon** | Fluent in multiple languages, can switch mid-promo |
| **Language Barrier Struggler** | Limited to one language, needs translation support |
| **Bilingual Native** | Natural fluency in two languages (heritage) |
| **Learned Fluency** | Acquired language skill through career/training |
| **Accent/Dialect Master** | Can modify speech patterns for different regions |

---

## Implementation Notes

### Region Language Data

```json
{
  "region_id": "quebec_montreal",
  "primary_languages": ["french"],
  "secondary_languages": ["english", "arabic"],
  "foreign_tolerance": 25,
  "language_sensitivity": 95,
  "notes": "French promos mandatory for maximum connection; English acceptable but French required for deep loyalty"
}
```

### Promo Language Check

```
IF promo_language NOT IN region.primary_languages:
    IF region.foreign_tolerance > 50:
        reaction_modifier = -10%
    ELSE:
        reaction_modifier = -30% to -50%
    
    IF presentation = "subtitled":
        reaction_modifier += 15%
    ELIF presentation = "translated_live":
        reaction_modifier += 20%
    ELIF presentation = "raw_untranslated":
        IF fanbase_type = "smart_progressive":
            reaction_modifier += 5%
        ELSE:
            reaction_modifier -= 20%
```

---

## RELATED SYSTEMS

- **[[Fanbase Region DNA]]:** Language profile storage
- **[[Promo System]]:** Delivery effectiveness calculation
- **[[Regional Gimmick Reception]]:** Cultural alignment
- **[[Worker Tags]]:** Language fluency tags

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Build comprehensive region language database
