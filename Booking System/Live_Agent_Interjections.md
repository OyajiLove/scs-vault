# LIVE AGENT INTERJECTIONS

📛 **NAME:** Live Agent Interjections System  
🧭 **CATEGORY:** Booking UI / Agent Interaction  
🔑 **KEYWORDS:** agent feedback, booking assist, real-time suggestions, road agent, producer  
📝 **SUMMARY:**

You're not booking alone anymore, and they've got opinions. During the match/segment booking phase, trusted agents can interrupt with live feedback: soft suggestions, warnings, or subtle jabs based on their psychology, loyalty, your booking patterns, and information you may have overlooked.

⚙️ **LOGIC OVERVIEW:**

- Agents comment during active booking, not hard stops
- Comments based on agent psychology, loyalty, alignment, your patterns
- Can ignore, adjust, or consult further
- Trust grows or fades based on your response
- Ignoring too many warnings = agent loyalty may shift

🔬 **LLM INTEGRATION:** High (dynamic comment generation, tone variation)

📌 **ORIGIN:** Vol 3 lines 499-500

📎 **CONNECTED SYSTEMS:**
- [[Booker_Memory_Engine]] - Agents reference your patterns
- [[Agent Personality Archetypes]] - Comment tone matches personality
- [[Worker Foundation/Worker Morale]] - Agent insights include morale data
- [[Emotional_Show_Flow]] - Agents warn about pacing issues

❓ **OPEN QUESTIONS:**
- Interjection frequency cap?
- Can players disable interjections?
- Agent accuracy based on psychology skill?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 499-500 | 🔒 LOCKED |

---

## WHAT IT IS

During the match/segment booking phase, trusted agents can interrupt with live feedback.

**These aren't hard stops.** They're soft suggestions, warnings, or subtle jabs based on:

- Their psychology (Protective, Brutal, Passive)
- Their loyalty to you
- Their alignment with the match you're booking
- The [[Booker_Memory_Engine]] (referencing your patterns)
- Fatigue + morale insight you may have overlooked

---

## INTERJECTION EXAMPLES

| Context | Agent Line |
|---------|------------|
| Booking back-to-back 20+ minute matches | "You're giving the crowd a reason to sit down." |
| Booking a protected guy to lose again | "That's twice this tour. Are we sending a message?" |
| Booking a fresh team instead of agent's boys | "They've been working house shows hard. Just flagging it." |
| Booking a swerve finish too soon after last | "You're chasing shock again. That trick's still cooling." |
| Booking a worker the agent personally trained | "Just so you know, he tweaked that shoulder on the loop." |

---

## HOW IT WORKS

| Trigger | What Happens |
|---------|--------------|
| Booking engine detects a red flag | Agent comments appear as floating note or soft pop-up |
| Commentary pulled from agent profile | Tone, loyalty, memory-driven |
| You can ignore, adjust, or consult more | "Thanks," "What do you suggest?", "Let it ride." |
| Reactions remembered | Ignoring too many times? Agent loyalty may shift |
| Trust grows or fades | Smart booking based on advice = agent loyalty grows |

---

## AGENT COMMENT TONE BY ARCHETYPE

| Archetype | Interjection Style |
|-----------|-------------------|
| **The Veteran** | Gruff, mentorish, references "the old days" |
| **The Politicker** | Subtle, might have ulterior motives |
| **The Numbers Guy** | Data-driven, unemotional observations |
| **The Wild Card** | Creative, chaotic suggestions |
| **The Ghost** | Rare, cryptic, usually accurate |
| **The Psychology Nerd** | Technical, focused on match structure |
| **The TV Brain** | Timing-focused, segment pacing |
| **The Worker Protector** | Safety-first, morale-conscious |
| **The Shark** | Outcome-focused, may suggest burying talent |

---

## RESPONSE OPTIONS

| Response | Effect |
|----------|--------|
| **Acknowledge** | Agent feels heard, trust maintained |
| **Request Suggestion** | Opens alternative booking suggestion |
| **Ignore** | Agent notes it, may affect trust over time |
| **Dismiss Rudely** | Agent loyalty drops, may spread dissent |

---

## IMPLEMENTATION NOTES

### Interjection Trigger Structure

```json
{
  "interjection_id": "interject_001",
  "agent_id": "agent_brennigan",
  "trigger": "back_to_back_long_matches",
  "context": {
    "previous_match_length": 22,
    "current_match_length": 18,
    "crowd_stamina": 45
  },
  "message": "You're giving the crowd a reason to sit down.",
  "tone": "gruff_mentor",
  "severity": "warning",
  "player_response": null,
  "trust_at_stake": 3
}
```

### Agent Trust Tracking

```json
{
  "agent_id": "agent_brennigan",
  "trust_with_player": 72,
  "interjections_given": 15,
  "interjections_acknowledged": 11,
  "interjections_ignored": 4,
  "trust_trend": "stable"
}
```

---

## RELATED SYSTEMS

- **[[Booker_Memory_Engine]]:** Agents reference your patterns
- **[[Agent Personality Archetypes]]:** Determines comment tone
- **[[Emotional_Show_Flow]]:** Pacing warnings based on show structure
- **[[Worker Foundation/Worker Morale]]:** Agent insights include morale data

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Integration with booking UI
