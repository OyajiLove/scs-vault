# WORLD BUILDER SYSTEM

📛 **NAME:** World Builder System
🧭 **CATEGORY:** Game Setup / Customization
🔑 **KEYWORDS:** world builder, sliders, customization, kayfabe, templates, alternate history, sandbox
📝 **SUMMARY:**

The World Builder allows players to customize the game world's fundamental characteristics through slider-based controls. Adjust kayfabe strength, workrate appreciation, violence tolerance, women's wrestling status, and more. Use historical templates or create alternate history scenarios.

⚙️ **LOGIC OVERVIEW:**

- Slider-based world configuration (0-100 scales)
- Historical snapshot templates for quick setup
- Custom configurations saved and shared
- Sliders affect all game systems

🔬 **LLM INTEGRATION:** Low (template descriptions only)

📌 **ORIGIN:** Vol 1 Extraction #141

📎 **CONNECTED SYSTEMS:**
- [[Era System]] - Era templates use World Builder
- [[Crowd_Memory]] - Crowd behavior affected by sliders
- [[Territory System/_Territory System Index|Territory System]] - Regional variation within world settings

❓ **OPEN QUESTIONS:**
- Exact slider-to-mechanic mappings
- Template creation workflow
- Mid-game slider adjustments allowed?

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #141 | 🔒 LOCKED (concept) |

---

## CUSTOMIZATION SLIDERS (#141)

### Core Sliders

| Slider | Range | Effect |
|--------|-------|--------|
| **Kayfabe Strength** | 0-100 | How protected is wrestling's secrets |
| **Workrate Appreciation** | 0-100 | How much fans value in-ring work |
| **Character Importance** | 0-100 | How much gimmicks/personality matter |
| **Violence Tolerance** | 0-100 | Acceptable blood/hardcore content |
| **Women's Wrestling Status** | 0-100 | Integration and respect level |

### Extended Sliders

| Slider | Range | Effect |
|--------|-------|--------|
| **Fan Loyalty** | 0-100 | How sticky fan allegiances are |
| **Scandal Impact** | 0-100 | How much backstage issues affect careers |
| **Title Prestige** | 0-100 | Starting importance of championships |
| **International Awareness** | 0-100 | How visible foreign wrestling is |
| **Media Scrutiny** | 0-100 | How much press covers wrestling |

---

## SLIDER EFFECTS

### Kayfabe Strength (0-100)

| Level | Effect |
|-------|--------|
| 0-20 | Everyone knows it's fake, worked shoots everywhere |
| 21-40 | Smart fans dominant, kayfabe breaks common |
| 41-60 | Mixed audience, kayfabe somewhat protected |
| 61-80 | Kayfabe respected, breaks are scandals |
| 81-100 | Full kayfabe, breaks destroy careers |

### Workrate Appreciation (0-100)

| Level | Effect |
|-------|--------|
| 0-20 | Matches don't matter, only characters |
| 21-40 | Basic competence expected, stars over workers |
| 41-60 | Good matches help, great matches elevate |
| 61-80 | Workrate primary driver of popularity |
| 81-100 | Ring work is everything, characters secondary |

### Violence Tolerance (0-100)

| Level | Effect |
|-------|--------|
| 0-20 | PG content only, no blood ever |
| 21-40 | Mild violence, rare blood |
| 41-60 | Standard wrestling violence acceptable |
| 61-80 | Blood feuds, hardcore matches |
| 81-100 | Deathmatches, extreme content normalized |

---

## HISTORICAL TEMPLATES

### Pre-Built Configurations

| Template | Era | Description |
|----------|-----|-------------|
| **1985 NWA** | Territory Peak | High kayfabe, blood feuds, regional focus |
| **1998 WWF** | Attitude | Low kayfabe, edgy content, star-driven |
| **2003 NJPW** | Strong Style | High workrate, moderate kayfabe, stiff work |
| **2010 WWE** | PG Era | Low violence, character-driven, family audience |
| **2020 AEW** | Modern Hybrid | Low kayfabe, high workrate, smart fan focus |
| **1980 AJPW** | King's Road | High workrate, strong kayfabe, tradition |

### Template Slider Values (Example: 1998 WWF)

```json
{
  "template_name": "1998 WWF Attitude",
  "sliders": {
    "kayfabe_strength": 25,
    "workrate_appreciation": 45,
    "character_importance": 90,
    "violence_tolerance": 75,
    "womens_status": 30,
    "fan_loyalty": 60,
    "scandal_impact": 40,
    "title_prestige": 55,
    "international_awareness": 35,
    "media_scrutiny": 70
  }
}
```

---

## ALTERNATE HISTORY SCENARIOS

### Example Configurations

| Scenario | Description |
|----------|-------------|
| **Kayfabe Never Dies** | What if the internet never exposed wrestling? |
| **Women's Revolution Early** | What if women's wrestling was equal from the start? |
| **No National Expansion** | What if territories survived Vince? |
| **Japan Dominant** | What if Japanese wrestling conquered the world? |
| **Hardcore World** | What if ECW became the industry standard? |

---

## IMPLEMENTATION NOTES

### World Configuration Structure

```json
{
  "world_id": "world_001",
  "name": "My Custom World",
  "template_base": "1998_wwf",
  "sliders": {
    "kayfabe_strength": 30,
    "workrate_appreciation": 60,
    "character_importance": 85,
    "violence_tolerance": 70,
    "womens_status": 50
  },
  "regional_overrides": {
    "japan": {
      "workrate_appreciation": 90
    },
    "mexico": {
      "kayfabe_strength": 70
    }
  },
  "created_date": "2025-12-25",
  "author": "player_001"
}
```

---

## CONNECTED MECHANICS

- [[Era System]] - Era templates combine with World Builder
- [[Crowd_Memory]] - Crowd tolerance affected by sliders
- [[Popularity_System]] - What makes workers popular shifts with sliders
- [[Media System/_Media System Index|Media System]] - Media scrutiny slider affects coverage

---

## OPEN QUESTIONS

- [ ] Can sliders drift over time based on events?
- [ ] Regional slider overrides for specific territories?
- [ ] Steam Workshop template sharing?
- [ ] Preset starting roster combinations with templates?

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define exact slider-to-mechanic formulas
