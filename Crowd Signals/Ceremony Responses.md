# Ceremony Responses

📛 **MECHANIC:** Ceremony Responses
🔗 **PARENT SYSTEM:** [[_Crowd Signals Index|Crowd Signals System]]
🧭 **CATEGORY:** Crowd Psychology / Audience Response
🔑 **KEYWORDS:** ceremony, retirement, tribute, mask retirement, posthumous, farewell
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

Crowd behavior at special events like retirements, tributes, and ceremonies. These moments have heightened emotional stakes and follow different rules than regular segments.

---

## Ceremony-Specific Signals

| Segment Type | Expected Signal |
|--------------|-----------------|
| **Mask Retirement** | "Thank you [Name]," silence during handoff, then eruption |
| **Final Match** | Standing ovation on entrance/exit, "You Still Got It" if performance lands |
| **Title Surrender** | Mixed chant + quiet acceptance or gasps |
| **Gimmick Death** | Booed if unearned; chanted for if earned; "One More Time" if crowd disagrees |
| **Posthumous Tribute** | Standing silence, ritual chant, funeral salute (10-bell, flowers, mask in ring) |

---

## Earned vs Unearned

| Ceremony Quality | Crowd Response |
|------------------|----------------|
| **Emotionally earned** | Full participation, tears, standing ovations |
| **Forced/premature** | Polite but hollow, scattered boos |
| **Wrong worker for moment** | Rejection, "We want [X]" chants |
| **[[Legacy Tracker/_Legacy Tracker Index|Legacy]] too low** | Awkward silence, go-away heat |

---

## Commentary Response Layer

Commentary interprets through cultural lens:

| Era/Region | Commentary Style |
|------------|------------------|
| **1980s US** | "This crowd is electric, they want blood!" |
| **1990s Japan** | "Listen to that silence... hanging on every hold." |
| **2020s UK** | "These fans are singing his name louder than his music!" |

---

## Regional Ceremony Expectations

| Region | Ceremony Norm |
|--------|---------------|
| **Japan** | Flowers, streamers, formal bows, tears acceptable |
| **Mexico** | Mask ceremonies sacred, family involvement expected |
| **US Modern** | Video packages, speeches, potential for hijacking |
| **UK** | Singalongs, community celebration feel |

---

## Connected Mechanics

- [[Signal Types]] - ceremonies trigger specific signal types
- [[Region Era Profiles]] - regional ceremony expectations
- [[Hall of Fame/Legend Status Effects|HOF Induction]] - induction ceremonies use these rules
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - ceremonies create permanent snapshots
- [[Gimmick System/Cultural Immortality|Cultural Immortality]] - immortal ceremonies have special weight

---

## Open Questions

- Ceremony hijacking mechanics (when does crowd reject the moment?)
- Multi-worker ceremonies (tag team retirements)
- Virtual/remote ceremony rules (pandemic era)
- Full ceremony booking mechanics
- Failed ceremony recovery options

---

## Ceremony Types & Triggers

| Ceremony | Trigger | Memory Impact |
|----------|---------|---------------|
| **Retirement** | Worker retirement | Permanent anchor |
| **Mask Handoff** | Lucha tradition, legacy transfer | Major memory event |
| **Tribute Show** | Death, major anniversary | Permanent anchor |
| **HOF Induction** | Hall of Fame ceremony | Permanent anchor |
| **Gimmick Funeral** | Character ending (Kane unmasking, etc.) | Major memory event |
| **Title Coronation** | First championship win | Moderate memory |
| **10 Bells** | In-memoriam tribute | Permanent anchor |

**Note:** Mask handoffs transfer legacy between workers, creating lineage chains.

---

## Implementation Notes

```json
{
  "ceremony_segment": {
    "segment_id": "seg_ceremony_001",
    "ceremony_type": "retirement",
    "worker_id": "w_001",
    "legacy_score": 82,
    "earned_status": true,
    "expected_signals": ["thank_you", "ritual_chant", "emotional_break"],
    "region": "japan",
    "ceremony_elements": ["flowers", "streamers", "formal_bow"],
    "crowd_response": {
      "intensity": 95,
      "tone": "reverent",
      "hijack_risk": 0.05
    }
  }
}
```
