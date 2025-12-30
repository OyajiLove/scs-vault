# Fan Reaction System

📛 **SYSTEM:** Fan Reaction & Management  
🧭 **CATEGORY:** Audience Simulation / Meta-Layer  
🔑 **KEYWORDS:** fans, audience, backlash, loyalty, fanbase types, scandal tolerance, career perception, crowd behavior  
📝 **SUMMARY:** Umbrella system governing how different fan types perceive, react to, and remember workers across their careers. This is the meta-layer that determines WHO the fans are and HOW they behave, while connected systems handle the granular mechanics of in-show reactions, memory, and popularity tracking.

⚙️ **LOGIC OVERVIEW:**
- Different fanbase types have different values, tolerances, and loyalties
- Fan loyalty creates protective buffers against scandals and bad booking
- Fans react differently based on era, region, and promotion context
- Career arcs affect fan perception over time (rises, falls, comebacks)
- Institutional loyalty (to promotions/stars) can override scandal severity
- Fan memory interacts with current events to create layered reactions

🔬 **LLM INTEGRATION:** Yes
- Generates fan reaction narratives
- Creates social media backlash/support flavor text
- Simulates crowd chant selection based on fanbase type
- Describes fan perception shifts over time

📌 **ORIGIN:** Vol 2 Chunk 05 (Fan Loyalty Resistance), Vol 6 (Crowd Signals), Vol 4 (Crowd Memory)

✅ **STATUS:** LOCKED

---

## VERSION HISTORY

**Version 1.0 (Vol 2 Chunk 05) [CURRENT]**
- Fan Loyalty Resistance system formalized
- Fanbase types defined with tolerance levels
- Institutional protection mechanics
- Career arc perception outlined

---

## Connected Systems (Granular Mechanics)

This system provides the META-LAYER. These connected systems provide GRANULAR MECHANICS:

| System | What It Handles | Relationship |
|--------|-----------------|--------------|
| [[Crowd Signals/_Crowd Signals Index\|Crowd Signals]] | In-show reactions: chants, garbage, heat signals | Fan Reaction tells Crowd Signals WHO is watching; Crowd Signals determines HOW they react in the moment |
| [[Fan Memory Engine/_Fan Memory Index\|Fan Memory Engine]] | Long-term memory of events, feuds, matches | Fan Reaction determines memory WEIGHT by fanbase type; Fan Memory tracks WHAT is remembered |
| [[Popularity System/Popularity_System\|Popularity System]] | Worker popularity ratings, draw power | Fan Reaction affects popularity CHANGES; Popularity tracks current LEVELS |
| [[Scandal System/_Scandal System Index\|Scandal System]] | Scandal types, severity, redemption | Fan Reaction determines backlash INTENSITY; Scandal System handles event MECHANICS |

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Fanbase Types]] | Definition of different fan populations | Locked |
| [[Fan Loyalty Resistance]] | How fans resist or embrace scandals | Locked |
| [[Career Perception Arcs]] | How fan perception shifts over career stages | Locked |
| [[Institutional Loyalty]] | How fans defend promotions and top stars | Locked |
| [[Promotion Fan Composition]] | How different promotions attract different fan mixes | Locked |
| [[Fanbase DNA System]] | Core fanbase composition and evolution | Locked |
| [[Fanbase_Trust_and_Betrayal]] | Trust mechanics between fans and workers/promotions | Locked |
| [[Fanbase_Cultural_Mutation]] | How fanbases change with cultural shifts | Locked |
| [[Fan_Subculture_Infighting]] | Internal fanbase conflicts and faction wars | Locked (Vol 5) |
| [[Golden_Era_Flag_Planting]] | When golden eras begin and are recognized | Locked (Vol 5) |
| [[Golden_Era_Collapse_Memory]] | How golden era deaths create lasting scars | Locked (Vol 5) |
| [[Fanbase_Emotional_Exodus]] | How fanbases migrate away after collapse | Locked (Vol 5) |

---

## Fanbase Types (LOCKED)

Each promotion attracts a specific mix of fanbase types. Each fanbase type has distinct values and tolerances.

| Fanbase Type | Core Values | Scandal Tolerance | Loyalty Style |
|--------------|-------------|-------------------|---------------|
| **Hardcore Company Loyalists** | Brand devotion, tradition, stars | High | Will defend promotion/stars unless murder-level bad |
| **Indie Hardcore Fans** | Workrate, authenticity, anti-corporate | Very Low | Turn on "hypocrites" fast; purity tests common |
| **Family-Friendly Fans** | Wholesomeness, heroes, role models | Very Low | Scandals involving drugs, abuse, children = instant rejection |
| **Deathmatch Outlaw Fans** | Authenticity, toughness, spectacle | Medium-High | Tolerate a lot if it feels "real"; hate cowardice |
| **Lucha Traditionalists** | Tradition, masks, legacy, local pride | Medium | Protect local icons; slower to forgive outsiders |
| **Joshi Superfans** | Purity, dedication, idol culture | Low | Betrayals and sleaze are devastating; parasocial intensity |
| **Edgy Attitude Era Types** | Antiheroes, controversy, shock value | Medium-High | Love bad behavior if it's "badass"; hate weakness |
| **Casual Mainstream Fans** | Entertainment, stories, big moments | Medium | Follow media narrative; susceptible to PR spin |
| **Smark/Internet Fans** | Insider knowledge, workrate, booking critique | Low-Medium | Quick to turn; appreciate self-awareness |

---

## Promotion Fan Composition

Each promotion has a fanbase composition that affects overall reactions:

### Example Compositions

| Promotion Style | Primary Fanbase | Secondary | Tertiary |
|-----------------|-----------------|-----------|----------|
| WWE-style Major | Hardcore Company Loyalists (40%) | Casual Mainstream (35%) | Family-Friendly (25%) |
| AEW-style Alternative | Smark/Internet (35%) | Indie Hardcore (30%) | Edgy Attitude (20%) |
| NJPW-style Prestige | Hardcore Company Loyalists (45%) | Smark/Internet (35%) | Casual Mainstream (20%) |
| Joshi Promotion | Joshi Superfans (60%) | Hardcore Loyalists (25%) | Casual (15%) |
| Deathmatch Indie | Deathmatch Outlaw (55%) | Indie Hardcore (30%) | Edgy Attitude (15%) |
| Family Indie | Family-Friendly (50%) | Casual Mainstream (35%) | Hardcore Loyalists (15%) |
| Lucha Promotion | Lucha Traditionalists (50%) | Casual Mainstream (30%) | Hardcore Loyalists (20%) |

### Composite Tolerance Calculation

When a scandal occurs, the promotion's composite tolerance is:

```
Composite Tolerance = Σ (Fanbase % × Fanbase Tolerance)
```

This creates the "crowd" reaction that the worker and promotion must navigate.

---

## Career Perception Arcs

How fans perceive workers changes across career stages:

| Career Stage | Fan Perception Tendencies |
|--------------|---------------------------|
| **Rookie** | Curiosity, benefit of doubt, excitement for potential |
| **Breakout** | Surge of support, bandwagon fans, "discovered them first" pride |
| **Established Star** | Stable loyalty, higher tolerance for missteps, brand identification |
| **Declining Star** | Nostalgia vs "move on" tension, sensitivity to "burying young talent" |
| **Crisis/Scandal** | Test of loyalty; fanbase type determines response |
| **Comeback Attempt** | Skepticism vs hope; authenticity heavily scrutinized |
| **Legend Status** | Protective nostalgia, "earned the right" tolerance, legacy focus |

### Success Changes People (Fan Awareness)

Fans notice when success changes workers:

| Worker Change | Fan Reaction |
|---------------|--------------|
| Stays humble despite success | Increased loyalty, "deserves it" narrative |
| Becomes arrogant/political | Smark backlash, "sold out" accusations |
| Declines gracefully | Respect, appreciation, farewell tours |
| Refuses to step aside | "Hogging the spotlight" resentment |
| Genuine reinvention | Renewed interest, "evolution" praise |
| Desperate clinging to past | Pity or mockery depending on fanbase |

---

## Institutional Loyalty

Fans develop loyalty not just to workers, but to promotions themselves.

### Promotion Loyalty Levels

| Loyalty Level | Fan Behavior |
|---------------|--------------|
| **Casual** | Watches when convenient, no strong attachment |
| **Regular** | Consistent viewer, defends promotion in mild debates |
| **Devoted** | Deeply invested, buys merch, attends shows, active online |
| **Tribal** | Promotion is identity; attacks critics; overlooks scandals |
| **Cult** | Promotion can do no wrong; conspiracy thinking about critics |

### Institutional Protection Effect

High institutional loyalty creates scandal shielding:

| Promotion Loyalty | Scandal Response |
|-------------------|------------------|
| Casual fans | React to scandal itself |
| Regular fans | Wait for promotion's response |
| Devoted fans | Give benefit of doubt |
| Tribal fans | Defend worker/promotion regardless |
| Cult fans | Attack accusers, deny evidence |

This explains how major promotions survive repeated scandals while small ones collapse from single incidents.

---

## Open Questions

- [ ] Exact fanbase composition for each era/region
- [ ] How do individual fans shift between types over time?
- [ ] Generational changes in fanbase composition
- [ ] Social media amplification mechanics
- [ ] Interaction between fanbase types (do they influence each other?)

---

## Implementation Notes

```json
{
  "promotion_fanbase": {
    "promotion_id": "promo_001",
    "era": "2020s",
    "region": "usa_national",
    "composition": {
      "hardcore_company_loyalists": 0.40,
      "casual_mainstream": 0.35,
      "family_friendly": 0.15,
      "smark_internet": 0.10
    },
    "composite_scandal_tolerance": 0.58,
    "institutional_loyalty_distribution": {
      "casual": 0.30,
      "regular": 0.35,
      "devoted": 0.20,
      "tribal": 0.12,
      "cult": 0.03
    }
  }
}
```

---

**Document Status:** In Progress  
**Last Updated:** 2025-12-26  
**Next Step:** Pull regional profiles from Era System, consolidate with Crowd Signals region data
