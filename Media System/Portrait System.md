# PORTRAIT SYSTEM

📛 **NAME:** Portrait System
🧭 **CATEGORY:** Visual / Presentation
🔑 **KEYWORDS:** portrait, visual, aging, injury, appearance, AI generation, evolution
📝 **SUMMARY:**

The Portrait System manages worker visual representation with dynamic changes over time. Portraits evolve based on age, injuries, lifestyle choices, and style changes. AI-generated variations allow for era-appropriate styling while maintaining worker identity. Hot-swappable art supports modding.

⚙️ **LOGIC OVERVIEW:**

- Base portraits with overlay system for changes
- Age progression affects visual appearance
- Injuries can leave visible scars/damage
- Lifestyle choices (partying, drugs) show wear
- Style changes (hair, gear, physique) tracked
- Era-appropriate visual adjustments

🔬 **LLM INTEGRATION:** Low (AI image generation integration)

📌 **ORIGIN:** Vol 1 Extraction #147

📎 **CONNECTED SYSTEMS:**
- [[Aging System/_Aging System Index|Aging System]] - Age affects portraits
- [[Injury System/_Injury System Index|Injury System]] - Injury scars
- [[Hidden_Personality]] - Lifestyle affects appearance
- [[Era System]] - Era-appropriate styling

❓ **OPEN QUESTIONS:**
- AI generation model selection
- Portrait update frequency
- Mod format specifications

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #147 | 🔒 LOCKED (concept) |

---

## VISUAL CHANGES OVER TIME (#147)

### Age Effects

| Factor | Visual Effect |
|--------|---------------|
| **20s** | Peak physical appearance |
| **30s** | Subtle signs of experience |
| **40s** | More visible aging, possible weight changes |
| **50s+** | Gray hair, wrinkles, physique changes |

### Injury Effects

| Injury Type | Visual Effect |
|-------------|---------------|
| **Facial Cuts** | Scar overlays |
| **Eye Damage** | Visible impairment |
| **Neck Surgery** | Scar, posture change |
| **Knee Surgery** | Possible brace visible |
| **Accumulated Damage** | General worn look |

### Lifestyle Effects

| Lifestyle | Visual Effect |
|-----------|---------------|
| **Clean Living** | Ages well, healthy appearance |
| **Heavy Partying** | Premature aging, tired look |
| **Drug Use** | Visible deterioration |
| **Steroid Use** | Physique changes, later health effects |
| **Wellness Focus** | Maintains appearance longer |

### Style Changes

| Change Type | Examples |
|-------------|----------|
| **Hair** | Cuts, color, loss, facial hair |
| **Gear** | Costume evolution, mask changes |
| **Physique** | Bulk up, slim down, natural aging |
| **Accessories** | Championship belts, manager presence |

---

## PORTRAIT ARCHITECTURE

### Base + Overlay System

```
Portrait Composition:
├── Base Portrait (core likeness)
├── Age Overlay (wrinkles, gray hair)
├── Injury Overlays (scars, visible damage)
├── Lifestyle Overlays (wear, health effects)
├── Style Overlays (current hair, gear)
└── Era Filter (period-appropriate styling)
```

### Overlay Types

| Layer | Purpose |
|-------|---------|
| **Base** | Core facial structure, body type |
| **Age** | Progressive aging effects |
| **Scars** | Permanent injury markers |
| **Condition** | Current health/lifestyle state |
| **Style** | Current look choices |
| **Era** | Period-appropriate filter |

---

## AI GENERATION INTEGRATION

### Generation Triggers

| Trigger | Generation Type |
|---------|-----------------|
| **New Worker** | Full base portrait |
| **Major Style Change** | Style variation |
| **Significant Aging** | Age progression |
| **Serious Injury** | Injury overlay |
| **Era Transition** | Era-appropriate update |

### Generation Parameters

| Parameter | Options |
|-----------|---------|
| **Style** | Realistic, stylized, comic, pixel |
| **Era** | 70s, 80s, 90s, 2000s, modern |
| **Quality** | Low, medium, high |
| **Format** | Square, portrait, full body |

---

## ERA-APPROPRIATE STYLING

### Visual Markers by Era

| Era | Visual Style |
|-----|--------------|
| **1970s** | Grainy, muted colors, specific hair styles |
| **1980s** | Bright colors, big hair, neon accents |
| **1990s** | Edgier, darker, attitude aesthetic |
| **2000s** | HD clarity, modern styling |
| **2010s+** | Social media ready, polished |

### Attire Evolution

| Era | Typical Gear |
|-----|--------------|
| **Territory** | Simple trunks, boots, authentic look |
| **WWF 80s** | Colorful, character-driven costumes |
| **Attitude** | Edgy, leather, casual streetwear |
| **Modern** | Athletic wear, custom designs |

---

## MODDING SUPPORT

### Hot-Swappable Art

| Format | Purpose |
|--------|---------|
| **PNG** | Standard portrait format |
| **Layered PSD** | Moddable with overlays |
| **Pack Format** | Multiple poses/expressions |

### Community Integration

- Steam Workshop sharing
- Custom portrait packs
- Historical photo integration
- Fan art support

---

## IMPLEMENTATION NOTES

### Portrait Data Structure

```json
{
  "worker_id": "worker_001",
  "portrait": {
    "base_id": "portrait_001_base",
    "current_age_stage": "30s",
    "overlays": {
      "age": "age_30_mild",
      "scars": ["scar_forehead_1"],
      "condition": "healthy",
      "style": "short_hair_beard"
    },
    "era_filter": "attitude",
    "last_generated": "2025-12-25",
    "generation_history": [
      {"date": "2020-01-01", "trigger": "debut", "age": 25},
      {"date": "2023-06-15", "trigger": "injury", "type": "scar"},
      {"date": "2025-12-25", "trigger": "style_change", "type": "beard"}
    ]
  }
}
```

### Portrait Generation Request

```json
{
  "request_id": "gen_001",
  "worker_id": "worker_001",
  "trigger": "age_progression",
  "parameters": {
    "base_portrait": "portrait_001_base",
    "target_age": 35,
    "style_reference": "current",
    "era": "modern",
    "quality": "high"
  }
}
```

---

## CONNECTED MECHANICS

- [[Aging System/_Aging System Index|Aging System]] - Age progression triggers
- [[Injury System/_Injury System Index|Injury System]] - Injury scar overlays
- [[Hidden_Personality]] - Lifestyle trait effects
- [[Era System]] - Era-appropriate styling

---

## OPEN QUESTIONS

- [ ] AI model selection and costs
- [ ] Portrait update frequency limits
- [ ] User-uploaded portrait support
- [ ] Multiple pose/expression sets
- [ ] Portrait consistency across generations

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define AI generation pipeline
