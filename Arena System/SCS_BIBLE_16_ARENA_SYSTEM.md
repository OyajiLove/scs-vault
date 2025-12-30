# SCS_BIBLE_16_ARENA_SYSTEM.md

📛 **NAME:** Arena/Venue System  
🧭 **CATEGORY:** World Systems / Physical Infrastructure  
🔑 **KEYWORDS:** arena, venue, location, capacity, atmosphere, home venue, touring  
📝 **SUMMARY:** System governing physical venues where wrestling events take place, including capacity, atmosphere modifiers, venue-specific crowd behavior, and touring logistics. Venue memory is partially handled by Crowd Memory system.

⚙️ **LOGIC OVERVIEW:**
- Venues have capacity, atmosphere, and crowd behavior modifiers
- Some venues are "home" venues for specific promotions
- Venue history creates memory anchors (legendary venues)
- Venue selection affects show economics and crowd energy

🔬 **LLM INTEGRATION:** Minimal (venue descriptions, atmosphere flavor text)

📌 **ORIGIN:** Mentioned throughout volumes; venue memory in Crowd Memory system

📎 **CONNECTED SYSTEMS:**
- **CROWD-001:** Crowd Memory (location-based memory anchors)
- **ECON-001:** Economics (venue costs, gate revenue)
- **RINGSTATE-001:** Ringstate Factions (faction-specific venues)
- **TV-001:** TV Broadcast (production requirements by venue)

❓ **OPEN QUESTIONS:**
- Venue database structure
- Touring route optimization
- Venue booking/scheduling mechanics
- Historical venue templates

✅ **STATUS:** Scaffolding (Partial integration with Crowd Memory)

---

## 1. WHAT EXISTS (LOCKED IN OTHER SYSTEMS)

### 1.1 From Crowd Memory (CROWD-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Location-Based Memory** | Memory anchor types | Crowds remember significant events at specific locations |
| **Venue-Specific Reactions** | Crowd psychology | "This is where Misawa won the title" affects crowd behavior |
| **Regional Memory Banks** | Memory persistence | Crowds in different regions remember differently |

### 1.2 From Ringstate Factions (RINGSTATE-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Faction-Specific Venues** | Geographic distribution | Each faction has typical venue types and locations |
| **Underground Circuits** | Blade venues | Warehouses, coal pits, non-traditional venues |
| **CFPW Venues** | Indigenous spaces | Community centers, reservation locations |

### 1.3 From Popularity System (POP-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Regional Draw** | Pop calculations | Workers draw differently in different regions/venues |

---

## 2. WHAT MAY NEED STANDALONE BUILDING

### 2.1 Venue Database

| Attribute | Description |
|-----------|-------------|
| **Capacity** | Seated capacity (affects gate revenue) |
| **Atmosphere Type** | Intimate, arena, stadium, outdoor, unconventional |
| **Home Promotion** | Primary promotion that runs venue |
| **Crowd Behavior Modifiers** | Hardcore tolerance, rowdiness, loyalty strength |
| **Production Capability** | TV-ready, lighting quality, acoustics |
| **Cost** | Rental cost, production requirements |
| **Prestige** | Madison Square Garden vs local armory |
| **Region** | Geographic location |
| **Era Availability** | When venue exists/existed |

### 2.2 Legendary Venue System

Certain venues carry special weight:
- Madison Square Garden (NYC)
- Tokyo Dome (Japan)
- Korakuen Hall (Japan, smart fan crowd)
- ECW Arena (Philadelphia)
- Budokan Hall (Japan)
- Hammerstein Ballroom (NYC)
- Dallas Sportatorium (territory era)

**Legendary Venue Effects:**
- Higher crowd expectations
- Greater memory weight for events
- Prestige boost for workers who perform well
- Historical echoes (callbacks to past events)

### 2.3 Venue Booking Mechanics

- Availability scheduling
- Competing bookings (multiple promotions want same venue)
- Long-term venue deals
- Venue relationship scores (frequent promotions get better rates)

### 2.4 Touring Logistics

- Travel costs between venues
- Scheduling optimization
- Worker fatigue from touring
- Regional tour patterns

---

## 3. VENUE ATMOSPHERE TYPES

| Type | Characteristics | Example |
|------|-----------------|---------|
| **Intimate** | 500-2000 capacity, hot crowds, close to action | Korakuen Hall, ECW Arena |
| **Arena** | 5000-20000 capacity, standard setup | Most major venues |
| **Stadium/Dome** | 20000+ capacity, spectacle required | Tokyo Dome, WrestleMania venues |
| **Outdoor** | Variable capacity, weather factors | Stadium shows, festival settings |
| **Unconventional** | Non-traditional spaces | Warehouses (Blade), community centers (CFPW) |

### Atmosphere Effects on Shows

| Atmosphere | Effect |
|------------|--------|
| **Intimate** | +Crowd engagement, psychology rewarded, mistakes visible |
| **Arena** | Balanced, production matters more |
| **Stadium** | Spectacle required, subtle work lost, pyro matters |
| **Outdoor** | Weather risks, unique atmosphere, crowd unpredictability |
| **Unconventional** | Authenticity bonus, production limitations |

---

## 4. VENUE MEMORY INTEGRATION

### How Venues Create Memory Anchors

When significant events occur at venues:
1. Event logged to venue history
2. Crowd memory at that venue gains anchor
3. Future shows at venue may trigger callbacks
4. Legendary venues accumulate more anchor weight

### Memory Anchor Examples

- "This is where Bret screwed Bret" (Montreal)
- "Misawa won the triple crown here" (Budokan)
- "Shane McMahon jumped off the titantron" (venue-specific)
- "ECW's last show" (ECW Arena)

---

## OUTDOOR SHOW RING PROTECTION SYSTEM (#48)

📌 **Source:** Vol 1 Extraction #48

**Pre-Show Decision for Outdoor Venues:**

When booking outdoor stadium without dome/retractable roof:

| Option | Cost | Effect |
|--------|------|--------|
| **Pay for scaffolding** | Medium | Workers protected, matches mostly safe |
| **No scaffolding** | Free | Workers exposed to elements |
| **Full dome** (crazy expensive) | Very High | Everyone protected |

**Key Rules:**
- Fans remain exposed unless you pay for full dome setup
- Scaffolding protects ring only
- Weather still affects crowd energy even with ring cover
- Full dome = stadium tier expense

---

## WEATHER / OUTDOOR SHOW SYSTEM (#95)

📌 **Source:** Vol 1 Extraction #95

**Core Concept:** Any venue classified as "Outdoor Stadium" without a retractable roof or full cover is exposed to the elements.

### Regional Weather Tables

| Region/Season | Weather Risk |
|---------------|--------------|
| Florida in July | 80% humidity, daily rainstorms |
| Arizona in August | Dry but 110°F |
| Northeast US in March | Snow or cold rain risk |
| Japan in June | Rainy season |
| Texas in July | Brutal heat |

### Weather Effects on Performance

| Condition | Effect |
|-----------|--------|
| **Light Rain** | Minor slip risk on stage/ramp. Lowered fan energy. High flyers suffer small grade penalty. |
| **Heavy Rain** | Mat becomes slick. Workrate heavily impacted. Risk of match accidents rises. |
| **Thunderstorms** | Lightning nearby = legal liability = instant show stoppage risk. Potential match cancellations. Refund nightmares. |
| **Extreme Heat** | Worker stamina decays fast. Heavyweight brawlers suffer. Injuries from dehydration spike. |
| **Cold Weather** | Mat and ropes get stiffer, workers risk pulls and tears. Cold crowds = less energy = worse pops. |

### Weather Integration with Match Engine

- High flyers: -10% to -25% rating in rain
- Stamina drain: +50% in extreme heat
- Cold weather: +20% minor injury risk
- Thunderstorm: 50% chance of stoppage if nearby

---

## PRODUCTION / ENTRANCE MECHANICS (#127)

📌 **Source:** Vol 1 Extraction #127

**Core Concept:** Big entrance pyros only if you pay for it in production budget.

### Production Elements

| Element | Cost Tier | Effect |
|---------|-----------|--------|
| **Pyro** | High | Massive entrance pops, safety costs |
| **LED Heavy Stages** | Very High | Modern spectacle, power requirements |
| **Basic Stage** | Low | Functional, no spectacle |
| **Custom Entrance Sets** | Medium-High | Character-specific entrances |
| **Ring Apron Customization** | Low | Branding, sponsor logos |
| **Entrance Music System** | Medium | Quality affects atmosphere |

### Budget vs. Expectations

| Promotion Size | Fan Expectations |
|----------------|------------------|
| **Low-budget fed** | Fans expect low-end setups, don't punish as hard |
| **Big fed cheaping out** | Media and fans bury you for poor production |
| **Indie going big** | Surprise pop, buzz generation |
| **Major event skimping** | Disaster, looks cheap, damages prestige |

### AI-Generated Visual System

| Venue Tier | Visual Generation |
|------------|------------------|
| **Small** | Intimate, raw atmosphere |
| **Medium** | Standard arena look |
| **Big** | Professional production |
| **Stadium** | Epic spectacle required |

Player-customizable elements:
- Stages
- Ring aprons
- Entrance sets
- LED configurations

---

## VENUE / ARENA VISUALIZATION SYSTEM (#150)

📌 **Source:** Vol 1 Extraction #150

### Arena Types by Capacity

| Type | Capacity | Atmosphere |
|------|----------|------------|
| **Bingo Hall** | <500 | Intimate, loud, raw |
| **Mid-Size Venue** | 500-2000 | Classic indie feel |
| **Arena** | 2000-10000 | Professional atmosphere |
| **Stadium** | 10000-50000 | Epic, intimidating |
| **Mega Stadium** | 50000+ | Once-in-generation events |

### Visual Generation

| Feature | Description |
|---------|-------------|
| **AI-generated interior shots** | By venue tier, era-appropriate |
| **Era-specific aesthetics** | Smoky 70s vs. LED 2020s |
| **Player customization** | Stages, ring aprons, entrance sets |
| **Atmosphere effects** | Lighting, crowd density, noise |

### Era-Specific Venue Aesthetics

| Era | Visual Style |
|-----|--------------|
| **1970s** | Smoky, dim, intimate, industrial |
| **1980s** | Neon, bright, larger production |
| **1990s** | Pyro-heavy, attitude era grit |
| **2000s** | HD era, LED begins |
| **2010s+** | Full LED, social media integration |

---

## 5. ASSESSMENT

**Current Status:** Venue memory handled by Crowd Memory; other aspects need building.

**Recommendation:**

1. ✅ Crowd Memory: Location-based memory anchors (locked)
2. ⚠️ Venue Database: Needs creation with capacity, atmosphere, prestige
3. ⚠️ Touring Logistics: May be needed for realistic simulation
4. ⚠️ Venue Booking: Scheduling and availability mechanics

**Priority:** Medium, can function with minimal venue data initially.

---

## 6. IMPLEMENTATION NOTES

### Venue Data Structure

```
Venue {
    venue_id: string
    name: string
    location: Location {
        city: string
        region: string
        country: string
    }
    capacity: int
    atmosphere_type: enum (INTIMATE, ARENA, STADIUM, OUTDOOR, UNCONVENTIONAL)
    prestige: float (0.0-1.0)
    crowd_modifiers: CrowdModifiers {
        hardcore_tolerance: float
        rowdiness: float
        loyalty_strength: float
        smart_fan_ratio: float
    }
    production_tier: enum (BASIC, STANDARD, TV_READY, PREMIUM)
    base_cost: int
    home_promotions: list<promotion_id>
    era_range: EraRange
    legendary_status: bool
    memory_anchors: list<event_id>
}

VenueRelationship {
    promotion_id: string
    venue_id: string
    relationship_strength: float (0.0-1.0)
    shows_run: int
    cost_modifier: float
    priority_booking: bool
}
```

---

## RELATED SYSTEMS

- **CROWD-001:** Primary handler of venue memory and crowd behavior
- **ECON-001:** Venue costs and gate revenue
- **RINGSTATE-001:** Faction-specific venue types
- **TV-001:** Production requirements for broadcast

---

**Document Status:** Scaffolding, venue database and touring logistics TBD  
**Next Review:** Prioritize after core Tier 3 systems complete
