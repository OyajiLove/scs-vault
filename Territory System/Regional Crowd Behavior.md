# Regional Crowd Behavior

📛 **MECHANIC:** Territory-Specific Crowd Reactions
🔗 **PARENT SYSTEM:** [[_Territory System Index|Territory System]]
🧭 **CATEGORY:** Crowd Psychology
🔑 **KEYWORDS:** crowd, regional, behavior, reaction, heat, pop, style preference
📌 **ORIGIN:** Ringstate Atlas, Vol 1-4 (conceptual), Crowd Memory System, Vol 1 Extraction #47
✅ **STATUS:** Conceptual (some worldbuilding exists)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 0.5 | Vol 1-4 | 📐 CONCEPTUAL |
| 1.0 | Ringstate Atlas | 📐 WORLDBUILDING |

---

## Overview

Regional Crowd Behavior governs how different territories react to wrestling content. What gets a pop in the Deep South may get silence in the Northeast. Regional crowds have distinct style preferences, heat triggers, memory patterns, and cultural values.

---

## Crowd Behavior Attributes

### Style Preference

| Territory Type | Preferred Style | Disliked Style |
|---------------|-----------------|----------------|
| **Traditional Southern** | Brawling, blood feuds, clear alignment | Spotfests, flippy stuff |
| **Technical (Mid-Atlantic)** | Mat wrestling, psychology | Comedy, hardcore |
| **Spectacle (GWA Northeast)** | Characters, big names, moments | Slow builds, long matches |
| **Puroresu-Adjacent** | Strong style, fighting spirit | Excessive comedy |
| **Lucha-Adjacent** | High flying, tag wrestling | Slow brawling |
| **Deathmatch (Blade)** | Violence, chaos, blood | Clean wrestling |
| **Smart Crowds** | Workrate, psychology | Obvious pushes |

### Heat Triggers

| Territory Type | Easy Heat | Hard Heat |
|---------------|-----------|-----------|
| **Deep South** | Insulting local team/region, cowardice | Pure technical heel work |
| **Northeast** | Being boring, breaking character | Regional insults (too obvious) |
| **Midwest** | Class-based insults, union mockery | Southern stereotypes |
| **West Coast** | Regressive politics (in some areas) | Traditional heel tactics |
| **International** | Nationalism, cultural disrespect | Generic heel work |

### Memory Duration

| Territory Type | Memory Length | Memory Style |
|---------------|---------------|--------------|
| **Deep South** | 5-10 years | Never forget betrayals |
| **Traditional CCA** | 3-5 years | Respects history |
| **Northeast/GWA** | 1-2 years | Fast turnover, what have you done lately |
| **Smart Crowds** | Long for good workers | Remember workrate, forget angles |
| **Blade/Underground** | Forever | Tribal loyalty, long memories |

---

## Regional Crowd Profiles

### Deep South Crowds

**Cultural Values:**
- Clear good vs. evil
- Loyalty and betrayal matter
- Blood means sacrifice
- Outsiders must earn respect
- Family dynasties respected

**Reaction Modifiers:**

| Element | Modifier |
|---------|----------|
| Blood match | +20% crowd response |
| Clean heel tactics | +15% heat |
| Outsider main eventing | -15% response |
| Local hero winning | +25% pop |
| Betrayal | +30% heat, remembered 5+ years |
| Tweener alignment | -20% response (confusion) |

### Northeast/GWA Crowds

**Cultural Values:**
- Entertainment first
- Stars matter
- Production value
- Quick payoffs
- Cynical about kayfabe

**Reaction Modifiers:**

| Element | Modifier |
|---------|----------|
| Big name appearance | +25% response |
| Production spectacle | +15% response |
| Slow build | -10% response |
| Inside references | +10% (smart crowd) |
| Pure wrestling match | +0% (neutral) |
| Obvious scripting | -15% response |

### Midwest Crowds

**Cultural Values:**
- Working class solidarity
- Honest effort rewarded
- Distrust of outsiders
- Union mentality
- No nonsense

**Reaction Modifiers:**

| Element | Modifier |
|---------|----------|
| Working class babyface | +20% pop |
| Rich heel | +25% heat |
| Hard work narrative | +15% response |
| Flashy coward | +20% heat |
| Outsider from coasts | -10% initial response |
| Factory town show | +10% attendance |

### Smart/Smark Crowds

**Cultural Values:**
- Workrate above all
- Appreciate psychology
- Resistant to obvious pushes
- Respect authenticity
- Ironic enjoyment

**Reaction Modifiers:**

| Element | Modifier |
|---------|----------|
| Great match quality | +30% response |
| Obvious push of lesser talent | -25% response |
| Authentic performer | +15% response |
| Manufactured gimmick | -20% response |
| Smark bait (inside references) | +10% response |
| Meta commentary | Variable (+/- 15%) |

---

## Faction-Specific Crowd Behaviors

### CCA Crowds

| Expectation | Want | Hate |
|-------------|------|------|
| **Match Style** | Traditional psychology, clean finishes | Spotfests, short matches |
| **Storytelling** | Long-term builds, logical progression | Swerves, cheap heat |
| **Worker Presentation** | Respect for veterans | Disrespect to legends |
| **Kayfabe** | Traditional (don't break it) | Breaking character |
| **Memory** | 5+ year grudges | Forgotten history |

### GWA Crowds

| Expectation | Want | Hate |
|-------------|------|------|
| **Match Style** | Spectacle, moments, highlights | Long matches, rest holds |
| **Storytelling** | Quick payoffs, clear narratives | Slow burns |
| **Worker Presentation** | Stars, celebrities, production | Unknown workers |
| **Kayfabe** | Flexible (entertainment) | Too serious |
| **Memory** | What have you done lately | Old news |

### PWU Crowds

| Expectation | Want | Hate |
|-------------|------|------|
| **Match Style** | Disciplined, ideological theatre | Chaos, individualism |
| **Storytelling** | Collective triumph, state narratives | Personal glory seeking |
| **Worker Presentation** | Humble champions, national heroes | Egomaniacs |
| **Kayfabe** | Socialist realism | Western decadence |
| **Memory** | State-approved history | Counter-revolutionary acts |

### CFPW Crowds

| Expectation | Want | Hate |
|-------------|------|------|
| **Match Style** | Ceremonial, community-led | Colonial spectacle |
| **Storytelling** | Sovereignty narratives, elder wisdom | Exploitation |
| **Worker Presentation** | Cultural authenticity | Appropriation |
| **Kayfabe** | Sacred space | Commercialization |
| **Memory** | Ancestral, generational | Erasure |

### Blade Underground Crowds

| Expectation | Want | Hate |
|-------------|------|------|
| **Match Style** | Violence, chaos, authenticity | Sanitized |
| **Storytelling** | Survival, proving ground | Corporate narratives |
| **Worker Presentation** | Outlaws, survivors, refugees | Sellouts |
| **Kayfabe** | Irrelevant (shoot atmosphere) | Overproduced |
| **Memory** | Tribal, total | Betrayal never forgiven |

---

## Implementation Notes

### Regional Modifier Application

```
Adjusted Response = Base Response × Regional Modifier × Style Match × Memory Factor
```

**Example:**
- Base pop for babyface win: 50
- Deep South region: ×1.25 (local hero)
- Style match (brawling): ×1.15
- Memory factor (returning legend): ×1.20
- **Adjusted Response: 50 × 1.25 × 1.15 × 1.20 = 86.25**

---

## Connected Mechanics

- [[Territory Definitions]] - Territory attributes affect crowd
- [[_Crowd Memory System Index|Crowd Memory]] - Memory duration by region
- [[_Popularity System Index|Popularity]] - Regional popularity affected
- [[_Emotional Show Flow System Index|Emotional Show Flow]] - Region affects pacing preferences

---

## World Builder Regional Presets (#47)

High-level sliders for quickly defining regional fan cultures in world builder:

| Region | Fan Values |
|--------|------------|
| **Japan** | Fighting Spirit, Hard Work, Grit |
| **Mexico** | High Flyer Drama, Lucha Libre Traditions |
| **US (80s)** | Big Characters, Simpler Matches |
| **US (2000s)** | Spectacle, Workrate, Mic Skills |
| **Modern Indie** | Deathmatches, Irony, In-Ring Precision |

These presets provide starting values that can be customized per promotion/territory. They represent dominant cultural expectations, not hard rules.

---

## Open Questions

- [ ] Exact regional modifier values
- [ ] How do crowds change over time (1985 → 2005)?
- [ ] Mixed crowd situations (touring shows in unfamiliar territory)?
- [ ] Online/TV crowd vs. live crowd differences?
- [ ] Crowd education (can booking change regional preferences)?

---

**Document Status:** Conceptual
**Last Updated:** 2025-12-25
**Next Review:** Define exact regional modifier tables
