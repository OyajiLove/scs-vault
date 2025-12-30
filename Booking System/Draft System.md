# DRAFT SYSTEM

📛 **NAME:** Draft System
🧭 **CATEGORY:** Game Setup / Roster Management
🔑 **KEYWORDS:** draft, roster, war room, snake draft, auction, free agency, all-time, fantasy
📝 **SUMMARY:**

The Draft System governs how players acquire workers at game start and manage rosters over time. Multiple draft formats support different playstyles, from competitive snake drafts to fantasy all-time peak modes. The War Room AI assistant helps players make informed picks during timed selections.

⚙️ **LOGIC OVERVIEW:**

- Multiple draft formats (snake, auction, territorial, free agency)
- War Room AI suggests picks based on player prompts
- Roster limits and management mechanics
- All-Time Peak mode for fantasy scenarios
- Handicap system adjusts AI assistance based on player preference

🔬 **LLM INTEGRATION:** High (War Room suggestions, pick analysis)

📌 **ORIGIN:** Vol 1 Extraction #114, #145, #229

📎 **CONNECTED SYSTEMS:**
- [[Contract System/_Contract System Index|Contract System]] - Post-draft contracts
- [[Scouting System]] - Information available during draft
- [[Era System]] - Era affects available workers
- [[Financial System]] - Auction budgets

❓ **OPEN QUESTIONS:**
- Exact War Room prompt processing
- Draft timer durations
- Roster limit numbers by promotion size
- Trade mechanics post-draft

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #114, #145, #229 | 🔒 LOCKED (concept) |

---

## DRAFT FORMATS (#145)

| Format | Description | Best For |
|--------|-------------|----------|
| **Snake Draft** | Alternating picks, order reverses each round | Balanced competitive play |
| **Auction** | Budget-based bidding on workers | Strategic depth, varied rosters |
| **Territorial** | Geographic restrictions on picks | Historical accuracy |
| **Free Agency** | Open market, simultaneous offers | Multiplayer competition |
| **Predetermined** | Start with historical roster | Scenario play |

### Snake Draft Details

| Aspect | Mechanic |
|--------|----------|
| **Order** | Determined by random draw or scenario |
| **Rounds** | Configurable (typically 15-30) |
| **Timer** | Per-pick time limit (30s-5min) |
| **Reversal** | Order flips each round |

### Auction Draft Details

| Aspect | Mechanic |
|--------|----------|
| **Budget** | Starting money pool (equal for all) |
| **Nominations** | Players take turns nominating workers |
| **Bidding** | Open ascending bid until no challengers |
| **Minimum Bid** | $1 or configurable floor |
| **Roster Fill** | Must fill roster, may get bargains late |

### Territorial Draft Details

| Aspect | Mechanic |
|--------|----------|
| **Regions** | Players assigned or choose territories |
| **Local Priority** | First pick on workers from your region |
| **Imports** | Limited slots for out-of-region workers |
| **Historical** | Based on actual territorial boundaries |

---

## WAR ROOM INTERFACE (#114)

### Core Concept

AI assistant during timed drafts that suggests picks based on player prompts.

### How It Works

1. **Type Short Prompts:** "great heels for surfer sting", "top young tag teams 1987"
2. **War Room Suggests:** 5-15 relevant picks based on query
3. **Quick View:** Click to open profile (stats, personality, history, injury risks)
4. **Make Pick:** Informed decision without panicking

### Example Prompts

| Prompt | War Room Returns |
|--------|------------------|
| "best brawlers available" | Top brawlers by skill, filtered by undrafted |
| "cheap monster heels" | Monster heels with low contract demands |
| "technical workers Japan" | Japanese technicians available |
| "future main eventers under 25" | Young workers with high potential |
| "veterans to mentor rookies" | Workers with Veteran Leader tag |

### War Room Features

| Feature | Description |
|---------|-------------|
| **Style Awareness** | Knows your promotion style, suggests culturally appropriate picks |
| **Quick Filters** | Top Charisma, Best Brawlers, Most Marketable, etc. |
| **Personality Warnings** | "Mercenary" (may jump ship), "Headcase" (locker room drama) |
| **Era Sensitivity** | Suggestions appropriate to game era |
| **Contract Estimates** | Rough salary expectations |

### Handicap System

| Setting | Description |
|---------|-------------|
| **Infinite Uses** | War Room always available (casual/new fans) |
| **Limited Uses** (1, 3, 5) | Strategic resource for experienced players |
| **Zero Uses** | "No Training Wheels Mode" for hardcore players |

---

## ROSTER MANAGEMENT (#145)

### Roster Limits

| Promotion Size | Active Roster | Developmental |
|----------------|---------------|---------------|
| **Small Indie** | 15-25 | 0-5 |
| **Regional** | 25-40 | 5-10 |
| **National** | 40-60 | 10-20 |
| **Major** | 60-80+ | 20-30 |

### Roster Categories

| Category | Description |
|----------|-------------|
| **Active** | Main roster, appears on shows |
| **Developmental** | Training territory, not on main shows |
| **Injured Reserve** | Out with injury, doesn't count against active limit |
| **Legends/Part-Time** | Special appearances only |

### Post-Draft Management

| Mechanic | Description |
|----------|-------------|
| **Loans** | Temporarily send workers to other promotions |
| **Trades** | Exchange workers between promotions |
| **Waiver Wire** | Claim released workers |
| **Free Agent Signing** | Sign unattached workers |
| **Releases** | Cut workers from roster |

---

## ALL-TIME PEAK DRAFT MODE (#229)

### Core Concept

Fantasy draft where every historical worker is available at their absolute peak form.

### Key Features

| Feature | Description |
|---------|-------------|
| **Era Fusion** | 70s bruisers vs. 2020s hybrid monsters in same pool |
| **Peak Versions** | Each worker at their career best |
| **Fantasy Feuds** | Dream matchups across eras |
| **Complete Packages** | Tag teams and managers at peak included |

### Peak Version Examples

| Worker | Peak Version | Year |
|--------|--------------|------|
| Ric Flair | '89 | 1989 |
| Bret Hart | '97 | 1997 |
| Kenta Kobashi | '03 | 2003 |
| The Rock | '00 | 2000 |
| Kenny Omega | '18 | 2018 |
| Road Warriors | '86 | 1986 |

### Optional House Rules

| Rule | Description |
|------|-------------|
| **Promotion Limit** | "Only 5 workers per real-life promotion" |
| **Decade Diversity** | "Must draft at least 1 worker per decade" |
| **Style Balance** | "Maximum 3 of any single archetype" |
| **Custom Restrictions** | Player-defined rules |

### Booking Challenges

All-time rosters create unique challenges:

| Challenge | Description |
|-----------|-------------|
| **Everyone's a Star** | Balancing main event expectations |
| **Ego Management** | Multiple legends with high ego stats |
| **Style Clashes** | Era-appropriate psychology varies |
| **Money Demands** | Peak workers expect peak pay |

---

## DRAFT UI FLOW

### Pre-Draft

1. **Format Selection:** Choose draft type
2. **Settings:** Configure rounds, timer, roster limits
3. **Era/Pool Selection:** Historical, all-time, custom
4. **Player Assignment:** Human vs. AI, draft order

### During Draft

1. **Timer Display:** Countdown per pick
2. **Available Pool:** Searchable, filterable list
3. **War Room Panel:** AI suggestions
4. **Drafted Rosters:** All players' picks visible
5. **Quick Compare:** Side-by-side worker stats

### Post-Draft

1. **Roster Review:** Full team overview
2. **Gap Analysis:** "You're weak at tag teams"
3. **Contract Setup:** Finalize terms with drafted workers
4. **Game Start:** Begin booking

---

## IMPLEMENTATION NOTES

### Draft State Structure

```json
{
  "draft_id": "draft_001",
  "format": "snake",
  "settings": {
    "rounds": 20,
    "timer_seconds": 120,
    "war_room_uses": 5
  },
  "participants": [
    {
      "player_id": "player_001",
      "is_human": true,
      "draft_position": 1,
      "roster": [],
      "war_room_remaining": 5
    }
  ],
  "available_pool": ["worker_001", "worker_002"],
  "current_round": 1,
  "current_pick": 1,
  "pick_order": [1, 2, 3, 4, 4, 3, 2, 1],
  "status": "in_progress"
}
```

### War Room Query Structure

```json
{
  "query": "great heels for surfer sting",
  "context": {
    "player_promotion_style": "character_driven",
    "era": "national_expansion",
    "existing_roster": ["worker_001", "worker_002"],
    "roster_gaps": ["heel_main_event", "tag_team"]
  },
  "results": [
    {
      "worker_id": "worker_050",
      "name": "Ted DiBiase",
      "match_score": 0.92,
      "reasoning": "Top heel, great talker, can work long programs"
    }
  ]
}
```

---

## CONNECTED MECHANICS

- [[Contract System/_Contract System Index|Contract System]] - Drafted workers need contracts
- [[Scouting System]] - Draft info limited by scouting in some modes
- [[Era System]] - Era affects pool and expectations
- [[Financial System]] - Auction budgets, salary implications

---

## OPEN QUESTIONS

- [ ] AI draft behavior personality types
- [ ] Draft pick trade mechanics
- [ ] Compensatory picks for imbalanced trades
- [ ] Historical draft recreation mode
- [ ] CPU auto-draft quality settings

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define War Room AI prompt processing
