# Career Memory Management System (MDOD)

📛 **NAME:** Career Memory Management System (Memory Decompression On Demand)  
🧭 **CATEGORY:** Technical System / Save File Management  
🔑 **KEYWORDS:** memory, compression, decompression, save file, optimization, biography, history, bloat, pruning  
📝 **SUMMARY:** Technical backbone system governing how SCS handles long-term memory across decades of gameplay without bloating save files or losing emotional depth. Uses three-tier memory classification, auto-decompression on view, and manual pinning for favorites. Ensures 50+ year saves remain playable while preserving all meaningful history.

⚙️ **LOGIC OVERVIEW:**
- Three-tier memory classification (Major Anchors → Significant Shifts → Minor Mechanical)
- Title matches ALWAYS preserved regardless of emotional weight
- Legendary workers (Immortal Icons, Era Stars) never compressed
- Auto-decompress on view, auto-recompress on exit unless manually pinned
- Rediscovery system can resurrect forgotten matches into permanent memory
- Applies to Workers, Titles, and Promotions equally

🔬 **LLM INTEGRATION:** Minimal (deterministic compression rules; LLM could generate biography narratives from compressed data)

📌 **ORIGIN:** Vol 5 lines 321-410 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Golden_Era_Worker_Forging]] - Determines worker tier for compression rules
- [[Title System]] - Title match preservation
- [[Crowd_Memory]] - Fan memory of events
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Emotional event logging
- [[Survivor_Promotion_Mechanics]] - Defunct promotion handling

❓ **OPEN QUESTIONS:**
- Exact threshold for "significant" vs "minor" emotional shifts
- Rediscovery event frequency and triggers
- Maximum pinned favorites before performance impact
- Cross-save memory sharing (if any)

✅ **STATUS:** Locked

---

## 1. THREE-TIER MEMORY CLASSIFICATION

| Tier | Examples | Preservation Rule |
|------|----------|-------------------|
| **Major Emotional Anchors** | Legendary matches, career betrayals, redemption arcs, Golden Era forging moments, major scandal arcs | ✅ Never compressed. Lives permanently in save. |
| **Significant Emotional Shifts** | Big loyalty swings, faction shifts, mass worker exits, survivor promotion events | ✅ Archived in compressed emotional form after 10-15 years but emotional effects (loyalty scars, trust bonuses) still fully functional |
| **Minor Mechanical Shifts** | +1/-1 loyalty after random TV matches, random backstage snipes between lower midcarders | ✅ Compressed or pruned automatically after 5-10 years. No fan emotional memory loss, no world memory impact. |

### Memory Classification Philosophy

> "Memory compression is surgery, not a trash compactor. If a match or moment genuinely hurt, healed, changed, scarred, or saved a worker, promotion, or fanbase: it stays real forever. No exceptions. No fake systems."

---

## 2. TITLE MATCHES PRESERVATION (ABSOLUTE RULE)

**ALL title matches kept permanently regardless of emotional magnitude.**

| Category | Preservation |
|----------|--------------|
| **Title Wins and Losses** | Fully logged: date, event, opponent, stipulation, outcome |
| **Title Defenses** | Fully logged, even low-profile defenses |
| **Vacant Title Matches** | Logged in full detail (new champions, interim reigns, tournaments) |
| **Multiman Title Changes** | Logged accurately (battle royals, four-ways, tournaments) |

### Why This Matters

| Reason | Impact |
|--------|--------|
| **Historical Continuity** | Fans, players, historians care deeply about clean title lineage |
| **Career Integrity** | Workers who had short reigns still deserve full archival respect |
| **Promotion Mythology** | Belt histories build world emotional resonance over decades |

---

## 3. WORKER MEMORY PRIORITY BY TIER

| Worker Tier | Memory Handling |
|-------------|-----------------|
| **Immortal Icons** | Full detailed biography and career memory kept forever, including non-title matches, big undercard arcs, midcard betrayals |
| **Era Stars** | Full career memory kept with lighter compression allowed for truly irrelevant filler matches |
| **Beloved Pillars** | Compressed only if needed, but major arcs always preserved |
| **Master Technicians** | Light compression permitted for minor matches without emotional impact |
| **Average Workers** | Compressed on retirement, decompressed on viewing |

---

## 4. REDISCOVERY SYSTEM

Matches can be elevated from compressed/pruned status to permanent memory if "rediscovered" by the wrestling world.

| Mechanic | Behavior |
|----------|----------|
| **World Rediscovery Events** | Media outlets, HOF committees, wrestler biographies, forums randomly "rediscover" old matches every few years |
| **Memory Resurrection** | Rediscovered matches tagged with emotional weight, saved permanently even for long-retired workers |
| **Career Re-evaluation** | Workers may gain slightly increased prestige post-retirement if hidden greatness surfaces |

### Example

Sangre Chicana's 1983 bloodbath brawls against MS-1 and Perro Aguayo, forgotten for 20 years, get picked up by DVDVR as hidden classics → retroactively tagged as permanent memory, career re-evaluated.

---

## 5. AUTO-DECOMPRESS ON VIEW (CORE MECHANIC)

| Action | Behavior |
|--------|----------|
| **Player opens retired worker / defunct title / defunct promotion profile** | ✅ Full decompression happens automatically (0.01-0.5 seconds depending on career depth) |
| **Player exits the profile** | ✅ Memory recompresses automatically unless player has pinned it |
| **Player clicks zipper icon while viewing** | ✅ Permanently decompresses that entity forever |
| **Pinned entities** | ✅ Always fully expanded until manually unpinned |

### Decompression Time Estimates

| Career Type | Data Size | Time |
|-------------|-----------|------|
| **Average Worker (midcarder)** | 50-100 KB | ~0.01-0.05 seconds (instant) |
| **Heavy Career (top star)** | 200-500 KB | ~0.05-0.2 seconds (instant) |
| **Monster Career (30+ year icon)** | 1-2 MB | ~0.2-0.5 seconds (small flicker) |

---

## 6. DECOMPRESSED BIOGRAPHY CONTENTS

When viewing a decompressed worker:

| Section | What's Visible |
|---------|----------------|
| **Title Matches** | All wins, defenses, losses (dates, opponents, outcomes, event names) |
| **Legendary Matches** | Career-defining, era-defining, mythology-building (highlighted/starred) |
| **Rediscovered Hidden Gems** | Flagged separately with discovery context |
| **Standard Singles Matches** | Opponent, event/location, outcome, star rating |
| **Tag/Trios Matches** | Partners, opponents, outcome, feud notation |
| **Tournament Matches** | Participation, advancement, elimination details |
| **Special Gimmick Matches** | Cages, bullrope, apuestas (mask/hair) highlighted |
| **Betrayal Matches** | Emotional flag if tied to heel turn, faction betrayal |
| **Comeback Matches** | Milestone flag for returns from injury/scandal/retirement |

### Bio Layout Structure

| Section | Description |
|---------|-------------|
| **Career Overview** | Short summary: title wins, major feuds, highlights |
| **Match History Tab** | Full chronological log with filters (title matches, legendary, feud matches) |
| **Legendary Matches Section** | Pulled separately and highlighted |
| **Rediscovered Matches Section** | Hidden gems flagged if rediscovered post-career |

---

## 7. UI IMPLEMENTATION

### Zipper Icon System

| Element | Behavior |
|---------|----------|
| **Icon Placement** | Discrete zipper icon on compressed entities (retired workers, defunct titles, defunct promotions) |
| **Visibility** | Only visible after auto-decompression during profile view |
| **Hover Text** | "Click to keep full career memory expanded permanently" |
| **Click Action** | Permanently decompresses, no more auto-recompression |

### Applies to All Entity Types

| Entity | Compression Behavior |
|--------|---------------------|
| **Retired/Dead Workers** | Compress after retirement, reversible instantly on viewing |
| **Defunct Titles** | Compress after title retirement/deactivation, reversible on viewing |
| **Defunct Promotions** | Compress after full promotion death, reversible on viewing |

---

## 8. TECHNICAL OPTIMIZATION STRATEGIES

| Strategy | Effect |
|----------|--------|
| **Emotional Memory Compression** | Minor emotional changes collapsed into summarized flags |
| **Critical Event Priority** | Only life-changing events get full archival detail |
| **Match/Event Memory Caps** | Only best 3-5 matches kept in full emotional record per worker (others compressed) |
| **Delta Saves** | Only save changes since last major snapshot |
| **Modular World Saves** | Promotions, workers, titles, fanbases in independent blocks |
| **Archival on Retirement/Death** | Collapse memory data into final biography node |
| **Decaying Minor Data** | Loyalty shifts smaller than threshold decay passively |
| **Batch Processing** | Nightly world events processed in grouped clusters |
| **Asynchronous Processing** | Non-player promotions process in lower CPU priority |
| **Memory Layering** | Only emotionally active promotions/top-card workers fully processed nightly |
| **Fanbase Modeling** | Group emotional dynamics, not individual fans |

---

## 9. SAVE FILE PROJECTIONS

### With Optimizations (After 15 Years In-Game)

| Metric | Projection |
|--------|------------|
| **Save File Size** | 40-80 MB |
| **Nightly Processing Speed** | 10-20% slowdown vs fresh game |
| **Save/Load Time** | 5-15 seconds |

### Comparison

| Approach | Outcome |
|----------|---------|
| **Full global decompression always** | Save file bloat, performance loss |
| **Total deletion of minor events** | Faster, but loses emotional realism |
| **MDOD (This System)** | ✅ Perfect balance: depth when wanted, efficiency when not |

---

## 10. LOCKED PRINCIPLES

| Principle | Rule |
|-----------|------|
| **Significance over Volume** | Simulate emotional history, not spam event logs |
| **Modular Saves** | No promotion or worker unnecessarily loads if not touched |
| **Career Completion Compression** | No bloat for retired/dead workers |
| **Fanbase Modeling** | Group emotional dynamics, not granular single fans |
| **Title Match Sanctity** | All title matches preserved regardless of significance |
| **Legendary Permanence** | Immortal Icons and Era Stars never compressed |
| **Rediscovery Respect** | Hidden gems can be resurrected at any time |

---

## 11. PHILOSOPHY STATEMENTS

> "History breathes where it matters, fades where it doesn't. Players protect what they love, but the world moves on without clutter. Emotional memory is sacred. Mechanical noise is forgotten."

> "If you care enough to view, the history lives. If you care enough to cherish, the history stays."

> "We compress events, but preserve emotion. If it moved a fan, broke a worker, forged a legend, killed a promotion: it stays. Forever. If it was a random Thursday night win that nobody remembers? It gets gently forgotten, just like real life."

---

## 12. IMPLEMENTATION NOTES

```json
{
  "memory_management": {
    "worker_id": "sangre_chicana",
    "status": "RETIRED",
    "tier": "BELOVED_PILLAR",
    "compression_state": "COMPRESSED",
    "pinned": false,
    "permanent_memories": [
      {"type": "LEGENDARY_MATCH", "event": "EMLL Anniversary 1983", "opponent": "MS-1"},
      {"type": "TITLE_REIGN", "title": "Regional Light Heavyweight", "start": "1988", "end": "1989"},
      {"type": "REDISCOVERED", "event": "DVDVR Hidden Classic 2030", "original_date": "1983"}
    ],
    "compressed_memories": {
      "count": 847,
      "years_covered": "1980-1995",
      "size_kb": 125
    },
    "decompression_time_ms": 50
  }
}
```

---

## 13. RELATED SYSTEMS

- [[Golden_Era_Worker_Forging]] - Worker tier determines compression rules
- [[Title System]] - Title match preservation
- [[Crowd_Memory]] - Fan memory layer
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Emotional event logging
- [[Survivor_Promotion_Mechanics]] - Defunct promotion handling
- [[Golden_Era_Collapse_Memory]] - Major event preservation

---

**Document Status:** Locked  
**Source:** Vol 5 lines 321-410  
**Next Review:** Integration with Biography Generation UI
