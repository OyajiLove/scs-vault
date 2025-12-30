# MATCH PRESENTATION SYSTEM

📛 **NAME:** Match Presentation System  
🧭 **CATEGORY:** User Interface, Match Output, Show Reporting  
🔑 **KEYWORDS:** match presentation, show report, result display, highlights, play-by-play, PBP, condensed recap  
📝 **SUMMARY:** Determines how match results are displayed to the player. Three primary modes available: Straight Up Result (fast), Result + Highlights (default immersive), and Condensed Storyline Recap (optional toggle). Full play-by-play is deferred to future development phases.

⚙️ **LOGIC OVERVIEW:**

- Player chooses preferred match presentation style
- Presentation mode affects information density and emotional immersion
- All modes use same underlying match simulation; only output changes
- Can be toggled per-show or as global preference
- MVP focuses on Result + Highlights as default

🔬 **LLM INTEGRATION:** Yes. LLM generates highlight moments, condensed recaps, and (future) play-by-play based on match simulation data.

📌 **ORIGIN:** Vol. 2 (system decision)

📎 **CONNECTED SYSTEMS:** [[Match Engine/_Match Engine Index|Match Engine]], Show Reporting, [[Tags_System]] (highlight generation), [[Worker_Skills]]

❓ **OPEN QUESTIONS:**

- How many highlight moments per match? (2-4 typical?)
- Condensed recap length: paragraph or 2-3 sentences?
- Future PBP: Fire Pro style or text adventure style?

✅ **STATUS:** Locked (Vol 2)

---

## VERSION HISTORY

**Version 1.0 (Vol 2) [LOCKED]**
- Three presentation modes defined
- Full PBP deferred to distant future
- Default set to Result + Highlights

---

## PRESENTATION MODES

### 1. Straight Up Result (Default Fast)

**Description:** Winner, time, finish move only. TEW-style minimal output.

**Format:**
```
[Winner] def. [Loser] via [Finish Move] ([Time])
```

**Example:**
```
Goto def. Honma via GTR (15:26)
```

**Use Case:** Fast booking sessions, tournament simulations, house show summaries.

---

### 2. Result + Highlight Moments (Default Immersive)

**Description:** Result plus 1-3 key moments from the match. Adds flavor without overwhelming.

**Format:**
```
[Winner] def. [Loser] via [Finish Move] ([Time])
[1-3 highlight sentences describing key moments]
```

**Example:**
```
Goto def. Honma via GTR (15:26)
Honma battered Goto with a relentless headbutt assault, but Goto rallied late, catching Honma with a sudden GTR to steal the victory.
```

**Use Case:** Default show viewing, emotional engagement, understanding match dynamics.

---

### 3. Condensed Storyline Recap (Optional Toggle)

**Description:** Paragraph-length narrative summary capturing the emotional arc of the match.

**Format:**
```
[Winner] def. [Loser] via [Finish Move] ([Time])
[Paragraph describing match flow, emotional beats, key moments, and finish]
```

**Example:**
```
Goto def. Honma via GTR (15:26)
In a hard-fought clash, Honma battered Goto with a relentless assault of headbutts, targeting the neck and shoulders. Goto absorbed tremendous punishment, his fighting spirit carrying him through near-falls. In the final stretch, Goto dodged a diving kokeshi and caught Honma with a sudden GTR to steal the victory. Tanahashi's resilience stole the crowd's heart once again, overcoming brutal body shots to claim victory.
```

**Use Case:** Storytelling-focused players, major matches, PPV main events.

---

### 4. Full Play-by-Play (Future, Deferred)

**Description:** Move-by-move match simulation with detailed commentary. NOT IMPLEMENTED for MVP.

**Status:** Way down the road. Requires:
- Complete moveset database
- Style-specific spot libraries
- AI logic trees for match flow
- Extensive QA testing

**Rationale for Deferral:**
- Massive scope creep risk
- QA nightmare for move accuracy
- Most players prefer faster result digestion
- Core sim focus must be protected

---

## HIGHLIGHT GENERATION

Highlights are generated based on:

| Source | Example Highlights |
|--------|-------------------|
| **Finish Quality** | "Clean pinfall after devastating lariat" |
| **Near Falls** | "Survived a burning hammer at 2.9" |
| **Signature Spots** | "Landed a perfect moonsault to the floor" |
| **Crowd Reaction Spikes** | "Crowd erupted as underdog mounted comeback" |
| **Injury/Drama Moments** | "Worked through visible leg injury" |
| **Tag Interactions** | "Never Say Die spirit triggered late rally" |

### Tag-Based Highlight Modifiers

Worker tags influence highlight generation:

| Tag | Highlight Influence |
|-----|---------------------|
| **Spirit Bomb** | Late-match comebacks emphasized |
| **Psychology Monster** | Match structure and pacing noted |
| **Flashy** | Spectacular moves highlighted |
| **Blood Soaked** | Blade jobs and violence noted |
| **Submission Specialist** | Hold sequences emphasized |

---

## IMPLEMENTATION NOTES

### Data Structure (Conceptual)

```json
{
  "match_id": "MATCH_12345",
  "presentation_mode": "highlights",
  "result": {
    "winner": "Goto",
    "loser": "Honma",
    "finish": "GTR",
    "time": "15:26",
    "finish_type": "pin"
  },
  "highlights": [
    {
      "moment_type": "near_fall",
      "description": "Honma's diving kokeshi nearly ended it at 2.9",
      "timestamp": "14:30"
    },
    {
      "moment_type": "finish",
      "description": "Goto caught Honma with a sudden GTR to steal the victory",
      "timestamp": "15:26"
    }
  ],
  "recap_text": "In a hard-fought clash, Honma battered Goto..."
}
```

### Player Settings

```
Match Presentation:
[ ] Straight Up Result (fastest)
[x] Result + Highlights (default)
[ ] Condensed Storyline Recap

[ ] Show highlights for all matches
[x] Show highlights for featured matches only
```

---

## DESIGN PHILOSOPHY

### Why Not Full PBP?

1. **Scope Protection:** Core sim must come first
2. **QA Burden:** Move accuracy testing would take months
3. **Player Preference:** 95%+ prefer faster result digestion
4. **Resource Allocation:** AI/logic focus stays on world simulation
5. **Quality Bar:** Half-assed PBP would hurt the game more than help

### Future PBP Path (If Ever)

- Phase 1: Limited PBP for title matches only
- Phase 2: Optional PBP for main events
- Phase 3: Full AI-assisted PBP with simplified match engines
- Only if technology allows without derailing core sim

---

## RELATED SYSTEMS

- [[Match Engine/_Match Engine Index|Match Engine]]: Provides simulation data
- [[Commentary Hooks]]: Generates flavor text
- [[Tags_System]]: Tag-based highlight modifiers
- [[Emotional_Show_Flow]]: Crowd reaction data
- Show Reporting: Aggregates match presentations

---

**Document Status:** Locked (Vol 2 extraction)  
**Last Updated:** 2025-12-25  
**Next Review:** Integration with Show Reporting system
