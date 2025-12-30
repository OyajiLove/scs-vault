# Crowd Energy System

📛 **SYSTEM:** Crowd Energy
🧭 **CATEGORY:** Show Simulation / Atmosphere
🔑 **KEYWORDS:** crowd energy, venue size, attendance, atmosphere, optics, packed house, half-empty
📝 **SUMMARY:** Models how venue capacity vs actual attendance affects crowd energy, show atmosphere, and worker/promotion perception. Half-empty arenas kill shows; packed small venues build legends.

⚙️ **LOGIC OVERVIEW:**
- Crowd energy depends on fill percentage, not raw attendance
- 50% or less full = crowd energy drops significantly
- 80-100% full = max energy potential
- Smaller packed venues outperform larger half-empty arenas
- Fanbase loyalty modifies expected energy levels

🔬 **LLM INTEGRATION:** Minimal

📌 **ORIGIN:** Vol 2 Chunk 09

📎 **CONNECTED SYSTEMS:**
- [[_Arena System Index|Arena System]] - Venue capacity
- [[Match Quality Factors]] - Atmosphere affects match ratings
- [[Morale System]] - Worker morale affected by crowd energy
- [[Crowd_Memory|Crowd Memory]] - Memorable atmosphere creates memories
- [[Financial System]] - Revenue vs atmosphere tradeoffs

❓ **OPEN QUESTIONS:**
- Exact formula for energy calculation
- Hardcore fanbase modifier values
- TV perception vs live perception differences

✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 09 | 🔒 LOCKED (Concept) |

---

## Core Principle

**Energy first. Optics second. Raw numbers third.**

A packed armory of 500 screaming fans creates more memorable moments than a half-empty 10,000 seat arena with 3,000 bored attendees.

---

## Venue Fill Percentage Effects

| Fill Percentage | Crowd Energy Level | Atmosphere |
|-----------------|-------------------|------------|
| 90-100% (Sellout) | Maximum | Electric, memorable |
| 80-89% | High | Strong atmosphere |
| 70-79% | Moderate | Decent but noticeable gaps |
| 60-69% | Below Average | Energy struggles |
| 50-59% | Low | Buzzkill territory |
| Below 50% | Critically Low | Dead crowd, hollow feel |

---

## Key Effects of Crowd Energy

| Area | High Energy Effect | Low Energy Effect |
|------|-------------------|-------------------|
| **Match Atmosphere Ratings** | Bonus to perceived match quality | Penalty to atmosphere scores |
| **Worker Morale** | Boost during and after show | Drain, especially for workers who need validation |
| **TV Audience Perception** | Shows feel "hot," builds interest | Shows feel cold, casual viewers tune out |
| **Angle Success/Failure** | Emotional turns and climaxes land harder | Big moments fall flat |
| **Future Ticket Sales** | Good buzz = repeat attendance | "That show sucked" reputation |

---

## Venue Size vs Attendance Math

### Example Scenarios

| Scenario | Capacity | Attendance | Fill % | Energy Level |
|----------|----------|------------|--------|--------------|
| Packed indie show | 500 | 500 | 100% | Maximum |
| Good arena show | 10,000 | 8,500 | 85% | High |
| Disappointing PPV | 15,000 | 8,000 | 53% | Low |
| Half-empty stadium | 50,000 | 20,000 | 40% | Critically Low |

**Key insight:** 500 people in a 500-seat venue creates MORE energy than 8,000 in a 15,000-seat arena.

---

## Fanbase Loyalty Modifiers

Some fanbases "overperform" for their size:

| Fanbase Type | Energy Modifier | Example |
|--------------|-----------------|---------|
| Hardcore cult following | +15-25% | '90s ECW, early ROH |
| Emotionally invested locals | +10-15% | Territory strongholds |
| Casual mainstream fans | Baseline | Standard WWE house shows |
| Corporate/tourist crowds | -10-15% | WrestleMania weekend casual attendees |

**Note:** A 60% full ECW Arena might feel like 80% full due to rabid fanbase engagement.

---

## Venue Booking Strategy

### Smart Promotion Approach

| Situation | Recommended Strategy |
|-----------|---------------------|
| Uncertain draw | Book slightly smaller venue to guarantee sellout energy |
| Hot momentum | Stretch to larger venue, accept risk |
| Returning to market | Start small, build up over multiple shows |
| PPV/major event | Prioritize atmosphere over capacity unless confident |

### Optics vs Revenue Tradeoff

| Choice | Revenue | Atmosphere | Optics |
|--------|---------|------------|--------|
| Large venue, 60% full | Higher gross | Poor | Looks like failure |
| Small venue, sellout | Lower gross | Excellent | Looks like success |

**Lesson:** Sometimes less money = better long-term reputation.

---

## Show-Level Application

### Pre-Show Check

```
expected_attendance = calculate_draw()
venue_capacity = selected_venue.capacity
fill_percentage = expected_attendance / venue_capacity

if fill_percentage < 0.5:
    energy_level = "critically_low"
    warn("Consider smaller venue")
elif fill_percentage < 0.7:
    energy_level = "below_average"
elif fill_percentage < 0.8:
    energy_level = "moderate"
elif fill_percentage < 0.9:
    energy_level = "high"
else:
    energy_level = "maximum"
```

### During Show

- Energy level modifies all match atmosphere calculations
- Can be boosted by exceptional performances
- Can be drained by bad segments, long delays, cold matches

---

## Historical Examples

| Show | Venue/Attendance | Energy Level | Result |
|------|-----------------|--------------|--------|
| ECW Barely Legal '97 | Small ECW Arena, sellout | Maximum | Legendary atmosphere, career-making moments |
| WrestleMania IX | Caesar's Palace, outdoor, weird setup | Below Average | Flat atmosphere despite star power |
| Tokyo Dome NJPW | 40,000+ sellout | Maximum | "Tokyo Dome quality" becomes a meme |
| Half-empty Nitro tapings | Large arenas, declining attendance | Low | Exposed WCW's waning popularity |

---

## Implementation Notes

```json
{
  "show_id": "show_001",
  "venue_capacity": 15000,
  "actual_attendance": 12500,
  "fill_percentage": 0.833,
  "base_energy_level": "high",
  "fanbase_modifier": 1.10,
  "final_energy_multiplier": 1.15,
  "atmosphere_grade": "A-"
}
```

---

## Connected Mechanics

- [[Arena Prestige]] - Venue reputation vs fill risk
- [[Financial System]] - Revenue tradeoffs
- [[Morale System]] - Workers react to crowd energy
- [[Match Quality Factors]] - Atmosphere component
- [[Crowd_Memory|Crowd Memory]] - Legendary atmospheres create lasting memories

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-26
**Next Review:** Define exact formulas and modifiers
