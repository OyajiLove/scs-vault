# Road Agent Suggestions

📛 **MECHANIC:** Road Agent Suggestions
🔗 **PARENT SYSTEM:** [[_Booking Trails Index|Booking Trails]]
🧭 **CATEGORY:** Booking & Simulation / Long-Term Planning
🔑 **KEYWORDS:** road agent, AI suggestions, booking assistant, pattern check, warning flags
📌 **ORIGIN:** Vol 5, Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Optional AI assistant that provides booking logic recommendations during trail planning. Can be toggled on/off based on player preference. Named after real wrestling road agents who help structure matches and storylines.

---

## Suggestion Types

| Type | Example |
|------|---------|
| **Segment Suggestion** | "If you're running the tag split at Show 3, we could preview tension in a backstage shot at Show 2." |
| **Warning Flag** | "Careful: that betrayal is close to the anniversary show. Crowd might expect something bigger." |
| **Pattern Check** | Warns of emotional redundancy, burnout, or inconsistent logic |
| **Callback Opportunity** | "This worker has unfinished business with [X] from 6 months ago." |
| **Pacing Alert** | "Three consecutive brawl segments may fatigue the crowd." |

---

## Warning Categories

| Category | Checks For |
|----------|-----------|
| **Emotional Redundancy** | Same beat repeated without escalation |
| **Pacing Issues** | Too fast (burnout risk) or too slow (interest loss) |
| **Logic Gaps** | Missing setup for planned payoff |
| **Calendar Conflicts** | Trail intersects with major shows awkwardly |
| **Character Conflicts** | Worker [[Hidden_Personality|personality]] clashes with planned arc |

---

## Agent Personality Modifiers

Different AI booker types give different suggestions:

| Booker Type | Suggestion Style |
|-------------|-----------------|
| **Traditionalist** | "The old way says we need a handshake before the turn." |
| **Chaos Artist** | "What if we skip the build and just have them brawl now?" |
| **Star Maker** | "This is a chance to elevate [young worker]. Give them the moment." |
| **Realist** | "The numbers say crowds lose interest after week 6 without a twist." |

---

## Toggle Options

| Setting | Effect |
|---------|--------|
| **Off** | No suggestions, full player control |
| **Passive** | Suggestions appear but don't interrupt |
| **Active** | Suggestions with confirmation prompts |
| **Aggressive** | AI flags issues and requests resolution |

---

## Connected Mechanics

- [[Trail Planning]] - where suggestions appear
- [[Trail Templates]] - AI can recommend templates
- AutoBooker - shares logic with Road Agent

---

## Open Questions

- Suggestion quality scaling with AI booker stats?
- Player trust/reputation affecting suggestion frequency?

---

## LLM Integration

Road Agent is a primary LLM integration point:
- Generates natural language suggestions
- Considers trail history, worker psychology, regional preferences
- Can explain reasoning if player asks "why?"

---

## Implementation Notes

```json
{
  "suggestion": {
    "trail_id": "tr_001",
    "type": "warning_flag",
    "message": "This betrayal is scheduled close to the anniversary show. Consider moving it to the bigger stage for maximum impact.",
    "severity": "medium",
    "dismissed": false,
    "booker_personality": "star_maker"
  }
}
```
