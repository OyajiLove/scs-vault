# TAGS SYSTEM

📛 **NAME:** Tags System  
🧭 **CATEGORY:** Worker Flavor, Specialization & Memory  
🔑 **KEYWORDS:** tags, traits, anchors, behavioral flags, style specialization, memory markers  
📝 **SUMMARY:**

Tags are the primary method for expressing worker specialization, personality flavor, and unique characteristics without stat bloat. ~394 unique tags exist across multiple categories. Tags are **active, present-tense traits**. Anchors (separated in Vol 10-11) are **memory-based, past-event markers** used for commentary/booking callbacks.

⚙️ **LOGIC OVERVIEW:**

- Workers are assigned multiple tags (typically 3-10) that flavor their abilities and behavior
- Tags modify how stats are applied (e.g., two workers with Technical 15 play differently based on tags)
- Tags are **not stats** in the traditional sense, but can have **percentage strength** (0-100%) for nuanced expression
- **Non-Binary Tag System** (Vol 2 Chunk 04): Tags range from 0% (absent) to 100% (defining trait), allowing career evolution
- Clear distinction between **Tags** (active traits) and **Anchors** (past memories)
- Tags can be earned/lost over career based on booking, training, or major events
- Some tags are **rare** (Innovator of Violence, Deathmatch Poet), others common (Never Say Die)

🔬 **LLM INTEGRATION:** Yes: LLM uses tags to generate appropriate commentary, promo flavor, match descriptions, and booking suggestions

📌 **ORIGIN:** Vol. 1 (concept), Vol. 2 (initial list + Chunk 04 expansion), Vol. 3 (finalized at 394 tags), Vol. 10-11 (Tag/Anchor separation, V5 master list)

📎 **CONNECTED SYSTEMS:** [[Worker_Skills]], [[Hidden_Personality]], Match Engine, Commentary System, [[Crowd_Memory]], Training/Development, [[Support_Role_Tags]]

❓ **OPEN QUESTIONS:**

- Can workers have conflicting tags? (e.g., "Style Versatile" + "Style Locked")
- Tag acquisition rate: how many per year can be earned through training?
- Tag loss triggers: when do negative tags fade or positive tags decay?

✅ **STATUS:** LOCKED (Vol 3 for base count, Vol 11 for Tag/Anchor distinction, Vol 2 Chunk 04 for non-binary strength system)

📎 **EXPANSION FILE:** [[Tags_Vol2_Chunk04_Expansion]] (100+ new tags, non-binary mechanics, era modifiers)
📎 **EXPANSION FILE:** [[Tags_Vol2_Chunk05_Expansion]] (200+ new tags, fan loyalty system, career arcs)

---

## VERSION HISTORY

**Version 1.0 (Vol 1)**
- Tags concept introduced as alternative to stat bloat
- Workers have Boolean flags for specialization
- Initial tag categories proposed

**Version 2.0 (Vol 2)**
- Initial tag list developed
- Tag/stat interaction defined
- Category structure refined

**Version 3.0 (Vol 3) [LOCKED]**
- 394 unique tags finalized
- Tag acquisition/loss mechanics defined
- Tag density guidelines established

**Version 4.0 (Vol 10-11) [LOCKED]**
- Critical Tag vs. Anchor separation
- Tags = present-tense (what you ARE)
- Anchors = past-tense (what HAPPENED)
- 11 category structure finalized
- V5 master list structure locked
- CSV format defined for implementation

**Version 5.0 (Vol 2 Chunk 04) [CURRENT - LOCKED]**
- **Non-Binary Tag Strength System**: Tags now have 0-100% strength instead of Boolean
- Era/Region modifiers for certain tags (e.g., Trainee Tyrant backlash varies by culture)
- Ethnic Folk Hero cross-checking system (worker ethnicity vs regional demographics)
- 100+ new tags added (see [[Tags_Vol2_Chunk04_Expansion]])
- Total tags now estimated at 440+

---

## MATCH & PERFORMANCE TAGS (Vol 1 Extraction)

### Match Calling Tags (#121)

Tags that affect in-match behavior and match construction:

| Tag | Effect |
|-----|--------|
| **Calls It In Ring** | Improvises match structure during performance |
| **Needs Agent Help** | Requires road agent layout for good matches |
| **Stubborn Caller** | Won't deviate from planned spots |
| **Generous Seller** | Prioritizes making opponent look good |
| **Spot Caller** | Likes to string signature sequences |
| **Story Caller** | Focuses on narrative over moves |

**Impact:** Determines match quality with different partner types and booking styles.

### Crowd Interaction Tags (#104)

| Tag | Effect |
|-----|--------|
| **Crowd Worker** | Excels at playing to audience |
| **Stoic Performer** | Ignores crowd, focused on match |
| **Crowd Hype Man** | Gets fans involved, leads chants |
| **Deaf to Crowd** | Doesn't adjust based on reactions |
| **Crowd Antagonist** | Heels who rile fans expertly |

**Impact:** High crowd interaction in dead crowds = can wake them up. In hot crowds, over-pandering can look desperate.

### Selling Style Tags (#210)

| Style | Description | Examples |
|-------|-------------|----------|
| **Ragdoll Seller** | Bounces around for opponent's offense | Ziggler, Shawn Michaels |
| **Stoic Seller** | Minimal but meaningful, fights through | Kawada, Hansen |
| **Dramatic Seller** | Big expressions, theatrical | Flair, Rock |
| **Technical Seller** | Sells body parts consistently | Bret Hart, Danielson |
| **No-Sell Monster** | Absorbs damage, delayed reaction | Undertaker, Lesnar |
| **Inconsistent Seller** | Quality varies match to match | Many |

**Impact:** Determines how matches feel, affects partner's offense perception.

### Promo Style Tags (#161)

| Promo Style | Good For | Examples |
|-------------|----------|----------|
| **Righteous Fury** | Intense face promos | Sid, Warrior, peak Cena |
| **Dangerous Madman** | Unhinged heel energy | Steiner, Terry Funk, Moxley |
| **Smooth Operator** | Polished heel/face | Flair, Rock, early Shawn |
| **Snarky Wit** | Meta/clever heel | MJF, Punk, Heenan |
| **Rugged Everyman** | Working class appeal | Dusty, Foley, Eddie Kingston |

**Usage:** You book the KIND of promo, and the system interprets worker ability to land it based on their style fit.

### Finisher Protection Tags (#132)

Political tags affecting how workers take losses:

| Tag | Effect |
|-----|--------|
| **Kick Out at 3.1** | Engine triggers late kickout animation in losses |
| **Demands Visual Dominance** | Won't sell weakness in defeat |
| **Refuses Submission Losses** | Only loses to pins or KO |
| **No-Sell Mentality** | Takes pin but refuses to bump cleanly |
| **Demands Strong Post-Loss Angles** | Requires revenge beatdown after loss |

**Context Sensitivity:**
- Bigger mismatch = more politicking
- Company culture affects tolerance (AJPW = "Protect Your Aura", WWE = "Obey the Script")

### Physical Cost Tags (#250, #251)

📌 **Source:** Vol 1 Extraction #250-251

**Fragile Warrior (#250):**

| Tag | Effect |
|-----|--------|
| **Fragile Warrior** | Delivers incredible performances but at high physical cost. Prone to injury, body breaks down faster. |

**Examples:** Dynamite Kid, Hayabusa, early Jeff Hardy  
**Booking Consideration:** Space out their big matches, use sparingly.

**Selective Big Man Seller (#251):**

| Tag | Effect |
|-----|--------|
| **Selective Big Man Seller** | Monster/giant who doesn't sell for everyone but will bump huge for select opponents. |

**Mechanics:**
- Default: No-sell mode against most opponents
- Triggered: When facing top babyface or in title match, sells dramatically
- Creates special moment feel

**Example:** Undertaker selling for Shawn Michaels but not for midcarders.

---

## TAG VS. ANCHOR DISTINCTION (Vol 10-11)

### Tags (Active Traits)

- **Present-tense**
- Describe current abilities, tendencies, or characteristics
- Used in match simulation, booking decisions, training
- Examples: "Never Say Die", "Submission Specialist", "Locker Room Politician"

### Anchors (Memory Markers)

- **Past-tense or memory-based**
- Record significant career moments, incidents, relationships
- Used for commentary callbacks, booking memory, feud depth
- Dynamically generated from gameplay, not pre-assigned
- Examples: "Screwed at WrestleMania", "Betrayed by Mentor", "Cover-Up Incident"
- **Separate system** with own seed list

**Critical Design Rule:** Tags = what you ARE. Anchors = what HAPPENED to you.

---

## TAG CATEGORIES

Based on Vol 10-11 audit structure:

1. **Behavior** - Backstage conduct, locker room tendencies
2. **Booking** - How they're used, push patterns, crowd manipulation
3. **Style** - In-ring approach, specialty moves, match preferences
4. **Performance** - Technical execution, reliability, consistency
5. **Personality** - Character traits, emotional patterns (overlaps with Hidden Personality)
6. **Entertainment** - Promo style, crowd work, presentation
7. **Lifestyle** - Outside the ring behaviors, dedication, personal life
8. **Legacy** - Career history markers, reputation elements
9. **Political** - Backstage power, influence, relationships
10. **Division** - Weight class, gender, specialty divisions
11. **Gimmick** - Alignment proficiency, character archetypes (e.g., "Monster Heel", "Underdog Babyface")

---

## KEY TAGS (Examples from Locked Volumes)

### Match Specialty Tags

- **Pain Tolerance (High/Low)** - Affects hardcore match performance
- **Innovator of Violence** - Creative weapon use, unique deathmatch spots
- **Submission Specialist** - Excels in submission-heavy technical matches
- **High Flyer** - Aerial move proficiency
- **Power Fighter** - Slams and power moves
- **Deathmatch Poet** - Spiritual hardcore connection
- **Technical Wizard** - Mat wrestling mastery
- **Strong Style** - Stiff striking, realistic aggression
- **Lucha Libre** - Traditional lucha execution
- **King's Road** - Epic escalation, dramatic selling

### Personality/Behavior Tags

- **Never Say Die** - Late-match resilience, fighting spirit bonus
- **Pressure Cooker** - Performs better in high-stakes matches
- **Locker Room Politician** - Backstage maneuvering tendency
- **Territory Lifer** - Regional loyalty, resents outsiders
- **Freelance Superstar** - Refuses long-term contracts
- **Ritual Purist** - Resists gimmick/style changes (lucha traditionalist)
- **Cultural Icon** - Deep regional/cultural connection
- **Buzz Chaser** - Chases trends, social media obsessed
- **Old School** - Traditionalist, resists modern booking
- **Company Man** - Loyal soldier, does what's asked

### Career/Legacy Tags

- **Hall of Fame Bound** - Legendary status trajectory
- **Flash in the Pan** - Short peak, rapid decline
- **Late Bloomer** - Slow developer, long career
- **Journeyman** - Solid worker, never quite breaks through
- **Glass Ceiling** - Can't get main event push despite ability
- **Push Victim** - Crowd sympathy from burial booking
- **Legacy-Obsessed** - Protects reputation fiercely

### Performance Tags

- **Spot Timing Virtuoso** - Perfect execution timing
- **Botch-Prone** - High error rate
- **Stiff Worker** - Works snug, may injure opponents (see regional reception below)
- **Safe Worker** - Protects opponents, low injury risk
- **Psychology Monster** - Master storyteller in-ring
- **Reliable** - Consistent quality every night
- **Big Match Performer** - Elevates in important matches

---

## REGIONAL RECEPTION MECHANICS (#5)

📌 **Source:** Vol 1 Extraction #5

Some tags have different effects depending on regional/cultural context:

### Stiff Worker Tag

| Region | Reception |
|--------|----------|
| **Japan (AJPW, NJPW, NOAH)** | Preferred, praised as "real" wrestling |
| **Strong-style indies, modern AEW** | Neutral to positive |
| **80s-90s American mainstream** | Negative, causes complaints, potential heat with office |
| **Family-friendly promotions** | Very negative, may lead to release |

**Examples:** Vader, Kawada, Ishii, Suzuki, Finlay, Danielson, Lesnar

### Lucha Traditionalist Tag

| Region | Reception |
|--------|----------|
| **CMLL, traditional lucha** | Essential for respect |
| **AAA** | Less important |
| **US promotions** | Neutral |
| **Japanese promotions** | Neutral to positive |

### Hardcore/Deathmatch Tags

| Region | Reception |
|--------|----------|
| **FMW, BJW, CZW** | Celebrated |
| **ECW** | Core identity |
| **Mainstream US (WWE, WCW)** | Controversial, limited use |
| **Traditional puroresu** | Negative |

---

### Vol 1 Extracted Tags (Locked)

#### Stiff Worker - Regional Reception Table

| Region/Style | Reception | Notes |
|--------------|-----------|-------|
| Japan (AJPW, NJPW, NOAH) | Preferred, praised | Expected in main event style |
| Strong-style indies, modern AEW | Neutral to positive | Appreciated by hardcore fans |
| 80s-90s American mainstream | Negative | Causes complaints, "unsafe" label |
| Family-friendly WWE | Negative | Restricted, liability concern |

**Examples:** Vader, Kawada, Ishii, Suzuki, Finlay, Danielson, Lesnar

#### Fragile Warrior

**Definition:** Tough as hell but often injured due to reckless bumping or chronic conditions  
**Character Impact:** Adds pathos, fans worry about them, matches feel dangerous  
**Mechanical Effect:** Higher injury risk, but emotional investment bonus in major matches  
**Examples:** Akira Hokuto, Dynamite Kid, Bryan Danielson, Hayabusa

#### Selective Big Man Seller

**Definition:** Will sell for specific opponents when story demands it, otherwise no-sells like a tank  
**Application:** Big men who selectively enter "babyface selling mode" for the right opponent/story  
**Mechanical Effect:** Selling stat contextual based on opponent overness and match importance  
**Examples:** Stan Hansen, Vader (both could sell their ass off when motivated)

#### Weekend Warrior

**Definition:** Worker not full-time professional; wrestling is hobby or temporary side gig  
**Effects:**
- Rapid skill decline when not active
- Higher chance of leaving industry
- Very low Drive to improve
- Increased no-show chance if injured/discouraged
- Minimal backstage political impact

**Application:** Ham and Eggers, very low-level enhancement workers in regional/territory feds

#### Scar Tissue

**Definition:** Body shows heavy scarring from previous battles (deathmatches, blade jobs)  
**Effects:**
- Menace +1-3 based on existing score
- Slight penalty for "clean image" promotions
- Bonus for hardcore audience connection

**Dynamic Acquisition:** Can appear during career from accumulated health damage (not just assigned at creation)  
**Examples:** Onita, Foley, Abdullah, Necro Butcher, Jun Kasai

#### Beauty In Struggle

**Definition:** Emotional resonance through hardship arcs; the chase more beautiful than the reign  
**Application:** Workers whose appeal comes from fighting against odds, not from victories  
**Mechanical Effect:** Boosts emotional investment in major matches, especially long arcs of hardship  
**Design Origin:** Core SCS philosophy tag, represents the soul of the project  
**Examples:** Kawada, Hokuto, Dusty Rhodes, Eddie Guerrero, Hangman Adam Page

---

## INJURY VULNERABILITY TAGS (#79)

📌 **Source:** Vol 1 Extraction #79

Body part specific vulnerability tags that increase injury risk and wear accumulation:

| Tag | Effect |
|-----|--------|
| **Troublesome Neck** | More wear and tear to head section, more likely neck-related injury |
| **Troublesome Back** | More wear and tear to body section, more likely back-related injury |
| **Troublesome Shoulder** | More wear and tear to arms section, more likely shoulder-related injury |
| **Troublesome Knee** | More wear and tear to legs section, more likely knee-related injury |
| **History of Concussions** | Increased chance of injury being a concussion |
| **Brittle Bones** | Increased chance of injury being severe |
| **Rubber Bones** | Decreased chance of injury being severe |

**Acquisition:** Can be pre-assigned based on career history or dynamically gained through accumulated injuries.

**Connected Systems:** [[Injury System/_Injury System Index|Injury System]], [[Injury System/Wear and Tear System|Wear and Tear]]

---

## CAREER FUTURE & MOBILITY TAGS (#80, #133)

📌 **Source:** Vol 1 Extraction #80, #133

### Retirement Destiny Tags

Determine what workers do after active competition:

| Tag | Effect |
|-----|--------|
| **Future Referee** | Will choose to be available as referee upon retirement |
| **Future Play By Play** | Will choose to be available as play-by-play commentator upon retirement |
| **Future Colour Commentator** | Will choose to be available as colour commentator upon retirement |
| **Future Manager** | Will choose to be available as manager upon retirement |
| **Future Personality** | Will choose to be available as personality upon retirement |
| **Future Road Agent** | Will choose to be available as road agent upon retirement |
| **Natural Trainer** | Much higher chance of running own dojo after retirement |

### Retirement Behavior Tags

| Tag | Effect |
|-----|--------|
| **Desperado** | Won't retire until very old unless forced by injury |
| **Heart's Not In It** | Tends to retire younger than normal |
| **Wrestling In The Blood** | Will never retire from business no matter how old |
| **Can't Stay Away** | Considerably easier to talk into coming out of retirement |
| **Unable To Wrestle Again** | Cannot be talked into coming out of retirement |

### Mobility Tags

Determine worker movement patterns:

| Tag | Effect |
|-----|--------|
| **Loyal** | More inclined to stay for long time rather than seek new challenges |
| **Itchy Feet** | More inclined to leave after few years to seek new challenges |
| **Homebody** | Will not become available in new game areas |
| **World Traveler** | Higher chance of choosing to become available in new game areas |
| **Deep Roots** | Settled where they are, will never move house to new region |

**Connected Systems:** [[Retirement System/_Retirement System Index|Retirement System]], [[Contract System/_Contract System Index|Contract System]]

---

## WORKER MEDICAL REACTION TAGS (#176)

📌 **Source:** Vol 1 Extraction #176

Personality-based reactions to medical advice and injury management:

| Tag | Behavior |
|-----|----------|
| **Driven to Destruction** | Furious about being asked to slow down, pushes through injuries, risk of painkiller addiction |
| **Fragile/Lazy** | Accept medical advice easily, may milk injuries politically |
| **Loyalist** | Listen if respected by management, work with reduced loads |
| **Bitter** | Leak resentment, cause morale issues, potential no-show |

**System Interaction:** These tags affect outcomes when medical exams trigger intervention decisions.

**Historical Example (Kurt Angle 2005):**
WWE sends for evaluation → Severe neck flagged → Time off suggested → "Driven to Destruction" tag triggers fury → Threatens to leave → Builds painkiller addiction → Leaves for TNA → Rebuilds career in new arc → Legacy becomes tragic-heroic.

**Connected Systems:** [[Injury System/_Injury System Index|Injury System]], [[Injury System/Addiction Risk System|Addiction Risk System]]

---

## GROWTH & DECLINE TAGS (#78)

📌 **Source:** Vol 1 Extraction #78

These tags affect worker development arcs over their career:

### Physical Potential Tags

| Tag | Effect |
|-----|--------|
| **Stud Athlete** | Hidden caps on Power, Athleticism, and Stamina always higher than normal |
| **Gymnastic Background** | Hidden caps on Athleticism, Aerial, and Flashiness always higher than normal |
| **Amateur Wrestling Background** | Hidden caps on Athleticism, Basics, Stamina, and Technical always higher than normal |

### Learning Rate Tags

| Tag | Effect |
|-----|--------|
| **Prodigy** | Improves skills at faster rate during maturity phase |
| **Not A Natural** | Improves skills at slower rate during maturity phase |

### Aging & Decline Tags

| Tag | Effect |
|-----|--------|
| **Age Is Just A Number** | Loses skills at slower rate during decline phase |
| **Can't Fight Time** | Loses skills at faster rate during decline phase |

### Physical Condition Tags

| Tag | Effect |
|-----|--------|
| **Iron Man** | Physical condition declines at slower rate from natural wear and tear |
| **Frail** | Physical condition declines at faster rate from natural wear and tear |
| **Quick Healer** | Recovers from significant injuries far quicker than normal |

### Body Composition Tags

| Tag | Effect |
|-----|--------|
| **Fitness Fanatic** | Less likely to become out of shape, better able to keep toned/muscular physique |
| **Bodybuilder** | More likely to get bigger, better able to keep muscular/ripped physique |
| **Skinny Genes** | Less likely to get fat or out of shape |

### Career Longevity Tags

| Tag | Effect |
|-----|--------|
| **Desperado** | Unless forced through injury, will not retire until very old |
| **Natural Trainer** | Naturally gifted at training others, higher chance of running own dojo |

---

## CREATIVITY & ADAPTABILITY TAGS (#82)

📌 **Source:** Vol 1 Extraction #82

These tags govern innovation, character flexibility, and era navigation:

### Core Innovation Tags

| Tag | Description | Examples |
|-----|-------------|----------|
| **Creative Dynamo** | Regularly innovates fresh spots, match structures, gimmicks, or promos | Chris Jericho, Kenny Omega, Mick Foley |
| **Promo Innovator** | Brings fresh promo styles, catchphrases, presentation | The Rock, Dusty Rhodes, CM Punk |
| **Spot Innovator** | Excels at inventing new moves, high spots, signature sequences | Will Ospreay, Kenta Kobashi |
| **Finisher Architect** | Creates iconic finishing moves or transitions | Kobashi (Burning Hammer), AJ Styles |

### Character/Persona Flexibility Tags

| Tag | Description | Examples |
|-----|-------------|----------|
| **Gimmick Chameleon** | Can seamlessly reinvent persona without losing credibility | Undertaker, Chris Jericho, Kenny Omega |
| **Character Immersion Expert** | Becomes the gimmick completely. Sells with body language alone. | Mankind, Suzuki |
| **Anti-Gimmick Purist** | Wants nothing but pure competition/presentation. Avoids flashy personas. | Low Ki, Malenko |

### Era Navigation Tags

| Tag | Description | Examples |
|-----|-------------|----------|
| **Era Shifter** | Naturally adapts to evolving styles and audiences | Chris Jericho, Rey Mysterio |
| **Old School Purist** | Believes in traditional wrestling presentation. Struggles to adapt. | Harley Race, Jim Cornette |
| **One-Trick Pony** | Highly skilled but limited creatively. Struggles to reinvent when act goes stale. | Ultimate Warrior, Sid |

### Style/Structure Flexibility Tags

| Tag | Description | Examples |
|-----|-------------|----------|
| **Style Wanderer** | Can borrow from multiple styles and blend | Danielson, Finlay, Ibushi |
| **Hard Style Adapter** | Can adjust stiffness or structure depending on territory | Danielson, Kobashi |
| **Deathmatch Artist** | Uses weapons/violence for genuine storytelling | Jun Kasai, Onita, Kudo |
| **Style Versatile** | Can adapt ringwork naturally across multiple styles | Danielson, Jericho, Ibushi |

---

## TAG ASSIGNMENT

### Generated Workers

- Assigned 3-10 tags at generation based on:
  - Archetype (Hidden Personality)
  - Skill ratings (high Technical → "Submission Specialist" candidate)
  - Region/Era (1980s Japan → "Strong Style" common)
  - Career stage (veteran → "Ring General", rookie → "Green")

### Tag Acquisition (Career Development)

- **Training:** Can focus on earning specific style tags
- **Booking:** Repeated hardcore bookings → "Hardcore Specialist"
- **Feuds:** Long blood feud → "Rivalry Expert"
- **Title Runs:** Successful defense streak → "Champion Mentality"
- **Major Events:** Retirement match → "Legacy Match"

### Tag Loss

- **Injury:** May lose physical specialty tags temporarily
- **Booking Change:** "Main Event Star" lost if buried to midcard for extended period
- **Retirement/Return:** Some tags persist, others fade
- **Age:** "High Flyer" may decay to "Grounded Veteran"

---

## TAG INTERACTIONS WITH STATS

Tags **modify** how stats are expressed, they don't replace them.

### Example 1: Technical Wrestling 15

**Worker A:** Technical 15 + "Submission Specialist" + "Mat Wizard"

- Excels in submission-focused grappling
- Crowd pops for hold transitions
- Commentary emphasizes technical mastery

**Worker B:** Technical 15 + "Catch Wrestling" + "Stiff Worker"

- Excels in aggressive, shoot-style grappling
- Crowd reacts to realistic intensity
- Commentary emphasizes toughness and danger

### Example 2: Striking 16

**Worker A:** Striking 16 + "Strong Style" + "King's Road"

- Brutal, escalating elbow wars
- Crowd expects stiff exchanges
- High injury risk for opponent

**Worker B:** Striking 16 + "Lucha Libre" + "Aerial Grace"

- Flashy kicks integrated with flips
- Crowd expects athleticism, not brutality
- Low injury risk

### Example 3: Charisma 14

**Worker A:** Charisma 14 + "Promo Wizard" + "Cult of Personality"

- Captivating promos, crowd hangs on every word
- Can get over with mic work alone

**Worker B:** Charisma 14 + "Silent Badass" + "Aura Over Words"

- Crowd connection through presence, not talking
- Weak promos but strong entrance/body language

---

## TAG CONFLICTS & SYNERGIES

### Conflicting Tags (Should Not Coexist)

- "Style Versatile" ↔ "Style Locked"
- "Safe Worker" ↔ "Stiff Worker"
- "Flash in the Pan" ↔ "Long-Term Draw"
- "Locker Room Leader" ↔ "Locker Room Cancer"

**Note:** Vol 10-11 audit should flag these conflicts for cleanup.

### Synergistic Tags (Amplify Each Other)

- "Never Say Die" + "Pressure Cooker" = Epic comeback specialist
- "Psychology Monster" + "Ring General" = Match flow master
- "Innovator of Violence" + "Deathmatch Poet" = Hardcore legend
- "Lucha Traditionalist" + "Ritual Purist" = Mask-focused legend
- "Promo Wizard" + "Cult of Personality" = Megastar potential

---

## TAG VISIBILITY

### Player-Visible Tags

- Most tags are visible to player in worker profile
- Help player make booking decisions
- Guide training focus

### Hidden Tags (Rare)

- Some personality/behavior tags may be hidden
- Revealed through emergent behavior
- Example: "Backstage Politician" might not display but affects locker room events

### Commentary-Only Tags

- Some tags only affect commentary flavor
- Don't impact mechanics significantly
- Example: "Charismatic Entrance", "Crowd Favorite"

---

## TAG DENSITY BY WORKER TYPE

| Worker Type | Typical Tag Count | Focus |
|-------------|-------------------|-------|
| **Main Event Star** | 8-12 | Broad skillset, multiple specialties |
| **Midcard Specialist** | 5-8 | Focused niche, clear identity |
| **Jobber/Enhancement** | 3-5 | Basic traits, room to grow |
| **Veteran** | 10-15 | Accumulated over career, some legacy tags |
| **Rookie** | 2-4 | Potential tags, few earned tags |
| **Legend** | 12-20 | Full career history reflected |

---

## V5 MASTER LIST STRUCTURE (Vol 11)

Final CSV format:

```
Tag Name, Type, Category, Description, Notes, Visibility, Classification, Converted From Anchor
```

**Total Tags (Vol 3):** 394 unique tags  
**Classification (Vol 10-11):** Separating Tags (active) from Anchors (memory)  
**Status:** V5 master list structure locked, final audit in progress (weekend classification pass)

### Audit Process (Vol 11)

1. Manual classification: Tag / Anchor / Both
2. Present-tense conversion (past-tense → anchors)
3. Redundancy check
4. Category alignment
5. Final lock: `SCS_Tag_List_V5_FINAL_MASTER_LOCKED.csv`

---

## ANCHOR SYSTEM (Separate but Related)

### Anchor Purpose

- Record **unique, story-carving moments** in worker history
- Used for:
  - Commentary callbacks
  - Booking memory
  - Feud depth
  - Crowd reaction modifiers

### Anchor Generation

- **Seeded:** Base list of common anchors (title wins, betrayals, injuries)
- **Dynamic:** Best anchors emerge from gameplay
  - Screwed finish in big match
  - Mentor betrayal
  - Career-threatening injury
  - Scandal cover-up
  - Faction implosion
  - Legendary match

### Anchor Examples

- "Screwed at [Event Name]"
- "Betrayed by [Wrestler Name]"
- "[Body Part] Injury (Career-Threatening)"
- "Barroom Incident ([Date])"
- "Cover-Up Scandal"
- "Faction Leader (Defunct)"
- "Legendary Match vs. [Opponent]"

### Anchor Decay

- Some anchors **never fade** (career-defining moments)
- Others decay over time (minor incidents forgotten)
- Crowd memory system determines anchor weight

---

## INJURY VULNERABILITY TAGS (#79)

📌 **Source:** Vol 1 Extraction #79

Body part-specific vulnerability tags that increase injury risk:

| Tag | Effect |
|-----|--------|
| **Troublesome Neck** | More wear and tear to head section, more likely to be neck-related injury |
| **Troublesome Back** | More wear and tear to body section, more likely to be back-related injury |
| **Troublesome Shoulder** | More wear and tear to arms section, more likely to be shoulder-related injury |
| **Troublesome Knee** | More wear and tear to legs section, more likely to be knee-related injury |
| **History of Concussions** | Increased chance of injury being a concussion |
| **Brittle Bones** | Increased chance of injury being severe |
| **Rubber Bones** | Decreased chance of injury being severe |

**Usage:** Applied to workers with known problem areas. Affects [[Injury System/_Injury System Index|Injury System]] calculations.

---

## CAREER FUTURE TAGS (#80, #133)

📌 **Source:** Vol 1 Extraction #80, #133

### Retirement Destiny Tags

| Tag | Effect |
|-----|--------|
| **Future Referee** | Will choose to be available as referee upon retirement |
| **Future Play By Play** | Will choose to be available as play-by-play commentator upon retirement |
| **Future Colour Commentator** | Will choose to be available as colour commentator upon retirement |
| **Future Manager** | Will choose to be available as manager upon retirement |
| **Future Personality** | Will choose to be available as personality upon retirement |
| **Future Road Agent** | Will choose to be available as road agent upon retirement |
| **Natural Trainer** | Much higher chance of running own dojo after retirement |

### Retirement Behavior Tags

| Tag | Effect |
|-----|--------|
| **Desperado** | Won't retire until very old unless forced by injury |
| **Heart's Not In It** | Tends to retire younger than normal |
| **Wrestling In The Blood** | Will never retire from business no matter how old |
| **Can't Stay Away** | Considerably easier to talk into coming out of retirement |
| **Unable To Wrestle Again** | Cannot be talked into coming out of retirement |

### Mobility Tags

| Tag | Effect |
|-----|--------|
| **Loyal** | More inclined to stay for long time rather than seek new challenges |
| **Itchy Feet** | More inclined to leave after few years to seek new challenges |
| **Homebody** | Will not become available in new game areas |
| **World Traveler** | Higher chance of choosing to become available in new game areas |
| **Deep Roots** | Settled where they are, will never move house to new region |

### Scheduling/Availability Tags (#254)

📌 **Source:** Vol 1 Extraction #254

| Tag | Effect |
|-----|--------|
| **Weekend Warrior** | Worker not fully committed to wrestling, works limited dates |
| **Full-Time Road Warrior** | Works maximum dates, always available |
| **Special Attraction Only** | Only booked for big events |

**Weekend Warrior Implications:**
- Can't build consistent momentum
- May be used for special attractions
- Lower injury risk (less wear)
- Harder to push as consistent star
- Contract negotiations reflect limited availability

**Examples:** Part-timers, workers with day jobs, semi-retired legends

**Booking Considerations:**
- Don't build storylines requiring weekly presence
- Excellent for one-off dream matches
- Can maintain mystique through scarcity
- Risk: fans forget them between appearances

---

## VOL 2 EXTRACTED TAGS

📌 **Source:** Vol 2 Extraction

### Style Presentation Tags

| Tag | Effect |
|-----|--------|
| **Flashy** | Prioritizes move beauty, spectacle, and visual pop. Risk-taking, even if psychology or selling suffers. Crowd loves the dazzle. |

**Design Note:** Flashy is a TAG, not a skill. Skill scores are about functional execution; tags are about flavor, audience perception, and meta. Flashiness is often surface-level: you can be flashy but bad at match logic (early Jack Evans). Some workers evolve beyond being flashy.

**Associated Archetype:** [[Indie_Darling_Archetype|Indie Darling]]

### Good Hand Archetype Tags

| Tag | Effect |
|-----|--------|
| **Professional** | Fine with losing often without morale collapse. Prioritizes the show over ego. |
| **Ring Glue** | Matches involving Good Hands are less likely to have botches, storytelling issues, or crowd tuning out. |
| **Occasional Bone** | Loyalty/consistency may occasionally trigger a midcard title shot or showcase match. |
| **Backbone** | Valued deeply by bookers, smart fans, and peers. Provides a steady, reliable presence across cards and eras. |

**Associated Archetype:** [[Good_Hand_Archetype|Good Hand]]

### Fighting Spirit Archetype Tags

| Tag | Effect |
|-----|--------|
| **Never Say Die** | Rally boosts when badly damaged but still fighting. Late-match resilience, fighting spirit bonus. |
| **Spirit Bomb** | Able to draw surges from crowd when critically injured. Massive comebacks when crowd fully invested. |
| **Pressure Cooker** | Finishing stretches become more dangerous after long battles. Performs better in high-stakes matches. |

**Associated Archetype:** [[Fighting_Spirit_Archetype|Fighting Spirit]]

---

## MEDICAL REACTION TAGS (#176)

📌 **Source:** Vol 1 Extraction #176

Personality-based reactions to medical advice and intervention:

| Tag | Behavior |
|-----|----------|
| **Driven to Destruction** | Furious about being asked to slow down, pushes through, risk addiction |
| **Fragile/Cautious** | Accept medical advice easily, may milk injuries politically |
| **Loyalist Listener** | Listen if respected, work with reduced loads willingly |
| **Bitter Resister** | Leak resentment, cause morale issues, potential no-show |

**Usage:** Determines worker response when [[Injury System/Medical Exam System|Medical Exam System]] recommends intervention.

---

## IMPLEMENTATION NOTES

### Data Structure

```json
{
  "worker_id": "WORK_12345",
  "tags": [
    "Never Say Die",
    "Submission Specialist",
    "King's Road",
    "Psychology Monster",
    "Ring General",
    "Veteran Presence"
  ],
  "anchors": [
    {
      "anchor_id": "anchor_67890",
      "type": "Betrayal",
      "description": "Betrayed by tag partner at WrestleWar 2024",
      "date": "2024-05-15",
      "weight": 0.85,
      "decay_rate": 0.05
    }
  ],
  "tag_history": [
    {"date": "2023-08", "tag": "High Flyer", "action": "added", "trigger": "training"},
    {"date": "2024-11", "tag": "High Flyer", "action": "removed", "trigger": "injury"}
  ]
}
```

### Tag Limits

- **Soft cap:** ~12-15 tags for most workers
- **Hard cap:** 20 tags maximum (prevents bloat)
- Oldest/least relevant tags pruned when new ones added

### Tag Categories for Filtering

- Player can filter worker search by tags
- AI booker can request workers with specific tag combinations
- Training system suggests tags to pursue based on stats

---

## RELATED SYSTEMS

- [[Worker_Skills]]: Tags modify stat expression
- [[Hidden_Personality]]: Some personality tags overlap
- Match Engine: Tags affect match quality calculation
- Commentary System: Tags generate flavor text
- [[Crowd_Memory]]: Anchors affect crowd reactions
- Training System: Tag acquisition through development

---

**Document Status:** System locked (Vol 3), V5 structure locked (Vol 11), final audit in progress  
**Last Updated:** 2025-12-25 (Vol 2 Chunk 03 expansion)  
**Next Review:** After weekend classification pass, check for final master list

---

## VOL 2 CHUNK 03 EXPANSION

📌 **Source:** Vol 2 Chunk 03 (massive tag discussion)

### Skill Clarifications

#### Legitimacy vs Believability

| Skill | Meaning | Category | Examples |
|-------|---------|----------|----------|
| **Legitimacy** | How good a worker is in a real fight: actual toughness, amateur wrestling, striking, grappling, MMA background. | Physical Attribute | Minoru Suzuki (20), Brock Lesnar (20), CM Punk (low) |
| **Believability** | How convincing the worker is in their performance: making strikes, holds, selling look real to the crowd. | Performance Attribute | Jake Roberts (20), The Miz (8-10), Hulk Hogan (deceptively high) |

#### Athleticism Umbrella

Athleticism covers: speed, agility, body control, flexibility, movement quality. No separate "Agility" skill needed.

---

### Era-Specific Tags

| Tag | Description |
|-----|-------------|
| Old School Worker | Favors mat-based pacing, hates modern flips |
| Territory Veteran | Grew up in territorial system |
| Attitude Era Survivor | Thrives in edgier content |
| Ruthless Aggression Graduate | Product of 2002-2008 era |
| Modern Hybrid Star | Cross-trained in multiple styles |
| 80s Cartoon Hero | Larger-than-life, colorful gimmicks |
| New Generation Struggler | Survivor of awkward 1993-96 era |
| Deathmatch Evangelist | Believes deathmatch is valid art |
| Post-Kayfabe Babyface | Plays to "we're in on it" crowds |
| Strong Style Warrior | Japanese strong style influence |
| TV Match Expert | Optimized for TV time formats |

---

### Lifestyle Tags

| Tag | Description |
|-----|-------------|
| Straight Edge | No drugs, alcohol, or tobacco |
| Barroom Regular | Drinks heavily, party culture |
| Crash and Burn | Reckless lifestyle choices |
| Juice Fiend | Heavy PED usage |
| Party Burner | Lives for the party |
| Walking Recovery | In active addiction recovery |
| Functional Addict | Maintains despite substance issues |
| Big Spender | Spends money recklessly |
| Financial Disaster | Terrible with money |
| Family-Oriented | Prioritizes family life |
| Homebody | Prefers staying close to home |
| Globetrotter | Loves traveling internationally |
| Mirror Chaser | Obsessed with physique |
| Iron Temple | Gym devotee |

---

### Regional/Cultural Tags

| Tag | Description |
|-----|-------------|
| Southern Tag Specialist | Excels in southern tag psychology |
| Rebel Without a Cause | Never-say-die underdog spirit (southern) |
| Big City Lights | Prefers larger markets |
| Family First | Won't leave home region for family |
| Kayfabe Defender | Believes protecting illusion is sacred |
| Kayfabe or Die | Extreme kayfabe protection, violent if needed |
| Work-Shoot Believer | Blurs reality in promos constantly |
| No-Sell Era Graduate | Grew up on indie overkill |
| Family Business Legacy | Multi-generation wrestler |
| Forbidden Door Traveller | Loves crossing promotions |
| Influencer Mindset | Prioritizes social media presence |
| Spotlight Addict | Must be featured constantly |
| Stable General | Excels in faction politics |
| No Mudshow For Me | Anti-deathmatch, traditional wrestling only |
| Shuns Spotlight | Fiercely private, separates work/life |

---

### Emotional/Psychological Tags

| Tag | Description |
|-----|-------------|
| Jealous | Resents peers' success |
| Vengeful | Carries grudges, seeks payback |
| Forgiving | Lets slights go easily |
| Bitter Veteran | Believes industry passed them by |
| Humble Student | Remains open to learning |
| Inflated Legacy | Believes they're bigger than they are |
| Insecure Performer | Fears losing spot constantly |
| Charitable Soul | Shares opportunities, helps others |
| Opportunist | Takes any opening without shame |
| Survivor | Ruthlessly adapts to survive |

---

### Career Mindset Tags

| Tag | Description |
|-----|-------------|
| Stepping Stone | Sees wrestling as avenue to other careers |
| Lifer | Will never leave the business |
| FOREVER! FOREVER! | Retires and unretires constantly |
| One More Match | Easy to talk out of retirement |
| Health First | Retires early to protect long-term health |
| Real-World Politician | Aspires to political office beyond wrestling |

---

### Scandal Tags

**Note:** Scandal impact varies by era (easier to hide in 80s, harder in modern era) and by star power (bigger stars weather scandals better).

| Tag | Description |
|-----|-------------|
| Pedophile | Child abuse involvement (career-ending) |
| Racist | Exposed for racist behavior |
| Sexist | Mistreats/degrades women |
| Transphobic | Anti-trans attitudes |
| Homophobic | Anti-gay attitudes |
| Jingoist | Xenophobic/nationalist (regional reactions vary) |
| Scumbag | Exploits others, abuses power |
| Seedy | Financial predator, scams lower-carders |
| If He Dies He Dies | Intentionally hurts opponents |
| Pick A Hand | Won't start fights but won't back down |
| Predator | Sexual harassment, mainly targeting women |
| Blackmailer | Abuses influence to pressure others |
| Rookie Abuser | Brutalizes/hazes trainees dangerously |

---

### Non-Wrestler Tags

#### Announcers

| Tag | Description |
|-----|-------------|
| Company Man (Announcer) | Toes company line hard |
| Voice of the People | Cheers faces, criticizes heels |
| Professional Actor | Treats it 100% legit |
| Meme Factory | Viral, social media savvy |

#### Bookers

| Tag | Description |
|-----|-------------|
| Booking Genius | Creative visionary |
| Politician Booker | Plays favorites politically |
| Short-Term Booker | Good at hot shots, bad long-term |
| Storytelling Visionary | Long-form narrative master |
| Old-School Traditionalist | Resistant to evolution |
| Risk-Taker Booker | Bold, experimental booking |
| Burnout Risk | Prone to creative exhaustion |
| Future Builders | Prioritizes young talent development |

#### Managers

| Tag | Description |
|-----|-------------|
| Heat Magnet Manager | Draws heat for clients |
| Nostalgia Manager | Manages veteran stars |
| Passive Corner Man | Minimal involvement |
| Mic Saver | Covers for weak talkers |
| Cult Builder | Manages stables effectively |

#### Owners/Executives

| Tag | Description |
|-----|-------------|
| Ruthless Capitalist | Profit above all |
| Philanthropic Boss | Genuinely cares about workers |
| Legacy Protector | Defends family/company name |
| Vanity Owner | Wants to be on TV |
| Invisible Hand | Manipulates behind scenes |
| King of the Boys | Blurs boss/worker lines, parties with talent |
| Interchangeable Parts Mentality | Treats workers as expendable |
| Unsafe At The Top | Pushes stunts without safety precautions |
| Social Media Propagandist | Pays influencers, attacks rivals online |
| Dirty Tricks Specialist | Sabotage, blackballing, misinformation |
| Image Management Expert | Excellent at damage control |
| Cowboy Booker | Wild west mentality, no formal contracts |

#### Referees

| Tag | Description |
|-----|-------------|
| Invisible Ref | Stays out of the way |
| Spotlight Hog Ref | Tries to get themselves over |
| Authority Symbol | Big match gravitas |
| Screwjob Risk | High chance of angle involvement |

---

### Booking Behavior Tags

| Tag | Description |
|-----|-------------|
| Booking Traditionalist | Insists on old-school logic |
| Retirement Enforcer | Believes workers should retire by certain age |
| Conservative Women's Division | Books women less aggressively |
| Respect the Elder Code | Protects/pushes veterans |
| Scapegoater | Blames others for declining business |
| Mentorship Legacy | Teaches and uplifts younger talent |
| Passion First | Loves wrestling itself |
| Loyalty Maker | Creates strong bonds with allies |
| Redemption Seeker | Trying to redeem past failures |
| Cautious Innovator | Blends tradition with new ideas carefully |

---

### Scandal Events (Not Tags)

Some scandals are events rather than permanent personality tags:
- Animal Abuse Incident
- DUI/Car Crash
- Lawsuit
- Contract Breach
- Screwjob Incident
