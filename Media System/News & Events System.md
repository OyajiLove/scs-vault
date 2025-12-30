# NEWS & EVENTS SYSTEM

📛 **NAME:** News & Events System
🧭 **CATEGORY:** World Simulation / Information
🔑 **KEYWORDS:** news, events, injuries, scandals, contracts, media, dirt sheets, observer
📝 **SUMMARY:**

The News & Events System generates and presents dynamic world events including injuries, scandals, contract news, industry developments, and media coverage. News presentation changes by era (newsletters in the 70s, websites in the 2000s, social media in the 2020s). Some dirt sheet rumors are true, others are false.

⚙️ **LOGIC OVERVIEW:**

- Dynamic events generated based on worker traits and world state
- Era-appropriate news presentation format
- Observer-style match ratings and analysis
- Dirt sheet rumors with variable accuracy
- Events trigger consequences across game systems

🔬 **LLM INTEGRATION:** High (news article generation, rumor flavor)

📌 **ORIGIN:** Vol 1 Extraction #139

📎 **CONNECTED SYSTEMS:**
- [[Era_UI_System]] - News presentation format by era
- [[Scandal System/_Scandal System Index|Scandal System]] - Scandal events
- [[Injury System/_Injury System Index|Injury System]] - Injury events
- [[Contract System/_Contract System Index|Contract System]] - Contract news

❓ **OPEN QUESTIONS:**
- Event generation frequency
- Rumor accuracy percentages
- Player news filter options

✅ **STATUS:** Locked (Concept)

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #139 | 🔒 LOCKED (concept) |

---

## EVENT TYPES (#139)

### Core Event Categories

| Type | Examples |
|------|----------|
| **Injuries** | Random or match-caused, severity varies |
| **Scandals** | Based on worker traits, backstage incidents |
| **Contract News** | Expirations, negotiations, signings, releases |
| **Industry News** | Other feds, deaths, retirements, returns |
| **Media Coverage** | Reviews, interviews, exposés, ratings |
| **Business News** | TV deals, venue changes, financial issues |

### Injury Events

| Injury Type | Source |
|-------------|--------|
| **Match Injury** | Triggered by match simulation |
| **Training Injury** | Random, affected by worker traits |
| **Accumulated Wear** | Long-term damage from schedule |
| **Freak Accident** | Random, rare |

### Scandal Events

| Scandal Type | Triggers |
|--------------|----------|
| **Backstage Altercation** | Ego clashes, clique conflicts |
| **Personal Scandal** | Based on hidden personality |
| **Legal Issues** | Criminal behavior, lawsuits |
| **Substance Problems** | Drug/alcohol based on traits |
| **Relationship Drama** | Romantic entanglements |

---

## NEWS PRESENTATION BY ERA (#139)

### Era-Appropriate Formats

| Era | Primary Format |
|-----|----------------|
| 1970s | Local papers, wrestling magazines |
| 1980s | Newsletters, magazines, hotlines |
| 1990s | Early websites, newsletters, AOL |
| 2000s | Wrestling websites, forums |
| 2010s | Social media, podcasts, websites |
| 2020s | Twitter/X, Instagram, TikTok, podcasts |

### Format Features

| Format | Characteristics |
|--------|-----------------|
| **Newsletter** | Observer-style, delayed, in-depth |
| **Hotline** | Voice recording, teaser style |
| **Website** | Immediate, varied quality |
| **Social Media** | Instant, viral potential, noise |
| **Podcast** | Commentary, interviews, analysis |

---

## OBSERVER-STYLE MATCH RATINGS

### Star Rating System

| Stars | Quality |
|-------|---------|
| ★★★★★ | All-time classic |
| ★★★★½ | Excellent |
| ★★★★ | Great |
| ★★★½ | Very Good |
| ★★★ | Good |
| ★★½ | Average |
| ★★ | Below Average |
| ★½ | Poor |
| ★ | Bad |
| DUD | Disaster |

### Rating Publication

- Match ratings published in era-appropriate format
- Historical memory tracks career rating averages
- High-rated matches become memory anchors
- Ratings affect worker reputation and popularity

---

## DIRT SHEET RUMORS

### Rumor Accuracy

| Source Quality | Accuracy Range |
|----------------|----------------|
| **Reliable Source** | 85-95% accurate |
| **Inside Scoop** | 60-80% accurate |
| **Speculation** | 30-50% accurate |
| **Wild Rumor** | 10-30% accurate |

### Rumor Types

| Type | Content |
|------|---------|
| **Contract Rumors** | Signing talks, releases, expiring deals |
| **Backstage Heat** | Real or exaggerated conflict reports |
| **Push Changes** | Booking plan leaks, may be works |
| **Personal Issues** | Health, relationships, substance |
| **Business Rumors** | TV deals, buyouts, closures |

### Player Interaction

- Player can investigate rumors (costs time/resources)
- Some rumors are planted works
- Rumor accuracy varies by era (easier to verify in modern era)
- Ignoring true rumors can have consequences

---

## MEDIA COVERAGE

### Coverage Types

| Type | Content |
|------|---------|
| **Show Reviews** | Match ratings, segment analysis |
| **Interviews** | Worker quotes (kayfabe or shoot) |
| **Exposés** | Investigation pieces, scandals |
| **Business Analysis** | Ratings, attendance, financial |
| **Historical Pieces** | Retrospectives, anniversary coverage |

### Media Impact

| Coverage | Effect |
|----------|--------|
| **Positive Review** | Buzz boost, morale up |
| **Negative Review** | Buzz hit, may affect booking |
| **Exposé** | Scandal damage, public reaction |
| **Mainstream Coverage** | Crossover potential, casual eyes |

---

## IMPLEMENTATION NOTES

### Event Structure

```json
{
  "event_id": "event_001",
  "type": "injury",
  "subtype": "match_injury",
  "date": "1985-03-15",
  "affected_workers": ["worker_001"],
  "severity": "moderate",
  "details": {
    "injury_type": "knee",
    "recovery_weeks": 6,
    "caused_by": "match_001"
  },
  "news_coverage": {
    "public": true,
    "format": "newsletter",
    "headline": "Top Star Injured at House Show"
  }
}
```

### Rumor Structure

```json
{
  "rumor_id": "rumor_001",
  "type": "contract",
  "date_reported": "1985-03-10",
  "source_quality": "inside_scoop",
  "accuracy": 0.75,
  "is_true": true,
  "content": "Worker X in contract talks with rival promotion",
  "related_workers": ["worker_001"],
  "player_investigated": false,
  "resolution_date": null
}
```

---

## CONNECTED MECHANICS

- [[Scandal System/_Scandal System Index|Scandal System]] - Scandal events feed news
- [[Injury System/_Injury System Index|Injury System]] - Injury events feed news
- [[Era_UI_System]] - News format presentation
- [[Buzz System/_Buzz System Index|Buzz System]] - News affects buzz

---

## OPEN QUESTIONS

- [ ] Player news customization (filters, sources)
- [ ] Can player plant rumors?
- [ ] News archive searchability
- [ ] Competitor news visibility (fog of war)

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Define event generation probabilities
