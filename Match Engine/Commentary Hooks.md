# Commentary Hooks

📛 **MECHANIC:** Commentary Hooks
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Match Simulation / Presentation
🔑 **KEYWORDS:** commentary, announce team, play-by-play, color commentary, callbacks, history
📌 **ORIGIN:** Vol 1-2 (conceptual), LLM integration notes
✅ **STATUS:** 💭 CONCEPTUAL (Design Intent Only)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-2 | 📐 CONCEPTUAL |

---

## ⚠️ STATUS WARNING

This mechanic is **CONCEPTUAL**. General design intent exists but no specifications are locked. Captures vision for LLM-generated commentary.

---

## Design Intent

Commentary enhances match presentation by:
- Describing action
- Providing historical context
- Building drama
- Referencing feuds
- Acknowledging crowd reactions

LLM integration allows dynamic, contextual commentary rather than canned lines.

---

## Commentary Types

| Type | Purpose | Trigger |
|------|---------|---------|
| **Play-by-play** | Describe moves as they happen | Match flow |
| **Color commentary** | Analysis, opinion, hype | Between big moments |
| **Historical callback** | Reference past matches/feuds | Feud Memory data |
| **Psychology commentary** | Explain story being told | Match psychology tag |
| **Crowd acknowledgment** | React to crowd energy | Crowd state change |
| **Stakes reminder** | Emphasize what's on the line | Periodic |
| **Finish call** | Climactic moment | Match end |

---

## Data Hooks

Commentary draws from:

| Source | Commentary Use |
|--------|----------------|
| [[Feud_Memory\|Feud Memory]] | "These two have a history..." |
| [[Crowd_Memory\|Crowd Memory]] | "The fans remember that betrayal..." |
| Worker [[Tags_System\|Tags]] | "Known for his submission game..." |
| [[Match Types/House Styles\|House Style]] | "This is classic King's Road..." |
| [[Booking Trails/_Booking Trails Index\|Booking Trail]] | "This is what they've been building to..." |
| [[Predictability_Stakes\|Stakes]] | "Everything on the line here..." |
| Current match state | Momentum, near falls, injuries |

---

## Commentary Flavor by Era/Region

| Context | Flavor |
|---------|--------|
| **1980s Territory US** | Gordon Solie-style, measured, legitimizing |
| **1990s AJPW** | Emotional Japanese calls, escalating intensity |
| **Attitude Era WWE** | JR-style, emotional, "BAH GAWD" energy |
| **Modern US** | Meta-aware, acknowledges workrate |
| **Lucha** | Spanish passion, family lineage focus |
| **UK** | Technical appreciation, football crowd energy |

---

## Example Commentary Hooks

### Move Called
```
Input: Worker A hits vertical suplex on Worker B
Tags: Worker A has "Technical Wizard"
Output: "Beautiful vertical suplex by [A], textbook form from the technical master."
```

### Feud Reference
```
Input: Near fall in title match
Feud Memory: 6-month rivalry, Worker A screwed Worker B at last PPV
Output: "He's got him! No, kickout at two! You have to wonder if [B] is thinking about what happened three months ago..."
```

### Crowd Reaction
```
Input: Crowd energy shifts to "hot"
Match State: Face making comeback
Output: "Listen to this crowd! They're on their feet, they can feel it!"
```

### History Callback
```
Input: Finisher teased
Crowd Memory: Same move ended legendary match 5 years ago
Output: "He's going for it! The same move that ended their classic at [Event]!"
```

---

## Announce Team Personalities

Different commentators have different tendencies:

| Personality | Tendency |
|-------------|----------|
| **Historian** | References past, provides context |
| **Cheerleader** | Hype machine, sells everything big |
| **Analyst** | Technical breakdown, workrate focus |
| **Neutral** | Calls action without bias |
| **Biased** | Favors face or heel, adds drama |
| **Comedy** | Lightens mood, quips |

---

## Integration with LLM

**Prompt structure:**
```
Context: [Match state, participants, feud history, crowd energy]
Event: [What just happened]
Announce team: [Personality types]
House style: [Era/region]
Generate: [1-2 lines of commentary]
```

**Constraints:**
- Stay in character for era
- Reference relevant history naturally
- Match energy to crowd state
- Don't over-explain
- Avoid repetition

---

## Open Questions (Many)

- Real-time generation vs pre-generated pools?
- How often does commentary fire?
- Multiple voices coordination
- Text-to-speech integration (future)?
- Player control over commentary style
- Commentary for replays/highlights

---

## Connected Mechanics

- [[Match Simulation]] - provides events to commentate
- [[Feud_Memory|Feud Memory]] - history references
- [[Crowd_Memory|Crowd Memory]] - fan knowledge
- [[Match Types/House Styles|House Styles]] - flavor context
- [[Emotional_Show_Flow|Emotional Show Flow]] - crowd state

---

## Implementation Notes

```json
{
  "commentary_hook": {
    "status": "conceptual",
    "trigger": "vertical_suplex",
    "match_id": "m_001",
    "context": {
      "worker_a_tags": ["technical_wizard"],
      "feud_intensity": "high",
      "crowd_energy": "hot",
      "era": "1990s",
      "region": "japan"
    },
    "announcer_personality": "historian",
    "generated_line": "Beautiful vertical suplex form, reminiscent of the Funk dojo training.",
    "llm_model": "tbd",
    "generation_time_ms": "tbd"
  }
}
```
