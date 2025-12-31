# Memory Snapshots

📛 **MECHANIC:** Memory Snapshots
🔗 **PARENT SYSTEM:** [[_Fan Memory Index|Fan Memory Engine]]
🧭 **CATEGORY:** Crowd Psychology / Long-Term Tracking
🔑 **KEYWORDS:** snapshots, memorable moments, high-emotion events, permanent memory
📌 **ORIGIN:** Vol 5-6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5-6 | 🔒 LOCKED |

---

## Overview

Memory Snapshots are discrete memories created when high-emotion events occur. They capture the moment, the participants, and the emotional tone, then persist in the fan memory system.

---

## Snapshot Triggers

### General Triggers

| Event Type | Emotion Required |
|------------|------------------|
| Title change | High (surprise or catharsis) |
| Betrayal | Very High (shock) |
| Return from absence | High (nostalgia + surprise) |
| Career-defining match | Very High (awe) |
| Retirement | High (closure) |
| Death (in-universe or real) | Permanent snapshot |
| Controversial moment | High (outrage or confusion) |

### Vol 6 Trigger Categories (with Memory Weights)

| Trigger Type | Description | Memory Weight |
|--------------|-------------|---------------|
| 🔥 **Peak Buzz + Emotional Tag** | Match or angle hits Buzz 16+ and carries tags like Catharsis, Betrayal, Redemption | High |
| 🕊 **Career Moment** | Retirement, return from injury, breaking losing streak, unmasking, etc. | Medium-High |
| 🩸 **Cultural Shock** | Violent match, screwjob, pipebomb, deathmatch moment | Medium |
| ❤ **Emotional Loyalty Turn** | Betrayal or alliance that splits fanbases | High (if sustained) |
| 🏟 **Historic Setting** | Big venue, anniversary show, famous territory | Memory Multiplier |

---

## Snapshot Components

| Component | Description |
|-----------|-------------|
| **Event** | What happened |
| **Participants** | Who was involved |
| **Emotional Tone** | Joy, shock, rage, sadness, etc. |
| **Context** | Show, date, circumstances |
| **Intensity** | How strong the memory is |
| **Valence** | Positive or negative |

---

## Snapshot Types

| Type | Duration | Examples |
|------|----------|----------|
| **Permanent** | Never decays | Deaths, retirements, once-in-lifetime moments |
| **Long-term** | Years to decay | Title changes, betrayals, major feuds |
| **Medium-term** | Months to decay | Good matches, memorable promos |
| **Short-term** | Weeks to decay | Weekly show moments |

---

## Simulation Effects of Snapshots

What happens when a snapshot is created:

| Effect | Outcome |
|--------|----------|
| **Legacy Boost** | Helps Hall of Fame voting, endgame contracts |
| **Fanbase Loyalty Surge** | Crowd sticks with them through cold periods |
| **Pop Decay Reduction** | Their Popularity fades more slowly |
| **AI Booker Reconsideration** | Some AI bookers give them another chance due to history |
| **Promo Fuel** | Can be referenced in future segments ("He never forgot that night in Osaka...") |
| **Feud Rekindling Trigger** | Used to restart old rivalries ("unfinished business") |

---

## System Integration

| System | Connection |
|--------|------------|
| **[[Buzz System/_Buzz System Index\|Buzz]]** | Buzz 15-20 with emotional tag required to trigger most snapshots |
| **[[_Fan Memory Index\|Fan Memory Engine]]** | Stores 3-10 top memories per worker depending on career length |
| **Promotion Legacy** | Snapshot moments improve company reputation ("remember that legendary feud in 2026?") |
| **Push Conflict Logic** | AI might say "they've cooled, but the fans still believe..." |

---

## Snapshot Creation Example

```
EVENT: Hangman Page wins AEW Title
PARTICIPANTS: Hangman, Omega
TONE: Catharsis, redemption
CONTEXT: Full Gear 2021
INTENSITY: 95
VALENCE: Positive
TYPE: Long-term
```

---

## Fictional Worker Examples (Vol 6)

| Worker Name | Snapshot Type | Tags | Long-Term Impact |
|-------------|---------------|------|------------------|
| **"The Hollow Saint" Sera Koizumi** | Refused to tap in 38-minute epic | Courage + Buzz 18 | Legacy-defining snapshot |
| **"Diamond" Darren Holt** | Screwed in title match with fake ref | Betrayal + Buzz 16 | Years-long feud anchor |
| **"Big Gun" Sal Devlin** | Moonsault in bloody deathmatch | Spectacle + Nihilism + Buzz 17 | Permanent aura boost |

> "That night she refused to tap to the armbar in front of her hometown crowd — even in a loss — is still her most remembered moment."

---

## Connected Mechanics

- [[Memory Aging]] - how snapshots decay
- [[Memory Reactivation]] - how snapshots resurface
- [[Buzz Spikes and Crashes]] - spike events create snapshots

---

## Open Questions

- Maximum snapshots per worker?
- Snapshot merging (similar events combining)?
- Snapshot inheritance (new fans adopting old memories)?

---

## Implementation Notes

```json
{
  "snapshot": {
    "snapshot_id": "snap_001",
    "event_type": "title_change",
    "participants": ["w_hangman", "w_omega"],
    "emotional_tone": ["catharsis", "redemption"],
    "context": {
      "show": "full_gear_2021",
      "date": "2021-11-13"
    },
    "intensity": 95,
    "valence": "positive",
    "snapshot_type": "long_term",
    "decay_rate": 0.02
  }
}
```
