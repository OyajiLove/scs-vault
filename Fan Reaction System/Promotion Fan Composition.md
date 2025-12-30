# Promotion Fan Composition

📛 **COMPONENT:** Promotion Fan Composition  
🧭 **PARENT SYSTEM:** [[_Fan Reaction Index|Fan Reaction System]]  
🔑 **KEYWORDS:** fanbase mix, audience demographics, promotion style, crowd composition, regional audiences  
📝 **SUMMARY:** Defines how different promotion styles attract different mixes of fanbase types. This composition determines the "character" of a promotion's audience and affects all fan reaction calculations including scandal tolerance, crowd behavior, and loyalty patterns.

✅ **STATUS:** LOCKED

📌 **ORIGIN:** Vol 2 Chunk 05 (Fan Reaction discussion)

📎 **CONNECTED SYSTEMS:**
- [[Fanbase Types]] (composition draws from these types)
- [[Fan Loyalty Resistance]] (composition determines composite tolerance)
- [[Institutional Loyalty]] (composition affects loyalty distribution)
- [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] (composition affects in-show reactions)
- [[Era System/_Era System Index|Era System]] (era shifts composition over time)
- [[Territory System/_Territory System Index|Territory System]] (region affects available fanbase types)

---

## Core Concept

Every promotion attracts a specific mix of fanbase types based on:

1. **Promotion Style** (what kind of wrestling they present)
2. **Era** (when they exist)
3. **Region** (where they operate)
4. **History** (what they've been)
5. **Marketing** (who they target)

This mix determines the "personality" of their audience.

---

## Composition Templates by Promotion Style

### WWE-Style Major (Sports Entertainment Giant)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Hardcore Company Loyalists | 40% | Multi-generational fans, brand-identified |
| Casual Mainstream | 35% | Entertainment consumers, follow mainstream buzz |
| Family-Friendly | 25% | Parents with kids, PG-era target |

**Composite Scandal Tolerance:** Medium-High (0.58)  
**Institutional Loyalty:** Very High  
**Crowd Character:** Polite, chant-following, merch-buying, kid-friendly

---

### AEW-Style Alternative (Workrate-Focused National)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Smark/Internet | 35% | Dirtsheet readers, booking critics |
| Indie Hardcore | 30% | Workrate lovers, anti-WWE sentiment |
| Edgy Attitude Era | 20% | Want "real" wrestling back |
| Casual Mainstream | 15% | Curious crossovers |

**Composite Scandal Tolerance:** Low-Medium (0.38)  
**Institutional Loyalty:** Medium  
**Crowd Character:** Vocal, meta-aware, will turn on bad booking fast, chant creators

---

### NJPW-Style Prestige (Traditional Japanese Major)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Hardcore Company Loyalists | 45% | Puro purists, long-term devotees |
| Smark/Internet | 35% | International workrate fans |
| Casual Mainstream | 20% | Japanese general audience |

**Composite Scandal Tolerance:** Medium (0.52)  
**Institutional Loyalty:** Very High  
**Crowd Character:** Respectful, quiet during action, explosive for big moments, clap rhythms

---

### Joshi Promotion (Japanese Women's Wrestling)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Joshi Superfans | 60% | Dedicated, parasocial, protective |
| Hardcore Company Loyalists | 25% | Traditional joshi followers |
| Casual Mainstream | 15% | Japanese general audience |

**Composite Scandal Tolerance:** Low (0.35)  
**Institutional Loyalty:** High  
**Crowd Character:** Intensely emotional, graduation ceremonies, color-coded fan support

---

### Deathmatch Indie (Hardcore Underground)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Deathmatch Outlaw | 55% | Blood and guts devotees |
| Indie Hardcore | 30% | Workrate fans who appreciate hardcore artistry |
| Edgy Attitude Era | 15% | Nostalgic for ECW-style |

**Composite Scandal Tolerance:** High (0.62)  
**Institutional Loyalty:** Low  
**Crowd Character:** Rowdy, chanting, throwing things, participation expected

---

### Family Indie (Wholesome Regional)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Family-Friendly | 50% | Parents and kids |
| Casual Mainstream | 35% | Local entertainment seekers |
| Hardcore Company Loyalists | 15% | Local territory devotees |

**Composite Scandal Tolerance:** Low (0.32)  
**Institutional Loyalty:** Medium  
**Crowd Character:** Enthusiastic, kid-driven reactions, hero worship, villain booing

---

### Lucha Promotion (Mexican Traditional)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Lucha Traditionalists | 50% | Multi-generational lucha families |
| Casual Mainstream | 30% | Mexican general audience |
| Hardcore Company Loyalists | 20% | Arena Mexico regulars |

**Composite Scandal Tolerance:** Medium (0.48)  
**Institutional Loyalty:** High  
**Crowd Character:** Passionate, mask-focused, family attendance, regional pride

---

### Territory Revival (NWA-Style Regional)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Edgy Attitude Era | 35% | Nostalgic for "real" wrestling |
| Hardcore Company Loyalists | 35% | Territory-era devotees |
| Casual Mainstream | 30% | Local entertainment |

**Composite Scandal Tolerance:** Medium-High (0.55)  
**Institutional Loyalty:** Medium-High  
**Crowd Character:** Old-school reactions, respect for tradition, regional pride

---

### Super Indie (PWG/GCW-Style)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Indie Hardcore | 50% | Workrate obsessives |
| Smark/Internet | 35% | Online wrestling community |
| Deathmatch Outlaw | 15% | Appreciate the chaos |

**Composite Scandal Tolerance:** Very Low (0.28)  
**Institutional Loyalty:** Low  
**Crowd Character:** Insider chants, meta humor, will turn on anything "corporate"

---

### UK Scene (British Wrestling)

| Fanbase Type | Percentage | Notes |
|--------------|------------|-------|
| Indie Hardcore | 40% | Technical wrestling appreciation |
| Smark/Internet | 30% | Online community overlap |
| Casual Mainstream | 20% | World of Sport nostalgia |
| Edgy Attitude Era | 10% | 90s crossover fans |

**Composite Scandal Tolerance:** Low (0.34)  
**Institutional Loyalty:** Medium  
**Crowd Character:** Singing, creative chants, pub atmosphere, technical appreciation

---

## Composite Tolerance Calculation

When calculating overall fan reaction to events:

```
Composite Tolerance = Σ (Fanbase % × Fanbase Base Tolerance)
```

### Base Tolerance Values

| Fanbase Type | Base Tolerance |
|--------------|----------------|
| Hardcore Company Loyalists | 0.75 |
| Indie Hardcore | 0.30 |
| Family-Friendly | 0.35 |
| Deathmatch Outlaw | 0.60 |
| Lucha Traditionalists | 0.50 |
| Joshi Superfans | 0.40 |
| Edgy Attitude Era | 0.55 |
| Casual Mainstream | 0.45 |
| Smark/Internet | 0.35 |

---

## Era Shifts in Composition

Promotion fan composition shifts over time as culture changes:

### Example: WWE Composition Over Eras

| Era | Primary | Secondary | Tertiary |
|-----|---------|-----------|----------|
| **Hulkamania (1984-1992)** | Family-Friendly (50%) | Casual Mainstream (35%) | Hardcore Loyalists (15%) |
| **New Generation (1993-1996)** | Family-Friendly (45%) | Casual Mainstream (30%) | Smark (25%) |
| **Attitude Era (1997-2001)** | Edgy Attitude (40%) | Casual Mainstream (35%) | Hardcore Loyalists (25%) |
| **Ruthless Aggression (2002-2007)** | Hardcore Loyalists (35%) | Edgy Attitude (30%) | Smark (25%) |
| **PG Era (2008-2015)** | Family-Friendly (40%) | Hardcore Loyalists (35%) | Casual Mainstream (25%) |
| **Modern Era (2016+)** | Hardcore Loyalists (40%) | Casual Mainstream (35%) | Family-Friendly (25%) |

---

## Regional Modifiers

Different regions have different available fanbase pools:

| Region | Dominant Types | Rare Types |
|--------|----------------|------------|
| **USA Northeast** | Smark, Hardcore Loyalists | Lucha Traditionalists |
| **USA South** | Family-Friendly, Edgy Attitude | Joshi Superfans |
| **USA West Coast** | Indie Hardcore, Smark | Lucha Traditionalists available |
| **Mexico** | Lucha Traditionalists, Family-Friendly | Smark (growing) |
| **Japan** | Hardcore Loyalists, Joshi Superfans | Deathmatch Outlaw (niche) |
| **UK** | Indie Hardcore, Smark | Lucha Traditionalists |
| **Europe** | Casual Mainstream, Smark | Most types available in mix |

---

## Creating Custom Promotion Composition

When building a new promotion, determine composition based on:

### Step 1: Identify Style
What kind of wrestling do they present?

### Step 2: Identify Era
When do they exist?

### Step 3: Identify Region
Where do they operate?

### Step 4: Identify History
Are they new or established? Did they evolve from something else?

### Step 5: Calculate Composite Values

Use the templates as starting points, adjust based on specific factors:

| Factor | Adjustment |
|--------|------------|
| TV deal | +10% Casual Mainstream |
| Streaming focus | +10% Smark/Internet |
| Family marketing | +15% Family-Friendly |
| Hardcore focus | +15% Deathmatch Outlaw |
| Workrate reputation | +10% Indie Hardcore |
| Long history | +10% Hardcore Loyalists |
| Controversial owner | -10% Family-Friendly |

---

## Implementation Notes

```json
{
  "promotion_fan_composition": {
    "promotion_id": "promo_001",
    "style": "aew_alternative",
    "era": "2020s",
    "region": "usa_national",
    "composition": {
      "smark_internet": 0.35,
      "indie_hardcore": 0.30,
      "edgy_attitude": 0.20,
      "casual_mainstream": 0.15
    },
    "composite_scandal_tolerance": 0.38,
    "composite_turn_speed": "fast",
    "crowd_character_tags": ["vocal", "meta_aware", "chant_creators", "quick_to_turn"],
    "historical_shifts": [
      {"date": "2019-05-25", "event": "founding", "composition_snapshot": {...}}
    ]
  }
}
```

---

## Open Questions

- [ ] How quickly can composition shift with major booking changes?
- [ ] Do individual shows have different compositions than the promotion overall?
- [ ] How do TV vs live event compositions differ?
- [ ] International expansion composition effects?

---

**Document Status:** Locked  
**Last Updated:** 2025-12-26  
**Source:** Vol 2 Chunk 05, synthesized with Era System and Territory System references
