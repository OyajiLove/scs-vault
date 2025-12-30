# Scouting System

📛 **SYSTEM ID:** SCOUT-001
🧭 **CATEGORY:** Talent Acquisition / Information
🔑 **KEYWORDS:** scouting, fog of war, talent evaluation, discovery, tape trading, foreign talent, hidden gems
📝 **SUMMARY:** 

The Scouting System governs how promotions discover, evaluate, and recruit talent. In an era-sensitive fog of war model, the player's knowledge of workers depends on their fame, regional exposure, and dedicated scouting efforts. Scouts can be deployed to specific territories or tasked with finding specific archetypes. The system makes talent discovery feel like excavation, not shopping.

⚙️ **LOGIC OVERVIEW:**
- Workers exist in "fog" until discovered through exposure or scouting
- Era determines baseline information availability (pre-internet vs. post-internet)
- Scout skill affects accuracy and speed of evaluation
- Big companies can afford full-time scouts; small promotions rely on tape trading and word of mouth
- Discovery should feel exciting but not require grinding

🔬 **LLM INTEGRATION:** Medium (scout report generation, worker assessment flavor text)

📌 **ORIGIN:** Vol 1 Extraction #93, #169

📎 **CONNECTED SYSTEMS:** 
- [[Popularity_System|Popularity System]] - Fame determines baseline visibility
- [[Territory System/_Territory System Index|Territory System]] - Regional focus for scouting
- [[Contract System/_Contract System Index|Contract System]] - Poaching detected workers
- [[Hidden_Personality|Hidden Personality]] - Hidden traits revealed through full scouting

❓ **OPEN QUESTIONS:**
- Scout hiring costs and salary structure
- Scouting mission duration formulas
- Hidden gem discovery probability
- False positive rate for scout assessments

✅ **STATUS:** Locked (Concept), Formulas Open

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #93, #169 | 🔒 LOCKED (concept) |

---

## CORE MECHANICS

### Fog of War Model (#93)

Workers exist on a visibility spectrum based on exposure:

| Knowledge Level | Information Available |
|-----------------|----------------------|
| **Unknown** | Age, height, weight, name only |
| **Basic Knowledge** | General look, rough role ("brawler," "high flyer"), country of origin |
| **Full Scouting** | All stats, personality traits, hidden potential, contract status |

**Key Principle:** "The more famous a wrestler is (TV, title wins, major shows), the more automatic data you get."

### Era-Sensitive Information Availability (#93)

| Era | Baseline Visibility | Scouting Requirement |
|-----|--------------------|--------------------|
| **Pre-90s** | International/regional talent hidden under heavy fog | Must scout or watch tapes manually |
| **Post-Internet** | More footage available, baseline info auto-unlocked | Deeper stats still need real scouting |
| **Modern (2010s+)** | Most workers have social media presence | Hidden personality still requires evaluation |

**Examples:**
- 1987 Hulk Hogan: Full exposure (everyone knows everything)
- 1987 Shawn Michaels: Needs scouting unless you catch him mid-breakout
- 2025 indie darling: Basic exposure through social media, full stats need scouting

---

## EXPOSURE MODEL (#93)

### Automatic Exposure Triggers

| Trigger | Knowledge Gained |
|---------|-----------------|
| **National TV appearance** | Basic Knowledge minimum |
| **Title win in major promotion** | Full exposure for that promotion's audience |
| **Main event of major PPV** | Near-full exposure nationally |
| **Viral moment** (modern era) | Global basic exposure |
| **Long territorial reign** | Regional full exposure |

### Exposure Decay

Workers can fade from public awareness:
- Years of inactivity reduce exposure
- Regional stars unknown outside their territory
- Era changes reset some exposure (1980s star unknown to 2020s fans)

---

## SCOUT ASSIGNMENT SYSTEM (#93, #169)

### Scout Types

| Type | Cost | Speed | Accuracy |
|------|------|-------|----------|
| **Full-Time Scout** | High salary | Fast | High |
| **Part-Time/Consultant** | Per-project fee | Medium | Medium |
| **Tape Trader Network** | Minimal | Slow | Variable |
| **Personal Connections** | Free | Immediate | Limited scope |

### Scouting Missions

Big companies hire full-time scouts who can be deployed to:

| Target | Description |
|--------|-------------|
| **Specific Territories** | "Scout the Memphis territory" |
| **Entire Regions** | "Cover the Midwest indie scene" |
| **Talent Archetypes** | "Find me a cheap monster heel" |
| **Specific Workers** | "Get full report on this guy I saw on tape" |

**Mission Examples:**
- "Find me a hot high flyer"
- "Scout Japanese junior heavyweights"
- "Find me a future ace"
- "Report on all available heels in the Southeast"

### Scout Skill System (#169)

Bookers, promoters, and scouts have "Talent Evaluation" skills:

| Skill Type | Effect |
|------------|--------|
| **Tape Trader Mentality** (Tony Khan type) | Big boost to raw knowledge of foreign/indie talent |
| **Myopic/Old School** (early Vince type) | Poor foreign or indie knowledge |
| **Eye for Talent** | More accurate assessments |
| **Hidden Gem Finder** | Better at identifying undervalued workers |
| **Physical Obsessed** | Overvalues look, undervalues work rate |

**Higher Skill =**
- More accurate stat assessments
- Faster scout reports
- Better hidden gem detection
- Lower false positive rate

---

## DISCOVERY FLOW (#93)

The system should feel exciting but smooth:

1. **Set scouting mission**
   - Choose target (territory, region, or archetype)
   - Assign scout(s)
   - Set duration

2. **Get notified**
   - "Scout Report Complete: 3 Potential Main Event Heels Found in Southeast USA"
   - Notification appears, no spam

3. **Review player cards**
   - Click into report
   - See discovered workers with available info
   - Decide whether to pursue

**Design Goal:** "You don't need to click 500 times. You set a scouting mission and then get notified."

---

## SCOUTING REPORT FORMAT

### Report Contents

| Section | Information |
|---------|-------------|
| **Overview** | Worker name, age, current promotion, contract status |
| **Physical** | Height, weight, look assessment |
| **In-Ring** | Estimated skill levels, style tags |
| **Personality** | Revealed traits (full scouting only) |
| **Potential** | Scout's assessment of ceiling |
| **Concerns** | Injury history, attitude problems, baggage |
| **Recommendation** | Scout's hiring advice |

### Scout Accuracy

Reports are estimates, not perfect information:
- Low-skill scout: ±15% on stat estimates
- High-skill scout: ±5% on stat estimates
- Hidden personality traits: May miss 30-50% even with full scouting
- Hidden potential: Always somewhat uncertain

---

## TAPE TRADING MECHANICS (#93, #169)

### Pre-Internet Era

Tape trading networks provide alternative to professional scouting:

| Method | Speed | Accuracy | Cost |
|--------|-------|----------|------|
| **Personal collection** | Immediate | High (for owned tapes) | Initial investment |
| **Trade network** | Weeks | Variable | Tapes as currency |
| **Japanese tapes** | Months | Good quality | Import costs |
| **British tapes** | Months | Good quality | Import costs |
| **Lucha tapes** | Variable | Quality varies | Connection-dependent |

### Tape Trader Mentality Tag

Workers or bookers with this tag:
- Know about foreign talent before mainstream awareness
- Can provide scouting intel without formal mission
- Network provides leads on hidden gems

**Examples:** Tony Khan (modern), Jim Cornette (historical knowledge), Paul Heyman (ECW era)

---

## CONNECTED MECHANICS

### With Popularity System
- High national popularity = automatic full exposure
- Regional popularity = exposed in that region only
- Zero popularity = requires active scouting

### With Contract System
- Scouted workers can be approached for contract talks
- Contract status revealed through scouting
- Poaching negotiations require knowing the worker

### With Hidden Personality
- Surface traits visible at Basic Knowledge
- Deep traits (Ego, Drive, Loyalty) require Full Scouting
- Some traits only revealed through working relationship

### With Territory System
- Territorial scouts have regional expertise
- Cross-territory scouting costs more
- Foreign territories harder to scout (language, access)

---

## IMPLEMENTATION NOTES

### Scout Data Structure

```json
{
  "scout_id": "scout_001",
  "name": "Jim Ross",
  "talent_evaluation_skill": 85,
  "specialties": ["American_South", "technical_workers"],
  "biases": {
    "overvalues": ["look", "size"],
    "undervalues": ["foreign_style"]
  },
  "tape_trader_mentality": false,
  "current_assignment": {
    "type": "region",
    "target": "Southeast_USA",
    "archetype_filter": "monster_heel",
    "start_date": "1985-03-01",
    "expected_completion": "1985-04-15"
  }
}
```

### Scouting Mission Structure

```json
{
  "mission_id": "mission_123",
  "scout_id": "scout_001",
  "target": {
    "type": "archetype",
    "archetype": "high_flyer",
    "region": "Mexico"
  },
  "status": "in_progress",
  "progress": 0.6,
  "discovered_workers": [],
  "cost_to_date": 5000,
  "estimated_completion": "1985-05-01"
}
```

### Worker Visibility Structure

```json
{
  "worker_id": "worker_456",
  "visibility": {
    "global": "unknown",
    "by_region": {
      "Japan": "full_scouting",
      "USA_Northeast": "basic_knowledge",
      "Mexico": "unknown"
    },
    "by_promotion": {
      "promo_001": "full_scouting",
      "promo_002": "basic_knowledge"
    }
  },
  "last_scouted_date": "1985-02-10",
  "scout_reports": []
}
```

---

## OPEN QUESTIONS

- [ ] Exact scouting duration formulas by region/distance
- [ ] Scout salary ranges by skill level
- [ ] Hidden gem probability calculations
- [ ] False positive rate mechanics
- [ ] How do rivalries affect cross-territory scouting access?
- [ ] Can scouts be poached by other promotions?
- [ ] Tape availability by era and region

---

## RELATED SYSTEMS

- [[Popularity_System|Popularity System]] - Fame determines baseline visibility
- [[Territory System/_Territory System Index|Territory System]] - Regional scouting focus
- [[Contract System/_Contract System Index|Contract System]] - Poaching scouted talent
- [[Hidden_Personality|Hidden Personality]] - Deep traits revealed through scouting

---

**Document Status:** Locked (Concept), Formulas Open
**Last Updated:** 2025-12-25
**Next Review:** Define exact scouting duration and cost formulas
