# HIDDEN PERSONALITY SYSTEM

📛 **NAME:** Hidden Personality System  
🧭 **CATEGORY:** Worker Foundation, Behavioral Simulation  
🔑 **KEYWORDS:** ego, loyalty, morality, traditionalism, paranoia, drive, archetypes, psychology  
📝 **SUMMARY:** Each wrestler carries 6 hidden personality ratings (1-20) that inform their emotional responses, booking compliance, loyalty decisions, and backstage behavior. Workers are assigned 1-2 personality archetypes that set suggested ranges for these traits. Tags define the TARGET of traits like loyalty (what they're loyal to), while ratings define the STRENGTH.

⚙️ **LOGIC OVERVIEW:**
- 6 core hidden ratings drive all behavioral simulation
- Archetypes provide suggested trait ranges but allow individual variation
- Tags modify and specify trait application (e.g., loyalty TARGET)
- Traits evolve slowly over time, with major events causing sharper shifts
- Archetypes are NOT visible to player, revealed through emergent behavior
- Workers can have 1 primary + 1 optional secondary archetype

🔬 **LLM INTEGRATION:** Yes, behind-the-scenes dialogue, promo tone, long-term character memory, decision-making in emergent events

📌 **ORIGIN:** Vol. 1 (foundation), Vol. 3 (12 core archetypes), Vol. 4 (final 6-rating lock, 51+ archetypes with stat ranges)

📎 **CONNECTED SYSTEMS:** Tags System, Turn Engine, Morale System, Contract System, Backstage Politics, Feud Memory, Booking Engine

❓ **OPEN QUESTIONS:**
- How quickly do traits change after major events? (Linear drift vs sharp shifts?)
- Can archetypes mutate over career (e.g., Chronic Underdog → Fading Star)?
- Should there be a "trait history" visible to player after enough time?

✅ **STATUS:** LOCKED (Vol 4 Final)

---

## THE 6 HIDDEN PERSONALITY RATINGS (LOCKED)

**Scale:** 1-20 (Football Manager style)

| Rating | Purpose | Low (1-6) | High (16-20) |
|--------|---------|-----------|--------------|
| **Ego** | Pride, pushback risk, resentment against management or peers | Accepts jobbing, invisible risk | Demands spotlight, may go into business for self |
| **Loyalty** | Emotional attachment to something larger than self | Opportunistic, jumps ship easily | Fierce defender, stays through hardship |
| **Morality** | Ethical standards, scandal threshold, line-crossing willingness | Crosses lines easily, scandal-prone | Strong ethical compass, resists dirty tactics |
| **Traditionalism** | Old-school mindset vs modern innovation acceptance | Embraces change, hybrid styles | Resists evolution, defends "pure" wrestling |
| **Paranoia** | Trust issues, betrayal perception, backstage anxiety | Trusting (exploitable) | Sees burial in every loss, creates tension |
| **Drive** | Ambition, resilience, work ethic, improvement speed | Coasts on talent, retires early | Trains constantly, pushes through injuries |

**CRITICAL DESIGN NOTE:** Hidden Personality Ratings ≠ Tags. Tags = modifiers/targets. Ratings = core psychological engine.

---

## LOYALTY SUBTYPE SYSTEM (LOCKED)

Loyalty is ONE rating. Tags define what they're loyal TO.

| Tag | Loyalty Target |
|-----|----------------|
| Regional Icon | Loyalty to specific territory/city/fanbase |
| Sacred Mask Icon | Loyalty to cultural/lucha heritage |
| Faction Loyalist | Loyalty to stable/faction |
| Promotion Soldier | Loyalty to company |
| Bloodline Defender | Loyalty to family/ancestry (Anoa'i, Casas dynasty) |
| Purist Idealist | Loyalty to philosophy (King's Road, Deathmatch Purity) |
| Charismatic Mercenary | Low loyalty tag, highest bidder wins |

**Simulation Examples:**
- High Loyalty + Regional Icon = refuses to leave Memphis no matter what money offered
- High Loyalty + Sacred Mask Icon = treats mask match as life-or-death, spirals if mask lost
- Low Loyalty + Cult Favorite = jumps promotions chasing buzz with no anchor

---

## PERSONALITY ARCHETYPES

Workers assigned **1 primary + 1 optional secondary** archetype. Ranges allow individuality within archetype soul.

### Vol 3 Core Archetypes (12)

| Archetype | Core Concept | Key Trait Ranges | Inspiration |
|-----------|--------------|------------------|-------------|
| **Ace Complex** | Needs to be the main character | Ego 14-20, Drive 15-20 | Top guys who crumble without spotlight |
| **Chronic Underdog** | Thrives when doubted, struggles when elevated | Ego 6-10, Resilience 14-18 | Daniel Bryan, Mick Foley |
| **Mercenary Soul** | Money/spotlight over loyalty | Loyalty 1-8, Ego 12-18 | Brock Lesnar, Bret Hart (WWF exit) |
| **Loyal Soldier** | System over ambition | Loyalty 16-20, Ego 6-12 | Arn Anderson, Dean Malenko |
| **Ghost Walker** | Quiet, can vanish suddenly | All traits moderate/low except Morality | Bray Wyatt, Jeff Hardy |
| **Bombthrower** | Instigator, court jester | Ego 14-18, Morality 4-10, Traditionalism 2-8 | CM Punk, Roddy Piper |
| **Martyr Spirit** | Sacrifices for greater good | Loyalty 14-18, Drive 12-16, Ego 4-10 | Mick Foley, Dusty Rhodes |
| **Self-Destructive** | Sabotages own success | Morality 3-8, Paranoia 14-20 | Jeff Hardy, Scott Hall |
| **Backstage Politician** | Actively maneuvers for power | Ego 14-20, Paranoia 10-16 | Hulk Hogan, Triple H |
| **Fading Star** | Fears best days are behind them | Ego 12-18, Paranoia 12-18, Drive 8-14 | Ric Flair (late), Sting (TNA) |
| **Innocent Idealist** | Believes in pure wrestling vision | Morality 14-20, Traditionalism 12-18, Paranoia 2-6 | Daniel Bryan, Dean Malenko |
| **Pressure Cooker** | Performs better under chaos | Risk-Taking 14-20, Resilience 14-20 | Steve Austin, Eddie Guerrero |

### Vol 4 Regional/Historical Archetypes

**Batch 1:**

| Archetype | Description | Ego | Loyalty | Morality | Traditionalism | Paranoia | Drive | Risk-Taking | Inspiration |
|-----------|-------------|-----|---------|----------|----------------|----------|-------|-------------|-------------|
| **Territorial Kingpin** | Local legend, resents outsiders, commands regional booking pull | 14-20 | 16-20 (territory) | - | 15-20 | - | - | 2-7 | Jerry Lawler, Wahoo McDaniel, Nick Gulas-era |
| **Lucha Traditionalist** | Mask/ritual devotion, resists hybridization and hardcore | - | 17-20 (tradition) | 14-18 | 18-20 | - | - | 4-8 | Atlantis, El Dandy, Blue Panther, Negro Casas |
| **Deathmatch Devotee** | Pain as art, spiritual hardcore connection | 8-14 | 14-18 (scene) | 4-10 | - | - | - | 17-20 | Jun Kasai, Sick Nick Mondo, Takeda, Matt Tremont |
| **Joshi Firebrand** | Victory through guts, emotional volatility, pushes until cracking | 6-12 | - | 10-18 | - | - | - | 15-20 | Manami Toyota, Akira Hokuto, Mayumi Ozaki, Arisa Nakajima |
| **Outlaw Independent** | Refuses long-term contracts, lives off buzz and fear | 12-18 | 1-6 | - | - | - | 12-18 | 15-20 | Bruiser Brody, Eddie Kingston, Minoru Suzuki, Nick Gage |

**Tags for Batch 1:**
- Territorial Kingpin: Territory Lifer, Disgruntled Veteran, Locker Room Politician
- Lucha Traditionalist: Ritual Purist, Cultural Icon, Sacred Space Defender
- Deathmatch Devotee: Deathmatch Poet, Crimson Specialist, Hardcore Icon
- Joshi Firebrand: Victory Through Guts, Iron-Willed, Fated Survivor
- Outlaw Independent: Freelance Superstar, Chaos Agent, Cult Follower Favorite, Reluctant Icon

**Batch 2:**

| Archetype | Description | Ego | Loyalty | Morality | Traditionalism | Paranoia | Drive |
|-----------|-------------|-----|---------|----------|----------------|----------|-------|
| **King's Road Stoic** | Carries burden of legacy, grim, enduring, awe-inspiring | 8-14 | 16-20 (to ethos) | 12-18 | 16-20 | 6-12 | 18-20 |
| **Joshi Villain Queen** | Charismatic heel, forms factions, manipulates, reigns through intimidation | 16-20 | 8-14 (to faction) | 2-8 | 8-14 | 14-20 | 16-20 |
| **Indie Chaos Goblin** | Thrives on mayhem, viral moments, irony, insanity | 10-18 | 4-10 | 6-14 | 2-8 | 10-18 | 12-18 |
| **International Mercenary** | Globe-trotting, fights for prestige/money/glory, not allegiance | 14-18 | 2-8 | 8-14 | 6-14 | 8-16 | 16-20 |
| **Fragile Genius** | Undeniable brilliance, fragile psychology or crumbling body | 12-18 | 8-14 | 10-18 | 6-12 | 12-20 | 10-16 |

**Tags for Batch 2:**
- King's Road Stoic: King's Road Soldier, Iron-Willed, Burden Bearer, Endurance Icon
- Joshi Villain Queen: Faction Leader, Sadistic Performer, Tragic Queen, Ruthless Strategist
- Indie Chaos Goblin: Cult Favorite, Unpredictable, Meme God, Spotfest Addict
- International Mercenary: World Traveler, Mercenary Icon, Hired Gun, Territory Tourist
- Fragile Genius: Technical Virtuoso, Self-Destructive, Injury Magnet, Flawed Prodigy

**Batch 3:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Self-Mythologizer** | Obsessively crafts own legend, prophetic or delusional | 16-20 | 8-14 | 8-16 | 10-18 | 12-20 | 14-20 | Moderate (collapses if narrative control lost) |
| **Monster Heel** | Dominant big men/women, fear-based booking, emotionally isolated | 10-18 | 6-14 | 4-12 | 10-18 | 8-16 | 14-20 | Low physical, moderate crowd if overexposed |
| **Defiant Soul** | Embodies beauty of struggle, never fully wins or loses | 8-14 | 14-20 | 14-20 | 10-16 | 6-12 | 18-20 | Low |
| **Tragic Innovator** | Revolutionaries who burn bodies/minds/reputations changing the style | 12-18 | 6-12 | 8-16 | 2-8 | 10-16 | 14-18 | High (injuries + industry rejection) |
| **Ruthless Opportunist** | Cutthroat survivors, alliances/ethics disposable | 14-20 | 2-8 | 2-10 | 4-10 | 12-20 | 16-20 | Low (causes others' burnout) |

**Tags for Batch 3:**
- Self-Mythologizer: Self-Created Legend, Myth Weaver, Shoot Interview King, Unreliable Narrator
- Monster Heel: Monster Attraction, Crushing Aura, Fear Projection, Silent Assassin
- Defiant Soul: Never Say Die, Sympathetic Underdog, Beautiful Struggle, Anti-Destiny Warrior
- Tragic Innovator: Evolution Catalyst, Style Destroyer, Doomed Genius, Anti-Traditionalist
- Ruthless Opportunist: Opportunist, Power Chaser, Political Assassin, Golden Rat

**Batch 4:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Charismatic Con Artist** | Lives on wit, charm, deception | 14-20 | 4-10 | 2-10 | 6-12 | 10-18 | 12-18 | Moderate (collapses if charm fades) |
| **Brawling Everyman** | Relatable fighters, blue-collar beloved | 8-14 | 14-20 | 12-20 | 10-16 | 6-12 | 16-20 | Low |
| **Cerebral Technician** | Cold, methodical technical masters | 10-16 | 8-14 | 10-16 | 12-18 | 6-12 | 14-20 | Low |

**Tags for Batch 4:**
- Charismatic Con Artist: Smooth Operator, Heat Seeker, Mic Wizard, Snake in the Grass
- Brawling Everyman: Working Class Hero, Rough & Ready, Blue Collar Icon, Crowd's Champion
- Detached Strategist: Mastermind, Mind Over Body, Strategic Coldness, Psychological Edge
- Daredevil Risk-Taker: Spot Monkey, Adrenaline Addict, Crash and Burn Hero, Highlight Reel Daredevil
- Wounded Philosopher: Veteran Survivor, Broken Idealist, Redemption Seeker, Wisdom Over Victory

**Batch 4 (Continued):**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Detached Strategist** | Masters of control, patience, mental warfare; view wrestling as pure calculation | 10-16 | 8-14 | 10-16 | 12-18 | 6-14 | 14-20 | Low-Moderate |
| **Daredevil Risk-Taker** | Adrenaline junkies defying gravity and sanity; careers short but spectacular | 10-16 | 8-14 | 6-14 | 4-10 | 8-16 | 14-20 | High (physical) |
| **Wounded Philosopher** | Veterans shaped by trauma, loss, reflection; seek meaning beyond wins | 6-12 | 14-20 | 14-20 | 8-16 | 8-14 | 12-18 | Moderate |

**Batch 5:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Cold-Blooded Professional** | Ultimate businessperson, no emotion or politics, wrestles for money | 8-14 | 4-10 | 6-12 | 10-16 | 6-12 | 16-20 | Low |
| **Franchise Workhorse** | Consistently excellent bedrock, rarely centerpiece, holds companies together | 6-12 | 16-20 | 14-20 | 12-18 | 4-10 | 16-20 | Moderate |
| **Boom or Bust Star** | Transcendent when working, spectacular flameouts when not | 16-20 | 4-10 | 6-14 | 4-12 | 12-20 | 12-18 | High |
| **Cult Follower Favorite** | Not mainstream, inspires fierce devotion among hardcore fans | 8-16 | 12-18 | 10-18 | 6-12 | 8-16 | 14-20 | Moderate-High |
| **Cosmic Wanderer** | Mysterious souls drifting between styles/promotions, treated like myths | 10-16 | 4-10 | 10-18 | 6-14 | 10-18 | 12-18 | Moderate |

**Tags for Batch 5:**
- Cold-Blooded Professional: Business-First, Mercenary Professional, Locker Room Ghost, Match Assassin
- Franchise Workhorse: Foundation Piece, Underrated Ace, Quiet Veteran, Locker Room Backbone
- Boom or Bust Star: Volatile Star, Human Firework, Rise and Fall Legend, Self-Saboteur
- Cult Follower Favorite: Cult Legend, Indie Icon, Anti-Mainstream Hero, Loyalty Magnet
- Cosmic Wanderer: Drifter Icon, Mystic Loner, Shaman of the Ring, Dream Match Specialist

**Batch 6:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Glory-Obsessed Hero** | Lives to chase transcendence, cares about legacy-defining victories | 14-20 | 8-14 | 10-18 | 8-16 | 6-12 | 16-20 | Moderate |
| **Nomadic Survivor** | Quiet, hardened souls enduring across federations without belonging | 8-14 | 4-10 | 10-16 | 6-14 | 10-18 | 14-18 | Low-Moderate |
| **Locker Room Saint** | Beloved behind curtain, pillars of support and mentorship | 4-10 | 18-20 | 16-20 | 12-18 | 2-8 | 16-20 | Moderate |
| **Paranoid Schemer** | Sees enemies everywhere, career defined by distrust and politicking | 12-18 | 4-10 | 4-10 | 8-14 | 18-20 | 14-18 | Moderate-High |
| **Fallen Idol** | Once beloved, now broken by scandal/injuries/betrayal | 8-16 | 8-16 | 6-14 | 8-16 | 10-18 | 6-14 | High |

**Tags for Batch 6:**
- Glory-Obsessed Hero: Moment Maker, Big Match Hero, Glory Seeker, Legacy Chaser
- Nomadic Survivor: Survivor of Eras, Lonely Veteran, Traveler Spirit, Federation Drifter
- Locker Room Saint: Morale Anchor, Mentor Spirit, Respected Veteran, Locker Room Anchor
- Paranoid Schemer: Locker Room Politician, Invisible Knife Fighter, Plotter in Shadows, Trust No One
- Fallen Idol: Tragic Legend, Scandal Magnet, Redemption Arc Candidate, Forgotten Hero

**Batch 7:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Toxic Messiah** | Idealists turned bitter, still charismatic but corroded by betrayal | 14-20 | 6-12 | 10-18 | 4-12 | 14-20 | 16-20 | High |
| **Mercenary Entertainer** | Will say/do anything to stay relevant, masters of adapting | 12-18 | 2-8 | 4-12 | 6-14 | 10-18 | 14-20 | Moderate |
| **Fate-Defying Underdog** | Make careers surviving impossible odds, embody hope | 6-12 | 14-20 | 14-20 | 10-16 | 4-10 | 18-20 | Low |
| **Silent Guardian** | Protect others, loyal enforcers, never seek glory | 2-8 | 16-20 | 12-20 | 8-16 | 4-10 | 14-20 | Moderate |
| **Unmoored Dreamer** | Artists lost at sea, imaginative and eccentric, emotionally volatile | 8-16 | 6-14 | 8-16 | 4-10 | 10-18 | 10-16 | High |

**Tags for Batch 7:**
- Toxic Messiah: Bitter Prophet, Broken Idealist, Shooter Mentality, Cult of Personality
- Mercenary Entertainer: Promo Chameleon, Buzz Chaser, Opportunist Talker, Spotlight Surfer
- Fate-Defying Underdog: Eternal Underdog, Miracle Worker, Sympathy Magnet, Hope-Bringer
- Silent Guardian: Bodyguard Archetype, Shield Bearer, Unsung Hero, Locker Room Defender
- Unmoored Dreamer: Dreamer Without Anchor, Eccentric Icon, Spirit Walker, Unstable Genius

**Special Batch (Emotional Archetypes):**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Prima Donna** | Sky-high expectations, glass-jawed commitment, walks if not anointed | 16-20 | 4-10 | 6-14 | 8-14 | 10-16 | 4-10 | **Very High** |
| **Carny Operator** | Wrestling as grift, loyalty only to hustle | 10-18 | 4-10 | 2-8 | 6-14 | 12-20 | 12-18 | Low |
| **Tyrant of Tradition** | Bloody-handed defender of old ways, feared and revered | 16-20 | 10-16 | 4-10 | 18-20 | 14-20 | 16-20 | Low (kills promotion evolution) |
| **Overzealous Believer** | Views wrestling as sacred art, rigid pride, self-sabotages | 14-20 | 10-16 | 10-18 | 16-20 | 8-14 | 16-20 | Moderate-High |
| **Ticking Timebomb** | Walking chaos, brilliance and disaster side by side | 12-18 | 4-12 | 2-8 | 4-12 | 12-20 | 10-16 | **Extremely High** |

**Tags for Special Batch:**
- Prima Donna: Golden Mirage, Fragile King, Flash of Greatness, Walkout Artist
- Carny Operator: Grifter Supreme, Side Hustler, Con Artist's Apprentice, Smiling Shark
- Tyrant of Tradition: Tradition's Last Bastion, Iron Fist Booker, Backstage Despot, Blood and Leather Guardian
- Overzealous Believer: Sacred Craftsman, True Believer, Wrestling Ascetic, Stone Temple Disciple
- Ticking Timebomb: Locker Room Bomb, Chaos Incarnate, Wildfire Talent, Tragedy Clock, Criminal Risk (common), Reckless Behavior, Controversial Outbursts

**Batch 9:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Corporate Climber** | Sees wrestling as career ladder, angling for office power | 12-18 | 6-14 | 6-12 | 10-16 | 8-14 | 16-20 | Low |
| **Eccentric Mentor** | Weird, unpredictable but brilliant teachers | 8-14 | 14-20 | 10-18 | 8-16 | 6-12 | 14-20 | Low |
| **Terminal Nomad** | Destined to drift forever, no company or home | 6-14 | 2-8 | 8-16 | 4-12 | 8-14 | 10-16 | Moderate |
| **Oblivious Narcissist** | Blissfully unaware of how they come across | 18-20 | 6-12 | 8-16 | 8-16 | 6-14 | 14-20 | Low (others burn out) |
| **Redemption Seeker** | Haunted by past failures, fights for meaning | 8-14 | 14-20 | 14-20 | 8-16 | 6-12 | 14-20 | Moderate |

**Tags for Batch 9:**
- Corporate Climber: Company Man, Future Booker, Career Politician, Gold Watch Chaser
- Eccentric Mentor: Unorthodox Teacher, Mad Sage, Cosmic Coach, Spirit Guide
- Terminal Nomad: Federation Vagabond, No Fixed Home, Eternal Drifter, Beloved Nowhere
- Oblivious Narcissist: Unaware Heel, Self-Love Warrior, Cringe Icon, Locker Room Repellant
- Redemption Seeker: Fallen Hero, Redemption Arc, Soul Survivor, The Long Road Back

**Batch 10:**

| Archetype | Description | Ego | Loyalty | Morality | Trad | Paranoia | Drive | Burnout Risk |
|-----------|-------------|-----|---------|----------|------|----------|-------|-------------|
| **Fading Megastar** | Once-in-a-generation talents whose aura is slipping | 14-20 | 8-16 | 8-16 | 10-16 | 10-18 | 10-18 | High |
| **Privileged Legacy** | Born into business with advantages | 10-18 | 8-16 | 8-16 | 10-18 | 6-12 | 8-18 | Moderate |
| **Brutal Realist** | Sees business through unfinching survival lens | 10-16 | 6-14 | 8-14 | 8-16 | 10-16 | 14-20 | Low |
| **Ambition-Consumed Prodigy** | Youthful phenoms obsessed with reaching top fast | 14-20 | 4-10 | 6-12 | 4-12 | 10-16 | 18-20 | **Extremely High** |
| **Professional Lifer** | Just loves wrestling, willing to evolve and adapt | 6-14 | 14-20 | 12-20 | 8-16 | 4-10 | 16-20 | Low |

**Tags for Batch 10:**
- Fading Megastar: Fading Icon, Twilight Warrior, Bitter Legacy, Golden Ghost
- Privileged Legacy: Bloodline Heir, Entitled Hopeful, Dynastic Weight, Inherited Spotlight
- Brutal Realist: Hard Truth Dealer, Cold Eye of the Business, Cynical Survivor, Locker Room Weather-Vane
- Ambition-Consumed Prodigy: Chosen One, Future Ace (or Future Tragedy), Burnout Kid, Spotlight Addict
- Professional Lifer: Wrestling is Home, Generational Chameleon, Silent Legacy, Eternal Journeyman

**✅ 50 ARCHETYPES COMPLETE**

---

## ARCHETYPE COMPOSITION METHOD

**Locked Design Rule (Vol 4):**

For well-known, layered workers (especially major stars), worker profiles are built by **blending multiple Hidden Personality Archetypes**, pulling ranges and tags proportionally based on real-life emotional character.

- **Primary Archetype** = dominant weighting (60-70%)
- **Secondary Archetype(s)** = influencing weighting (30-40%)
- **Additional Tags** = spice in the final flavor

### Example: Hulk Hogan

| Trait | Primary Influence | Secondary Influence | Final Range |
|-------|-------------------|---------------------|-------------|
| Ego | Self-Mythologizer (high) | Paranoid Schemer (high) | 18-20 |
| Loyalty | Self-Mythologizer (low-mod) | Ruthless Opportunist (low) | 4-8 |
| Morality | Self-Mythologizer (middle) | Paranoid Schemer (low) | 4-10 |
| Traditionalism | Mythologizer (mod-high) | Opportunist (moderate) | 12-18 |
| Paranoia | Paranoid Schemer (very high) | Mythologizer (high) | 16-20 |
| Drive | Self-Mythologizer (high) | Opportunist (high) | 16-20 |

**Tags:** Self-Created Legend, Legacy Manipulator, Backstage Politician, Paranoid Politicker, Face of a Generation

### Reference: Major Personalities Mapped

| Real-World Figure | Primary Archetype | Secondary Archetype(s) |
|-------------------|-------------------|------------------------|
| Hulk Hogan | Self-Mythologizer | Boom or Bust Star (later) |
| Ric Flair (young) | Charismatic Con Artist | Mercenary Entertainer, Prima Donna |
| Ric Flair (old) | Fading Megastar | Self-Mythologizer |
| Bret Hart | King's Road Stoic | Glory-Obsessed Hero |
| Shawn Michaels (Prime) | Boom or Bust Star | Mercenary Entertainer |
| Steve Austin | Brawling Everyman | Defiant Soul |
| The Rock | Mercenary Entertainer | Cult Follower Favorite |
| CM Punk | Toxic Messiah | Self-Mythologizer |
| John Cena | Franchise Workhorse | Glory-Obsessed Hero |
| Mitsuharu Misawa | King's Road Stoic | Locker Room Saint |
| Toshiaki Kawada | Defiant Soul | Fate-Defying Underdog |
| Antonio Inoki | Self-Mythologizer | Cosmic Wanderer, Tyrant of Tradition |
| Shinya Hashimoto | King's Road Stoic | Defiant Soul |
| Vader | Monster Heel | (single archetype) |
| Dump Matsumoto | Joshi Villain Queen | (single archetype) |
| Minoru Suzuki | Outlaw Independent | Monster Heel |
| Terry Funk | Cosmic Wanderer | Tragic Innovator |
| Mick Foley | Defiant Soul | Fragile Genius |
| Vince McMahon (young) | Self-Mythologizer | Corporate Climber |
| Vince McMahon (old) | Tyrant of Tradition | Self-Mythologizer |
| Pat Patterson | Eccentric Mentor | Locker Room Anchor, Carny Operator |
| Ricky Steamboat | Defiant Soul | Professional Lifer + Family First tag |
| Dusty Rhodes | Self-Mythologizer | Toxic Messiah, Fading Megastar |
| Dustin Rhodes | Redemption Seeker | Fate-Defying Underdog |

---

## ARCHETYPE SPECIAL MECHANICS

### Unique Quirks by Archetype

| Archetype | Unique Mechanic |
|-----------|-----------------|
| Lucha Traditionalist | Causes backstage unrest if booked on mixed-style cards too frequently |
| Deathmatch Devotee | Can enter "Sacrificial Mode" late in career (boosts crowd memory at cost of long-term health) |
| Joshi Firebrand | Near-unrivaled "Match Memory" score in emotionally brutal bouts |
| Outlaw Independent | Prone to jumping ship or going into business for themselves if disrespected |
| Fragile Genius | Burnout risk baked in (moderate: career collapses if narrative control lost) |

### Burnout Risk by Archetype

| Archetype | Burnout Risk | Notes |
|-----------|--------------|-------|
| King's Road Stoic | Low | But if cracked, leads to catastrophic crash |
| Joshi Villain Queen | Low-Moderate | Stable unless faction collapses |
| Indie Chaos Goblin | High | Emotional burnout from crowd turn, self-destruction |
| International Mercenary | Low | Adaptable, but may cause locker room burnout in others |
| Fragile Genius | High | Both physical (injuries) and mental (industry rejection) |

---

## BEHAVIORAL TRIGGERS

### High Ego (16-20)
- Demands main event booking
- Resists jobs to younger talent
- May refuse to put others over cleanly
- High risk of "going into business for themselves"

### Low Ego (1-6)
- Willing to job frequently
- Accepts midcard booking gracefully
- Good for putting others over
- Risk: becomes invisible, loses crowd connection

### High Loyalty (16-20)
- Stays with promotion through rough patches
- Defends promotion publicly
- Mentors younger talent
- Low exodus risk even with bad booking

### Low Loyalty (1-6)
- Jumps ship for better offers
- Leaks backstage info
- High exodus risk
- May form factions to gain leverage

### High Paranoia (16-20)
- Sees every loss as political burial
- Creates locker room tension
- Demands creative control clauses
- May refuse to work with certain opponents

### High Drive (16-20)
- Trains constantly, skills improve faster
- Pushes through injuries (good and bad)
- Attempts comebacks even when past prime
- High burnout risk if overbooked

---

## TRAIT EVOLUTION TRIGGERS

| Event | Trait Changes |
|-------|---------------|
| Title Win | Ego +2-4, Drive +1-3, Paranoia -1-2 |
| Long-term Injury | Drive -2-4, Paranoia +2-4, Resilience tested |
| Betrayal (turned on) | Loyalty -3-6, Paranoia +4-8, Morality may shift |
| Extended Burial | Ego -2-4, Paranoia +3-6, Drive varies by archetype |
| Contract Dispute | Loyalty -2-5, Ego +1-3, may trigger archetype shift |
| Mentor Death/Retirement | Traditionalism +2-4, Drive varies |
| Scandal | Morality -2-6, Paranoia +3-8, Loyalty tested |

---

## IMPLEMENTATION NOTES

### Data Structure
```json
{
  "worker_id": "WORK_12345",
  "hidden_personality": {
    "ratings": {
      "ego": 16,
      "loyalty": 8,
      "morality": 14,
      "traditionalism": 12,
      "paranoia": 11,
      "drive": 18
    },
    "archetypes": {
      "primary": "Pressure Cooker",
      "secondary": "Mercenary Soul"
    },
    "loyalty_targets": ["promotion", "faction"],
    "trait_history": [
      {"date": "2024-03", "trait": "ego", "change": +3, "trigger": "title_win"}
    ]
  }
}
```

### Trait Change Frequency
- **Slow drift:** ±1 per year naturally
- **Event-triggered:** Immediate shifts based on career moments
- **Archetype mutation:** Rare, only after multiple aligned trait shifts

---

## RELATED SYSTEMS

- [[Worker_Skills_System]] - Visible abilities
- [[Tags_System]] - Flavor/specialization, loyalty targets
- [[Turn_Engine]] - Betrayal mechanics
- [[Morale_System]] - Booking satisfaction
- [[Backstage_Politics]] - Power struggles
- [[Contract_System]] - Negotiations, exodus

---

## VERSION HISTORY

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Vol 1 | Foundation concept |
| 2.0 | Vol 3 | 12 core archetypes locked |
| 3.0 | Vol 4 | **FINAL: 6 ratings locked**, 51+ archetypes with stat ranges, loyalty subtype via tags |

---

**Document Status:** LOCKED (Vol 4 Final)  
**Next Review:** Extract remaining archetypes from Vol 4 (Batches 3-8)
