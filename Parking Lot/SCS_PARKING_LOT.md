# SCS Parking Lot

## 📦 Purpose

This document tracks half-baked ideas, undefined concepts, and exploratory systems that emerged during the 11-volume design process but lack full specifications. These are preserved for future development, not lost to synthesis.

---

## 🔴 CRITICAL GAPS (Need Design, Not Extraction)

### Match Engine Simulation Mechanics
**Status:** Inputs/Outputs LOCKED, Internal Simulation EXPLORATORY
**What Exists:** Match Engine folder has locked specs for:
- Match inputs (workers, stakes, stipulations)
- Processing framework (structure phases)
- Consequences (popularity, crowd memory, injuries)

**What's Missing:** The actual simulation logic that determines:
- How matches play out beat-by-beat
- Spot selection and timing
- Quality calculation formulas
- Detailed injury risk calculations

**Decision Needed:** Is this designed during implementation, or do we need formal specs first?

---

### Economics/Financial System
**Status:** Conceptual only
**What Exists:** References to:
- Gate revenue
- TV deal income
- Merch sales
- Operational costs
- Territory economics

**What's Missing:**
- Revenue calculation formulas
- Expense models
- Break-even thresholds
- Economic failure cascades
- Financial decision triggers

**Priority:** HIGH for promotion management gameplay

---

## 🟡 UNDEFINED CONCEPTS

### VOL 4 HALF-BAKED IDEAS

📌 **Source:** Vol 4 lines 1-100 extraction

#### Archetype Seeds (Mentioned but NOT Developed)

| Archetype | Notes | Priority |
|-----------|-------|----------|
| Outsider Ace | Non-native top star in foreign territory | Medium |
| Japanese Comedy Artist | Comedy specialists in puro context | Low |
| AJPW Company Man | Loyal promotion soldiers (Kobashi-type) | Medium |
| Southern Promo Artist | Territory-era mic workers | Medium |
| Territory Psychologist | In-ring storytellers from territory days | Medium |
| Lucha Mystic | Spiritual/supernatural lucha characters | Low |
| Deathmatch Loner | Isolated hardcore specialists | Low |

#### System Seeds (Conceptual, Not Built)

| Concept | Description | Priority |
|---------|-------------|----------|
| Booking Conflict Flags | Archetype-specific booking conflicts that trigger morale/pushback | High |
| Tag Synergies | How tags interact with each other for emergent behavior | High |
| Archetype Tree Visual | Visualization of archetype relationships and evolution paths | Low |
| Sacrificial Mode | Deathmatch Devotee late-career mechanic: boost crowd memory at cost of health | Medium |
| Match Memory Score | Per-worker score for emotionally brutal bouts (Joshi Firebrand has "near-unrivaled" score) | Medium |
| Memory Degradation Variants | Different decay rates for emotional arc vs match quality memory | Medium |
| **Booking Exposure Stress System** | Workload pushes stress meter, interacts with burnout | High |
| **Burnout Event Triggers** | Fires when accumulated stress > resilience threshold | High |

#### Burnout Mechanics (Clarified in Vol 4)
**How Burnout Works:**
- Tags set lifestyle/stress level (Fragile, Cult Hero, Spotfest Addict, etc.)
- Hidden Personality (Drive + Paranoia + Loyalty) sets resilience
- Booking Exposure pushes stress meter higher
- Burnout Event Triggers fire based on accumulated stress vs resilience
- **Status:** Conceptual formula, needs formal stress meter system

#### Criminality Tags (NEW - Vol 4 lines 146-149)

| Tag | Description | Notes |
|-----|-------------|-------|
| **Criminal Risk** | Likely to commit future legal trouble (arrests, DUIs, fights) | Predictive, background tag |
| **Severe Criminal Potential** | High risk of catastrophic acts (murder, sexual assault, etc.) | Very rare, dark trajectories |

**Design Note:** These tags live in background, rarely seen unless scandals erupt. Separates minor chaos from true horror. Ticking Timebomb archetype commonly has Criminal Risk.

#### Career Arc Templates (Conceptual)

| Arc Type | Description |
|----------|-------------|
| Meteoric Rise | Rapid ascent, high burnout risk |
| Journeyman Grind | Slow build, steady career |
| Tragic Fall | Peak followed by collapse |
| Late-Career Redemption | Comeback after decline |

#### Role Evolution Path
**Concept:** wrestler → manager → booker career transitions
**Status:** Mentioned as "early sketch," no mechanics built
**Priority:** Medium (adds post-ring career depth)

#### Era-Based Office UI
**Status:** ✅ Now documented in [[Era_Based_Office_UI]]
**Origin:** Vol 4 lines 52-59, half-baked concept elevated to full system doc

---

### VOL 1 HALF-BAKED IDEAS (Watch List for Vol 2+)

📌 **Source:** Vol 1 Extraction Batch G

These concepts appeared in Vol 1 but weren't locked. Track in later volumes:

| ID | Concept | Notes | Priority |
|----|---------|-------|----------|
| HB-6 | Multiplayer Draft Mode | Players draft rosters, venues, belts; async turns | Medium |
| HB-7 | Talent Tampering & Poaching | CPU feds scout/steal workers; era-based AI aggressiveness | High |
| HB-8 | Press Conferences | Media interaction mechanic; regional variations | Low |
| HB-11 | Fighting Spirit Meter | Invisible system for match psychology; develops over career | High |
| HB-14 | Push Authenticity (Media Leaks) | "MAKE ROMAN LOOK STRONG" style leaks affecting perception | Medium |
| HB-15 | Worker Self-Improvement Arcs | Adversity triggers growth; injury forces reinvention | High |
| HB-24 | Agent/Trainer Influence | Road agents and trainers affecting worker development | Medium |
| HB-27 | Body Damage Visuals | Taped wrists, limping, visible wear during matches | Low |
| HB-29 | Crowd Density Visualization | Empty seats, tarps, crowd energy visuals | Low |
| HB-34 | Relationship Sharing Templates | AJPW/NOAH exodus as reusable relationship pattern | Medium |

### Open Archetype Questions

Archetypes mentioned but not fully locked in Vol 1:

| Archetype | Status | Notes |
|-----------|--------|-------|
| Comedy Worker | Possibly subtype of Charismatic Entertainer | Check Vol 2+ |
| Tag Team Specialist | Mentioned, needs full build | Check Vol 2+ |
| Authority Figure | Deferred | Non-active worker role |
| Beauty Star | May be tag cluster instead | Check Vol 2+ |
| Prodigy/Late Bloomer | May be tags not archetypes | Check Vol 2+ |

### Fourth Mental Attribute

**Status:** Still TBD placeholder from Vol 1

Current Mental stats: Psychology, Focus, Consistency, Adaptability

Possible candidates for fourth slot:
- Creativity?
- Ring Awareness?
- Instinct?

Check Vol 2+ for resolution.

---

### Twin Gate Cycle
**Source:** Mentioned in volumes, no definition found
**Status:** Unknown, possibly deprecated
**Action:** Ask tovarisch for clarification or deprecate

---

### Angle Director
**Source:** Early volumes
**Status:** Possibly subsumed by Booking Trails
**Notes:** May have been an early name for storyline planning tools
**Action:** Confirm with tovarisch, likely deprecated

---

### Soul Engine
**Source:** Project naming discussions
**Status:** Unclear if system name or project codename
**Notes:** May refer to the core simulation engine, or may be deprecated terminology
**Action:** Confirm with tovarisch

---

### Fourth Path Feds
**Source:** Ringstate worldbuilding
**Status:** Now documented in Ringstate Atlases
**Notes:** Refers to promotions outside the six major alliances (CCA, GWA, PWU, CFPW, LGBTQW+, Blade Underground)
**Resolution:** ✅ Extracted to atlas documents

---

## 🌙 DREAM FEATURES (Long-Term Vision, 2027+)

📌 **Source:** Vol 1 Extraction Batch G

Aspirational features far beyond MVP scope:

| ID | Feature | Description |
|----|---------|-------------|
| HB-1 | Full 3D Match Visualization | "Sit ringside and watch matches play out" with AI arenas, camera angles, voice acting |
| HB-2 | FPW++/TEW+++ Hybrid | Book in TEW-style, watch in FPW engine (the holy grail) |
| HB-3 | AI-Generated Cutscenes | Dynamic scenes from personality/relationships, not templates |
| HB-4 | Voice Cloning & Commentary | AI commentary that knows feuds and history |
| HB-5 | Multi-Sport Sim Universe | OOTP Basketball/Football style, cross-game integration |

### Sprite Generation Pipeline (HB-20)

Tech concepts for visual generation:
- ComfyUI + ControlNet
- Stable Diffusion
- Mage.Space
- Hot-swappable art system for modding

### Development Vision Timeline (HB-21)

| Year | Target |
|------|--------|
| 2025 | Text-based MVP |
| 2026 | 2.5D visual layer |
| 2027 | Voice AI integration |
| 2030 | Full immersion |

---

## 🟢 WORLDBUILDING (Extracted)

### Ringstate Lore
**Status:** ✅ Fully extracted
**Location:**
- [[Ringstate_Factions]] - Core 6 alliances
- [[RINGSTATE_ATLAS_MASTER_INDEX]] - Global coverage
- [[RINGSTATE_ATLAS_NORTH_AMERICA]] - US/Canada detail
- [[RINGSTATE_ATLAS_LATIN_AMERICA_CARIBBEAN]] - Mexico, Central/South America
- [[RINGSTATE_ATLAS_WORLD_REGIONS]] - Japan, Europe, USSR, Africa, Oceania
- [[RINGSTATE_WORKER_PROFILES_FIXED]] - 150+ named workers

### Character Profiles
**Status:** ✅ Major characters documented
**Location:** Character profile files in vault

---

## 🔵 LLM & TECHNICAL CONCEPTS (Extracted)

### AI Booker / LLM Integration
**Status:** ✅ Documented in [[AI_Tiered_Integration]]
**Covers:**
- Local-first architecture
- Tiered system (Ultra/High/Medium/Low)
- Ollama integration
- Free cloud API fallbacks
- AI Booker Assistant modes
- CPU Opponent Intelligence
- Template fallbacks
- Graceful degradation

### Hydration System / Simulation Fidelity
**Status:** ✅ Documented in AI_Tiered_Integration
**Concept:** Platform scaling that adjusts simulation depth based on device capabilities
**Implementation:** Compression/decompression of historical archives for memory management

### Memory Compression
**Status:** ✅ Documented
**Source:** Line 127222 in locked_systems_tracker: "Career, Title, Promotion Memory Handling"
**Function:** System decompresses archived match records, title defenses, loyalty drift logs for specific sessions/views

---

## ⚫ PROBABLY DEPRECATED

### Heat Types (Face/Heel/Go-Away/Shoot)
**Status:** Likely subsumed by Buzz System
**Notes:** Vol 5 evolved Heat into Buzz with more nuanced mechanics
**Action:** Confirm Buzz System fully replaces this concept

### Prestige System
**Status:** Distributed across other systems
**Notes:** 
- Worker prestige → Popularity
- Title prestige → Title System
- Promotion prestige → Federation/Reputation
**Action:** No standalone system needed, concept is distributed

---

## 📋 EXTRACTION PRIORITIES (Vol 5-7 Evolved Systems)

These systems have locked mechanics in Vol 5-7 that may refine earlier versions:

| System | Volume | Status |
|--------|--------|--------|
| Booking Trails | Vol 5-6 | ✅ Extracted (6 files) |
| Buzz System | Vol 5-6 | ✅ Extracted (7 files) |
| Hall of Fame | Vol 6 | ✅ Extracted (7 files) |
| Gimmick System | Vol 6 | ✅ Extracted (10 files) |
| Crowd Signals | Vol 6 | ✅ Extracted (8 files) |
| Promo Response | Vol 7 | ✅ In Segment Promo System |

---

## 🎯 RECOMMENDATIONS

### For MVP Development:
1. **Match Engine** - Design simulation during implementation (abstract resolution acceptable for MVP)
2. **Economics** - Design basic financial model (gate + TV revenue, basic expenses)
3. **Use locked inputs/outputs** - Match Engine's inputs and consequences are solid

### For Phase 2 (Post-MVP):
1. **Full Match Simulation** - Detailed beat-by-beat play
2. **Advanced Economics** - Complex financial modeling
3. **Agent AI** - Autonomous worker behavior
4. **Aging/Career Arcs** - Long-term play depth

### To Deprecate or Clarify:
1. **Twin Gate Cycle** - Ask or deprecate
2. **Angle Director** - Likely deprecated
3. **Soul Engine** - Clarify terminology
4. **Heat Types** - Confirm Buzz replaces this

---

## 🛠️ TECHNICAL & META SYSTEMS (Vol 1 Extraction)

These meta-level systems from Vol 1 are not core gameplay but supporting infrastructure:

### Save/Load & Mod Support (#138)

📌 **Source:** Vol 1 Extraction #138

**Save Features:**
| Feature | Description |
|---------|-------------|
| Multiple Saves | Separate save slots |
| Autosave | Configurable frequency |
| Save Branching | Create alternate timeline saves |
| Cloud Sync | Optional cloud backup |

**Mod Support:**
| Format | Purpose |
|--------|--------|
| .wres | Worker data files |
| .arena | Venue files |
| .logic | Custom AI behavior |
| .fed | Promotion templates |

Steam Workshop integration planned for community sharing.

---

### Multiplayer/Online Modes (#146)

📌 **Source:** Vol 1 Extraction #146

**Modes:**
| Mode | Description |
|------|-------------|
| Head-to-Head | Two players, competing feds |
| League | Multiple players, shared world |
| Async | Turn-based, email-style |
| Spectator | Watch AI-run worlds |

**Features:**
- Cross-promotion booking
- Talent trading
- Shared events
- Competition for ratings/attendance

**Status:** Future expansion, not MVP.

---

### Development Timeline Estimate (#230)

📌 **Source:** Vol 1 Extraction #230

**Playable Alpha Estimate:** ~200-250 hours of back-and-forth work

| Phase | Hours | Description |
|-------|-------|--------------|
| Worker Construction | 30-40h | Finish archetypes, tags, skill system |
| Promotion/World Building | 20-30h | Promotion templates, world database basics |
| Draft + Roster Systems | 20-30h | Draft, war room, contracts, rosters |
| Booking Engine Basics | 40-50h | Match/angle booking UI, event simulation |
| AI Booking Logic | 30-40h | CPU opponents book logically |
| Front-End Interface | 20-30h | Basic menus, windows (playable but ugly) |
| Testing + Debugging | 20-30h | Playtesting, balancing, fixes |
| Optional Flavour | 20-30h | Promo generation, media, news, merch |

**Notes:**
- Basic ugly prototype possible at ~150h
- Beautiful/modern feel requires full 200-250h

---

### Godot Engine Selection (#231)

📌 **Source:** Vol 1 Extraction #231

**Recommendation:** Godot Engine for front-end development

| Benefit | Description |
|---------|-------------|
| Free | Open source, no licensing issues |
| Lightweight | Not overkill like Unity |
| Professional | Can polish later if needed |
| Cross-Platform | Works everywhere |
| Sim-Friendly | Perfect for modular menu-based games |

**Learning Curve:** ~3-5 hours/week casual = dangerous within 2 months

**Alternatives Considered:**
- Unity (overkill, licensing weirdness)
- Electron.js (fast dev, not performance-heavy)
- Python + PyQt (pure control, less beautiful)
- C# WinForms (ugly unless heavily customized)

---

## 📝 NOTES FOR FUTURE DEVELOPMENT

**Document Purpose:** This parking lot prevents ideas from being lost during synthesis. Every concept mentioned across 11 volumes is tracked here if not fully specified elsewhere.

**Usage:**
- Reference when users ask "what about X system?"
- Check before designing "new" features (may already be half-baked here)
- Use as future expansion roadmap

---

## 🟡 VOL 2 CHUNK 01 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 01 discussion threads

These concepts were discussed during archetype development but not formalized:

### Match Presentation System (3-Tier)
**Status:** Conceptual, explicitly deferred
**Concept:** Three-tier match output system:
- Tier 1: Straight Result (quick text outcome)
- Tier 2: Result + Highlights (key spots, finishes)
- Tier 3: Condensed Storyline Recap (narrative summary)

**Deferred:** Full PBP (play-by-play) was pushed "way down the road"
**Half-Baked Components:**
- Tags influencing which highlights appear (mentioned but not formalized)
- Show Report Template (offered but deferred)
**Priority:** Medium (affects how matches are presented to player)

---

### Match DNA System
**Status:** Conceptual only, NOT FORMALIZED
**Concept:** Different psychological match models based on archetype philosophy:

| DNA Type | Match Philosophy |
|----------|------------------|
| Fighting Spirit DNA | Offensive, unpredictable, submissions credible throughout, sudden finishes, martial arts realism |
| King's Road DNA | Defensive, structured escalation, predictable phases, head drops in final stage, classical storytelling |
| Lucha DNA | (Not detailed) |

**Related Concepts:**
- Structured Escalation Engine (King's Road)
- Sudden Death Threat (Fighting Spirit)
- Style Clash mechanics when different DNAs meet

**Priority:** High (affects match engine design fundamentally)

---

### Worker Creation Templates
**Status:** Offered, never built
**Concept:** Templates for creating workers based on archetype/subtype/tag combinations
**Use Case:** Quick worker generation, consistent stat allocation
**Priority:** Medium (useful for database building)

---

### Hybrid Archetype System
**Status:** Discussed extensively, mechanics not formalized
**Concept:** Primary Archetype + Secondary Traits/Tags structure
**Examples Given:**
- Benoit: Fighting Spirit primary → Junior Puroresu secondary
- Dynamite Kid: Junior Puroresu primary → Fighting Spirit secondary
- Oba Femi: Athletic Entertainer + Monster hybrid

**Mechanics Needed:**
- How primary vs secondary weights affect match logic
- Weighting system (Light/Heavy secondary influence)
- Career phase transitions between archetypes
- How hybrid workers behave in match engine

**Priority:** High (fundamental to worker complexity)

---

### Promo Style System
**Status:** Example-driven, not systematized
**Concept:** Promo delivery patterns and verbal signatures
**Example Given:** Percy Pringle/Paul Bearer "ends sentences with 'maaaaaan' like spitting poison"
**Mechanics Needed:**
- Promo style templates by archetype
- Verbal signature generation
- Regional promo preferences
**Priority:** Low (flavor enhancement)

---

### Age Phase Shift System
**Status:** Mentioned as possibility, not developed
**Concept:** Workers transitioning across subtypes over their career
**Examples Given:**
- Orange Crush → Iron Man → Senior Circuit Hero (King's Road aging path)
- Junior Puroresu → Fighting Spirit (style evolution)

**Mechanics Needed:**
- Transition triggers (age, injury, booking, personal choice)
- Skill/tag changes during transitions
- Fan perception during transitions
**Priority:** Medium (adds career depth)

---

## 🟡 VOL 2 CHUNK 02 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 02 discussion threads (Archetype finalization session)

These concepts emerged during archetype locking but weren't formalized:

### Worker Graduation System (Archetype Transitions)
**Status:** Conceptual, examples given, no formal mechanics
**Concept:** Workers "graduate" across archetypes as careers evolve

**Examples Given:**
- Junior Phase → Fighting Spirit Phase
- Tag Specialist Phase → Singles Bruiser Phase
- Orange Crush → Iron Man → Senior Circuit Hero (King's Road aging path)
- Young Dynamite Kid (Junior Puroresu) → Prime Dynamite Kid (Fighting Spirit)
- Young Benoit (Junior Puroresu) → Prime Benoit (Fighting Spirit)

**Mechanics Needed:**
- Graduation triggers (age, injury, booking decisions, personal evolution)
- How skill priorities shift during transitions
- Fan perception during archetype shifts
- Timeline expectations (how long before graduation possible)
**Priority:** High (fundamental to career simulation)

---

### Hybrid Warrior Tag
**Status:** Mentioned, not locked
**Concept:** Tag for workers who operate across two archetypes without penalty
**Use Case:** Benoit, Dynamite Kid, Oba Femi types
**Related Tag Suggested:** Explosive Technician (bonus for dynamic high-impact technical sequences)
**Priority:** Medium (enhancement to hybrid system)

---

### Fragile Monster Tag
**Status:** Mentioned as "maybe later," not locked
**Concept:** Workers who seem indestructible but are injury-prone IRL
**Examples:**
- Early Lashley
- Lex Luger (post-roid shrink)
- Braun Strowman (when overpushed)
**Use Case:** Creates realistic injury risk for powerhouse types despite dominant presentation
**Priority:** Low (enhancement to Injury System)

---

### King's Road Subtype Tags (Proposed but not all locked)
**Status:** Some mentioned, status unclear

| Tag | Description | Status |
|-----|-------------|--------|
| Nostalgia Pop | Senior Circuit Hero bonus crowd reaction despite declining match quality | Check if locked |
| Big Body Weapon | Heavy Bruisers gain boosted strike/grapple damage but stamina drains faster | Check if locked |
| Flashstarter | Ark Genius/Golden Phoenix types pop early but can gas out later | Check if locked |
| Gatekeeper | Undercard Strivers earn respect by holding down midcard | Check if locked |
| Spirit Grinder | Hardheaded Underdogs become harder to kill at high damage thresholds | Check if locked |

**Priority:** Medium (need to verify which are locked vs half-baked)

---

### Savage Monster Racial Backlash Mechanics
**Status:** Concept noted, mechanics not built
**Concept:** Modern era fans may criticize racially insensitive gimmicks (Kamala, Abdullah types)
**Era Evolution:**
- 70s-80s: Accepted, popular
- 90s-00s: Growing criticism
- 2010s+: Significant backlash from portions of audience

**Mechanics Needed:**
- Fan demographic splits on reaction
- Regional variation (some areas more/less critical)
- Era-specific tolerance levels
- How to handle legacy workers vs new workers using similar gimmicks
**Priority:** Medium (adds cultural realism)

---

### Dark Weavers Subtype Details (Partially Locked)
**Status:** Archetype LOCKED, but some subtype mechanics need verification
**Subtypes Confirmed:**
- Cult Leader (Bray Wyatt, Kevin Sullivan)
- Cold Blood (Jake Roberts types)
- Outcast (Raven, early Darby Allin vibe)
- Broken Prophet (Waylon Mercy, post-broken Bray)
- Dark Trickster (Danhausen dark side, Joker Sting)

**Tags Proposed (Status Unclear):**

| Tag | Description |
|-----|-------------|
| Fear Aura | Opponents suffer morale penalties in feuds |
| Psychological Trap | Increased effectiveness after pre-match promo segment |
| Slow Death | Matches build slowly but devastatingly if booking allows space |

**Priority:** Low (verify which tags are locked)

---

### Model Appeal Tag
**Status:** Proposed, not explicitly locked by user
**Concept:** Workers with mainstream beauty/fitness model backgrounds receive:
- Automatic marketing/brand appeal boosts
- Social media growth bonuses
- Casual audience interest even if matches are bad

**Examples:**
- Stacy Keibler
- Torrie Wilson
- Mandy Rose
- Early Trish Stratus

**Priority:** Low (verify lock status)

---

### Showman Subtype Expansion (Bulk Added)
**Status:** Many subtypes proposed and discussed, need verification which are locked
**New Subtypes Discussed:**

| Subtype | Description | Example |
|---------|-------------|--------|
| Athletic Entertainer | Green but physically gifted | Oba Femi, Tiffany Stratton |
| Technical Showman | Skilled wrestlers with crowd-popping showmanship | Chad Gable |
| Lovable Dynamo | Beloved for earnestness and comedic timing | Otis, R-Truth |
| Arrogant Athlete | Sports crossovers who see wrestling as beneath them | Early Baron Corbin |
| Gimmick Attraction | Pure gimmick workers, colorful characters | Boogeyman, Repo Man |
| Reality Crossover Star | Reality TV, IG, Twitch backgrounds | Logan Paul, early Miz |
| Muscle Showstopper | Bodybuilder presentation with major crowd pops | Lex Luger (Narcissist), Rick Rude |
| Broken Entertainer | Absurd, surreal, "broken reality" character work | Broken Matt Hardy, Bray |
| Occupational Gimmick Worker | Profession-based gimmicks for casual audiences | Duke Droese, IRS |
| Sports Entertainer (Pure) | WWE/PC trained, timing and entertainment beats | Post-polish Baron Corbin |
| Calculated Predator | Methodical, apex predator psychology | Randy Orton (Legend Killer), Triple H |

**Priority:** Medium (verify all locks, may be partially in Bible already)

---

### Heel Ace Mind-Game Specialist (Absorbed into Dark Weavers)
**Status:** Initially proposed as Heel Ace subtype, then evolved into separate archetype
**Resolution:** Dark Weavers archetype created to house these workers
**Note:** If Dark Weavers ever deprecated, Mind-Game Specialist could fold back into Heel Ace

---

## 🟡 VOL 2 CHUNKS 03-05 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunks 03-05 discussion threads (Tag System deep dive)

These concepts emerged during the massive 385+ tag creation session:

### Non-Binary Tag Strength System
**Status:** Concept AGREED, implementation specs NOT written
**Concept:** Tags have 0-100% strength instead of binary on/off

| Strength % | Meaning |
|------------|--------|
| 0% | Doesn't have trait |
| 1-30% | Minor influence, rarely triggers |
| 31-60% | Moderate, noticeable but secondary |
| 61-90% | Strong, regular influence |
| 91-100% | Defining, core identity |

**Use Cases:**
- Tags can grow/decay over career
- Young Roman: Cool Heel 30%, Big Match Player 40%
- Modern Roman: Cool Heel 80%, Big Match Player 90%

**Mechanics Needed:**
- How % affects actual gameplay triggers
- Growth/decay formulas
- UI display of partial tags
**Priority:** High (fundamental to tag system evolution)

---

### Scandal Shielding System
**Status:** Started but not completed
**Concept:** How promotions hide/delay scandal exposure
**Factors Identified:**
- Era sensitivity (80s easy to hide, 00s+ impossible)
- Promotion size (bigger = more shield)
- Star power of accused
- Company protection willingness

**Mechanics Needed:**
- Shield strength calculation
- Delay duration formulas
- Cover-up failure cascades
- Media exposure triggers
**Priority:** High (core to scandal system)

---

### Fan Loyalty Resistance System
**Status:** Formula sketched, not formalized
**Concept:** How resistant fans are to turning on stars/promotions during scandal

**Formula Sketch:**
```
Fan Resistance % = Base Loyalty + Star Power Modifier + Promotion Size Modifier - Scandal Severity Modifier - Era Outrage Modifier
```

**Fanbase Types with Tolerance Levels:**

| Fanbase Type | Scandal Tolerance |
|--------------|-------------------|
| Hardcore Company Loyalists | High (unless murder-level) |
| Indie Hardcore | Very Low (hypocrisy triggers) |
| Family-Friendly | Very Low (child/drug/abuse kills) |
| Deathmatch Outlaw | Medium-High (authenticity matters more) |
| Edgy Attitude Era Types | Medium-High (antihero worship) |

**Priority:** High (core to fan behavior)

---

### Career Arc System (Stages)
**Status:** Stages outlined, event triggers not formalized
**Stages Identified:**

| Stage | Description |
|-------|-------------|
| Rookie Years | Low pop, basic traits, underdog/green/hungry |
| Breakout | Miracle match, angle, or political opening |
| Fame | Success pressure, ego tests |
| Physical Decline | Injuries, aging, passion loss |
| Crisis | Scandals, betrayals, being passed |
| Reinvention | New persona attempts |
| Retirement Attempts | Some leave, some unretire (One More Match) |
| Legacy | Legends or forgotten |

**Mechanics Needed:**
- Event triggers for stage transitions
- How tags evolve per stage
- Randomizers for injury/scandal/political events
**Priority:** High (core to long-term simulation)

---

### Regional Demographics System
**Status:** Conceptual, ties to Ethnic Folk Hero tag
**Concept:** Game auto-detects ethnicity match with regional population

**Mechanics:**
- Workers tagged with ethnicity
- Regions have demographic profiles (% Italian, % Black, % Hispanic, etc.)
- Ethnic Folk Hero triggers bonus loyalty when match found

**Examples:**
- JYD + Black + Mid-South = huge loyalty boost
- Sammartino + Italian + Northeast = massive cultural bond
- Mismatched = no automatic boost (unless Grassroots Hero Build earned)

**Generational Evolution:** Some regions' demographics shift over decades

**Priority:** Medium (adds cultural authenticity)

---

### Promotion-Attached Fanbase Types
**Status:** Types defined, attachment mechanics not built
**Concept:** Each promotion has dominant fanbase type(s) affecting behavior

**Fanbase Types Identified:**
- Hardcore Company Loyalists
- Indie Hardcore
- Family-Friendly
- Deathmatch Outlaw
- Lucha Traditionalists
- Joshi Superfans
- Edgy Attitude Era Types

**Mechanics Needed:**
- How to assign fanbase types to promotions
- Multi-type fanbase composition
- How fanbase type affects all systems (scandal, booking, etc.)
**Priority:** High (foundational to fanbase system)

---

### Institutional Rot System
**Status:** Conceptual only
**Concept:** Promotions surviving scandals but corruption bleeding into:
- Locker room morale
- Long-term perception
- Media relationships
- Sponsor trust
- Worker recruitment

**Examples:**
- WWE post-Vince: survived but institutional trust damaged
- Promotions that "get away with it" still suffer slow rot

**Mechanics Needed:**
- Rot accumulation formula
- Long-term consequences vs short-term survival
- Reform paths to heal rot
**Priority:** Medium (adds institutional depth)

---

## 🟡 VOL 2 CHUNK 04 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 04 discussion threads (2025-12-25)

These concepts were discussed but not formally locked:

### Observer/Magazine PDF Processing Pipeline
**Concept:** Upload zipped PDFs of newsletters (Observer, Torch), books, magazines to mine for historical accuracy data
**Status:** Exploratory, infrastructure idea for database building
**Use Case:** Building historically accurate non-binary tag percentages for real wrestlers based on documented behavior
**Priority:** Medium (would massively improve historical database accuracy)

### Percentage-Based Wrestler Profiles
**Concept:** Building real-world wrestlers with non-binary tag strengths (0-100%)
**Status:** System mechanics defined in Tags_Vol2_Chunk04_Expansion.md, needs implementation framework
**Example:** Kevin Nash: Cool Heel 95%, Storyteller 90%, Is This Mania? 85%
**Note:** Non-binary tag system itself is LOCKED, but building actual historical profiles needs work

### Scandal Risk Calculators
**Concept:** Calculate scandal probability based on tag clusters
**Status:** Conceptual, ties to Scandal System
**Example:** Party Animal + Ring Intoxicated + Low Morality = high substance scandal risk
**Priority:** Medium (adds emergent behavior depth)

### Multi-generational Worker Bloodlines
**Concept:** Von Erichs, Anoa'i Family systems with inherited traits and curse mechanics
**Status:** Mentioned, needs formal design
**Mechanics to Design:**
- Trait inheritance probability
- "Cursed Legacy" tag triggering family tragedy events
- Dynasty reputation affecting new generation's starting popularity
- Family political power in promotions
**Priority:** Medium (adds generational storytelling)

### Gimmick Prison vs Career Chameleon Paths
**Concept:** Different evolution routes for worker persona development
**Status:** Tags exist (Gimmick Prisoner, Career Chameleon, Reinvention Artist), formal path system not designed
**Mechanics to Design:**
- When does a gimmick become a "prison"?
- Reinvention attempt success/failure rates
- Fan rejection of new personas
- Nostalgia pops for returning to old gimmicks
**Priority:** Low (tags capture most behavior already)

### Worker Generator System
**Concept:** Creating fictional workers using tag templates and archetype combinations
**Status:** Mentioned, ties to World Builder
**Use Case:** Generating roster for fictional promotions or filling out historical rosters
**Priority:** Medium (useful for scenario building)

### Master Tag CSV Export
**Concept:** Trait Name | Description | Category format for database export
**Status:** Format defined, not generated
**Use Case:** Import into game engine, spreadsheet analysis, community sharing
**Priority:** Low (implementation detail)

---

---

## 🟡 VOL 2 CHUNK 07 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 07 discussion threads (2025-12-26)

### PWI 500 Historical Database
**Status:** Mentioned as valuable, not built
**Concept:** Build complete history of PWI 500 lists year-by-year
**Use Case:** Track "fan/pop perception" arcs (e.g., "Why was X seen as rising in '94 and forgotten by '96?")
**Data Source:** PWI magazine archives
**Priority:** Medium (valuable for pop system calibration)

---

### Archive Processing Pipeline
**Status:** Conceptual infrastructure idea
**Concept:** Systematic methodology for mining Observer/Torch/DVDVR for specific data types
**Components:**
- Scandal extraction protocol
- Career arc tracking methodology
- Chemistry/psychology mapping from DVDVR reviews
- Regional fanbase evolution tracking

**Priority:** Low (infrastructure, not gameplay system)

---

### DVDVR Psychology Mapping
**Status:** Resource identified, extraction not designed
**Concept:** Use 170+ DVDVR video reviews to map worker psychology/chemistry
**Philosophy Note:** DVDVR prefers psychology and emotion over flashiness; would rate Shibata/Okada higher than Omega/Okada
**Use Case:** Calibrating worker chemistry ratings and psychology tags
**Priority:** Medium (excellent for worker system depth)

---

### Multi-Source Scandal Verification
**Status:** Methodology noted, not formalized
**Concept:** Use Observer + Torch together for two-source validation of scandal severity, timing, public fallout
**Value:** More accurate scandal baselines than single-source
**Priority:** Low (research methodology, not game system)

---

## 🟡 VOL 2 CHUNK 06 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 06 discussion threads (2025-12-26)

These concepts were discussed but explicitly "pinned" for later development:

### Union System (PINNED)
**Status:** Explicitly deferred, rich concept for future development
**Components:**

| Component | Description |
|-----------|-------------|
| **Unionization Attempt Triggers** | Low morale, financial exploitation, high injury rates, scandals building distrust |
| **Management Response Tags** | Union Buster (aggressive suppression) / Union Ambivalence (reluctant tolerance) |
| **Worker Class Split** | Top stars rarely join unless personally motivated (Ventura, ZSJ-types); midcarders and lower carders lead the push |
| **Negotiation Outcomes** | Weak unions win partial rights (healthcare, basic contracts); Strong unions win formal recognition, salaries, benefits |
| **Strike Risk** | If union busting too aggressive, walkouts and strikes become real risks |
| **Era Sensitivity** | 70s-80s easier to crush; 90s-2000s possible with media pressure; 2020s far harder without PR death spiral |

**Historical Examples:**
- Jesse Ventura's union attempt in WWF (crushed by Hogan snitching)
- Wrestlers have never successfully unionized in US
- Other sports (MLB, NFL, NBA) provide templates for mechanics

**Management Tags (LOCKED in Bible):**
- Union Buster (Management Behaviour) ✅
- Union Ambivalence (Management Behaviour) ✅

**Worker Tags (HALF-BAKED, not locked):**
- Pro-Union Ally (rare workers who support unions despite being top stars, like Ventura, ZSJ)
- Corporate Loyalist (workers who side with management over fellow workers)

**Priority:** Medium (adds political depth but not MVP-critical)

---

### Mini Locker Room Council Meetings
**Status:** Mentioned, not designed
**Concept:** When crisis hits, player can choose WHO to brief first
**Risk Factor:** Some workers may be spies who leak information
**Use Case:** Adds intrigue to crisis management
**Priority:** Low (enhancement to Crisis Response System)

---

### PR Officer Role
**Status:** Mentioned, not designed
**Concept:** Hire/fire PR experts who affect scandal spin success
**Mechanics Needed:**
- PR Officer stats/tags
- Spin success modifiers
- Cost/benefit of good vs cheap PR
**Priority:** Low (could be part of Staff System)

---

### Sponsor Pressure System
**Status:** Mentioned, not fully designed
**Concept:** TV networks and sponsors quietly demand firings or pull funding
**Current State:** Basic mechanics in [[Toxic Worker Consequences]]
**Needs Design:**
- Sponsor types and tolerance levels
- Network contract mechanics
- Pressure escalation timeline
- Public vs private pressure
**Priority:** Medium (important for business simulation)

---

### Fan Hypocrisy Deep Mechanics
**Status:** Concepts documented in [[Fan Loyalty Resistance]] and [[Fanbase DNA System]]
**Future Expansion Ideas:**
- Individual fan memory of "what they forgave"
- Hypocrisy backlash when fans forgive one but not another
- Fan self-awareness mechanics (some fans KNOW they're hypocrites)
- Parasocial relationship intensity affecting forgiveness
**Priority:** Low (current systems capture core behavior)

---

### Regional PR Response Options
**Status:** Concept in [[Fanbase DNA System]], mechanics not built
**Concept:** Handle PR differently in different regions
**Example:** Apologize heavily in Japan, stay silent in US
**Mechanics Needed:**
- Region-specific PR actions
- Cost/risk of regional strategies
- How conflicting regional responses interact
**Priority:** Medium (adds depth to international promotion play)

---

### Half-Baked Management Tags
**Status:** Mentioned in AI suggestions but NOT locked by user
**Source:** Vol 2 Chunk 06 discussion

| Tag | Description | Why Not Locked |
|-----|-------------|----------------|
| Expansionist Visionary | Obsessed with national/international growth; risks scandals for exposure | User only locked 9 core + 2 union tags |
| Talent Hoarder | Signs too many workers (even scandalous ones) to deny them to competitors | User only locked 9 core + 2 union tags |

**Priority:** Low (could be added to Management Behaviour Tags if needed)

---

### Burnout/Collapse States
**Status:** ✅ LOCKED - Now in Bible
**Location:** [[Burnout Collapse States]]
**Source:** Vol 2 Chunk 07

~~Previously half-baked, now fully documented with stages, triggers, symptoms, and recovery options.~~

---

### Shield Wear Down Over Time
**Status:** ✅ LOCKED - Now in Bible
**Location:** [[Shield Wear Down Over Time]]
**Source:** Vol 2 Chunk 07

~~Previously half-baked, now fully documented with decay tables, severity modifiers, and collapse consequences.~~

---

---

## 🟡 VOL 2 CHUNK 06 HALF-BAKED IDEAS (ADDITIONAL)

📌 **Source:** Vol 2 Chunk 06 discussion threads (2025-12-26)

These concepts were offered but user moved on:

### Management Evolution Paths
**Status:** Offered, user moved on
**Concept:** How management itself can rot, reform, or double down over decades
**Mechanics to Design:**
- Booker/owner personality drift over time
- Crisis points that trigger evolution
- Generational management transitions
- Reform vs entrenchment paths
**Priority:** Medium (adds long-term depth to promotion play)

---

### Sample Management Profiles
**Status:** Offered, user moved on
**Concept:** Build example profiles using Management Behaviour Tags
**Examples to Build:**
- Giant Baba (Clean Hands + Homegrown Purist + Worker First)
- Vince McMahon (Dirty Loyalty + Corporate Overlord + Deny At All Costs)
- Paul Heyman (Outlaw Spirit + Booker's Playground + Crisis Reformer tendencies)
- Eric Bischoff (Corporate Overlord + Strategic Scapegoater + Firefighting Opportunist)
- Atsushi Onita (Outlaw Romanticizer + Self-Preserver)
- Gedo (Homegrown Purist + Crisis Reformer)
**Use Case:** Reference examples for promotion building
**Priority:** Low (can build as needed)

---

### Anti-Union Stooge Tag (Worker)
**Status:** Mentioned in union discussion, not locked
**Concept:** Worker who actively sides against union efforts, may snitch to management
**Historical Example:** Hulk Hogan informing Vince about Jesse Ventura's union attempt
**Pairs With:** Pro-Union Ally, Corporate Loyalist
**Priority:** Low (part of Union System expansion)

---

## 🟡 VOL 2 CHUNK 07 HALF-BAKED IDEAS (ADDITIONAL)

📌 **Source:** Vol 2 Chunk 07 discussion threads (2025-12-26)

### Sample Regional DNA Sheets
**Status:** Offered multiple times, user deferred to after scandals
**Concept:** Build starter templates for key regions showing:
- Demographic breakdowns
- Political leanings
- Scandal sensitivities
- Cultural values
- Era evolution

**Regions to Build:**
- US South (Louisiana, Mississippi, Arkansas, Texas)
- US Northeast (New York, Philadelphia, Boston)
- US Midwest (Chicago, Detroit, Minneapolis)
- Japan (Tokyo Metro vs Rural, era variations)
- Mexico (Mexico City, Monterrey, Guadalajara)
- Canada (Toronto, Montreal, Calgary, Vancouver)
- UK (London vs Regional)
- Puerto Rico

**Priority:** High (foundational for Fanbase DNA System implementation)

---

### DNA Shifts Over Eras Template
**Status:** Offered, user moved on
**Concept:** How fanbase demographics evolve decade by decade
**Example Shifts:**
- 1970s: Conservative, older, rural, male-heavy
- 1985: Libertarian attitude, "boys will be boys" tolerance
- 2000: Cultural splits emerging, younger fans want edgier content
- 2020: Massively diversified, younger socially aware, older nostalgia-driven

**Use Case:** Historical game starts reflect era-appropriate fan DNA
**Priority:** Medium (adds authenticity to era-based play)

---

### Sample Promotion Fanbase Composition
**Status:** Offered, user moved on
**Concept:** % breakdown of where fans are from geographically
**Examples Discussed:**
- Stardom 2020s: 70% Japan, 20% US, 5% Europe, 5% Rest
- WWE 2020s: 55% US, 20% Europe, 15% Latin America, 10% Rest
- NJPW 2020s: 65% Japan, 20% US, 10% Europe, 5% Rest
- AEW 2020s: 70% US, 15% Europe, 10% Canada, 5% Rest

**Use Case:** Multi-region scandal fallout, international expansion strategy
**Priority:** Medium (ties to Fanbase Mutation System)

---

### Shield Strength Calculation Example
**Status:** Offered, user moved on
**Concept:** Full walkthrough showing sample promotion handling series of scandals
**Purpose:** Illustrative example for documentation
**Priority:** Low (documentation enhancement)

---

### Scandal Cascade Flowchart
**Status:** Offered, user asked about management tags instead
**Concept:** Visual showing: shield crack → courage cascade → memory resurgence → collapse/reform
**Components:**
- Initial exposure (first victim speaks)
- Cascade trigger (others feel safe to speak)
- Memory resurgence (old scandals resurface)
- Chain reaction (new lawsuits, mass leaks)
**Priority:** Low (documentation enhancement)

---

### Owner Archetypes (Beyond Tags)
**Status:** AI suggested 5 types, user locked only the 9 Management Tags
**Archetypes Discussed:**

| Archetype | Behavior |
|-----------|----------|
| Ruthless Dictator | Deny, delay, fight tooth and nail; image > ethics; burn everything to protect throne |
| Corporate Bureaucrat | Step down or force resignation quickly to minimize brand risk; company > individual |
| Outlaw Promoter | Laugh it off publicly; accelerate chaos; scandal becomes brand marketing |
| True Believer Idealist | Immediate firing and public apologies; morality > business |
| Political Survivor | Damage control spin; blame "bad actors"; sacrifice scapegoats while protecting leadership |

**Status:** May be redundant with Management Behaviour Tags, or could be composite profiles
**Priority:** Low (tags may already capture this)

---

### Fanbase Drift System
**Status:** Mentioned, mechanics not built
**Concept:** Promotions changing demographics over time based on booking/branding decisions
**Examples:**
- WWE going PG = younger fanbase, family-heavy
- ECW going edgy = male 18-35, hardcore loyalists
- NJPW international expansion = growing US percentage
**Mechanics Needed:**
- Drift triggers (booking style, branding, TV deal changes)
- Drift speed (how fast demographics shift)
- Stability thresholds (when fanbase "locks in")
**Priority:** Medium (adds long-term promotion evolution)

---

## 🟡 VOL 2 CHUNK 08 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 08 Part 1 discussion threads (2025-12-26)

### Global Event Database Starter Set
**Status:** AI offered to build 15-20 anchor events, user moved to weather topic
**Concept:** Core real-world events database 1980-2020+
**Examples to Include:**
- Desert Storm (1990-91): Patriotic surge, Middle Eastern heel gimmicks radioactive
- 9/11 (2001): Extreme nationalism surge, anti-American heels forced to alter gimmicks
- 2008 Recession: Promotions struggle, ticket prices critical, indie deaths
- COVID-19 (2020): Live event shutdowns, streaming dominance, hardcore loyalty hardens
- Internet Explosion (late 90s): Rise of smart marks, kayfabe death, scandal coverage explodes

**Use Case:** World events affect fan mood, booking viability, scandal tolerance, economics
**Priority:** High (core to Global Event Stream system)

---

### News Ticker & Headlines Feature
**Status:** Mentioned as "bonus layer," no explicit lock
**Concept:** In-game news headlines splash over calendar
**Examples:**
- "Iraq War Begins, Patriotism Surges in U.S."
- "Global Financial Crisis, Indie Scene Suffers Sharp Decline"
- "COVID-19 Outbreak, Live Crowds Suspended in Most Countries"
- "Social Media Boom, Fan Access to Stars Unprecedented"

**Priority:** Low (UI/presentation enhancement)

---

### Weather Adaptability Tags
**Status:** AI suggested, user didn't confirm specific tags
**Tags Proposed:**

| Tag | Effect |
|-----|--------|
| Rain Master | Thrives in rain, solid footing, embraces chaos |
| Sun Warrior | Performs best in clear hot outdoor settings |
| Ice Cold Professional | Works well in bitter cold, snowstorms |
| Weather Fragile | Falls apart when conditions aren't perfect |
| Show Must Go On | Takes no complaints, wrestles no matter what, gains loyalty |

**Priority:** Low (enhancement to Weather Risk System)

---

### Regulator Personality Types
**Status:** AI suggested, user moved on
**Types Proposed:**

| Type | Behavior |
|------|----------|
| Strict Moralist | Impossible to bribe, enforces all regulations |
| Pragmatic Greaser | Easy bribes, looks the other way |
| Reluctant Go-Along | Can be pressured into compliance |
| Vengeful Crusader | Actively hunts promotions, personal vendettas |

**Use Case:** State athletic commissions, licensing, blood/weapon restrictions
**Priority:** Medium (adds regional political depth)

---

### Regional Gimmick Tags
**Status:** AI suggested, user asked follow-ups but didn't lock
**Tags Proposed:**

| Tag | What It Represents |
|-----|--------------------|
| Anti-Nationalist | Slams nationalism of one region while uplifting another (Bret Hart '97) |
| Nationalist Hero | Celebrates local pride, hero at home, heel elsewhere |
| Culture Clash Artist | Brings foreign values/culture to unsettle audience |
| Globalist Diplomat | Tries to connect all cultures, may bore some, beloved by others |
| Regional Patriot | Plays directly to local fans ("Texas Forever") |
| Political Provocateur | Pushes divisive political stances |
| Regional Antihero | Flawed/bitter regional star, defended at home, booed elsewhere |
| Iconoclast | Attacks industry legends/sacred traditions |

**Use Case:** Regional Gimmick Reception System, face/heel varies by location
**Priority:** Medium (ties to gimmick system expansion)

---

### Bret Hart '97 Gimmick Tag Example
**Status:** Example discussed in depth, not formalized
**Tags Identified for Bret's 1997 Gimmick:**
- Cultural Traditionalist: Respects "old values," slams modern cultural changes
- Anti-American Critic: Specific hostility toward American culture's greed/selfishness
- Internationalist Hero: Openly embraces Canada, Europe, Japan
- Honor-Based Character: Personal/professional honor above cheap victories
- Moral Superiority Complex (Mild Heel Trait): Thinks he's better than modern society
- Family Loyalty Focus: Constantly references Hart Foundation ties

**Use Case:** Template for building context-sensitive gimmicks
**Priority:** Low (example for documentation)

---

### Worker Mental Health Modifier
**Status:** Listed as "Optional Deeper Layer"
**Concept:** Depression, burnout, anxiety, PTSD modifying injury risk and behavior
**Potential Effects:**
- Increased injury risk when mental health low
- Accelerated retirement consideration
- Scandal trigger points
- Creative output quality variation

**Priority:** Low (enhancement to Injury Risk System, potentially sensitive content)

---

### Gameplay Tools (Optional UI Features)
**Status:** Mentioned as optional tools, not locked
**Tools Proposed:**

| Tool | Function |
|------|----------|
| Gimmick Regional Alignment Tracker | Shows where gimmick plays as face/heel/volatile |
| Smart Booking Suggestion | "Crowd likely to boo [worker] in [region], consider turn" |
| AI Promo Modifier | Adjusts promo tone depending on territory expectations |
| Commentary Customization | Commentary reacts differently by region |

**Priority:** Low (UI/UX enhancements for later phases)

---

### Pick and Choose Custom Mode
**Status:** Listed as option, not confirmed
**Concept:** Granular control over which aspects of history are strict vs random
**Combinations:**
- Strict real-world history + wrestling world chaos
- Alt-history world events + strict wrestling scandals
- Full chaos everything
- Custom per-system toggles

**Priority:** Medium (player customization for Alt-History Mode)

---

### Regional Climate Modeling Examples
**Status:** AI built table, user moved on
**Regions Mapped:**

| Region | Typical Weather Risks |
|--------|----------------------|
| Tokyo | Humid summers, typhoons July-September, rainstorms common |
| Osaka | Similar to Tokyo but hotter inland, sweltering heat risk |
| Northern Japan (Sapporo) | Heavy snow winters, dangerous transport but hardcore snow shows possible |
| Texas | Heatwaves summer, flash thunderstorms, occasional tornadoes |
| Florida | High summer rain, hurricanes August-October |
| California (Southern) | Very dry, minimal rain, good for outdoor shows |
| Mexico City | Rainy season May-October, afternoon rains destroy evening outdoor cards |
| Toronto | Cold winters, outdoor summer rain risk, blizzards rare December-February |
| UK | Light rain often, heavy rain sporadic |

**Priority:** Medium (data for Weather Risk System implementation)

---

## 🟡 VOL 2 CHUNK 09 HALF-BAKED IDEAS

📌 **Source:** Vol 2 Chunk 09 discussion threads (2025-12-26)

These concepts were discussed but explicitly deferred or offered without lock:

### Women & Vulnerable Groups Cultural Shift Engine (PARKED)
**Status:** Explicitly marked "parked future module"
**Concept:** Time-dependent system for how fans/promotions react to women/LGBTQ+/racial minority workers

**Era Evolution Noted:**
| Era | Typical Treatment |
|-----|-------------------|
| 1980s | "Frailty," managers as accessories (Elizabeth, Missy Hyatt); rare exceptions (Sherri Martel) |
| 1990s (early) | More aggressive characters but still sidepieces; not seen as serious threats |
| 1998-2001 (Attitude) | Extreme sexualization/objectification ("divas"); crowd buys in hard |
| 2000s (late) | Seeds of Women's Revolution; workrate rises, fan expectations shift slowly |
| 2010s-2020s | Full push toward serious, competitive divisions (Sasha, Becky, Asuka, Giulia, Hayter); lingering disparities (AEW criticism is real) |

**Mechanics Needed:**
- Era-specific tolerance levels for exploitation
- Fanbase demographic splits on how women/minorities are treated
- Regional variation (some areas more progressive earlier)
- Promotion reputation effects based on treatment decisions
- Historical backlash triggers (when did objectification become unacceptable?)

**Priority:** High (adds cultural authenticity, could be controversial if done poorly)

---

### Sample Climate Profiles (Regional Weather Sheets)
**Status:** AI offered to build profiles for Tokyo, Texas, Mexico City, Toronto, UK; user only requested Tampa which was completed
**Concept:** Detailed seasonal risk tables for major wrestling regions

**Regions Still To Build:**
- Tokyo (with 80s/90s vs modern climate evolution)
- Texas (heatwaves, flash thunderstorms, tornadoes)
- Mexico City (rainy season May-October)
- Toronto (cold winters, summer rain)
- UK (light rain often, heavy rain sporadic)
- Monterrey (mentioned as alternative)

**Priority:** Medium (data for Weather Risk System implementation)

---

### Generational Shifts for Fanbase DNA
**Status:** Mentioned as "could deepen realism later," not locked
**Concept:** Fan expectations mutate every decade even without major real-world events

**Examples:**
- Aging boomer fans changing what they tolerate
- Rise of Gen Z with different values
- Shifts in gender/racial diversity expectations
- Technology changing engagement (social media, streaming)

**Mechanics Needed:**
- Decade-based demographic drift formulas
- Generational cohort preferences
- How to blend old fans with new fans in same promotion

**Priority:** Low (current era-based systems capture most of this)

---

### Super Detailed Sub-Region Splits
**Status:** Mentioned as future extension, not urgent
**Concept:** Splitting major regions into culturally distinct sub-regions

**Examples:**
- California: NorCal (tech-heavy, progressive) vs SoCal (entertainment industry, diverse)
- Texas: Houston/Dallas (urban, diverse) vs rural Texas (conservative, traditional)
- UK: London (cosmopolitan) vs Regional (traditional wrestling culture)
- Japan: Tokyo Metro vs Rural prefectures

**Priority:** Low (adds granularity but not essential for MVP)

---

### Regional Booking Hotspots
**Status:** Mentioned but not developed
**Concept:** Certain match types or booking styles resonate more strongly in specific regions

**Examples to Design:**
- Texas Death Match more over in Texas (obviously)
- Lucha trios rules resonate in SoCal, Texas, Mexico
- Strong style/King's Road pacing expectations in Japan
- Hardcore/deathmatch hotspots (Philadelphia, FMW regions of Japan)
- British rounds style in UK

**Mechanics Needed:**
- Match type regional bonuses/penalties
- Style expectation matching
- Crowd confusion when unfamiliar styles presented

**Priority:** Medium (adds regional authenticity)

---

### Insurance/Risk Management System
**Status:** Mentioned briefly ("insurance payouts if purchased") but not designed
**Concept:** Promotions can purchase insurance against various risks

**Insurance Types to Design:**
- Event cancellation insurance (weather, disasters)
- Worker injury insurance
- Scandal liability insurance (legal defense funds)
- Venue damage insurance (deathmatches, pyro)

**Mechanics Needed:**
- Premium costs by promotion size/risk level
- Payout calculations
- Claim denial scenarios
- Financial planning integration

**Priority:** Medium (ties to Economics System)

---

### Promotion Tags: Dirty Cover-Up / Whistleblower Friendly
**Status:** Mentioned in Scandal Rumours section, not formally locked
**Concept:** How promotions handle media/journalist investigation of scandals

| Tag | Description |
|-----|-------------|
| Dirty Cover-Up | Actively suppresses scandal exposure; bribes, threats, legal action against accusers |
| Whistleblower Friendly | Encourages internal reporting; protects accusers; faster scandal resolution |

**Mechanics Interaction:**
- Dirty Cover-Up: Delays scandal exposure but increases severity when it finally breaks
- Whistleblower Friendly: Faster minor scandals but less catastrophic blowups

**Priority:** Medium (adds depth to Scandal System)

---

### Promotion Therapist/Trainer Support Feature
**Status:** Mentioned as Mental Health recovery path, not designed
**Concept:** Promotions can offer (or not offer) mental health support

**Features:**
- Therapist on staff (reduces mental health decay, faster burnout recovery)
- Trainer support programs (injury prevention, rehab quality)
- EAP (Employee Assistance Programs) for substance issues

**Mechanics Needed:**
- Cost to promotion
- Effect on worker mental health/morale
- Era availability (70s-80s: rare; 2020s: expected by workers)
- Reputation effects (promotions without support = harder recruitment)

**Priority:** Low (enhancement to Mental Health System)

---

### "Thank You, Tommy!" Easter Egg
**Status:** User wanted to name "Innovator of Violence" tag this as Deadlock podcast reference; deemed too niche
**Concept:** Hidden easter egg or alternate name visible in certain contexts
**Implementation Ideas:**
- Unlock after certain conditions met
- Hidden tooltip reference
- Rare random pop-up

**Priority:** Very Low (fun easter egg, not essential)

---

### Era-Based Booking Pattern Examples (AJPW Template)
**Status:** Detailed examples given but not formalized as templates
**Concept:** How promotion booking style evolves across eras

**AJPW Example (Documented in Discussion):**

| Era | Booking Pattern |
|-----|----------------|
| 1990-1992 | Heavy six/eight man tags monthly; escalating violence; long-term storytelling; cluster battle royals for fun/relaxation; Jumbo/Misawa feud drives booking |
| 1994-1998 | Serious singles and tag wars dominate; less battle royal/chaotic undercard clutter; King's Road escalation peaks (fatal bumps); Kawada vs Misawa era |

**Templates to Build:**
- NJPW 1987-1990 (gauntlets, UWF invasion)
- NOAH 2000-2005 (Captain's Fall, respect-focused)
- WCW 1997 (NWO chaos, bait-and-switch finishes)
- WWF Attitude Era (crash TV, extreme sports crossover)

**Use Case:** AI booking behavior, historical scenario accuracy
**Priority:** Medium (adds authenticity to AI bookers and historical play)

---

### Progress Percentage Tracking (Meta-Discussion)
**Status:** User asked about project completion; numbers given but methodology not formalized
**Estimates Given:**

| Layer | Completion |
|-------|------------|
| Core Systems | ~35-40% Conceptual |
| Fine Systems (Hidden Traits, Fanbase DNA, Scandal, Weather, etc.) | ~60-70% Conceptual |
| Database Work (Real World Workers/Promotions) | ~2% |
| UI/Player Interaction Planning | ~10-15% |
| Narrative/News/Event Systems | ~25-30% Conceptual |
| **Overall System Scaffolding** | **~5-6%** |

**Notes:**
- Conceptual = Blueprint done, not implemented
- Database work is the long tail
- 5-6% in one weekend is excellent pace

**Priority:** N/A (tracking metric, not gameplay system)

---

### AI Database Collaboration Workflow
**Status:** Discussed, methodology agreed but not documented
**Concept:** How Claude and user split database building work

| Task | Lead | Notes |
|------|------|-------|
| Core roster building (workers, promotions, titles, careers) | Claude | Generate raw templates from historical sources |
| Skill evaluations (workrate, psychology, charisma) | Claude + User | Claude drafts, user reviews/tweaks |
| Career arcs, hidden traits, scandal timelines | Claude (initial) + User (refinement) | Claude drafts major known arcs; user adjusts |
| Tag assignment (personality quirks, political behaviors) | Claude + User | Refine together, especially for major stars |
| Real-world title histories and major reigns | Claude (heavy lifting) | User tweaks prestige tiers |

**Philosophy:** Claude = line producer, User = executive producer
**Priority:** N/A (process methodology, not gameplay system)

---

---

## 🟡 VOL 5 HALF-BAKED IDEAS

📌 **Source:** Vol 5 lines 769-785 (Living Match Context discussion)

### Booker Philosophy Types
**Status:** Mentioned, NOT fully defined
**Types Listed:**
- Realist
- Chaos Merchant
- Myth Builder
- Corporate Safe Player

**Mechanics Needed:**
- Full definition of each type
- How philosophy affects booking decisions
- How philosophy interacts with promotion identity
- Philosophy evolution/drift over time
**Priority:** High (core to LMC system)

---

### World Historical Phase Definitions
**Status:** Mentioned, NOT fully defined
**Phases Listed:**
- Boom
- Collapse
- Civil War
- Renaissance
- (Stagnation mentioned elsewhere)

**Mechanics Needed:**
- Triggers for phase transitions
- How phases affect fan patience/loyalty
- Regional vs global phase tracking
- Duration expectations per phase
**Priority:** High (core to LMC system)

---

### Fatigue-to-Pacing Formulas
**Status:** Concept LOCKED, exact formulas NOT specified
**Concept:** Worker fatigue level affects match pacing recommendations
**What's Missing:**
- Exact % thresholds for fatigue levels
- Pacing modifier calculations
- How fatigue interacts with match flavor
- Cumulative wear vs single-match fatigue distinction
**Priority:** Medium (implementation detail)

---

### Soul Sounds System (PINNED for Phase 2)
**Status:** Explicitly pinned for Phase 2 polish
**Source:** Vol 5 lines 802-806
**Concept:** Player-created custom sound triggers for game events

**Core Features:**
- Completely optional (OFF by default)
- Player uploads sounds, creates weighted pools
- Assigns sounds to ANY system event
- Volume, cooldown, silence controls
- Shareable via SCS community servers

**Example Triggers Discussed:**
| Event | Sound Example |
|-------|---------------|
| Road Agent Urgent Warning | Navi "LISTEN!" or "LOOK. LISTEN!" clip |
| Bad Match Results | Mario death sound |
| Firing Injured Worker | Jim Ross "no conscience, no heart, no SOUL" |
| Show Opening | Ring bell or motivational speech |
| Worker Betrayal | Dramatic anime gasp |
| Ladder Match Booked | Zelda treasure chest sound |
| Worker Opens Vince Russo's Laptop | Wet fart sound |

**Trigger Categories:**
- Booking Layer (match booked, worker pulled, show confirmed)
- Agent Layer (warning, praise, advice)
- Worker Layer (betrayal, injury, firing, contract)
- Promotion Layer (show start, title change, financial disaster)
- World Layer (industry collapse, boom start, scandal)
- Miscellaneous (laptop, easter eggs, unlockables)

**Philosophy:** Lets players make the world feel as serious, chaotic, emotional, or funny as they want. Maximum player agency without canon-breaking.

**Priority:** Phase 2 Polish (not MVP)

---

### Live Mid-Match Agent Observation (PHASE 2)
**Status:** Explicitly marked Phase 2 expansion
**Source:** Vol 5 line 834
**Concept:** If live crowd drift simulation is built per match minute, agents could warn about mid-match burnout or unrest
**Current State:** Pre-Match and Pre-Segment warnings are LOCKED. Mid-match is future expansion.
**Mechanics Needed:**
- Per-minute crowd state tracking during matches
- Real-time agent observation triggers
- Mid-match audible options for player
**Priority:** Phase 2 (requires detailed match simulation)

---

### Road Agent Traits/Personality System
**Status:** Mentioned, not designed
**Source:** Vol 5 line 834 ("Bad agents might miss it or give dumb/misleading advice. More on that later when we build agent traits.")
**Concept:** Agents have varying quality and specializations
**Potential Traits:**
- Good agents warn clearly and accurately
- Bad agents miss warnings or give misleading advice
- Specialists in specific styles (technical, hardcore, comedy, etc.)
- Experience level affecting warning quality
**Mechanics Needed:**
- Agent stat system
- Warning accuracy modifiers
- Specialization bonuses
- Hiring/firing agents
**Priority:** Medium (adds depth to Road Agent system)

---

### Experience as Formal Skill vs History Log ✅ RESOLVED
**Status:** RESOLVED - No formal Experience stat
**Source:** Vol 5 lines 859-862
**Decision:** Experience is emergent from Career History Log, Age, Injury History, Accumulated World Memory, and Mental Skills (Psychology, Focus, Adaptability) that grow over career.

**Rationale:**
- Workers already show experience naturally through Age, Career Match Log, Titles held, Big Matches logged, Injuries overcome, Tours survived
- Non-wrestlers (agents, refs) handled same way: years active, matches agented/refereed, major moments, loyalty tags
- Booking AI can still read worker histories dynamically
- Aligns with "Tags Not Stats" design principle
- No artificial "Experience: 16/20" number needed
- Players can feel when someone's a veteran instead of seeing sterile number

**Resolution:** No new stat. Experience emerges organically. ✅ LOCKED

---

### Burning Ring Soul Database Concept
**Status:** Planning / Future Phase
**Source:** Vol 5 lines 981-985
**Concept:** Historical database feeding both SCS (soul memory/booking) and FPW+++ (match engine).

**Purpose:**
- Populate workers
- Populate titles and emotional histories
- Populate promotion founding myths
- Seed loyalty webs and feuds
- Seed early emotional booking trends

**Integration:**
- SCS = soul memory and booking
- FPW+++ = match realization of that soul memory (movesets, chaining sequences, character appearance, sell patterns)

**Data Sources:**
- Fire Pro Edits as draft layer (need refinement)
- AI video scraping (improving, needs human validation)
- Historical research

**Notes:**
- Summer 2026 dev sprint realistic
- Tuning/testing afterward still serious work
- Can open to handpicked editors/historians later

**Priority:** Post-SCS Core Systems

---

*Last Updated: 2025-12-29*
*Status: Vol 1 Extraction Complete, Vol 2 Chunks 01-09 Integrated, Vol 5 COMPLETE*

---

## 🅿️ Long-Term Booking Planner (Vol 5 lines 1182-1183)

**Status:** Half-Baked

**Core Concept:** Start with destination match (blow-off), book backwards from there with big picture angles/tags.

**Features:**
- Calendar with shows, click to plan segments
- Visual style options: notebook (pre-internet), early computer, modern PC, phone
- Assistant gives feedback/ideas
- See trajectory at a glance

**Naming Problem:** "Trajectory mode" rejected as clunky. Needs wrestling parlance name.

**Possible Names:**
- Planning Mode
- Long-Term Planning
- Roadmap Mode
- The Board
- Arc Builder
- Finish Line
- Payoff Planner

**Needs:** Wrestling-grounded name, UI spec, integration with AutoBooker and Feud Memory.
