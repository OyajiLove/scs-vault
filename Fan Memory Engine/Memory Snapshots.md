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

| Event Type | Emotion Required |
|------------|------------------|
| Title change | High (surprise or catharsis) |
| Betrayal | Very High (shock) |
| Return from absence | High (nostalgia + surprise) |
| Career-defining match | Very High (awe) |
| Retirement | High (closure) |
| Death (in-universe or real) | Permanent snapshot |
| Controversial moment | High (outrage or confusion) |

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
