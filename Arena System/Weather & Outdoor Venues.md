# Weather & Outdoor Venues

📛 **MECHANIC:** Outdoor Show Weather System
🔗 **PARENT SYSTEM:** [[_Arena System Index|Arena System]]
🧭 **CATEGORY:** Show Logistics / Match Conditions
🔑 **KEYWORDS:** weather, outdoor, stadium, rain, heat, scaffolding, ring protection, elements
📌 **ORIGIN:** Vol 1 Extraction #48, #95
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #48, #95 | 🔒 LOCKED (concept) |
| 1.1 | Vol 2 Chunk 09 | 🔒 LOCKED (refinements) |

---

## Overview

Any venue classified as "Outdoor Stadium" without a retractable roof or full cover is exposed to the elements. Weather affects worker performance, crowd energy, match safety, and can even force show stoppages. Booking outdoor shows requires weighing the spectacle of stadium wrestling against environmental risks.

---

## Core Concept

Outdoor shows create unique challenges:
- Workers are exposed to rain, heat, cold
- Mat conditions change with weather
- Fan comfort affects energy levels
- Legal liability for dangerous conditions
- Pre-show decisions about protection investment

---

## Regional Weather Risk Tables

| Region/Season | Weather Risk |
|---------------|--------------|
| **Florida in July** | 80% humidity, daily rainstorms |
| **Arizona in August** | Dry but 110°F heat |
| **Northeast US in March** | Snow or cold rain risk |
| **Japan in June** | Rainy season (tsuyu) |
| **Texas in July** | Brutal heat |
| **UK Year-Round** | Rain probable |
| **Mexico (dry season)** | Low risk, hot days |
| **Pacific Northwest** | Rain likely |

---

## Weather Condition Effects

| Condition | Match Effects | Crowd Effects | Risk Effects |
|-----------|--------------|---------------|--------------|
| **Light Rain** | Minor slip risk on stage/ramp, high flyers suffer small grade penalty | Lowered fan energy | Low injury risk increase |
| **Heavy Rain** | Mat becomes slick, workrate heavily impacted | Significant energy drop | Match accident risk rises |
| **Thunderstorms** | Lightning proximity = legal liability | Panic potential | Instant show stoppage risk, match cancellations, refund nightmares |
| **Extreme Heat** | Worker stamina decays fast, heavyweights suffer | Dehydration in stands | Dehydration injuries spike |
| **Cold Weather** | Mat and ropes stiffen, workers risk pulls and tears | Cold crowds = less energy = worse pops | Muscle injury risk up |
| **High Humidity** | Stamina drain, slippery conditions | Uncomfortable crowd | Heat exhaustion risk |
| **Wind** | Affects high spots, loose equipment hazard | Distracted crowd | Flying debris risk |

---

## Match Impact by Weather

### Style-Specific Penalties

| Wrestling Style | Light Rain | Heavy Rain | Extreme Heat | Cold |
|-----------------|------------|------------|--------------|------|
| **High Flying** | -10% grade | -25% grade | -5% grade | -15% grade |
| **Technical** | -5% grade | -15% grade | -10% grade | -10% grade |
| **Brawling** | No penalty | -10% grade | -15% grade | -5% grade |
| **Hardcore** | No penalty | -5% grade | -10% grade | No penalty |
| **Power/Hoss** | No penalty | -10% grade | -20% grade | -5% grade |

### Stamina Drain Modifiers

| Condition | Stamina Drain Multiplier |
|-----------|-------------------------|
| **Optimal (70°F, dry)** | 1.0x |
| **Light Rain** | 1.1x |
| **Heavy Rain** | 1.3x |
| **Extreme Heat (100°F+)** | 1.5x |
| **High Humidity (80%+)** | 1.4x |
| **Cold (Below 40°F)** | 1.2x |

---

## Ring Protection System (LOCKED)

### Pre-Show Decision

When booking an outdoor stadium without a dome/retractable roof, you face a decision:

| Option | Cost | Effect |
|--------|------|--------|
| **Pay for Scaffolding** | Moderate | Workers protected, matches mostly safe, fans still exposed |
| **No Scaffolding** | None | Workers and ring exposed to elements |
| **Full Dome Setup** | Very Expensive | Everyone protected (ring, workers, fans) |

### Protection Coverage

| Setup | Ring Protected | Workers Protected | Fans Protected |
|-------|----------------|-------------------|----------------|
| **No Cover** | ❌ | ❌ | ❌ |
| **Scaffolding/Tarp** | ✅ | ✅ (in ring) | ❌ |
| **Full Dome** | ✅ | ✅ | ✅ |

**Note:** Fans remain exposed unless you pay for full dome setup. This affects crowd energy in bad weather.

---

## Show Stoppage Mechanics

### Automatic Stoppage Triggers

| Condition | Response |
|-----------|----------|
| **Lightning within 5 miles** | Mandatory evacuation countdown begins |
| **Tornado warning** | Immediate evacuation |
| **Extreme wind (50+ mph)** | Show suspension |
| **Flash flood warning** | Emergency protocols |

### Stoppage Consequences

| Outcome | Financial Impact | Reputation Impact |
|---------|-----------------|-------------------|
| **Clean evacuation** | Refund costs, lost merch sales | Minor (safety first narrative) |
| **Mid-match stoppage** | Partial refunds, makeup show costs | Moderate (unfinished business) |
| **Injury due to weather** | Medical costs, potential lawsuit | Major (negligence questions) |
| **Fan injuries** | Massive liability | Catastrophic |

---

## Booking Considerations

### Risk vs. Reward

**Why Book Outdoor?**
- Stadium capacity (50,000+ fans)
- Spectacle factor (WrestleMania energy)
- Landmark venue prestige
- Summer event appeal

**Why Avoid Outdoor?**
- Weather unpredictability
- Higher costs (protection, contingencies)
- Legal liability
- Match quality variance

### Seasonal Planning

| Season | Outdoor Risk | Recommendation |
|--------|-------------|----------------|
| **Spring** | Moderate (rain) | Have contingency |
| **Summer** | Heat risk, thunderstorms | Evening shows preferred |
| **Fall** | Lower risk | Good window |
| **Winter** | Cold/snow risk | Avoid in most regions |

---

## Implementation Notes

```json
{
  "venue_id": "outdoor_stadium_001",
  "venue_type": "outdoor_stadium",
  "has_retractable_roof": false,
  "protection_level": "scaffolding",
  "weather_forecast": {
    "condition": "light_rain",
    "temperature_f": 75,
    "humidity_percent": 65,
    "wind_mph": 12,
    "lightning_risk": 0.15
  },
  "modifiers": {
    "high_flyer_penalty": -0.10,
    "stamina_drain_multiplier": 1.1,
    "crowd_energy_modifier": -0.15,
    "injury_risk_modifier": 1.05
  }
}
```

---

## Connected Mechanics

- [[Arena Prestige]] - Stadium prestige vs. weather risk tradeoff
- [[_Match Engine Index|Match Engine]] - Weather modifiers to match quality
- [[Financial System]] - Protection costs, refund scenarios
- [[_Health System Index|Health System]] - Weather-related injury risks
- [[Crowd_Memory|Crowd Memory]] - "Remember when it rained at WrestleMania?" moments

---

## Indoor vs Outdoor Risk Distinction

**Core Principle:** Indoor shows are mostly immune to weather, outdoor shows take full impact.

| Venue Type | Weather Exposure | Affected By |
|------------|-----------------|-------------|
| **Outdoor (No Protection)** | Full impact | Rain, heat, cold, wind, lightning, all conditions |
| **Outdoor (Partial Protection)** | Reduced rain impact | Wind and heat still dangerous, scaffolding protects ring only |
| **Indoor** | Minimal | Transportation shutdowns, crowd attrition, power outages, worker fatigue from travel |

### Indoor Show Weather Effects

Even indoor shows aren't fully immune:

| Weather Event | Indoor Show Effect |
|---------------|-------------------|
| **Blizzard/Ice Storm** | Reduced attendance (travel impossible), worker no-shows |
| **Hurricane/Tornado** | Possible cancellation, evacuation orders override venue |
| **Extreme Heat Wave** | AC strain, power grid issues, worker fatigue from heat outside |
| **Flooding** | Venue access blocked, parking lot disasters |

---

## Hurricane Season Mechanics

**Hurricane Season:** June-November (Atlantic), May-November (Pacific)

| Show Type | Hurricane Season Risk |
|-----------|----------------------|
| **Outdoor** | High cancellation risk, insurance nightmares |
| **Indoor** | Generally proceeds unless direct hit, airport closures, or evacuation orders |

### Typical Hurricane Season Effects

- **Lighter attendance:** Casual fans stay home, roads uncertain
- **Hardcore locals turn out:** Ride-or-die fanbase actually shows up
- **Flight disruptions:** Workers stranded, emergency card reshuffling
- **Venue damage:** Post-storm shows may face damaged facilities

---

## Climate Change Era Modifiers

**Key Insight:** Weather risks intensify over time. What was manageable in the 1980s becomes dangerous by the 2020s.

### Global Temperature Escalation

| Era | Summer Heat Risk | Notes |
|-----|-----------------|-------|
| **1970s-1980s** | Baseline | Summers hot but survivable |
| **1990s-2000s** | +15% risk | Heat waves more common, longer |
| **2010s** | +30% risk | Record-breaking summers regular |
| **2020s** | +50% risk | Extreme heat events normalized |

### Regional Example: Tokyo

| Era | Summer Temperature Range | Risk Level |
|-----|-------------------------|------------|
| **1980s** | 29-32°C (84-90°F) | Manageable with hydration |
| **2000s** | 31-34°C (88-93°F) | Uncomfortable, stamina drain |
| **2020s** | 33-37°C (91-99°F) | Dangerous, heat stroke deaths common |

### Increased Flash Flood Risk

- Urban outdoor venues face higher flash flood probability globally
- Drainage systems overwhelmed by intense rainfall events
- Climate change increases "100-year flood" frequency to near-annual in some regions

---

## Travel Blockade Mechanics

**Core Problem:** Airports shut down by storms = card chaos.

### Travel Disruption Effects

| Disruption Level | Effect on Show |
|-----------------|----------------|
| **Minor delays** | Late arrivals, rushed matches, modified card order |
| **Major airport closure** | Emergency card reshuffling, last-minute replacements |
| **Regional shutdown** | Multiple workers stranded, skeleton crew show |
| **Critical mass lost** | Tour collapse, show cancellation |

### Emergency Booking Options

- **Local talent call-up:** Territory workers or trainees fill gaps
- **Extended matches:** Fewer matches, longer times
- **Promo-heavy show:** Cover gaps with talking segments
- **Dark match promotion:** Move dark matches to main card
- **Cancellation:** If too many key workers missing

---

## Worker Adaptability

**No special weather tags needed.** Use existing Mental Skill: **[[Adaptability]]**

| Adaptability Level | Weather Performance |
|-------------------|--------------------|
| **High** | Minimal penalties, adjusts to conditions |
| **Average** | Standard weather modifiers apply |
| **Low** | Increased penalties, struggles with unexpected conditions |

Workers with high Adaptability:
- Adjust style to slippery/cold/hot conditions
- Maintain composure during weather interruptions
- Less morale damage from weather-affected shows

---

## Open Questions

- [ ] Exact weather probability tables by region/month
- [ ] Cost formulas for protection options
- [ ] Insurance/liability simulation depth
- [ ] Weather forecast accuracy (can it surprise you mid-show?)
- [ ] Historic outdoor show references for era authenticity

---

**Document Status:** Locked (v1.1 Refinements)
**Last Updated:** 2025-12-26
**Next Review:** Define cost formulas and weather probability tables
