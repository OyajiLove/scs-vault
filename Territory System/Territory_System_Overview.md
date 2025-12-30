# SCS_BIBLE_14_TERRITORY_SYSTEM.md

📛 **NAME:** Territory System  
🧭 **CATEGORY:** World Systems / Geographic Dynamics  
🔑 **KEYWORDS:** territory, region, geographic, touring, home base, territorial loyalty, cross-territory  
📝 **SUMMARY:** System governing how geographic regions affect wrestling dynamics, including territorial loyalty, regional crowd behavior, cross-territory talent movement, and territory-based booking constraints. Much of this system's functionality is distributed across other locked systems rather than existing as a standalone module.

⚙️ **LOGIC OVERVIEW:**
- Territories define geographic boundaries with distinct crowd behaviors and style preferences
- Workers can have territorial loyalty affecting where they perform best
- Cross-territory booking involves political negotiation (see CROSS-PROMOTION-001)
- Regional popularity tracked separately (see POP-001)
- Crowd memory and reactions vary by territory (see CROWD-001)

🔬 **LLM INTEGRATION:** Minimal

📌 **ORIGIN:** Mentioned throughout Vol 1-4; components distributed across other systems

📎 **CONNECTED SYSTEMS:**
- **CROSS-PROM-001:** Cross-Promotion System (handles inter-territory talent movement, raids, invasions)
- **TV-001:** TV Broadcast System (regional TV deals, territory-specific timeslots)
- **POP-001:** Popularity System (separate regional popularity scores)
- **CROWD-001:** Crowd Memory (location-based memory anchors, regional reactions)
- **HIDE-001:** Hidden Personality ("Territorial Kingpin" archetype)
- **RINGSTATE-001:** Ringstate Factions (faction territories and boundaries)

❓ **OPEN QUESTIONS:**
- Whether standalone Territory system is needed vs. using existing distributed components
- Territory boundary definition mechanics
- Territory collapse/absorption rules
- Inter-territory touring logistics

✅ **STATUS:** Scaffolding (Components locked in other systems)

---

## 1. WHAT EXISTS (LOCKED IN OTHER SYSTEMS)

### 1.1 From Hidden Personality (HIDE-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Territorial Kingpin** | Hidden Personality archetype | Workers who dominate and protect specific regions |
| **Home Territory Loyalty** | Worker trait | Affects performance and morale when working home vs away |

### 1.2 From Popularity System (POP-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Regional Popularity Scores** | Popularity tracking | Separate popularity values per region/territory |
| **Regional Variance** | Pop calculations | Same worker can be mega-star in one region, unknown in another |

### 1.3 From Crowd Memory (CROWD-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Location-Based Memory** | Memory anchor types | Crowds remember events that happened in their territory |
| **Regional Crowd Behavior** | Crowd reactions | Different regions have different tolerance, preferences |

### 1.4 From Cross-Promotion System (CROSS-PROM-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Territory Raids** | Cross-promotion mechanics | Predatory poaching of talent, TV deals from rival territories |
| **Territorial Protector Trait** | Promotion Exchange Traits | Promotions that defend their regional boundaries aggressively |
| **Cross-Territory Booking Politics** | Booking politics | How workers move between territories with protection clauses |

### 1.5 From TV Broadcast System (TV-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Regional TV Deals** | Era-based TV modeling | Territories had to PAY for TV time, made money on house shows |
| **Territory-Specific Timeslots** | TV deal structure | Local vs national broadcast differences |

### 1.6 From Ringstate Factions (RINGSTATE-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Faction Territories** | Geographic mapping | CCA, GWA, PWU, CFPW, LGBTQW+, Blade all have territorial claims |
| **Regional Style Preferences** | Faction philosophy | Each faction's territory has distinct booking expectations |

---

## 2. WHAT MAY NEED STANDALONE BUILDING

### 2.1 Territory Boundary System

If needed as standalone:
- Define geographic regions (states, countries, cities)
- Assign promotions to territories
- Track territory "ownership" and disputes
- Handle territory collapse/absorption

### 2.2 Touring Logistics

- Travel costs between territories
- Scheduling constraints for multi-territory tours
- Worker fatigue from touring
- Regional draw capacity

### 2.3 Territory Prestige

- Reputation of territory affects talent attraction
- Territory "health" metrics (financial, talent depth, fan engagement)
- Territory death spiral mechanics

---

## 3. ASSESSMENT

**Current Status:** Most territory functionality already exists in locked systems.

**Recommendation:** Rather than building standalone Territory System, ensure the following systems properly integrate territorial mechanics:

1. ✅ Cross-Promotion System: Handles inter-territory dynamics
2. ✅ Popularity System: Tracks regional popularity
3. ✅ Crowd Memory: Location-based memory and reactions
4. ✅ Hidden Personality: Territorial worker traits
5. ✅ Ringstate Factions: Geographic faction distribution
6. ⚠️ TV Broadcast: May need territory-specific TV deal templates

**If standalone system is built later,** it should primarily serve as a **coordination layer** connecting these existing systems rather than duplicating functionality.

---

## 4. IMPLEMENTATION NOTES

### Minimal Territory Data Structure (if needed)

```
Territory {
    territory_id: string
    name: string
    region: enum (NORTHEAST, SOUTH, MIDWEST, WEST, JAPAN, MEXICO, UK, etc.)
    primary_promotion: promotion_id (nullable)
    competing_promotions: list<promotion_id>
    crowd_behavior_modifiers: CrowdModifiers
    style_preferences: list<StyleTag>
    tv_market_size: enum (MAJOR, REGIONAL, LOCAL)
    economic_health: float (0.0-1.0)
}
```

---

## RELATED SYSTEMS

- **CROSS-PROM-001:** Primary system for inter-territory dynamics
- **POP-001:** Regional popularity tracking
- **CROWD-001:** Territory-specific crowd behavior
- **TV-001:** Territory TV deals and broadcast

---

**Document Status:** Scaffolding, awaiting decision on standalone vs. distributed approach  
**Next Review:** Evaluate if coordination layer is needed after Tier 3 systems complete
