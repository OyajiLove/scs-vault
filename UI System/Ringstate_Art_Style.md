# RINGSTATE ART STYLE

📛 **NAME:** Ringstate Art Style Guide  
🧭 **CATEGORY:** UI System, Visual Identity, Art Direction  
🔑 **KEYWORDS:** art style, visual direction, painterly, realism, aesthetic, portraits, renders, filters, overlays  
📝 **SUMMARY:** SCS employs a layered visual identity system. Key art uses mordançage photography for splash screens and promotional materials. In-game portraits use painterly-realism: realistic enough to feel like people, stylized enough to feel like wrestling. All character renders are transparent PNGs with modular overlays and backgrounds applied contextually.

⚙️ **LOGIC OVERVIEW:**
- Two distinct visual tracks: Key Art (mordançage) and In-Game Portraits (painterly-realism)
- Portraits generated as transparent renders, dressed with context-appropriate overlays/backgrounds
- Era, region, and narrative context modify visual presentation
- Modular system allows single render to serve multiple uses
- Style evokes high-end trading cards, magazine spreads, territory-era promotional photos

🔬 **LLM INTEGRATION:** No (purely visual/asset creation)

📌 **ORIGIN:** Design discussion (Dec 2024), portrait generation experiments

📎 **CONNECTED SYSTEMS:** [[Visual_Art_Direction]], [[Portrait_Generation_System]], [[Era_Based_Office_UI]], [[Era_System]]

❓ **OPEN QUESTIONS:**
- Exact color palettes per era (need hex codes)
- How many background variants needed for MVP?
- Regional color associations (Mexico = warm? Japan = cool?)
- Masked wrestler handling (full mask vs partial face)

✅ **STATUS:** CONCEPT LOCKED (Style direction confirmed, implementation ongoing)

---

## VISUAL IDENTITY TIERS

SCS uses distinct visual approaches for different purposes:

| Tier | Style | Use Case | Examples |
|------|-------|----------|----------|
| **Key Art** | Mordançage photography | Splash screen, box art, promotional | Figures dissolving, spectral, archival |
| **Portraits** | Painterly-realism | Roster, match cards, UI | Realistic but with paint texture |
| **UI Elements** | Era-appropriate design | Office, menus, calendars | Wood panels (70s) → Corporate (90s) → Modern (2010s) |
| **Icons/Props** | Clean, functional | Skill indicators, stat displays | Minimal, readable |

---

## PORTRAIT STYLE: PAINTERLY-REALISM

### Core Aesthetic

The portrait style lives in the space between:
- **Photorealism** (too uncanny, too "AI slop")
- **Illustration** (too cartoonish, loses wrestling's weight)

Target: **High-end trading card / wrestling magazine spread**

### Visual Characteristics

| Element | Description |
|---------|-------------|
| **Skin** | Realistic texture with slight sheen (studio lights), visible pores but not hyperdetailed |
| **Eyes** | Clear, focused, personality visible (not dead AI eyes) |
| **Hair** | Texture and movement, era-appropriate styling |
| **Clothing/Gear** | Accurate materials (spandex sheen, leather texture, velvet depth) |
| **Lighting** | Studio portrait style, dramatic but not extreme |
| **Background** | Transparent render (applied separately) |
| **Overall** | Brushstroke texture visible on close inspection, not smooth digital |

### What It's NOT

| Avoid | Why |
|-------|-----|
| Hyperrealism | Uncanny valley, reads as "trying too hard" |
| Smooth digital art | Looks like mobile game asset |
| Heavy stylization | Loses wrestling's physicality and weight |
| Obvious AI artifacts | Six fingers, melted ears, text garbage |
| Glamour filtering | Wrestlers should look like wrestlers, not Instagram models |

### Reference Touchstones

- 1980s WWF Magazine photo spreads (saturated, dramatic)
- Territory-era promotional 8x10s (grainy, honest)
- Japanese wrestling trading cards (clean but characterful)
- High-end sports portraiture (ESPN Magazine style)
- Oil painting portraits (texture, not photographic smoothness)

---

## MODULAR PORTRAIT SYSTEM

### Architecture

```
[Transparent Render] + [Filter/Overlay] + [Background] = Final Portrait
```

### Component Breakdown

**1. Transparent Render (Base Asset)**
- PNG with alpha channel
- Consistent framing (chest-up or 3/4 body)
- Neutral lighting (can be color-graded later)
- No background elements baked in

**2. Filter/Overlay Options**
- Texture overlays (paper grain, film grain, scratches)
- Color grading (era-specific, mood-specific)
- Vignettes (subtle edge darkening)
- Special effects (for specific contexts)

**3. Background Options**
- Solid colors (era/promotion palettes)
- Textured solids (like Leila's purple crackle)
- Gradient backgrounds
- Contextual backgrounds (ring ropes blur, crowd blur)

### Why Modular?

| Benefit | Explanation |
|---------|-------------|
| **Efficiency** | Generate render once, use everywhere |
| **Consistency** | Same base ensures character recognition |
| **Flexibility** | Context changes presentation, not identity |
| **Era Adaptation** | Same render, different era filter |
| **Special Events** | Hall of Fame gold, scandal red, memorial sepia |

---

## CONTEXT-BASED PRESENTATION

### Standard Contexts

| Context | Background | Filter | Mood |
|---------|------------|--------|------|
| **Default Roster** | Textured solid (promotion color) | Light grain, warm | Neutral, professional |
| **Match Card** | Dark gradient | High contrast | Dramatic, confrontational |
| **Profile View** | Clean solid | Minimal processing | Clear, informational |
| **Promo Segment** | Contextual (backstage, ring) | Era-appropriate grain | Narrative |
| **News Item** | Cropped headshot | Newspaper grain | Documentary |

### Special Contexts

| Context | Treatment | Notes |
|---------|-----------|-------|
| **Hall of Fame** | Gold tint, ornate frame overlay | Celebratory, legendary |
| **Scandal/Heat** | Red tint, heavy grain, desaturated | Crisis, shame |
| **Injury** | Desaturated, slight blur | Sidelined, vulnerable |
| **Retirement** | Sepia tone, soft vignette | Nostalgic, final |
| **Memorial/Death** | Black & white, film grain | Respectful, archival |
| **Championship** | Gold accents, clean background | Prestige, achievement |
| **Heel Turn** | Cooler tones, harder shadows | Shift in allegiance |
| **Face Turn** | Warmer tones, softer light | Redemption |

---

## ERA-BASED COLOR PALETTES

### 1970s Territory Era

| Element | Treatment |
|---------|-----------|
| **Dominant Colors** | Browns, oranges, mustard yellows, avocado greens |
| **Saturation** | Slightly faded, like old photographs |
| **Grain** | Heavy film grain |
| **Contrast** | Lower, softer |
| **Mood** | Smoky, intimate, regional |

### 1980s Boom Era

| Element | Treatment |
|---------|-----------|
| **Dominant Colors** | Bold primaries (red, blue, yellow), hot pink, electric blue |
| **Saturation** | High, punchy |
| **Grain** | Medium grain |
| **Contrast** | High |
| **Mood** | Energetic, larger than life, neon |

### 1990s Attitude Era

| Element | Treatment |
|---------|-----------|
| **Dominant Colors** | Black, silver, dark blue, blood red |
| **Saturation** | Selectively desaturated (skin pops, backgrounds muted) |
| **Grain** | Gritty, almost video-like |
| **Contrast** | Very high, crushed blacks |
| **Mood** | Edgy, aggressive, "extreme" |

### 2000s-2010s HD Era

| Element | Treatment |
|---------|-----------|
| **Dominant Colors** | Clean whites, corporate blues, LED-influenced |
| **Saturation** | Balanced, "broadcast ready" |
| **Grain** | Minimal to none |
| **Contrast** | Moderate, well-lit |
| **Mood** | Professional, polished, corporate |

### 2020s Modern Era

| Element | Treatment |
|---------|-----------|
| **Dominant Colors** | Teal and orange (cinema look), muted earth tones |
| **Saturation** | Stylized, cinematic color grading |
| **Grain** | Optional film emulation |
| **Contrast** | Lifted blacks, filmic |
| **Mood** | Prestige TV, streaming-era polish |

---

## REGIONAL COLOR ASSOCIATIONS

### North America

| Region | Color Palette | Notes |
|--------|---------------|-------|
| **Southern US** | Warm earth tones, reds, golds | Territory tradition, heat |
| **Northeast US** | Urban grays, blues, industrial | Madison Square Garden energy |
| **Midwest US** | Heartland colors, blues, whites | Working-class authenticity |
| **Mexico** | Warm oranges, reds, golds, greens | Lucha vibrancy |
| **Canada** | Cool blues, whites, reds | Northern, clean |

### International

| Region | Color Palette | Notes |
|--------|---------------|-------|
| **Japan** | Clean whites, blacks, deep reds | Precision, tradition |
| **UK** | Muted greens, grays, traditional | British reserve |
| **Europe** | Varies by nation | National flag influences |
| **Caribbean** | Tropical warmth, island colors | Regional variation |

---

## SPECIAL WORKER TYPES

### Masked Wrestlers (Lucha, etc.)

| Approach | When to Use |
|----------|-------------|
| **Full mask, no face visible** | Sacred masks (lucha tradition), never removed |
| **Mask with eyes visible** | Standard masked worker |
| **Unmasked (post-apuesta)** | After mask vs mask loss |

**Note:** Mask design is part of character identity. Render must capture mask details accurately.

### Managers/Valets

| Style | Notes |
|-------|-------|
| **Formal attire** | Suits, dresses, professional |
| **Character-specific** | Flamboyant managers get flamboyant presentation |
| **Posed differently** | Less "ready to fight," more "in control" |

### Authority Figures/Bookers

| Style | Notes |
|-------|-------|
| **Business attire** | Suits, office-appropriate |
| **Power poses** | Confidence, authority |
| **Different framing** | May be more formal, less dramatic |

### Legends/Retired

| Style | Notes |
|-------|-------|
| **Current appearance** | If active in non-wrestling role |
| **Prime-era appearance** | For historical context |
| **Memorial style** | For deceased legends |

---

## PROMOTION-SPECIFIC PALETTES

Each promotion in Ringstate should have associated colors for backgrounds:

| Alliance | Primary Colors | Secondary | Mood |
|----------|----------------|-----------|------|
| **CCA** | Deep blue, gold | White, burgundy | Traditional, legitimate |
| **GWA** | Corporate silver, black | Red accents | Slick, corporate |
| **PWU** | Red, black | Gold | Revolutionary, serious |
| **CFPW** | Earth tones, greens | Natural colors | Grounded, spiritual |
| **LGBTQW+** | Rainbow spectrum | Pink, purple | Vibrant, defiant |
| **Blade Underground** | Black, blood red | Silver | Dark, dangerous |
| **Independent** | Varies | Promotion-specific | Regional identity |

---

## QUALITY STANDARDS

### Must Have

- ✅ Consistent character recognition across contexts
- ✅ Era-appropriate feel when era filter applied
- ✅ Readable at small sizes (roster grids)
- ✅ Impressive at large sizes (profile view)
- ✅ No obvious AI artifacts (hands, ears, text)
- ✅ Personality visible in expression/pose

### Avoid

- ❌ Generic "AI portrait" look
- ❌ Inconsistent style across roster
- ❌ Overly glamorized/filtered appearance
- ❌ Baked-in backgrounds (limits flexibility)
- ❌ Wrong era clothing/hair for 1985 start
- ❌ Culturally insensitive representations

---

## IMPLEMENTATION PHASES

### Phase 1: Core Style Establishment
- Define exact prompt templates for painterly-realism
- Create 10-15 test portraits across worker types
- Establish overlay/background templates
- Lock color palettes with hex codes

### Phase 2: Roster Generation
- Generate transparent renders for named workers
- Apply default presentation (Leila-style overlay)
- Quality control pass for artifacts
- Store in asset database

### Phase 3: Context System
- Build filter/overlay application pipeline
- Create all context variants (HoF, scandal, etc.)
- Era filter implementation
- Regional palette implementation

### Phase 4: Special Cases
- Masked wrestler pipeline
- Manager/valet style variants
- Legend/memorial treatments
- Dynamic event-based modifications

---

## RELATED SYSTEMS

- [[Visual_Art_Direction]] - Key art mordançage style (separate from portraits)
- [[Portrait_Generation_System]] - Technical pipeline for creating portraits
- [[Era_Based_Office_UI]] - Era-specific UI design
- [[Era_System]] - Time period detection affecting visual presentation
- [[Gimmick_System]] - Gimmick may affect portrait presentation

---

**Document Status:** CONCEPT LOCKED (Style direction confirmed)  
**Next Review:** Define exact color palettes (hex codes), create prompt templates, test generation pipeline
