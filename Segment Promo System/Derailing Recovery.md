# Derailing Recovery

📛 **MECHANIC:** Derailing Recovery
🔗 **PARENT SYSTEM:** [[_Segment Promo Index|Segment & Promo System]]
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** derailing recovery, crowd hijack, lean into it, acknowledge pivot, fight crowd, promo save
📌 **ORIGIN:** Vol 7 (Promo Response System)
✅ **STATUS:** Locked

---

## Overview

Options when crowd hijacks a segment. Recovery choice affects whether segment can be salvaged, and has different risk/reward profiles. Best performers can turn derails into memorable moments.

---

## Recovery Options

| Option | Description | Risk | Reward |
|--------|-------------|------|--------|
| **Lean Into It** | Adopt crowd's energy, use their chants | Low | Turns crowd from enemy to ally |
| **Acknowledge and Pivot** | Address what's happening, redirect | Medium | Can save segment with new direction |
| **Fight the Crowd** | Double down, oppose their energy | High | Can create nuclear heat or total disaster |
| **Walk Off** | Abandon segment, exit | Low | Loses moment but stops bleeding |
| **Bring in Help** | Manager/partner intervenes | Medium | Shifts focus, may save or muddy |
| **Embrace the Chaos** | Turn segment into brawl/angle | Medium | Salvages through action, not words |

---

## Lean Into It

**When it works:**
- Crowd chanting something usable
- Worker has charisma to ride the wave
- Energy can be redirected positively

**Examples:**
- "What?" chants → Worker pauses intentionally, uses rhythm
- "You suck!" → Heel agrees, adds fuel
- "Boring!" → "You think THIS is boring? Wait until I..."

**Success factors:**
- High Crowd Connection skill
- Improvisational ability
- Ego low enough to adapt

**Outcome if successful:** Crowd becomes invested, segment recovers to Solid or better

---

## Acknowledge and Pivot

**When it works:**
- Clear reason for crowd's reaction
- Worker can address it without breaking character
- Alternative content ready

**Examples:**
- "I hear you want [other worker]. Well, let me tell you why THEY should be scared of ME."
- "Yeah, this is going long. Let me get to the point."
- Breaking into physical action instead of continuing promo

**Success factors:**
- Medium+ Mic Skills
- Good Ring Psychology (reading the room)
- Booking flexibility

**Outcome if successful:** Segment salvaged, may even create callback moment

---

## Fight the Crowd

**When it works:**
- Heel character who benefits from rejection
- Crowd energy can be channeled into heat
- Worker has presence to dominate room

**When it fails:**
- Face trying to fight crowd (disaster)
- Worker doesn't have presence
- Crowd too hostile to engage

**Examples:**
- "Boo all you want, it doesn't change the FACT that..."
- "Every single one of you PAID to see me!"
- Deliberate antagonism, playing into villain role

**Success factors:**
- Very high Mic Skills
- Heel alignment
- Strong character work
- [[Hidden_Personality|Ego]] actually helps here

**Outcome range:** Nuclear heel heat (best) to X-Pac heat (worst)

---

## Walk Off

**When appropriate:**
- Segment unsalvageable
- Continuing would damage worker further
- Strategic retreat

**Execution:**
- Stay in character (angry heel storms off, frustrated face shows emotion)
- Don't break fourth wall
- Can be written into story

**Risk:** Looks like defeat, but sometimes necessary

**Outcome:** Damage limited, moment lost, may need story explanation

---

## Bring in Help

**Options:**
- Manager takes over talking
- Tag partner creates distraction
- "Music hits" interruption
- Authority figure intervention

**When it works:**
- Helper has better crowd rapport
- Interruption feels organic
- Shifts to action/confrontation

**Risk:** Can feel like bailout, may damage primary worker's credibility

**Outcome:** Segment focus shifts, original performer protected but potentially diminished

---

## Embrace the Chaos

**Execution:**
- Abandon promo, start brawl
- Bring out opponent for physical confrontation
- Turn verbal segment into angle

**When it works:**
- Crowd wants action
- Opponent available
- Story supports escalation

**Examples:**
- Contract signing → Table flip → Brawl
- Interview → Attack from behind
- Promo → "Get out here and face me!"

**Outcome:** Saves through action, promo failure forgotten if brawl delivers

---

## Recovery by Worker Type

| Worker Type | Best Recovery | Worst Recovery |
|-------------|---------------|----------------|
| **Charismatic Heel** | Fight the Crowd, Lean Into It | Walk Off |
| **Technical Face** | Acknowledge and Pivot, Embrace Chaos | Fight the Crowd |
| **Comedy Character** | Lean Into It | Fight the Crowd |
| **Monster Heel** | Walk Off (menacing), Embrace Chaos | Acknowledge and Pivot |
| **Underdog Face** | Lean Into It, Embrace Chaos | Fight the Crowd |
| **Authority Figure** | Acknowledge and Pivot | Lean Into It |

---

## Post-Recovery Effects

| Recovery Outcome | Effect |
|------------------|--------|
| **Successful save** | Segment upgrades 1-2 tiers |
| **Partial save** | Limits damage, neutral outcome |
| **Failed recovery** | Worse than not trying |
| **Memorable save** | Creates positive memory anchor |

---

## Learning from Derails

System tracks:
- Which workers get derailed often
- Which recovery methods they use
- Success rate by method
- Crowd types that derail them

Can inform future booking:
- Shorter promos for derail-prone workers
- Manager assignment
- Different segment types
- Crowd composition awareness

---

## Connected Mechanics

- [[Promo Response]] - triggers recovery need
- [[Promo Evaluation]] - skills affect recovery success
- [[Segment Outcomes]] - post-recovery effects
- [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] - chant types determine options

---

## Open Questions

- Recovery success probability formula
- Multiple recovery attempts in one segment
- Training/improvement in recovery skills

---

## Implementation Notes

```json
{
  "derailing_recovery": {
    "segment_id": "seg_001",
    "derail_severity": "partial",
    "recovery_attempted": "lean_into_it",
    "worker_skills": {
      "mic_skills": 14,
      "crowd_connection": 16,
      "adaptability": 15
    },
    "crowd_chant_type": "what_chants",
    "recovery_roll": 72,
    "success_threshold": 65,
    "recovery_success": true,
    "segment_tier_change": 1,
    "final_outcome": "solid_segment",
    "memory_created": {
      "type": "positive",
      "note": "Handled crowd well, got them back"
    }
  }
}
```
