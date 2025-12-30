# SCS_BIBLE_15_MEDIA_SYSTEM.md

📛 **NAME:** Media System  
🧭 **CATEGORY:** World Systems / External Perception  
🔑 **KEYWORDS:** media, press, dirtsheets, coverage, interviews, social media, PR, public perception  
📝 **SUMMARY:** System governing how media outlets cover wrestling, including press conferences, interviews, dirtsheet reporting, and social media dynamics. Much of this functionality is distributed across Scandal, TV Broadcast, and Popularity systems rather than existing as standalone.

⚙️ **LOGIC OVERVIEW:**
- Media coverage affects worker and promotion reputation
- Different media types have different reach and credibility
- Era-based media evolution (dirtsheets → internet → social media)
- Press events can be booked as segment types
- Scandal coverage handled by Scandal System

🔬 **LLM INTEGRATION:** High potential (generate press coverage, interview dialogue, social media posts)

📌 **ORIGIN:** Mentioned throughout volumes; components distributed across other systems

📎 **CONNECTED SYSTEMS:**
- **SCAN-001:** Scandal System (media coverage of scandals, era-based response)
- **TV-001:** TV Broadcast System (media obligations, promo requirements)
- **POP-001:** Popularity System (media exposure affects pop growth)
- **BUZZ-001:** Buzz System (media-driven short-term heat)
- **BOOK-001:** Booking Engine (press conferences as segment type)

❓ **OPEN QUESTIONS:**
- Standalone system vs. coordination layer
- Media outlet types and reach formulas
- Interview system mechanics
- Social media posting (modern era)

✅ **STATUS:** Scaffolding (Components locked in other systems)

---

## 1. WHAT EXISTS (LOCKED IN OTHER SYSTEMS)

### 1.1 From Booking Engine Phase 3 (BOOK-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Press Conferences** | Segment types | Listed as bookable segment alongside promos, interviews, brawls |
| **Backstage Interviews** | Segment types | Pre-match and post-match interview segments |
| **Media Obligations** | Booking consequences | Workers may have media appearance requirements |

### 1.2 From Scandal System (SCAN-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Media Scandal Coverage** | Era-based response | How media covers scandals varies by era |
| **Leak Mechanics** | Scandal triggers | Backstage leaks reaching media outlets |
| **PR Fallout System** | Scandal consequences | Public statement and damage control mechanics |
| **Dirtsheet References** | Information spread | How insider information reaches public |

### 1.3 From TV Broadcast System (TV-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Promo & Media Obligations** | TV deal structure | Must make media rounds, do pre-show bites |
| **Network Feedback** | Creative pressure | Network-driven media coverage requirements |
| **Off-Screen Perception** | Ratings factors | Union stories, firings, backstage leaks affect ratings |

### 1.4 From Popularity System (POP-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Media Attention Effects** | Pop modifiers | Media coverage affects popularity growth/decay |
| **Crossover Star** | Pop mechanics | Workers who transcend wrestling media into mainstream |

### 1.5 From Buzz System (BUZZ-001)

| Component | Location | Description |
|-----------|----------|-------------|
| **Virality** | Modern era mechanic | Social media driven short-term buzz spikes |
| **Internet Synergy** | Buzz factors | Online discussion affecting buzz levels |

---

## 2. WHAT MAY NEED STANDALONE BUILDING

### 2.1 Media Outlet Types

| Type | Era | Reach | Credibility |
|------|-----|-------|-------------|
| **Wrestling Magazines** | All | Regional to National | Medium |
| **Dirtsheets** | 1980s+ | Niche, Insider | Low-Medium (varies) |
| **Newsletters** | 1990s+ | Niche, Smart Fan | Medium-High |
| **Wrestling Websites** | 2000s+ | Global | Varies wildly |
| **Social Media** | 2010s+ | Instant, Global | Low (but impactful) |
| **Mainstream Sports Media** | All | Massive | High |
| **Tabloids** | All | Massive | Low |

### 2.2 Interview System

If built as standalone:
- Pre-match interview segments (already in Booking Engine)
- Post-match interview reactions
- Shoot interview mechanics (breaking kayfabe risks)
- Media training effects on interview quality

### 2.3 Social Media Posting (Modern Era)

- Worker social media presence
- Viral moments
- Controversy generation
- Fan interaction metrics

---

## 3. SEGMENT TYPES (FROM BOOKING ENGINE)

The following segment types relate to media and are already defined:

| Segment Type | Description |
|--------------|-------------|
| **Press Conferences** | Formal announcements, contract signings with media present |
| **Backstage Interviews** | Classic interview format with announcer/interviewer |
| **In-Ring Promos** | Workers addressing crowd and camera directly |

### Segment Evaluation Factors (Locked)

- Mic skills
- Character work
- Crowd response
- Believability
- Advancement (of storyline)
- Catchphrase/memorable moment

### Segment Outcomes

- Promo kills (exceptional)
- Solid
- Weak
- Bombed
- Derailed

---

## 4. ASSESSMENT

**Current Status:** Media functionality substantially covered by existing systems.

**Recommendation:** Rather than standalone Media System, consider:

1. ✅ Scandal System: Handles media coverage of scandals
2. ✅ TV Broadcast: Media obligations and network pressure
3. ✅ Booking Engine: Press conferences and interviews as segments
4. ✅ Buzz System: Virality and internet synergy
5. ⚠️ Social Media subsystem: May need dedicated mechanics for modern era

**If standalone system is built later,** focus on:
- Media outlet database with reach/credibility stats
- Rumor/leak propagation mechanics
- Shoot interview consequences
- Era-specific media landscape templates

---

## 5. IMPLEMENTATION NOTES

### Minimal Media Data Structure (if needed)

```
MediaOutlet {
    outlet_id: string
    name: string
    outlet_type: enum (MAGAZINE, DIRTSHEET, NEWSLETTER, WEBSITE, SOCIAL, MAINSTREAM, TABLOID)
    era_active: EraRange
    reach: float (0.0-1.0)
    credibility: float (0.0-1.0)
    insider_access: float (0.0-1.0)
    relationships: map<promotion_id, float>
}

MediaCoverage {
    outlet_id: string
    subject_type: enum (WORKER, PROMOTION, SHOW, SCANDAL)
    subject_id: string
    coverage_type: enum (POSITIVE, NEUTRAL, NEGATIVE, SCANDAL, PUFF_PIECE)
    reach_modifier: float
    duration_days: int
}
```

---

## RELATED SYSTEMS

- **SCAN-001:** Primary handler of media scandal coverage
- **TV-001:** Media obligations in TV deals
- **BOOK-001:** Press conferences and interviews as segment types
- **BUZZ-001:** Virality and internet-era media dynamics

---

**Document Status:** Scaffolding, awaiting decision on standalone vs. distributed approach  
**Next Review:** Evaluate social media subsystem needs for modern era gameplay
