# ERA-BASED OFFICE UI SYSTEM

📛 **NAME:** Era-Based Booking Office UI  
🧭 **CATEGORY:** UI System, Immersion Layer  
🔑 **KEYWORDS:** office, era, desk, calendar, phone, customization, visual themes, immersion  
📝 **SUMMARY:** The player's booking office visually transforms based on promotion location, era, and player customization. Interactive desk elements (notebook, phone, calendar) serve as navigation hubs. Office evolves through decades and can be personalized with unlockables and legacy items.

⚙️ **LOGIC OVERVIEW:**
- Office appearance changes based on promotion region AND time period
- Clickable desk props function as UI navigation (notebook = booking, phone = comms, calendar = scheduling)
- Era templates provide different visual skins (wood panels → corporate → modern startup)
- Player can customize decor, unlock items through achievements
- Prestige/legacy items earned through gameplay decorate the space

🔬 **LLM INTEGRATION:** Minimal, mostly visual/UI system

📌 **ORIGIN:** Vol. 4 (lines 52-59, half-baked concept with detailed vision)

📎 **CONNECTED SYSTEMS:** Calendar System, Booking Engine, Era System, Legacy Tracker

❓ **OPEN QUESTIONS:**
- How many era/region combinations needed for MVP? (Start with 2-3?)
- Should office upgrades have mechanical effects or purely cosmetic?
- How to handle promotion changes mid-game (office transition animation?)
- Worker-sent gifts: what triggers these? Loyalty? Milestone moments?

✅ **STATUS:** HALF-BAKED (Detailed vision, needs implementation spec)

---

## CORE CONCEPT

The booking office is not just a menu screen. It's a **living space** that reflects:
1. **Where you are** (Memphis territory vs Tokyo corporate vs indie warehouse)
2. **When you are** (1980s wood panels vs 2020s minimalist)
3. **Who you've become** (earned trophies, worker gifts, legacy items)

---

## INTERACTIVE DESK ELEMENTS

| Prop | Click Action | Visual Evolution by Era |
|------|--------------|------------------------|
| 📖 **Notebook** | Opens booking screen | Leather bound (70s) → Spiral (80s) → Planner (90s) → Tablet (2010s+) |
| 📞 **Phone** | Opens comms/logistics | Rotary (70s) → Desk phone (80s) → Cordless (90s) → Cell/smartphone (2000s+) |
| 📅 **Calendar** | Opens scheduling UI | Wall calendar (70s) → Desk calendar (80s) → Day planner (90s) → Digital screen (2010s+) |
| 🖥️ **Computer** | Opens analytics/reports | N/A (pre-80s) → CRT (80s-90s) → Flatscreen (2000s) → Laptop/tablet (2010s+) |

### Calendar Zoom Levels
- **Date view:** Single day bookings
- **Week view:** Show planning
- **Month view:** Big picture/tour planning

---

## ERA TEMPLATES

| Era | Wall Style | Desk Type | Lighting | Vibe |
|-----|------------|-----------|----------|------|
| **1970s Territory** | Wood paneling, smoke-stained | Heavy oak desk | Warm, dim, incandescent | Backroom deals, cigar smoke |
| **1980s Boom** | Corporate wood + gold accents | Executive desk | Brighter, fluorescent | Money flowing, big dreams |
| **1990s Attitude** | Dark corporate, edgier | Modern black desk | Harsh, dramatic | War room, competition |
| **2000s Indie** | Warehouse brick, posters | Folding table/cheap desk | Natural light, bare bulbs | Scrappy, DIY energy |
| **2010s+ Modern** | Minimalist white/grey | Standing desk option | LED, clean | Startup vibe, corporate wrestling |

### Regional Variations

| Region | Visual Flavor |
|--------|---------------|
| **Southern US** | Wood panels, framed territory photos, wrestling boots on shelf |
| **Northeast US** | More corporate, MSG posters, urban view |
| **Japan** | Clean, organized, calligraphy, company banners |
| **Mexico** | Colorful, masks on wall, lucha posters |
| **UK** | Smaller office, football club vibe, tea mug |

---

## CUSTOMIZATION LAYER

### Player-Driven Personalization
- Wall color/material selection
- Poster/photo placement
- Desk accessories
- Lighting mood

### Unlockables
| Category | Examples | How Earned |
|----------|----------|------------|
| **Crowd Posters** | "Sold Out [Venue]" poster | Sell out major venue |
| **Belt Replicas** | Miniature title displays | Win/defend championships |
| **Trophies** | "Promotion of the Year" | Win year-end awards |
| **Worker Gifts** | Signed photo, personal item | High loyalty workers, milestone moments |
| **Legacy Items** | Framed iconic match poster | Historic moments in your fed |

### Prestige Display
- As promotion gains history and prestige, office fills with earned memorabilia
- Creates visual progression of your legacy
- Empty office (new fed) → Cluttered with history (legendary fed)

---

## IMPLEMENTATION PHASES

### Phase 1: Functional Desk Interface (Mid-Alpha)
- Basic flat image background (one era/region)
- Clickable objects as UI nodes overlaid on desk
- TextureRect + Button nodes in Godot
- 1-2 hardcoded era/region styles

### Phase 2: Visual Variants + Prop Swapping (Beta)
- Multiple era templates (Memphis 1980, Tokyo 1995, Indie 2005, Modern 2023)
- Swappable texture elements (wall, desk, phone, etc.)
- Theme selection menu OR automatic based on promotion/year
- Grouped scenes: `BookingDesk_Memphis.tscn`, `BookingDesk_Tokyo.tscn`

### Phase 3: Customization Layer (Post-Beta)
- Player-driven personalization options
- Unlockable system integration
- Prestige/legacy display

### Phase 4: Polish
- Subtle animations (phone rings, calendar page flip)
- Ambient sound per era (typewriter clicks, phone rings, crowd noise from TV)
- Dynamic lighting shifts

---

## ASSET REQUIREMENTS

| Asset Type | Source Options | Notes |
|------------|----------------|-------|
| Wall/desk textures | AI-generated, free packs | Match 70s-2020s moods |
| Phone/notebook/calendar props | Kenney packs, AI-generated PNGs | Swappable layers |
| Framed photos/memorabilia | AI-generated, abstracted | Avoid copyright |
| UI overlays (hover/click) | Built in Godot | Glows, outlines |

### AI Art Recommendations (from Vol 4)
- **DALLE-3:** Quick, clean icons and small props
- **Stable Diffusion XL:** Stylistic packs (retro computers, phones)
- **Ideogram:** Logos, badges, nameplates

### Free Asset Packs
- Kenney.nl (legendary free creator)
- Itch.io (filter by 2D UI)
- CraftPix.net freebies
- OpenGameArt.org
- Pixel Frog UI kits

---

## EXAMPLE PROMPTS FOR AI GENERATION

```
"Flat minimalist PNG of a 1980s office rotary phone, top-down view, soft shadow"
"Sticky note with blurred text, yellowish, soft drop shadow, isolated on transparent"
"Vintage desk calendar, spiral bound, showing generic month, 1985 aesthetic"
"Wood paneled office wall texture, 1970s style, warm tones, seamless tile"
```

---

## RELATED SYSTEMS

- [[Calendar_UI_System]] - Detailed scheduling interface
- [[Era_System]] - Time period detection and effects
- [[Legacy_Tracker]] - Achievement/history tracking for unlockables

---

**Document Status:** HALF-BAKED (Detailed vision from Vol 4, needs implementation spec)  
**Next Review:** Determine MVP era count, create asset list, build Phase 1 prototype
