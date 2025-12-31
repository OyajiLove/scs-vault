# Promotion Tone Tags

📛 **NAME:** Promotion Tone Tags
🧭 **CATEGORY:** Booking System / Hidden Layer
🔑 **KEYWORDS:** promotion, tone, personality, booking, commentary, bias
📝 **SUMMARY:** Hidden personality tags for each promotion that influence commentary, gimmick reception, believability, and bio tone. Drives promotion-specific narrative logic without exposing rules to player.

⚙️ **LOGIC OVERVIEW:**
- Each fed carries small set of personality tags (3-8)
- Tags don't show in UI unless player opts into advanced data
- Influence: commentary reaction, gimmick dips, believability arcs, bio phrasing, match summary voice
- Evaluated only during key narrative rendering (bio generation, segment feedback, commentary tone shift)
- Cached between shows unless overwritten by ownership change, commentary team replacement, or radical tonal shift

🔬 **LLM INTEGRATION:** Yes — for bio generation and commentary tone

📌 **ORIGIN:** Vol 6 (lines 521-528)

📎 **CONNECTED SYSTEMS:** Worker Bio Generator, Commentary System, Gimmick System, Booking Engine

❓ **OPEN QUESTIONS:**
- Full tag dictionary
- Auto-detection algorithm from booking history
- UI for modder tag assignment

✅ **STATUS:** Conceptual (needs implementation spec)

---

## Core Principle

**Promotion Bias > Alliance Bias**

Most players (especially in real-world saves) aren't working inside tight-knit alliances. They're booking feds — and those feds have history, politics, and voices of their own.

---

## Tag Categories

| Category | Example Tags |
|----------|--------------|
| **Tradition** | Protect Tradition, Push Bloodlines, Booking Is Sacred |
| **Pacing** | Slow Burn Preference, Flash Pop Culture Booking |
| **Gimmick Culture** | Gimmick Loyalty Bias, Style Clash Tolerance, Satire Tolerance |
| **Promo Bias** | Promo-Driven, Realism Only, Southern Yell School |
| **Match Structure** | Story Over Workrate, Hard Style Focus, Popcorn Pace |
| **Backstage Philosophy** | Worker-Led, Booker's Vision, Fan-Driven |
| **Narrative Lens** | Culture Forward Commentary, "Let the Work Speak", Heel Bias Mic |
| **Experimentalism** | High Weirdness, Soft Reality, Ritual-Driven Booking |

---

## What Tags Affect

| Feature | Driven By | Notes |
|---------|-----------|-------|
| Commentary Reaction | Fed's cultural tone + announcer tags | CCA might hate face turns. Indie fed might love chaos |
| Implementation Dip Severity | Certain feds more/less willing to accept sharp turns | Gimmick drift that would kill in one fed might thrive in another |
| Believability Momentum | Fed history + booking tone affect what "feels real" | Shoot-heavy fed won't tolerate gimmicks that fly in deathmatch comedy zones |
| Bio Tone | Fed reputation/history contributes to how world views worker | A gimmick over in Big Japan isn't seen the same in TNA |

---

## Data Structure

```json
{
  "promotion_id": "PSW",
  "tone_tags": [
    "Protect Tradition",
    "Style Clash Tolerance",
    "Ceremony-Driven Booking",
    "Slow Burn Push Preference",
    "Gimmick Loyalty Bias",
    "Culture Forward Commentary"
  ]
}
```

Could be as few as 3 tags, max ~6-8 for nuance.

---

## Processing

- Tags stored per promotion object
- Estimated impact on world tick: negligible (<100ms even with 500 promotions)
- Cached between shows unless overwritten

---

## Modding Workflow

**In Editor:**
- Drop-down or checkbox bank of pre-built tags
- Can assign manually or auto-suggest based on:
  - % of long vs short reigns
  - Promo styles used
  - Angle types and frequency
  - Match types (hardcore vs shoot vs theatrical)
  - Segment feedback ratings over time

**Auto-suggest prompt:**
> "This promotion emphasizes legacy, long arcs, and shoot realism. Add: 'Protect Tradition', 'Slow Burn Push Preference', 'Low Gimmick Tolerance'?"

---

## Save Evolution

Tags can shift if promotion radically reinvents itself.

**System flags:**
- "You've run 6 shoot-style programs in a row. Drop 'Gimmick Loyalty'? Add 'Hard Style Focus'?"
- "New commentary team hired. Tone softens toward experimental segments."

Players can:
- Lock tags to prevent changes
- Create custom tone blends for entirely unique feds

---

## Related Systems

- [[System Bible/UI and Display/Worker Bio Generator|Worker Bio Generator]]
- [[Commentary System]]
- [[Gimmick System]]
- [[Booking Engine]]
