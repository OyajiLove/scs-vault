# Trail Milestones

📛 **MECHANIC:** Trail Milestones
🔗 **PARENT SYSTEM:** [[_Booking Trails Index|Booking Trails]]
🧭 **CATEGORY:** Booking & Simulation / Long-Term Planning
🔑 **KEYWORDS:** milestones, emotional beats, story checkpoints, segment placeholders
📌 **ORIGIN:** Vol 5, Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Milestones are emotional checkpoints on a Booking Trail. They represent the *feeling* or *function* of a beat in the story, not fully scripted segments. Milestones get filled in with specific booking as each show approaches.

---

## Milestone Types

| Type | Function |
|------|----------|
| **Heat Builder** | Confrontation, brawl, promo exchange |
| **Stakes Raiser** | Title shot earned, contract signed, stipulation added |
| **Doubt Seed** | Setback, injury tease, ally friction |
| **Ally/Rival Shift** | New participant enters, betrayal hint |
| **Emotional Peak** | Moment of catharsis, revenge, or tragedy |
| **Resolution Setup** | Final promo, contract signing, face-off |

---

## Example Trail

**TRAIL TITLE:** Hangman's Redemption
**DESTINATION:** Title Win @ Winter Showdown

| Week | Milestone |
|------|-----------|
| Week 1 | "Loses tag match, doubts himself" |
| Week 2 | "Mentor promo + drinking tease" |
| Week 3 | "Brawl w/ titleholder" |
| Week 5 | "Wins #1 contender" |
| Week 6 | "Backstage silent stare" |
| Week 8 | **TITLE MATCH** (Destination) |

---

## Live Edit Features

| Feature | Function |
|---------|----------|
| **Drag segments** | Move a segment to a new show |
| **Revise destination** | Change the destination match without deleting the trail |
| **Split trails** | Break into Mini-Trails (e.g., prelude arc, then pivot after a twist) |
| **Merge trails** | Combine two converging storylines |
| **Abandon trail** | Mark as failed/cancelled (affects [[Fan Memory Engine/_Fan Memory Index|Fan Memory]]) |

---

## Connected Mechanics

- [[Trail Planning]] - where milestones get created
- [[Trail Templates]] - pre-built milestone sequences
- [[Trail Failure]] - what happens when milestones are missed

---

## Open Questions

- Maximum milestones per trail?
- Can milestones be conditional (if X happens, do Y)?

---

## Implementation Notes

```json
{
  "milestone_id": "ms_003",
  "trail_id": "tr_001",
  "week": 3,
  "type": "heat_builder",
  "description": "Brawl w/ titleholder",
  "status": "placeholder",
  "segment_id": null
}
```
