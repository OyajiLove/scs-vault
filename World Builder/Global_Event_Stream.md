# Global Event Stream System

📛 **NAME:** Global Event Stream System (GES)
🧭 **CATEGORY:** World Builder / Simulation Core
🔑 **KEYWORDS:** world events, real history, wars, recessions, cultural shifts, pandemic, terrorism, timeline
📝 **SUMMARY:** A Global Event Database runs alongside the wrestling world, including wars, terror attacks, economic conditions, cultural shifts, and technological revolutions. These events impact fan mood, booking viability, sponsor availability, scandal tolerance, and company survival.

⚙️ **LOGIC OVERVIEW:**
- Historical events stored with dates and effect profiles
- Events trigger at appropriate times (Strict Mode) or can be randomized (Alt-History)
- Multiple impact categories: economic, cultural, political, entertainment
- News headlines splash over in-game calendar
- Workers, promotions, and fanbases all react to global context
- Can be toggled on/off or customized per category

🔬 **LLM INTEGRATION:** Minimal (event triggering and modifier application)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Fanbase Region DNA]] (mood shifts)
- [[Alt-History Mode]] (randomization options)
- [[Financial System]] (economic conditions)
- [[Scandal System]] (tolerance modifiers)
- [[Booking System]] (angle viability)

❓ **OPEN QUESTIONS:**
- How many historical events to include in base database?
- Should players be able to add custom events?
- How to handle very recent/controversial events sensitively?

✅ **STATUS:** Locked

---

## Core Concept

The world doesn't freeze around the ring. The world crashes through it.

Global events affect:
- Fanbase mood and scandal tolerance
- Sponsorship availability
- TV ratings expectations
- Risk tolerance for edgy angles
- Worker mental health and movement
- Merchandise sales
- Venue availability and prices
- Company valuations
- Touring viability (wars block travel, recessions force workers to stay put)

---

## Event Categories

| Category | Examples |
|----------|----------|
| Military/War | Desert Storm, 9/11, Iraq War, conflicts blocking travel |
| Economic | Recessions, booms, bubbles, market crashes |
| Political | Elections, nationalism surges, civil unrest |
| Health/Pandemic | COVID-19, drug epidemics, health crises |
| Cultural Shifts | #MeToo, social media rise, streaming dominance |
| Technology | Internet explosion, cable TV decline, AI disruption |
| Entertainment Industry | Movie booms, sports competition, genre fads |
| Celebrity/Cultural Deaths | Major figure deaths outside wrestling |

---

## Player Mode Options

| Mode | Description |
|------|-------------|
| Strict Real-World History | Events happen as scheduled |
| Alt-History: Wrestling-Only Chaos | Real-world history accurate, wrestling world diverges |
| Alt-History: Full Chaos | Even world events randomized (recessions, wars shift) |
| Custom/Pick and Choose | Player selects which aspects are strict vs random |

---

## Sample Global Events Database

### Desert Storm (1990-91)

| Attribute | Value |
|-----------|-------|
| Date Range | August 1990 - February 1991 |
| Type | Military/War |
| **Effects:** |
| Patriotic Gimmicks | +40% effectiveness in US |
| Middle Eastern Heels | Very dangerous heat; radioactive risk |
| US Violence Tolerance | +10% short-term |
| Fan Mood | Elevated nationalism |

### 9/11 Terror Attacks (2001)

| Attribute | Value |
|-----------|-------|
| Date | September 11, 2001 |
| Type | Terrorism/Cultural Shock |
| **Effects:** |
| Patriotic Gimmicks | Extreme surge (Angle, Undertaker, Austin cheered wildly) |
| Anti-American Heels | Forced to alter/mask gimmicks |
| Violence on TV | Slightly toned down for months |
| Emotional Rawness | Very High (scandal backlash risks multiplied) |
| Fan Mood | Grieving, seeking heroes |

### 2008 Recession

| Attribute | Value |
|-----------|-------|
| Date Range | 2008-2010 |
| Type | Economic |
| **Effects:** |
| Promotion Finances | Struggle unless offering "hope" stories |
| Ticket Prices | Critical sensitivity |
| Worker Moonlighting | Increases significantly |
| Indie Promotion Deaths | Spike in closures |
| Worker Pay Demands | Drop slightly |
| Fan Mood | Anxious, seeking escapism |

### COVID-19 Pandemic (2020)

| Attribute | Value |
|-----------|-------|
| Date Range | March 2020 - ongoing |
| Type | Pandemic |
| **Effects:** |
| Live Events | Shutdown globally |
| Empty Arena Shows | Normalized briefly |
| Streaming | Becomes dominant |
| Small Promotions | Survive if TV exists, collapse otherwise |
| Hardcore Fan Loyalty | Hardens |
| Casual Fan Drift | Increases |

### Internet Explosion (Late 90s-Early 00s)

| Attribute | Value |
|-----------|-------|
| Date Range | 1997-2003 |
| Type | Technology/Cultural |
| **Effects:** |
| Smart Marks | Rise dramatically |
| Kayfabe Loyalty | Drops sharply |
| Scandal Coverage | Explodes in reach and speed |
| Indie Buzz | Becomes viable career builder |
| Promo/Style Adaptation | Must adapt to digital era |
| "Instant Backlash" Risk | Grows significantly |

---

## News Ticker Feature (Optional)

Headlines splash over in-game calendar:

- "Iraq War Begins - Patriotism Surges in U.S."
- "Global Financial Crisis - Indie Scene Suffers Sharp Decline"
- "COVID-19 Outbreak - Live Crowds Suspended in Most Countries"
- "Social Media Boom - Fan Access to Stars Unprecedented"

Wrestlers and promotions comment, adjust, or get swept up by events.

---

## Implementation Notes

### Event Data Structure

```json
{
  "event_id": "covid_19_pandemic",
  "name": "COVID-19 Pandemic",
  "type": "pandemic",
  "start_date": "2020-03-11",
  "end_date": null,
  "effects": {
    "live_events": "suspended",
    "streaming_importance": "+50%",
    "small_promotion_risk": "+80%",
    "casual_fan_retention": "-30%",
    "hardcore_fan_loyalty": "+20%"
  },
  "regions_affected": ["global"],
  "news_headline": "COVID-19 Outbreak - Live Crowds Suspended in Most Countries"
}
```

### Event Check Flow

```
[Month/Quarter Begins]
       ↓
[Check Global Event Database for Active Events]
       ↓
[Apply Effect Modifiers to:]
    - Fanbase DNA
    - Promotion Finances
    - Booking Viability
    - Scandal Tolerance
    - Worker Mood/Movement
       ↓
[Display News Headlines if enabled]
```

---

## RELATED SYSTEMS

- **[[Fanbase Region DNA]]:** Mood and tolerance shifts
- **[[Alt-History Mode]]:** Event randomization options
- **[[Financial System]]:** Economic condition effects
- **[[Scandal System]]:** Tolerance modifiers
- **[[Weather Risk System]]:** Environmental conditions

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Build comprehensive 1980-2020 event database
