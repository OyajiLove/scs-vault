# Weather Risk System

📛 **NAME:** Weather Risk System
🧭 **CATEGORY:** World Builder / Event Management
🔑 **KEYWORDS:** outdoor shows, climate, rain, typhoons, weather conditions, venue protection, worker adaptability
📝 **SUMMARY:** Weather patterns affect outdoor shows, creating risk and opportunity. Regions have climate profiles with seasonal risks. Venues have protection levels. Workers have adaptability tags. Legendary moments come from those who wrestle through storms.

⚙️ **LOGIC OVERVIEW:**
- Regions have base climate patterns and extreme weather risks by season
- Outdoor shows roll weather condition chances before event
- Venues have weather protection ratings (indoor, covered outdoor, uncovered)
- Workers have adaptability tags (thrives or struggles in conditions)
- Weather affects match quality, safety, crowd atmosphere, injuries, botches
- Creates memorable moments when workers fight through elements

🔬 **LLM INTEGRATION:** Minimal (roll calculations)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Arena System]] (venue protection levels)
- [[Worker Tags]] (adaptability tags)
- [[Match Engine]] (quality/safety modifiers)
- [[Injury Risk System]] (environmental injury factors)
- [[Booking System]] (event planning risk)

❓ **OPEN QUESTIONS:**
- Exact percentage modifiers for each weather condition
- Should weather affect promo/segment quality or just matches?
- How to model cancellation decisions?

✅ **STATUS:** Locked

---

## Weather Conditions

| Condition | Impact |
|-----------|--------|
| **Rain (Light)** | Minor footing issues; atmosphere potentially enhanced |
| **Rain (Moderate)** | Ring slippery; high flyers at risk; brawlers can thrive |
| **Rain (Heavy)** | Dangerous conditions; botch risk high; potential cancellation |
| **Wind (Mild)** | Minor effects on dives, banners |
| **Wind (Strong)** | Throws off top rope spots; lighting/staging issues |
| **Wind (Dangerous)** | Event should be cancelled or moved |
| **Cold Snap** | Cardio/endurance affected; crowd patience drops; injury risk up |
| **Heatwave** | Worker fatigue spikes; crowd enthusiasm drops faster; health risks |
| **Snow** | Rare but brutal; attendance drops; transportation issues; cancellations |
| **Thunderstorms** | Dangerous; high cancellation chance; emergency evacuations |
| **Typhoon/Hurricane** | Event cancellation mandatory unless suicidal |

---

## Regional Climate Profiles

| Region | Typical Weather Risks |
|--------|----------------------|
| **Tokyo** | Humid summers; typhoons (esp. July-September); rainstorms common |
| **Osaka** | Similar to Tokyo but hotter inland; sweltering heat risk |
| **Northern Japan (Sapporo)** | Heavy snow winters; dangerous transport but hardcore snow shows possible |
| **Texas** | Heatwaves summer; flash thunderstorms; occasional tornadoes |
| **Florida** | High summer rain; hurricanes August-October |
| **California (Southern)** | Very dry; minimal rain; good for outdoor shows |
| **Mexico City** | Rainy season May-October; afternoon rains can destroy evening outdoor cards |
| **Toronto** | Cold winters; outdoor summer rain risk; blizzards rare but possible Dec-Feb |
| **UK (General)** | Light rain often; heavy rain sporadic; outdoor shows must be resilient |
| **Puerto Rico** | Hurricane season June-November; tropical storms |

---

## Venue Weather Protection

| Protection Level | Description | Risk Modifier |
|------------------|-------------|---------------|
| Indoor (Arena/Dome) | Full protection | No weather risk |
| Outdoor with Cover | Roof/scaffolding over ring | -50% to -75% weather impact |
| Outdoor Uncovered | No protection | Full weather risk |
| Partial Cover | Crowd covered, ring exposed | -25% to -50% weather impact |

---

## Worker Adaptability Tags

| Tag | Effect |
|-----|--------|
| **Rain Master** | Thrives in rain; solid footing; embraces chaos (Okada, MiSu, AJW women) |
| **Sun Warrior** | Performs best in clear hot outdoor settings |
| **Ice Cold Professional** | Works well in bitter cold, snowstorms |
| **Weather Fragile** | Falls apart when conditions imperfect; botch risk, cardio loss, attitude decline |
| **Show Must Go On** | Takes no complaints; wrestles no matter what; gains fan loyalty in brutal conditions |

---

## Weather Effects on Matches

| Factor | Effect |
|--------|--------|
| Match Quality | Modified by worker adaptability vs conditions |
| Botch Risk | Increases in slippery/windy conditions |
| Injury Risk | Increases in extreme conditions |
| Crowd Atmosphere | Can be enhanced (legendary rain match) or devastated (miserable cold crowd) |
| Worker Mood | Affected by having to perform in harsh conditions |
| Fan Loyalty | Workers who perform through harsh conditions gain loyalty boost |

---

## Example: Suzuki 30th Anniversary Show (Rainstorm)

| Factor | Value |
|--------|-------|
| Condition | Heavy Rain |
| Venue | Outdoor Uncovered |
| Workers | MiSu + Okada (both Rain Master) |
| **Result:** |
| Ring | Dangerously slick |
| Adaptation | Modified pacing; storytelling embraces rain as epic drama |
| Crowd | 1,000 diehards in ponchos; loyalty boost |
| Outcome | Legendary atmosphere; minor injury risk accepted; major historical moment |

**It was unforgettable because it almost drowned.**

---

## Weather Roll Flow

```
[Outdoor Event Scheduled]
       ↓
[Check Regional Climate Profile for Season]
       ↓
[Roll Weather Condition]
       ↓
[Apply Venue Protection Modifier]
       ↓
[For Each Match:]
    - Check Worker Adaptability Tags
    - Calculate Quality/Safety Modifiers
    - Apply Injury Risk Adjustments
       ↓
[Post-Event:]
    - Calculate Fan Loyalty Changes
    - Record Historical Moment if exceptional
```

---

## Implementation Notes

### Regional Climate Data

```json
{
  "region_id": "tokyo",
  "climate": {
    "summer": {
      "avg_temp": "hot_humid",
      "rain_chance": 40,
      "typhoon_chance": 15,
      "typhoon_months": [7, 8, 9]
    },
    "winter": {
      "avg_temp": "cold",
      "rain_chance": 15,
      "snow_chance": 5
    }
  }
}
```

### Weather Roll

```
base_chance = region.season.rain_chance
venue_modifier = venue.protection_level
final_chance = base_chance * (1 - venue_modifier)

roll = random(1, 100)
IF roll <= final_chance:
    determine_severity()
    apply_weather_effects()
```

### Match Quality Modifier

```
FOR each worker in match:
    IF worker.has_tag("rain_master") AND weather = "rain":
        quality_modifier += 5%
    ELIF worker.has_tag("weather_fragile") AND weather != "clear":
        quality_modifier -= 15%
        botch_risk += 10%
```

---

## Philosophy

Wrestling fights itself.
Wrestling fights promoters.
Wrestling fights fans.
And sometimes, wrestling fights the sky.

Real wrestling lives in the mud, the rain, the heat, the cold.
The legends are the ones who fight through it.

---

## RELATED SYSTEMS

- **[[Arena System]]:** Venue protection levels
- **[[Worker Tags]]:** Adaptability tags
- **[[Match Engine]]:** Quality/safety calculations
- **[[Injury Risk System]]:** Environmental factors
- **[[Global Event Stream]]:** Extreme weather events

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Build comprehensive regional climate database
