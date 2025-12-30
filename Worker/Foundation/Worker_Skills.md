# WORKER SKILLS SYSTEM

📛 **NAME:** Worker Skills System  
🧭 **CATEGORY:** Worker Attributes, Performance & Booking  
🔑 **KEYWORDS:** skills, stats, ratings, bell-to-bell, physical, mental, entertainment, 1-20 scale  
📝 **SUMMARY:**

All visible worker abilities rated on a 1-20 scale (Football Manager style). Four categories: Bell-to-Bell (in-ring), Physical (athleticism), Entertainment (charisma), and Mental (psychology/composure). Tags provide flavor; stats provide mechanical foundation. Psychology is the key multiplier for match quality.

⚙️ **LOGIC OVERVIEW:**

- Workers have 22 total visible skill ratings across 4 categories
- Skills combine with tags to determine match quality, crowd reaction, and booking suitability
- Regional/era context modifies how same stat is perceived (Aerial 15 in 1990 ≠ Aerial 15 in 2020)
- Psychology multiplies other skills: high psych makes average technical work feel great
- Stats grow during peak years (28-35), decline with age/injury
- Drive was removed from Mental stats and moved to Hidden Personality system (Vol 2 decision)

🔬 **LLM INTEGRATION:** Minimal for core stats (numeric calculations), but LLM can generate commentary flavor based on skill combinations and suggest training focuses

📌 **ORIGIN:** Vol. 1 (foundation), Vol. 2 (refinement), Vol. 3 (locked final structure)

📎 **CONNECTED SYSTEMS:** [[Tags_System]], [[Hidden_Personality]], Match Engine, [[Crowd_Memory]], [[Popularity_System]], Injury System, Aging & Career Arcs

❓ **OPEN QUESTIONS:**

- Fourth Mental Attribute still TBD (Improvisation? Match IQ?)
- Stat caps by body type: should size limit aerial ability mechanically?
- Exact injury degradation formulas needed

✅ **STATUS:** LOCKED (Vol 3)

---

## VERSION HISTORY

**Version 1.0 (Vol 1)**

- Initial skill categories proposed
- Drive included as visible Mental stat
- Categories: Bell-to-Bell, Physical, Mental, Entertainment

**Version 1.5 (Vol 2)**

- Mental skills refined to 4 attributes
- Drive removed from visible stats
- Tag system introduced for specialty expression

**Version 2.0 (Vol 3) [CURRENT - LOCKED]**

- Final Mental skill set: 4 attributes
- Drive moved to Hidden Personality system
- Tags system finalized at 394 unique tags
- Skills confirmed as 1-20 scale (FM style)
- Bio/Background separated from core skills

---

## DESIGN PRINCIPLES

1. **Football Manager Style:** All visible skills rated 1-20
2. **Tag System for Flavor:** Use tags (not stats) for nuance and specialization
3. **No Stat Bloat:** Keep core attributes focused, express variation through tags
4. **Regional/Era Scaling:** Same stat value means different things in different contexts

---

## SKILL CATEGORIES

### 🔔 BELL-TO-BELL (In-Ring Performance)

**Purpose:** Core wrestling ability, what happens between the bells

| Skill | Description | Key Impact |
|-------|-------------|------------|
| **Technical Wrestling** | Mat work, holds, transitions, chain wrestling | Match quality in technical/grappling styles |
| **Striking** | Punches, kicks, chops, elbows, knees | Match quality in strike-heavy styles, believability |
| **Aerial/High Flying** | Dives, flips, top-rope moves, springboards | Match quality in high-flying styles, risk/reward |
| **Power Moves** | Slams, suplexes, power bombs, big throws | Match quality in power-based styles, impact moments |
| **Submission Skill** | Applying holds, selling pain, tap-out believability | Match quality in submission-focused matches |
| **Psychology** | In-ring storytelling, crowd manipulation, match pacing instinct | Overall match quality multiplier, feud intensity |
| **Match Pacing** | Rhythm control, knowing when to speed up/slow down | Prevents crowd fatigue, maximizes emotional peaks |
| **Selling** | Reacting to offense believably, sympathy generation | Crowd emotional investment, opponent elevation |
| **Basics** | Footwork, timing, ring movement smoothness, fundamental professionalism | Match flow, visible competence, training school perception |

**Notes:**

- Psychology is the **most important** bell-to-bell stat: it multiplies the value of other skills
- Basics is often invisible when high, but glaringly obvious when low (clunky movement, poor positioning)
- Low psychology + high technical = cold, robotic matches
- High psychology + medium technical = emotionally engaging matches that feel bigger than they are

---

### 💪 PHYSICAL ATTRIBUTES

**Purpose:** Natural physical capabilities and conditioning

| Attribute | Description | Key Impact |
|-----------|-------------|------------|
| **Strength** | Raw power, ability to execute power moves, resistance to opponent power | Power move success, believability against larger opponents |
| **Speed/Agility** | Quickness, reflexes, movement fluidity | High-tempo match quality, aerial move success |
| **Stamina/Cardio** | Endurance in long matches, recovery between shows | Long match performance, multi-show tours, injury resistance |
| **Durability/Toughness** | Pain tolerance, bump-taking ability, injury resistance | Hardcore match survival, injury risk reduction, recovery speed |
| **Size/Presence** | Physical stature and intimidation factor | Believability, crowd perception, certain match-ups |

**Notes:**

- Size/Presence is NOT height/weight (that's bio data): it's the **aura** and how they use their frame
- Example: Ishii (small) has HIGH presence through intensity
- Example: Great Khali (huge) had LOW presence through poor movement/aura

---

### 🎤 ENTERTAINMENT/CHARISMA

**Purpose:** Connection with crowd outside pure in-ring work

| Attribute | Description | Key Impact |
|-----------|-------------|------------|
| **Mic Skills/Promos** | Verbal ability, promo delivery, catchphrase creation | Segment quality, feud heat generation, crowd engagement |

**Promo Skill 3-Dimensional Breakdown (#83):**

The Problem: "How do we handle guys like Sid and Steiner? They aren't technically good promos in the sense they are smooth but they are so fucking awesome."

Solution: Split Promo Into 3 Sub-Attributes:

| Attribute | Description | Examples |
|-----------|-------------|----------|
| **Mic Fluency** | Technical smoothness, word choice, delivery flow | Rock (20), Flair (18), Steiner (7), Sid (6) |
| **Emotional Resonance** | Raw feeling transmission, conviction, making you believe | Steiner (18), Sid (17), Dusty (20), Austin (20) |
| **Memorable Moments** | Creating iconic lines, meme potential, quotable content | Steiner (19), Rock (20), Macho Man (18), Warrior (15) |

**Composite Score:** Weighted average, but situational bonuses for matching promo type to strength.

| Worker | Fluency | Resonance | Memorable | Notes |
|--------|---------|-----------|-----------|-------|
| The Rock | 20 | 18 | 20 | Perfect across all |
| Steiner | 7 | 18 | 19 | Terrible fluency, incredible presence |
| Sid | 6 | 17 | 14 | Same pattern, slightly less memorable |
| Dusty | 14 | 20 | 18 | Heart over polish |
| Malenko | 8 | 8 | 5 | Just not a promo guy |
| **Character Work** | Gimmick commitment, facial expressions, personality consistency | Crowd connection, memorability, merchandise potential |
| **Crowd Connection** | Natural rapport with audience, pop generation ability | Organic overness, crowd loyalty, resilience to bad booking |
| **Entrance/Presentation** | Aura, entrance execution, "bigness" feeling | First impression, main event feel, star quality perception |

**Notes:**

- Character Work ≠ Gimmick quality (that's a booking decision)
- Character Work = how well they **execute** whatever character they're given
- Crowd Connection can exist without mic skills (e.g., Benoit, Liger)

---

### 🧠 MENTAL ATTRIBUTES

**Purpose:** Psychological factors affecting performance and career decisions

**LOCKED SET (4 Attributes):**

| Attribute | Description | Key Impact |
|-----------|-------------|------------|
| **Ring Psychology** | In-match storytelling instinct, opponent reading, crowd manipulation | Match quality multiplier, elevates opponents, feud depth |
| **Adaptability** | Adjusting to unexpected situations, style versatility, learning speed | Multi-style success, botch recovery, international work |

**Adaptability Impact on Match Quality (#31):**

*Workers with high Adaptability (In-Ring) can:*
- Adjust to unfamiliar opponents
- Cover for less skilled partners
- Work multiple styles in one match

*Workers with low Adaptability:*
- Struggle outside comfort zone
- Need opponents who carry them
- Produce inconsistent results vs new styles

| **Composure** | Pressure handling, big-match temperament, focus maintenance | Performance in high-stakes matches, reliability in main events |
| **[Fourth TBD]** | Possibly Improvisation or Match IQ | [Needs final confirmation] |

**REMOVED FROM MENTAL:**

- **Drive** → Moved to Hidden Personality system (Vol 2 decision)
  - Rationale: Drive is personality/ambition, not in-match ability
  - Now lives as hidden trait affecting career arcs, not match performance

**Ring Generalship (#101):**

Separate skill for controlling match flow:

| Aspect | Description |
|--------|-------------|
| **Pacing** | Knowing when to speed up/slow down |
| **Positioning** | Always in right spot for moves/cameras |
| **Transitions** | Smooth movement between sequences |
| **Reading Crowd** | Adjusting on the fly to audience response |
| **Covering** | Hiding mistakes, covering botches |

**Who Has It:** Veterans, psychology masters, natural leaders  
**Who Lacks It:** Green workers, spot monkeys, selfish workers

**Safety Rating System (#102):**

| Rating | Description |
|--------|-------------|
| **Safe Worker** | Rarely hurts opponents, protects them |
| **Standard** | Normal injury rate |
| **Reckless** | Higher injury rate to opponents |
| **Dangerous** | Known for injuring others |
| **Liability** | Should not be trusted with top talent |

**Affected By:** Experience level, Style (aerial = more risk), Ego (selfish workers more reckless), State (tired, intoxicated = more dangerous)

**Notes:**

- Mental stats are **subtle multipliers**, not flashy showstoppers
- High mental stats = consistent quality even in bad situations
- Low mental stats = unreliable, botchy, can't adjust to chaos

---

## STAT INTERACTIONS

### Critical Combinations:

- **Psychology + Selling** = Sympathy Heat Engine
- **Psychology + Match Pacing** = Crowd Manipulation Masters
- **Adaptability + Psychology** = Style Chameleons (Jericho, Danielson)
- **Composure + Mic Skills** = Big Match Promos
- **Stamina + Durability** = Tour Warriors

### Style Archetypes Require:

- **Technical:** High Technical + High Psychology + Medium Stamina
- **Strong Style:** High Striking + High Durability + High Composure
- **High Flyer:** High Aerial + High Speed + Medium Psychology
- **Brawler:** High Striking + High Durability + Medium Power
- **King's Road:** High Everything + Insane Durability + Max Psychology

---

## TAG SYSTEM INTEGRATION

Skills provide the **numerical foundation**. Tags provide the **flavor and specialization**.

**Example 1:** Two workers with Technical 15

- Worker A has tags: "Submission Specialist", "Mat Wizard"
  → Excels in submission-heavy technical matches
- Worker B has tags: "Catch Wrestling", "Stiff"
  → Excels in shootstyle/aggressive technical matches

**Example 2:** Two workers with Aerial 16

- Worker A has tags: "Daredevil", "Innovator of Violence"
  → Insane high-risk dives in deathmatches
- Worker B has tags: "Lucha Traditionalist", "Aerial Grace"
  → Clean, beautiful tope suicidas in traditional lucha

**Critical Tags Referenced:**

- Pain Tolerance (High/Low): affects hardcore match performance
- Innovator of Violence: creative weapon use in brutal matches
- Never Say Die: late-match resilience bonus
- Pressure Cooker: performs better in high-stakes situations
- Style Versatile / Style Locked: adaptability flavor

*(See [[Tags_System]] for full 394-tag breakdown)*

---

## RATING GUIDELINES (1-20 Scale)

### Interpretation:

- **1-5:** Severe weakness, actively hurts matches
- **6-9:** Below average, noticeable limitation
- **10-12:** Average/competent, solid foundation
- **13-15:** Above average, reliable strength
- **16-17:** Elite level, company ace tier
- **18-19:** Generational talent, legendary
- **20:** Perfect, theoretical maximum (extremely rare)

### Examples:

- **Technical Wrestling:**
  - 20: Bret Hart, Zack Sabre Jr (peak)
  - 18: Bryan Danielson, Kurt Angle
  - 16: Chris Benoit, Eddie Guerrero
  - 14: AJ Styles, Samoa Joe
  - 12: John Cena, Randy Orton
  - 10: Batista, Goldberg
  - 8: Ultimate Warrior
  - 5: Great Khali

- **Psychology:**
  - 20: Ric Flair, Mitsuharu Misawa
  - 18: Shawn Michaels, Terry Funk
  - 16: CM Punk, Eddie Guerrero
  - 14: Steve Austin, The Rock
  - 12: Roman Reigns, Batista
  - 10: Jeff Hardy, Rob Van Dam
  - 8: Ryback
  - 5: Jinder Mahal

---

## REGIONAL/ERA SCALING

**CRITICAL DESIGN PRINCIPLE:**
Same numerical rating has **different real-world meaning** based on context.

### Example: Aerial 15

- **1990s WCW:** Rey Mysterio Jr level, revolutionary
- **2020s AEW:** Above average but not spectacular
- **1980s AJPW:** Impossible, doesn't exist in this context
- **2010s Dragon Gate:** Good but not top-tier

### Implementation:

- Stats are **absolute measures of ability**
- Context (era, region, promotion style) **modifies crowd reaction**
- Same worker with same stats gets different reception in different contexts

---

## WORKER BIO SECTION (#4)

📌 **Source:** Vol 1 Extraction #4

**Key Decision:** Size/Frame is **BIO DATA**, not a skill stat. Cleaner AI generation when detached from active skills.

### Bio Fields

| Bio Field | Description | Effect |
|-----------|-------------|--------|
| **Height** | Descriptive (5'6", 6'5", etc.) | Visual aura, bump physics, giant/cruiser classification |
| **Weight** | Descriptive (190lbs, 285lbs, etc.) | Visual size aura, weight class |
| **Body Type** | Physical build category | Affects believability of certain moves |
| **Debut Year** | When career started | Aging curves, historical alignment |
| **Nationality/Region** | Cultural background | Fan base connection, territory options |
| **Primary Style** | Optional starting style | Technician, Brawler, High-Flyer, etc. |

### Body Type Categories

| Type | Description | Stat Implications |
|------|-------------|-------------------|
| **Chiseled** | Classic athletic build | Balanced stats, high sex appeal potential |
| **Bulky** | Thick, muscular | Higher power ceiling, lower aerial ceiling |
| **Lanky** | Tall, thin | Reach advantage, lower power floor |
| **Heavyset** | Large, barrel-shaped | Higher durability, lower speed |
| **Compact** | Short, dense muscle | Lower presence, higher agility potential |
| **Lithe** | Slim, flexible | Higher aerial/agility, lower power |
| **Massive** | Very large (giant territory) | Presence boost, significant physical caps |
| **Average** | Unremarkable build | No bonuses or penalties |

### Body Type Effects

| Body Type | Aerial Ceiling | Power Floor | Speed Modifier | Presence Modifier |
|-----------|----------------|-------------|----------------|-------------------|
| Chiseled | 18 | 8 | +0 | +1 |
| Bulky | 12 | 12 | -1 | +2 |
| Lanky | 14 | 6 | +0 | +1 |
| Heavyset | 10 | 10 | -2 | +2 |
| Compact | 18 | 8 | +1 | -1 |
| Lithe | 20 | 4 | +2 | -1 |
| Massive | 6 | 16 | -3 | +4 |
| Average | 16 | 6 | +0 | +0 |

**Note:** These are soft caps and modifiers, not hard limits. Exceptional workers can exceed them.

---

## DEPENDENCIES

This system requires:

- **[[Tags_System]]** (locked, 394 tags): for flavor and specialization
- **[[Hidden_Personality]]** (locked): for Drive, Ego, Loyalty traits
- **Match Engine** (in progress): to calculate match quality from stats
- **[[Crowd_Memory]]** (locked): to track how stats affect reputation over time
- **[[Popularity_System]]** (locked, 0-100 scale): separate from skills

---

## IMPLEMENTATION NOTES

### Data Structure:

```json
{
  "worker_id": "worker_12345",
  "skills": {
    "bell_to_bell": {
      "technical": 16,
      "striking": 14,
      "aerial": 8,
      "power": 12,
      "submission": 15,
      "psychology": 18,
      "pacing": 16,
      "selling": 17,
      "basics": 15
    },
    "physical": {
      "strength": 11,
      "speed": 13,
      "stamina": 16,
      "durability": 15,
      "presence": 14
    },
    "entertainment": {
      "mic_skills": 14,
      "character_work": 16,
      "crowd_connection": 17,
      "entrance": 15
    },
    "mental": {
      "ring_psychology": 18,
      "adaptability": 15,
      "composure": 17,
      "fourth_attribute": null
    }
  },
  "tags": ["Never Say Die", "Submission Specialist", "King's Road"]
}
```

### Stat Growth:

- Young workers: +1-3 per year in trained skills
- Peak years: 28-35 for most styles (varies by type)
- Decline: -1 per year after peak, accelerated by injuries
- Psychology/Composure: Can INCREASE with age (experience)

---

## UNRESOLVED QUESTIONS

1. **Fourth Mental Attribute**: What should it be?
   - Options: Improvisation, Match IQ, Focus
   - Need to confirm in Vol 5+ or decide

2. **Stat Caps by Body Type**: Should size limit aerial? Should strength scale with size?
   - Currently: No hard caps, just believability modifiers
   - May need refinement

3. **Stat Degradation from Injuries**: How much? How long?
   - Concept exists, formulas needed
   - See INJURY SYSTEM document (in progress)

---

## RELATED SYSTEMS

- [[Tags_System]]: 394 tags for flavor/specialization
- [[Popularity_System]]: 0-100 scale, separate from skills
- [[Hidden_Personality]]: Drive, Ego, Loyalty traits
- Injury System: affects stat degradation
- Aging & Career Arcs: affects stat growth/decline

---

## CALIBRATION REFERENCE

For worker calibration examples (what specific stat values look like on real workers), see:

[[Worker Skill Baseline/_Worker Skill Baseline Index|Worker Skill Baseline]]

Includes calibrations for:
- Entertainment attributes (Rock, Vader, Austin, Cena, etc.)
- Puroresu workers (Misawa, Kawada, Hokuto, Hansen)
- Territory workers (Embry, Flair)
- Modern examples (FTR, Miz, Undertaker reality check)

---

**Document Status:** Complete, locked, ready for implementation  
**Next Review:** After Vol 5-11 analysis (check for any refinements)
