# BOOKING ENGINE (PHASES 1-3)

📛 **NAME:** Booking Engine (Core Systems)  
🧭 **CATEGORY:** Show Construction, Storyline Management & Crowd Manipulation  
🔑 **KEYWORDS:** booking, show structure, feuds, turns, segments, promos, match outcomes, stakes, predictability  
📝 **SUMMARY:**

The Booking Engine is the core system for constructing shows, managing storylines, and producing desired crowd reactions. Phases 1-3 (locked in Vol 2) cover: match/segment construction (Phase 1), momentum & popularity dynamics (Phase 2), and feud/story memory tracking (Phase 3). Booking isn't about control: it's about managing chaos, crafting emotion, and building long-term memory.

⚙️ **LOGIC OVERVIEW:**

- **Phase 1:** Match/segment inputs, booking philosophy, execution quality, consequences (ratings, morale, memory)
- **Phase 2:** Momentum vs. Popularity distinction, push strategies, crowd memory systems, false popularity detection
- **Phase 3:** Feud Memory Tracker, Segment/Promo Engine, Turn Engine + Fallout, Predictability & Stakes Logic
- Booking decisions affect: crowd reactions, worker morale, popularity trajectories, locker room politics, long-term fan memory
- Matches evaluated on: worker chemistry, card placement, crowd energy, execution, finish impact, narrative context
- System tracks booking patterns: crowds learn and react to predictable booking (50/50, Superman pushes, screwy finishes)

🔬 **LLM INTEGRATION:** Yes: LLM can suggest booking decisions, analyze fan sentiment patterns, generate promo content, create turn scenarios, and flag potential booking mistakes

📌 **ORIGIN:** Vol. 1 (concept), Vol. 2 (Phases 1-3 locked), Vol. 3-4 (Phase 4 Emotional Show Flow added)

📎 **CONNECTED SYSTEMS:** [[Crowd_Memory]], [[Popularity_System]], [[Worker_Skills]], [[Hidden_Personality]], Match Engine, [[Turn_Engine]], Morale, Backstage Politics, Scandal System

❓ **OPEN QUESTIONS:**

- Phase 5+ systems (Locker Room Politics, Business/TV Systems) not fully specified
- Exact formulas for momentum gain/loss
- AI Booker personality implementation (referenced but not built)

✅ **STATUS:** Phases 1-3 LOCKED (Vol 2), Phase 4 LOCKED (Vol 3-4), Phase 5+ in progress

---

## VERSION HISTORY

**Version 1.0 (Vol 1)**
- Booking engine concept introduced
- Match construction basics proposed
- Core inputs defined (participants, match type, stakes)

**Version 2.0 (Vol 2) [PHASES 1-3 LOCKED]**
- Phase 1: Match inputs, philosophy settings, processing layers, consequences
- Phase 2: Momentum vs. Popularity distinction, push strategies, false popularity
- Phase 3: Feud Memory Tracker, Segment/Promo Engine, Turn Engine, Predictability Index
- Booking pattern tracking introduced

**Version 2.5 (Vol 3-4)**
- Phase 4 (Emotional Show Flow) added as separate system
- Turn Engine fallout mechanics refined
- Predictability Index formula specified
- AI Booker concept introduced (not fully specified)

---

## PHASE 1: CORE STRUCTURE

### What Is a Booking?

Booking = The deliberate construction of a show's structure, outcomes, and arcs to produce desired crowd reactions and future narrative opportunities.

**Not just:**

- Picking winners
- Matching names

**But crafting:**

- Emotion
- Momentum
- Memory

### Core Match Inputs

| Input | Description |
|-------|-------------|
| **Participants** | Workers, teams, managers, special enforcers |
| **Match Type** | Singles, tag, ladder, cage, ironman, etc. |
| **Card Placement** | Opener, midcard, semi-main, main event, post-main |
| **Stakes** | Title, grudge, tournament, retirement, pride, or nothing |
| **Intended Outcome** | Who wins, how (pin/sub/DQ/countout), clean vs. dirty |
| **Booking Intent** | Pop crowd, build feud, rehab someone, shock value, test chemistry |
| **Agenting/Flow** | Pacing, dominance balance, spots, interference (auto or manual) |

### Booking Philosophy Settings

| Setting | Effect |
|---------|--------|
| **Match Importance Weighting** | Emphasize quality vs. storyline drama vs. crowd moments |
| **Fan Engagement Target** | Smart fans, casuals, regional loyalists, spectacle lovers |
| **Push Strategy** | Slow build, rocket push, 50/50 parity, veteran protection |
| **Booking Tone** | Realism, chaos, unpredictability, conservative, comedy, serious |
| **House Style Enforcement** | How strictly matches fit fed style (strong style, lucha, TV, hardcore) |

These influence how fans interpret and react to matches, not just if they "like" them.

### Match Processing Layers

| Layer | Evaluates |
|-------|-----------|
| **Worker Chemistry** | Style compatibility, personal tension, past matches |
| **Match Type Fit** | Are workers good at this match type? |
| **Card Placement** | Over/under-delivering for its slot? |
| **Crowd Energy** | Does it cool down hot crowd or revive dead one? |
| **Execution Quality** | Psychology, pacing, botches, charisma, improvisation |
| **Finish Impact** | Clean wins vs. dusty finishes, surprises, betrayals, screwjobs |
| **Narrative Context** | Does it move story forward or confuse the arc? |

### Booking Consequences

| Outcome | Effect |
|---------|--------|
| **Match Rating** | Fan perception, observer scores, promotion reputation |
| **Worker Momentum** | Short-term buzz (not always positive from winning) |
| **Popularity Adjustment** | Long-term gain/loss based on engagement and context |
| **Fanbase Reaction** | Cheers, boos, silence, split reactions, backlash |
| **Backstage Morale** | Veterans angry at usage, young workers lit up by big moment |
| **Scandal Risk** | Match misuse, tasteless content, blood overuse, injury |
| **Booking Memory** | If moment lands, fans remember. If not, it fades or haunts you |

### Segment Engine (Non-Match Booking)

Same engine for:

- Promos (in-ring, backstage, pre-taped)
- Betrayals / Reconciliations
- Surprise returns / Debuts
- Post-match brawls
- Contract signings
- Media stunts
- Fan interactions

Same evaluation: Intent, Tone, Placement, Fan Expectations, Execution Quality

Can attach to matches or run standalone.

---

## PHASE 2: MOMENTUM, POPULARITY & CROWD MEMORY

### Momentum vs. Popularity

**Momentum (Short-Term):**

- Week-to-week buzz
- Hot streaks, recent big wins
- Volatile: can spike or crash quickly
- Affects immediate booking decisions
- Example: Wrestler loses but gets massive crowd sympathy → momentum UP despite loss

**Popularity (Long-Term):**

- 0-100 scale by region/demographic
- Built over months/years
- Stable: changes slowly
- Affects drawing power, merch sales, contract value
- Example: John Cena always has high pop even when momentum is low

**Critical Distinction:** You can have high pop with low momentum (stale star) or low pop with high momentum (hot newcomer).

### Push Strategies

| Strategy | Description | Risk |
|----------|-------------|------|
| **Slow Build** | Gradual elevation over 6-12 months | Safe, organic, but requires patience |
| **Rocket Push** | Fast main event push (3-6 months) | High risk of false popularity backlash |
| **50/50 Booking** | Alternating wins/losses without story | Kills momentum, fans lose interest |
| **Veteran Protection** | Keep legends strong even declining | Blocks younger talent, staleness risk |
| **Hot Potato** | Title changes hands frequently | Devalues title, confuses fans |
| **Long Reign** | Extended title run (6+ months) | Builds prestige but risk of staleness |

### False Popularity Detection

When (Push Level - Organic Pop) ≥ 20 → Triggers backlash

- Crowd becomes hostile
- "Manufactured Star" tag applied
- Pop growth slows (0.5x multiplier)
- Must rebuild from scratch (turn heel, step back, or repackage)

### Crowd Memory Basics

- Tracks what fans remember from booking history
- Emotional moments have higher retention
- Memory decays over time (varies by intensity)
- Regional differences in memory loyalty
- Past booking affects future reactions

*(Full Crowd Memory system in: [[Crowd_Memory]])*

---

## PHASE 3: FEUD & STORY SYSTEMS

### 3.1 - Feud Memory Tracker

**Purpose:** Track long-term feud arcs, emotional heat, crowd investment

**Tracks:**

- Match history between workers
- Emotional peaks (betrayals, injuries, title changes)
- Crowd investment level (how much fans care)
- Feud fatigue (overexposure risk)
- Payoff timing (when to blow it off)

**Memory Decay:**

- High-emotion feuds decay slower (fans remember longer)
- Low-stakes feuds fade fast
- Time between matches affects anticipation vs. forgotten

**Feud Types:**

| Type | Duration | Intensity | Payoff |
|------|----------|-----------|--------|
| **Blood Feud** | 6-12 months | Maximum | Career-defining match |
| **Title Chase** | 3-6 months | High | Championship win/loss |
| **Rivalry** | Ongoing | Medium | Episodic, no clear end |
| **Quick Program** | 1-2 months | Low-Medium | Single PPV match |
| **One-Off** | Single show | Low | Filler, no story |

**Callbacks & Continuity:**

- System suggests callback opportunities from past feuds
- Long-dormant feuds can be resurrected (reunion pops)
- Overuse of callbacks = diminishing returns

---

### 3.2 - Segment & Promo Engine

**Purpose:** Non-wrestling content that builds feuds and characters

**Segment Types:**

- **In-Ring Promo** (solo or confrontation)
- **Backstage Interview** (controlled environment)
- **Ambush/Brawl** (chaos, physicality)
- **Contract Signing** (tension, eventual violence)
- **Return/Debut** (surprise, crowd pop)
- **Retirement Speech** (emotional send-off)
- **Press Conference** (media interaction, shoot elements)

**Promo Evaluation Factors:**

- **Mic Skills** (worker ability)
- **Character Work** (staying in gimmick)
- **Crowd Response** (heat generation)
- **Believability** (does it feel real?)
- **Advancement** (does it move story forward?)
- **Catchphrase/Memorable Moment** (quotability)

**Segment Outcomes:**

| Outcome | Effect |
|---------|--------|
| **Promo Kills** | Major heat generation, feud escalation |
| **Solid Promo** | Advances story, maintains interest |
| **Weak Promo** | Crowd loses interest, momentum stalls |
| **Bombed Promo** | Crowd turns on speaker, negative buzz |
| **Derailed Promo** | Crowd hijacks ("What?" chants, competing chants) |

**Promo Response System (Vol 7):**

- Era-locked behaviors ("What?" chants in 2000s US)
- Smart crowd vs. casual crowd reactions
- Derailing mechanics (crowd takes over)
- Recovery options (lean into it vs. fight it)

---

### 3.3 - Turn Engine + Fallout

**Purpose:** Manage heel/face turns and their consequences

**Turn Types:**

| Turn Type | Description | Setup Time | Impact |
|-----------|-------------|------------|--------|
| **Clean Turn** | Clear, decisive, immediate | 0-2 weeks | High initial pop, clean break |
| **Slow Burn** | Subtle hints over months | 3-6 months | Organic, crowd invested |
| **Shock Turn** | No warning, sudden betrayal | 0 (surprise) | Maximum heat, memorable |
| **Double Turn** | Both wrestlers switch alignment | Varies | Complex, requires skill |
| **Failed Turn** | Crowd rejects intended alignment | N/A | Booking disaster, requires pivot |

**Turn Mechanics:**

- **Setup Phase:** Teases, tension, foreshadowing (optional for shock turns)
- **Turn Moment:** Betrayal, attack, promo reveal
- **Immediate Fallout:** Crowd reaction, victim response, alignment shift
- **Long-term Consequences:** Morale shifts, faction realignment, feud begins

**Turn Fallout Tracking:**

| Factor | Effect |
|--------|--------|
| **Crowd Trust Decay** | If turn feels forced, fans reject it |
| **Victim Sympathy** | Babyface who got turned on gains pop |
| **Heat Generation** | New heel gets nuclear heat (if done right) |
| **Merchandise Impact** | Sales drop (heel turn) or spike (face turn) |
| **Locker Room Reaction** | Workers have opinions, may affect morale |
| **Feud Memory Anchor** | Creates lasting story anchor for callbacks |

**Failed Turn Recovery:**

- Acknowledge crowd rejection
- Pivot quickly (retcon, double-turn, or lean into chaos)
- Examples: Roman Reigns (forced face), Rocky Maivia (rejected babyface → Rock heel)

---

### 3.4 - Predictability & Stakes Logic

**Purpose:** Prevent booking from becoming formulaic and boring

**Predictability Index:**

Tracks how obvious match outcomes are to fans based on:

- Booking history patterns
- Win streak logic (undefeated streak = obvious winner)
- Title match placement (does champ always retain at TV? Lose at PPV?)
- Interference patterns (does heel always cheat same way?)
- Finish types (3 kickouts → finisher → win every time)

**Formula:**

Predictability Index = (Pattern Recognition Score × Booking Repetition) / Surprise Factor

**Effects of High Predictability:**

- Crowd checks out early ("we know how this ends")
- Lower match ratings despite quality
- Fan Cynicism Index grows (fans become jaded)
- "Booking is stale" reputation damage
- Requires booking swerves to reset

**Stakes Weighting:**

| Stakes Type | Crowd Investment | Risk |
|-------------|------------------|------|
| **No Stakes** | Low | Safe but forgettable |
| **Personal Pride** | Medium | Depends on characters |
| **Title Match** | High | Outcome matters long-term |
| **Career vs. Career** | Maximum | Must deliver emotionally |
| **Loser Leaves Town** | Very High | Rare, high-impact |
| **Mask vs. Mask** (Lucha) | Maximum | Cultural sacred match |

**Underdog Mechanics:**

- Underdog pop bonus when unlikely winner prevails
- Requires believable struggle (can't squash)
- Overuse = no longer underdog

**Fan Speculation Bonus:**

- When outcome is genuinely uncertain, crowd engagement spikes
- "Dream match" hype when both could realistically win
- Requires protecting multiple workers equally

**Booking Corner Penalties:**

When booking becomes too predictable:

- -5 to -10 match rating
- Crowd memory penalty (fans forget match faster)
- Staleness tag applied to promotion

**Solutions:**

- Swerve booking (occasional upsets)
- Vary finish types
- Clean finishes (not always screwy)
- Long-term storytelling (payoff unpredictability)

---

## IMPLEMENTATION NOTES

### Booking Decision Flow:

1. Select participants, match type, stakes
2. Set booking intent and desired outcome
3. System evaluates chemistry, placement, crowd energy
4. Match executes (using Match Engine)
5. Calculate consequences: rating, momentum, pop, morale, memory
6. Update feud tracker, predictability index, worker statuses
7. Generate fallout events if triggered (turns, injuries, scandals)

### AI Booker Integration (Phase 5+, not fully specified):

- AI can suggest match cards based on available workers
- Respects promotion philosophy settings
- Learns from crowd reactions (avoid repeated failures)
- Can be assigned booking "personality" (Gedo-style long-term, Vince Russo crash TV, etc.)

---

## RELATED SYSTEMS

- [[Worker_Skills]]: Affects execution quality
- [[Hidden_Personality]]: Affects booking compliance, backstage reactions
- [[Tags_System]]: Affects match specialty, promo ability
- [[Popularity_System]]: Affected by booking, affects drawing power
- [[Crowd_Memory]]: Tracks what fans remember
- [[Emotional_Show_Flow]]: Phase 4, pacing/rhythm
- Morale System: Booking affects worker satisfaction
- Scandal System: Tasteless booking triggers scandals

---

## PHASE 3.5: ADVANCED BOOKING MECHANICS (Vol 1 Extraction)

📌 **Source:** Vol 1 Extraction #32-42

### 3.5.1 - Cumulative Fatigue System (#32)

**Core Concept:** Every grueling match impacts next match stamina and bump resistance.

| Mechanic | Description |
|----------|-------------|
| **Post-Match Stamina Penalty** | Based on match length, stiffness, bump count, blood loss |
| **Cumulative Wear** | After 8-10 title defenses, workers degrade without rest |
| **Recovery Rate** | Varies by worker (ironmen like Misawa/Kobashi recover better) |
| **Injury Risk Link** | Heavy fatigue = higher injury risk, slower recovery |
| **Smart Booking** | Rest periods between major matches preserve worker longevity |

**In Practice Example (Locked):**
- Omega has 5 brutal G1 matches
- Stamina drops 15%
- Barely beats Naito in semis
- By final vs Goto, running on fumes
- Even if Omega loses, performance skyrockets popularity

**Key Insight:** "Tournaments organically create legends and tragic heroes without scripting."

---

### 3.5.2 - Push Organicity Score (#33)

**Core Concept:** Fans prefer pushes that feel earned. Force-pushing midcarders to main events instantly can backfire.

| Factor | Effect |
|--------|--------|
| **Gradual Buildup** | Positive modifier |
| **Major Feuds Won** | Positive modifier |
| **Instant Main Event Push** | Risk of rejection |
| **Only Looks, No Substance** | "X-Pac Heat" mechanic triggers |

**Era Sensitivity:**

| Era | Fan Tolerance |
|-----|---------------|
| Pre-1990s (Kayfabe) | Much more forgiving |
| 2000s+ | Highly critical, detect "fake pushes" |
| Social Media Era | Instant revolt possible, hashtag campaigns |

**Backstage Leak Risk (Modern Era):**
"MAKE ROMAN LOOK STRONG" type leaks can affect fan perception negatively.

---

### 3.5.3 - Tournament Burnout Tracker (#34)

**Core Rule:** Promotions spamming tournaments see:
- Fan disinterest
- Locker room fatigue
- Reduced buys

**Cultural Exception:** Tournament-heavy cultures (old RINGS/UWFi, modern G1) have higher tolerance.

---

### 3.5.4 - Era-Sensitive Fan Logic (#35)

**Core Framework:**

| Era | Fan Values |
|-----|------------|
| 1985 | Kayfabe, in-ring toughness |
| 2025 | Real-life character, authenticity, social media presence |

**Scandal Impact by Era:**

| Era | Scandal Handling |
|-----|------------------|
| 1950s-1980s (Kayfabe) | Scandals matter only if breaking kayfabe, otherwise swept under rug |
| 1990s-2000s (Post-Kayfabe) | Affects alignment, momentum, crowd respect |
| 2010s-Now (Social Media) | Instant explosion, fans expect apologies/suspensions/exile |

**Random Debut Era Adaptation:**
Workers from modern era dropped into older settings need "Era Adaptability" stat:
- **Omega in 1984 Crockett:** High spots = crowd boos "phony wrestler"
- **Must Adapt:** Learn to sell more, work gritty, minimize motion
- **Or Refuse:** Get marginalized, leave town

---

### 3.5.5 - Title Run Decay Curve (#37)

**Core Concept:** "The chase is always easier than the reign."

| System | Description |
|--------|-------------|
| **Momentum of the Chase Buff** | +10 momentum bonuses during chase |
| **Weight of the Crown Debuff** | Small automatic decay every month as champion |

**Decay Prevention Methods:**
- New hot challengers emerge
- Big matches redefine reign (instant classics)
- Booking assistant warnings: "The crowd loves [worker], but they're starting to crave something new."

**Alignment Difference:**

| Alignment | Decay Rate |
|-----------|------------|
| Babyface Champions | Struggle to stay hot, faster decay |
| Heel Champions | Decay slower (easier to hate), unless too cowardly/boring |

**Success Example:** Okada 2016-18: Fought decay successfully, created dynasty.

---

### 3.5.6 - Loss-Based Character Building (#40)

**Core Concept:** Losses can build momentum when handled right.

**Match Storytelling Engine:**

| Factor | Effect |
|--------|--------|
| Strong Psychology in Defeat | Builds crowd empathy |
| Desperation/Near Misses | Popularity ticks UP, not down |
| Gutsy Fighting Spirit | Triggers small bonuses |

**Loss Momentum Cooldown:** Fans only give so many "gutsy losses" before expecting payoff or losing interest.

**Legendary Loss Status:** Certain matches tagged as career-defining even if lost:
- Hardy vs Taker (ladder match)
- Omega vs Okada I

**Subtle Implementation (User-Locked):**
- No gamey "10 gutsy loss" counter popup
- Booking team/worker tells you: "hey, this guy has lost valiantly 10 times. It's stale."
- Penalties on match ratings increase the more you ignore

**Instant Classic System:** Matches rated "Instant Classic" automatically shift fan perception:
- "Hardy's gutsy fight has shifted fan perception. He's now seen as someone who could hang with top stars."

---

### 3.5.7 - Booking Pattern Recognition (#41, #97)

**Core Concept:** If you repeat the same show structure over and over, fans notice and engagement drops.

**What Fans Detect:**
- Push Authenticity (is this push earned or forced?)
- Same main event style getting stale
- Predictable booking patterns
- Repetitive show layouts

**Concrete Example (Locked):**
```
You run 20 Dynamite-style shows with same layout:
- Fast opener
- Promo
- Comedy segment
- Main event

Fans slowly lose engagement without you even noticing at first.
```

**Era Sensitivity:**
- Modern fans: Highly critical, suspicious, detect backstage leaks
- Kayfabe era: More forgiving, accept what booker presents

---

### 3.5.8 - Momentum Windows (#196)

📌 **Source:** Vol 1 Extraction #196

**Core Concept:** Workers have optimal push windows that must be captured.

| Window Type | Duration | Miss Penalty |
|-------------|----------|--------------|
| **Debut Pop** | 2-4 weeks | Fades to baseline quickly |
| **Hot Streak** | 1-3 months | Stalls out if not capitalized |
| **Organic Rise** | 6-12 months | Can be extended with right booking |
| **Career Peak** | Variable | May never return if squandered |

**System Warning Example:**
> "Worker X's momentum window is closing. Book them strong or risk permanent ceiling drop."

**Key Insight:** Timing matters as much as quality. A perfectly booked push in a closed window accomplishes nothing.

---

### 3.5.9 - Breakout Performance Triggers (#112)

📌 **Source:** Vol 1 Extraction #112

**Core Concept:** When a match exceeds crowd expectations by a large margin, a hidden "Career Trajectory Shift" can trigger.

**Effects:**
- Baseline skill perception bumps by 5-10 points over next 6 months
- Fan perception rises
- Crowd, locker room, media perception shift
- Skills rise faster for 1-2 years after breakout

**Example (DDP):**
```
DDP: 60 baseline attributes, 80 Potential Cap
Hidden Traits: "High Coachability," "Hard Worker," "Needs Rub"

You book DDP into a semi-main with Macho.
Match overdelivers.

Post-Match Report: "Crowd buzz: 'DDP stepped up to a new level tonight.'"
Career Trajectory quietly shifts.
```

**Key Insight:** "Not because he just 'leveled up' RPG-style. Because he fought, struggled, got the rub, and earned a new level."

---

### 3.5.10 - Surprise Value System (#197)

📌 **Source:** Vol 1 Extraction #197

**How Unexpected Outcomes Affect Engagement:**

| Outcome vs Prediction | Effect |
|----------------------|--------|
| **Expected Win** | Satisfaction, no bonus |
| **Mild Upset** | Excitement boost |
| **Major Upset** | Massive pop if earned, backlash if unearned |
| **Shocking Swerve** | Viral potential, risk of "cheap" label |

**Key:** Surprise must feel logical in hindsight, not random.

---

### 3.5.11 - Cultural Gravity & Style Drift (#115)

📌 **Source:** Vol 1 Extraction #115

**Core Concept:** Promotions can't change style overnight. Cultural inertia resists rapid shifts.

**Examples:**
- NJPW can't become GCW overnight
- WWE can't suddenly book like ECW
- AEW drifting from indie roots creates tension

| Factor | Effect |
|--------|--------|
| **Style Shift Speed** | Gradual = accepted, rapid = rejected |
| **Fan Expectation** | Established fans resist change |
| **Worker Fit** | New hires may clash with culture |
| **Roster Turnover** | New blood enables faster shift |

**Design Implication:** Federation identity should evolve slowly, with mechanics that resist sudden pivots.

---

### 3.5.13 - Tournament Wizard System (#96)

📌 **Source:** Vol 1 Extraction #96

**G1-Style League Wizard Example Setup:**

```
- Choose Tournament Name: [G1 Climax XXVI]
- Format: Blocked Round Robin (2 Blocks of 10)
- Match Style: 30-min Time Limit Matches
- Points System: Win = 2, Draw = 1, Loss = 0
- Fatigue: Moderate
- Injury Risk: Enabled (5%)
- Stakes: Winner challenges for World Heavyweight Title at Wrestle Kingdom
- Seeding: Top 5 Seeds / Random draw for rest
- Crowd Bias: Japan (pops more for Japanese workers, underdog foreigners)
- Optional Surprise: Draw limit chaos (fans get wild for time limit finishes)
```

**Dynamic Match Impacts:**

| Event | Effect |
|-------|--------|
| Worker A wins 5 matches straight in G1 | Slight fatigue (-5% stamina next matches) |
| Worker B wrestles 3 30-minute draws | Heavy fatigue (-15% stamina) |
| Worker C injures Worker D mid-tournament | Replacements, upset brackets, crowd pop |
| Worker D wins anyway, limping | Hero arc, MASSIVE fan love |

**Tournament Momentum Modifier:** "Winning the crowd during tournaments = big boosts even without winning the tourney."

**Smart Booking Assistance:**

| Situation | AI Assistance |
|-----------|---------------|
| Need to rest a star? | Suggests logical match layouts (short matches, DQ finishes) |
| Feud heating up? | Suggests angle or grudge match |
| Tournament is too chalky? | Suggests pulling an upset to keep crowd hot |

**Post-Tournament Fallout Automatically Handled:**
- Tournament winner earns automatic world title match at scheduled PPV
- Tournament MVP (even if they didn't win) gains popularity/momentum
- Tournaments can launch careers or tank reputations organically
- Tag Tournaments strengthen or fracture tag divisions

---

### 3.5.12 - Card Position System (#125)

📌 **Source:** Vol 1 Extraction #125

**Core Concept:** TV vs PPV vs house show dynamics affect expectations and outcomes.

**Show Types:**

| Show Type | Stakes Level | Crowd Expectation |
|-----------|-------------|-------------------|
| **House Show** | Low | Experiment with booking, test chemistry |
| **TV Taping** | Medium | Momentum matters, fan expectations higher |
| **PPV** | High | Career-defining moments, must deliver |

**Card Positions:**

| Position | Role | Worker Expectation |
|----------|------|--------------------|
| **Opener** | Set energy, hook crowd | Rising talent showcase |
| **Undercard** | Build show momentum | Midcard workers |
| **Midcard** | Maintain engagement | Established veterans |
| **Upper Midcard** | Pre-main stakes | Future main eventers |
| **Main Event** | Show climax | Top stars only |

**Key Insight:** "Shoving a midcarder to main events instantly can backfire."

Workers have ceiling expectations based on card history:
- 40 = Solid midcarder
- 70 = Possible regional star
- 90 = Possible world legend

---

## RELATED SYSTEMS (Updated)

- [[Worker_Skills]]: Affects execution quality
- [[Hidden_Personality]]: Affects booking compliance, backstage reactions, Drive/Goal Shift
- [[Tags_System]]: Affects match specialty, promo ability
- [[Popularity_System]]: Affected by booking, affects drawing power
- [[Crowd_Memory]]: Tracks what fans remember
- [[Emotional_Show_Flow]]: Phase 4, pacing/rhythm
- [[Gimmick System/_Gimmick_System_Index|Gimmick System]]: Gimmick Fit Formula
- [[Title System/_Title_System_Index|Title System]]: Title Run Decay
- Morale System: Booking affects worker satisfaction
- Scandal System: Tasteless booking triggers scandals
- [[Injury System/_Injury_System_Index|Injury System]]: Cumulative Fatigue links to injury risk

---

**Document Status:** Phases 1-3.5 fully locked (Vol 1-2), ready for implementation  
**Last Updated:** 2024-12-23  
**Next Review:** Phase 4 (Emotional Show Flow), Phase 5+ concepts
