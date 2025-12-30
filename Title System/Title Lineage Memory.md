# Title Lineage Memory

📛 **MECHANIC:** Championship Historical Tracking
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Legacy
🔑 **KEYWORDS:** lineage, title history, reign, champions, legacy, records
📌 **ORIGIN:** Vol 1-4 (Title lineage memory, career arc documentation), Vol 1 Extraction #131
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Every championship carries its history. Title lineage memory tracks all reigns, creating a living record that affects prestige, fan memory, and worker legacy. Workers who held short reigns deserve archival respect; legendary reigns become part of promotion mythology.

---

## Lineage Data Structure

Each reign records:

| Field | Description |
|-------|-------------|
| **Champion** | Worker who held the title |
| **Reign Number** | 1st reign, 2nd reign, etc. |
| **Start Date** | When they won |
| **End Date** | When they lost (or current if active) |
| **Length (Days)** | Duration of reign |
| **Defenses** | Number of successful title defenses |
| **How Won** | Match type, opponent, finish |
| **How Lost** | Match type, opponent, finish |
| **Quality Rating** | Overall reign quality (1-100) |
| **Notable Defenses** | List of significant matches |

---

## Reign Quality Factors

What makes a reign memorable:

| Factor | Quality Contribution |
|--------|---------------------|
| **Defense Quality** | Great matches add points |
| **Credible Challengers** | Quality opponents matter |
| **Feud Heat** | Hot feuds during reign |
| **Reign Length** | Longer (if maintained) adds weight |
| **MOTY Candidates** | Classic matches are major |
| **Clean Finishes** | Decisive victories build legitimacy |
| **Fan Investment** | Crowd cared about defenses |

---

## Historical Records Tracking

System tracks title records:

| Record | Description |
|--------|-------------|
| **Longest Reign** | Most days as champion |
| **Most Reigns** | Most separate title runs |
| **Most Defenses** | Successful defenses in single reign |
| **Shortest Reign** | Fewest days (often embarrassing) |
| **Youngest Champion** | Age at first win |
| **Oldest Champion** | Age at last win |
| **First Champion** | Inaugural holder |
| **Grand Slam** | Held multiple title types |

---

## Lineage Prestige Inheritance

Past affects present:

| Scenario | Effect |
|----------|--------|
| **Legendary lineage** | New champions get credibility boost |
| **Joke lineage** | New champions fight uphill for respect |
| **First champion sets tone** | Inaugural holder shapes title's identity |
| **Breaking records** | Major buzz and prestige spike |

---

## Multi-Champion Tracking

For titles with many holders:

| Metric | Use |
|--------|-----|
| **Average Reign Length** | Benchmark for expectations |
| **Average Defenses** | What's normal for this title |
| **Champion Tiers** | Group by reign quality |
| **Transitional Rate** | How often very short reigns |

---

## Title Unification Lineages

When titles merge:

| Scenario | Lineage Handling |
|----------|------------------|
| **Clean Unification** | Both lineages merge into unified history |
| **Absorption** | Absorbed title's lineage archived separately |
| **New Title Created** | Fresh lineage, old titles retired |
| **Split** | Unified title's lineage splits when separated |

---

## Vacancy Tracking

When titles are vacated:

| Reason | Record Entry |
|--------|--------------|
| **Injury** | Noted; champion's stats preserved |
| **Scandal** | Stripped; noted in lineage |
| **Departure** | Left promotion; noted |
| **Retirement** | Retired as champion (prestigious) |
| **Death** | Tragic entry; handled with care |

---

## Automatable Data

From sources like Cagematch:

| Data Type | Source Reliability |
|-----------|-------------------|
| **Reign dates** | High (well documented) |
| **Defense counts** | High |
| **Match results** | High |
| **Match quality** | Medium (subjective ratings) |
| **Feud context** | Medium (requires interpretation) |
| **Crowd response** | Low (rarely documented) |

---

## Lineage Display

For player reference:

| View | Content |
|------|---------|
| **Full Lineage** | Complete list of all champions |
| **Recent History** | Last 10-20 champions |
| **Legends View** | Greatest reigns highlighted |
| **Statistics** | Records, averages, milestones |
| **Timeline** | Visual representation over time |

---

## Dragon Lineage Tag (#131)

Optional title tag recognizing prestigious lineage:

| Attribute | Effect |
|-----------|--------|
| **Dragon Lineage** | Title has prestigious history spanning multiple generations |
| **Lineage Bonus** | Champion gains credibility vs. newer workers |
| **Legacy Matches** | Facing a Dragon Lineage champion feels significant |

Workers who hold Dragon Lineage titles gain a modifier when facing workers who have never held major titles.

---

## Travelling Champion System (#131)

Specific booking pattern for NWA-style touring champions:

### Core Concept

Elite worker trusted to elevate local babyfaces across territories while maintaining title credibility.

### Booking Priorities

| Priority | Description |
|----------|-------------|
| **Close matches with local faces** | Make locals look strong |
| **Escape wins** | Roll-ups, foot on ropes, distracted refs |
| **Protected finishes** | DQ if needed to save both parties |
| **Rare clean losses** | Only to legend-level faces |

### Champion Requirements

| Requirement | Reason |
|-------------|--------|
| **Ring work** | Must carry less experienced workers |
| **Professionalism** | Represents the entire federation |
| **Psychology** | Knows how to make others look good |
| **Travel tolerance** | Grueling schedule |
| **Political savvy** | Navigates territory politics |

### Performance Tracking

| Outcome | Effect on Champion |
|---------|-----------------|
| **Elevates locals successfully** | Gains Political Capital, renewed trust |
| **Buries locals** | Loses trust, possibly stripped |
| **Draws poorly** | Board pressure for title change |
| **Creates stars** | Legend-tier reputation boost |

---

## Career Integration

How title history affects workers:

| Effect | Description |
|--------|-------------|
| **Resume Building** | Past reigns on worker profile |
| **Credibility** | Former champions have booking cache |
| **Legacy Points** | Title reigns contribute to legacy score |
| **HOF Consideration** | Title history is major factor |
| **Nostalgia Returns** | Former champions can return for title |

---

## Connected Mechanics

- [[Title Prestige]] - Lineage quality affects current prestige |
- [[Title Run Dynamics]] - Each reign recorded and evaluated |
- [[Hall of Fame System]] - Title history affects eligibility |
- [[Crowd Memory]] - Classic reigns become memory anchors |
- [[Worker Legacy]] - Titles are major career milestones |

---

## Open Questions

- [ ] How to handle disputed reigns (kayfabe vs. shoot)
- [ ] Recognizing title history across promotion buyouts
- [ ] House show title changes (canon or not?)
- [ ] "Undisputed" lineage handling
- [ ] How lineage data imports from external sources

---

## Implementation Notes

```json
{
  "title_lineage": {
    "title_id": "title_001",
    "current_champion": "worker_001",
    "total_reigns": 45,
    "current_reign_number": 45,
    "history": [
      {
        "reign_number": 44,
        "champion_id": "worker_042",
        "start_date": "1984-06-15",
        "end_date": "1985-03-14",
        "length_days": 272,
        "defenses": 12,
        "how_won": { "match_type": "singles", "opponent": "worker_041", "finish": "pinfall_clean" },
        "how_lost": { "match_type": "cage", "opponent": "worker_001", "finish": "pinfall_clean" },
        "quality_rating": 85,
        "notable_defenses": ["match_102", "match_118", "match_134"]
      }
    ],
    "records": {
      "longest_reign": { "champion_id": "worker_015", "days": 803 },
      "most_reigns": { "champion_id": "worker_022", "count": 6 },
      "most_defenses": { "champion_id": "worker_015", "count": 28 }
    }
  }
}
```
