# Signal Types

📛 **MECHANIC:** Signal Types
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** signal types, chants, applause, silence, emotional break, angry chant
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

Categories of crowd responses in the simulation. Each signal type has distinct triggers, emotional meaning, and region/era availability.

---

## Signal Type List

| Signal Type | Description | Triggers |
|-------------|-------------|----------|
| **Unprompted Chant** | Fans begin chant with no prompt | Memory spike, organic moment |
| **Ritual Chant** | Recurring chant tied to worker or catchphrase | Legacy anchor, cultural connection |
| **Honor Clap** | Japanese-style measured applause | Respect moment, near-falls |
| **Silent Reverence** | No noise, on purpose | Retirement, mask handoffs, grief |
| **Emotional Break** | Visible tears, sobbing, gasps | Death angles, farewell losses |
| **Angry Chant** | Rejection ("Sellout," "You Screwed X") | Bad heel turn, booking betrayal |
| **Reclaim Chant** | Fans chanting for retired name/gimmick | Pushback against reboot, forced change |
| **Thank You [Name]** | Universal tribute call | Retirement, HOF, death shows |
| **This Is Awesome** | High-buzz peak moment chant | Region-locked: mostly Western fans |

---

## Signal Engine Checks

At any moment (especially ceremonies), the engine checks:

| Variable | Example |
|----------|---------|
| **Fan Type Distribution** | Hardcore, Traditionalist, Casual, Troll |
| **Region Style** | Japan = claps/silence; US = chants/heckles |
| **Booking Memory** | Has this angle been earned emotionally? |
| **[[Gimmick System/_Gimmick System Index|Gimmick]] State** | Iconic Lock, Immortal Status, Gimmick Death? |
| **Snapshot Activation** | Is this closing a memory arc? |
| **[[Legacy Tracker/_Legacy Tracker Index|Legacy]] Score** | 60+ = likely gratitude; 85+ = ritual chants almost guaranteed |
| **[[Popularity_System|Popularity]]** | Must match tone; fake tears for cold worker = rejection |

---

## Chants in Match Summaries

Chants appear in match write-ups for:

| Role | Function |
|------|----------|
| **Narrative Echoes** | Emotional shading |
| **Performance Feedback** | Signals when match over/underdelivered |
| **Angle Momentum Cues** | Tracks emotional crest |
| **[[Fan Memory Engine/_Fan Memory Index|Memory]] Triggers** | Unique chants create snapshots |
| **Booking Influence** | Soft push pressure on AI |

---

## Connected Mechanics

- [[Region Era Profiles]] - determines which signals are available
- [[Ceremony Responses]] - special signal rules for ceremonies
- [[Chant Memory]] - how signals persist over time
- [[Heat vs Hate]] - signal interpretation in modern era

---

## Open Questions

- Signal priority when multiple triggers fire simultaneously
- Signal fatigue (same chant too many times)
- Cross-promotion signal transfer

---

## Implementation Notes

```json
{
  "signal_event": {
    "show_id": "show_001",
    "segment_id": "seg_003",
    "signal_type": "ritual_chant",
    "text": "Goldberg! Goldberg!",
    "trigger": "legacy_anchor",
    "intensity": 18,
    "region_valid": true,
    "era_valid": true
  }
}
```
