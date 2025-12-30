# POPULARITY SYSTEM

📛 **NAME:** Popularity System  
🧭 **CATEGORY:** Worker Recognition, Crowd Connection & Drawing Power  
🔑 **KEYWORDS:** popularity, overness, regional variation, fan loyalty, drawing power, 0-100 scale  
📝 **SUMMARY:**

Worker popularity is rated 0-100 by region/demographic, separate from skill ratings. A worker can be a mega-star in Japan (Pop 85) and unknown in the US (Pop 15). Popularity affects crowd reactions, merchandise sales, main event viability, and contract value. It's built through booking, match quality, and crowd memory, not just pushed artificially.

⚙️ **LOGIC OVERVIEW:**

- Each worker has separate popularity ratings by: Region, Nation, City, Demographic (age/gender), Fan Type (casual/hardcore/smart)
- Popularity is **not skill**: a terrible worker (Skills 8-10) can be massively over (Pop 80+) through booking/character
- Popularity grows through: match quality, emotional storylines, winning streaks, title runs, crowd connection moments
- Popularity decays through: burial booking, absence, staleness, overexposure, scandal
- "False Popularity" possible: pushed without organic heat, leads to backlash and "manufactured star" tag
- Regional variation is extreme: different cultures react wildly differently to same worker

🔬 **LLM INTEGRATION:** Minimal (numeric tracking), but LLM can analyze popularity trends and suggest booking adjustments to maintain or rebuild heat

📌 **ORIGIN:** Vol. 1 (concept), Vol. 2 (regional variation emphasis), Vol. 3 (locked at 0-100 scale)

📎 **CONNECTED SYSTEMS:** [[Crowd_Memory]], [[Booking_Engine_P1-3]], Match Engine, [[Buzz System/_Buzz System Index|Buzz System]], Merchandise/Economics, Contract Negotiations, Push Momentum

❓ **OPEN QUESTIONS:**

- Exact formulas for popularity growth/decay rates per region
- How quickly does "false popularity" trigger backlash?
- Can popularity recover after extended burial, or is there a point of no return?

✅ **STATUS:** LOCKED (Vol 3 for 0-100 scale and regional variation principle)

---

## VERSION HISTORY

**Version 1.0 (Vol 1)**
- Popularity concept introduced
- Separate from skill ratings
- Affects booking viability and crowd reactions

**Version 1.5 (Vol 2)**
- Regional variation emphasized as core principle
- Demographic splits added (age, gender, fan type)
- False Popularity concept introduced

**Version 2.0 (Vol 3) [CURRENT - LOCKED]**
- 0-100 scale locked
- Growth/decay mechanics formalized
- Backlash threshold defined
- Regional/demographic tracking structure finalized

---

## CORE PRINCIPLES

### 1. Popularity ≠ Skill

- Dean Malenko: Technical 18, Pop 45 (respected but not over)
- Ultimate Warrior: Technical 6, Pop 85 (wildly over despite limitations)
- Misawa/Michaels: High skill + High pop (rare total package)

### 2. Regional Variation is Extreme

Same worker, vastly different reception by region

### 3. Demographic Splits

Kids vs. adults, men vs. women, casual vs. hardcore fans: all react differently

### 4. Pop Growth is Earned, Not Granted

Organic growth is sustainable. Artificial push without crowd buy-in triggers backlash.

---

## POPULARITY SCALE (0-100)

| Range | Status | Drawing Power |
|-------|--------|---------------|
| 90-100 | Mega-Star | Main events anywhere, sells out arenas |
| 80-89 | Top Star | Consistent main eventer, reliable draw |
| 70-79 | Upper Card | Main event ready, good draw in home region |
| 60-69 | Solid Mid-Upper | Can headline B-shows |
| 50-59 | Midcard | Needs support to draw |
| 40-49 | Lower Midcard | Filler matches |
| 30-39 | Undercard | Enhancement talent |
| 20-29 | Jobber Tier | Loses to build others |
| 10-19 | Unknown | Developmental level |
| 0-9 | Invisible | Fresh or buried beyond repair |

---

## GROWTH & DECAY MECHANICS

### Match Quality Impact

Pop Growth = (Match Rating / 10) × Emotional Investment × Booking Context

### Major Event Impacts

- Title Win: +10 to +15
- Screwjob Loss: +5 to +10 (sympathy)
- Betrayal Turn: +8 to +15
- Return (Injury): +10 to +20
- Retirement Match: +15 to +25

### Decay Triggers

- Absence (varies by length)
- Overexposure (appearing without storyline)
- Staleness (repetitive booking)
- Burial (extended jobbing)
- Scandal (varies by severity)

---

## VOL 1 EXTRACTED MECHANICS (Locked)

### Regional Tracking Example: Ric Flair 1983

| Region | Overness |
|--------|----------|
| Southeast US | 96 |
| Mid-Atlantic | 95 |
| Northeast | 75 |
| Midwest | 80 |
| Mexico | 40 |
| Japan | 65 |

**National Average:** ~75 (weighted by regional wrestling market size)

### Soft Caps

Workers have natural popularity ceilings based on:

| Factor | Impact on Cap |
|--------|---------------|
| Charisma | Primary driver of maximum potential |
| Believability | Affects sustainability at high levels |
| Cultural Fit | Region-specific; wrong style = hard cap |
| Promo Skill | Affects growth rate, not cap directly |
| Era Context | What works changes over time |

**Example Soft Caps:**
- Charisma 10 → Pop cap ~60 in most regions
- Charisma 15 → Pop cap ~80
- Charisma 20 → No hard cap, can reach 100
- Low Believability (8-10) → Pop unstable above 70, prone to backlash

### Overness Momentum

Workers aren't static; they're climbing or sliding:

| Status | Effect |
|--------|--------|
| **Climbing** | Recent booking success, crowd responding, growth rate +50% |
| **Stable** | Maintaining position, normal growth/decay |
| **Sliding** | Losing crowd, staleness setting in, decay rate +50% |
| **Freefall** | Major setback (burial, scandal), decay rate +200% |

**Momentum Triggers:**
- Win streak → Climbing
- Title run → Climbing
- Same match repeatedly → Sliding
- Absence without story → Sliding
- Screwjob loss → Can flip to Climbing (sympathy)

### Hidden Reputation Modifiers

Track long-term perception even when worker not actively booked:

- **Nostalgia Bonus:** Workers absent 2+ years gain nostalgia multiplier on return
- **Legacy Weight:** Past accomplishments create floor (legends don't drop below certain threshold)
- **Burned Bridges:** Bad exits create regional penalties that persist
- **Whisper Network:** Backstage reputation affects how willing promotions are to push

### Fan Type Reaction Modifiers

| Fan Type | Preferences | Rejection Triggers |
|----------|-------------|-------------------|
| Casual | Charisma, spectacle, clear stories | Complex booking, workrate focus |
| Hardcore | Workrate, psychology, callbacks | Dumbed-down booking, comedy |
| Smart | Meta-awareness, shoot references | Insulting intelligence, bad booking |
| Kids | Colorful, heroic, merchandise-friendly | Violence, complex morality |
| Traditional | Old school style, respect for history | Modern indie style, flippy stuff |

**Regional Fan Type Distribution:**
- Japan: More hardcore/traditional
- Mexico: Family audience, kids important
- US Attitude Era: Smart fans ascendant
- US Modern: Casual majority, smart vocal minority

---

## FALSE POPULARITY & BACKLASH

When pushed as star without organic support:

- Threshold: (Push Level - Organic Pop) ≥ 20
- Effects: Hostile crowd, "Manufactured Star" tag, slower growth
- Recovery: Turn heel, step back, rebuild organically (6-12 months)

---

## PUSH ORGANICITY SCORE (#33)

📌 **Source:** Vol 1 Extraction #33

### Core Concept

Fans prefer pushes that feel earned. Force-pushing midcarders to main events instantly can backfire.

### Organicity Factors

| Factor | Effect |
|--------|--------|
| Gradual Buildup | +Positive modifier to pop growth |
| Major Feuds Won | +Positive modifier |
| Title Chase Arc | +Strong positive modifier |
| Instant Main Event Push | Risk of rejection |
| Only Looks, No Substance | "X-Pac Heat" mechanic triggers |
| Crowd Rejection Signs | -Negative spiral begins |

### Era Sensitivity for Push Acceptance

**Quick Reference (Fan Mindset by Era):**

| Era | Fan Logic |
|-----|----------|
| 1970s-80s | Accept authority, trust booking |
| 1990s | Rebellious, reject "corporate" picks |
| 2000s-10s | Workrate-conscious, internet-informed |
| 2020s | Hyper-aware, meta-ironic, hashtag-ready |

**Detailed Breakdown:**

| Era | Fan Tolerance | Notes |
|-----|---------------|-------|
| Pre-1990s (Kayfabe) | High tolerance | Fans accept booking decisions more readily |
| 1990s-2000s (Post-Kayfabe) | Medium tolerance | Fans question but still follow |
| 2000s-2010s (IWC Era) | Lower tolerance | Online communities analyze everything |
| 2010s-Now (Social Media) | Lowest tolerance | Instant revolt possible, hashtag campaigns |

### Backstage Leak Risk (Modern Era)

"MAKE ROMAN LOOK STRONG" type leaks can affect fan perception negatively:

| Leak Type | Pop Impact |
|-----------|------------|
| Booking directive leak | -5 to -15 pop with smart fans |
| Protected status revealed | -10 to -20 pop, "corporate creation" tag |
| Political maneuvering exposed | Variable, depends on worker's existing rep |

### Push Organicity Calculation

```
Organicity Score = (
    (Feud Quality × 0.3) +
    (Match Quality Average × 0.3) +
    (Time in Position × 0.2) +
    (Crowd Response Trend × 0.2)
) - (Push Speed Penalty)
```

**Push Speed Penalty:**
- 0 months of buildup: -40
- 1-3 months: -20
- 3-6 months: -10
- 6-12 months: 0
- 12+ months: +10 ("Finally" bonus)

---

## ERA-SENSITIVE FAN LOGIC (#35)

📌 **Source:** Vol 1 Extraction #35

### Core Framework

Different eras have fundamentally different fan expectations and values:

| Era | Primary Fan Values |
|-----|--------------------|
| 1950s-1970s | Kayfabe, territory loyalty, in-ring toughness |
| 1980s | Larger-than-life characters, spectacle, heroes vs villains |
| 1990s | Edginess, attitude, rebellion, reality bleeding in |
| 2000s | Workrate emerging, smart fans vocal, post-kayfabe awareness |
| 2010s | Social media presence, authenticity, "real" characters |
| 2020s+ | Inclusivity, diverse styles, meta-awareness, crossover appeal |

### Scandal Impact by Era

How scandals affect workers differs dramatically by era:

| Era | Scandal Handling |
|-----|------------------|
| 1950s-1980s (Kayfabe) | Scandals matter only if breaking kayfabe, otherwise swept under rug |
| 1990s-2000s (Post-Kayfabe) | Affects alignment, momentum, crowd respect |
| 2010s-Now (Social Media) | Instant explosion, fans expect apologies/suspensions/exile |

### Era Adaptability for Time-Displaced Workers

When workers from one era are placed in another (historical mode, time jumps):

| Scenario | Effect |
|----------|--------|
| Modern worker in older era | High spots may get booed as "phony" |
| Classic worker in modern era | May seem slow/boring to modern fans |
| High Adaptability stat | Worker adjusts faster, smaller penalties |
| Low Adaptability stat | Struggles, marginalized, may leave |

**Example:** Kenny Omega in 1984 Crockett:
- High spots = crowd boos "phony wrestler"
- Must adapt: learn to sell more, work gritty, minimize motion
- OR refuse and get marginalized/leave town

### Era-Specific Pop Modifiers

| Worker Trait | 1980s Modifier | 2000s Modifier | 2020s Modifier |
|--------------|----------------|----------------|----------------|
| High Aerial | +5 | +10 | +8 |
| Strong Style | +8 | +12 | +15 |
| Pure Technical | +10 | +8 | +6 |
| Big Muscles | +15 | +8 | +5 |
| Mic Skills | +12 | +15 | +12 |
| Social Media Presence | N/A | +5 | +15 |
| Controversial Takes | -10 | +5 | ±10 |

### Implementation

Era context should modify:
- How stats translate to crowd reactions
- Which tags are valued vs penalized
- How scandals/controversies are handled
- Push organicity thresholds
- Soft caps on popularity by style

---

## REGIONAL & DEMOGRAPHIC TRACKING

Separate pop scores for:

- Regions (Japan, Mexico, US regions, UK, Europe)
- Age groups (kids, teens, young adults, adults, seniors)
- Gender
- Fan types (casual vs. smart/hardcore)

Regional multipliers affect growth/decay rates based on fan loyalty and cultural fit.

---

## OVERNESS SYSTEM (#6)

📌 **Source:** Vol 1 Extraction #6

### System Architecture (Locked)

| Component | Description |
|-----------|-------------|
| **Scale** | 0-100 (not 20-point like skills) |
| **Regional Tracking** | Each worker has overness per major territory/region |
| **National/World Average** | Auto-calculated across active regions |
| **Hidden Reputation** | Long-term perception tracking, separate from pop |
| **Soft Caps** | Based on charisma, believability, cultural fit |

### Soft Cap Mechanics

Workers have natural popularity ceilings based on their abilities:

| Charisma | Believability | Max Pop Soft Cap |
|----------|---------------|------------------|
| 20 | 20 | 100 (unlimited) |
| 18-19 | 18-19 | 95 |
| 16-17 | 16-17 | 85 |
| 14-15 | 14-15 | 75 |
| 12-13 | 12-13 | 65 |
| 10-11 | 10-11 | 55 |
| <10 | <10 | 45 |

**Note:** Exceptional booking, storylines, or cultural moments can temporarily exceed soft caps.

### Overness Momentum

| Status | Description |
|--------|-------------|
| **Climbing** | Pop increasing, positive booking trajectory |
| **Stable** | Maintaining current level |
| **Sliding** | Pop decreasing, negative trajectory |
| **Rocketing** | Rapid ascent (hot angle, breakout) |
| **Freefall** | Rapid descent (burial, scandal) |

### Hidden Reputation Layer

Separate from visible popularity:

| Component | Description |
|-----------|-------------|
| **Industry Respect** | How other workers/promoters view them |
| **Reliability Score** | Track record of showing up, delivering |
| **Backstage Standing** | Political capital within locker room |
| **Heat Level** | Negative reputation from incidents |

Hidden reputation affects:
- Contract negotiations
- Booking decisions by AI promoters
- Locker room dynamics
- Future opportunities

---

## IMPLEMENTATION NOTES

### Data Structure

```json
{
  "worker_id": "worker_12345",
  "popularity": {
    "global": 65,
    "regional": {
      "japan": 82,
      "mexico": 45,
      "us_northeast": 70,
      "us_south": 55,
      "uk": 60,
      "europe": 48
    },
    "demographic": {
      "kids": 45,
      "teens": 72,
      "young_adults": 78,
      "adults": 65,
      "seniors": 50
    },
    "fan_type": {
      "casual": 60,
      "hardcore": 75,
      "smart": 68
    }
  },
  "false_popularity": {
    "active": false,
    "gap": 0,
    "backlash_risk": 0
  }
}
```

---

## RELATED SYSTEMS

- [[Worker_Skills]]: Skill ≠ Popularity
- [[Tags_System]]: Tags affect how pop grows
- [[Crowd_Memory]]: Memory affects reaction intensity
- [[Booking_Engine_P1-3]]: Booking affects growth/decay
- [[Buzz System/_Buzz System Index|Buzz System]]: Social/media amplifies pop
- Economics: Pop affects merch/gate
- [[Contract System/_Contract System Index|Contract System]]: Pop affects value

---

**Document Status:** Locked (Vol 3), formulas need refinement  
**Last Updated:** 2025-12-22  
**Next Review:** Extract exact growth/decay formulas from later volumes
