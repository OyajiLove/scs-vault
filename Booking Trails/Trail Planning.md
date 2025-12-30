# Trail Planning

📛 **MECHANIC:** Trail Planning
🔗 **PARENT SYSTEM:** [[_Booking Trails Index|Booking Trails]]
🧭 **CATEGORY:** Booking & Simulation / Long-Term Planning
🔑 **KEYWORDS:** destination match, planning window, milestones, calendar integration
📌 **ORIGIN:** Vol 5, Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Trail Planning is the process of creating a Booking Trail: choosing a destination, setting the timeline, and placing emotional milestones along the path.

---

## Step 1: Choose Your Destination

| Element | Options |
|---------|---------|
| **Match type** | Singles, tag, gimmick match, battle royal, etc. |
| **Participants** | Can evolve later; initial targets |
| **Target show** | PPV, TV special, house show |
| **Emotional tone** | Redemption, Betrayal, Coronation, Tragedy, Revenge, etc. |

---

## Step 2: Set the Planning Window

| Window | Use Case |
|--------|----------|
| 4 weeks | Hot angles, quick feuds |
| 8 weeks | Standard PPV build |
| 12 weeks | Epic arcs, major title programs |
| Custom | Long-term retirement runs, year-long stories |

Short trails = intense heat, risk of burnout
Long trails = slow burn, risk of losing crowd attention

---

## Step 3: Add Milestones

Milestones are emotional beats, not fully detailed segments:

- "Tag fallout"
- "Backstage brawl"
- "Title challenge refused"
- "Injury fakeout"
- "Surprise partner debut"

Milestones are placeholders that get filled in as you approach each show.

---

## UI Presentation Options

Player-selectable interface aesthetics per era or promotion tone:

| Interface | Era Feel |
|-----------|----------|
| 🗒 **Notebook** | Pre-Internet Era (handwritten look) |
| 💾 **Early PC** | 90s Booking Software UI (green text, DOS-style) |
| 📱 **Modern Calendar App** | Clean, mobile-friendly view |
| 📺 **TV Producer Board** | Post-Its and strings (corkboard style) |

---

## Calendar Integration

| Feature | Function |
|---------|----------|
| **Show dates visible** | Week/month view of scheduled shows |
| **Destination show marked** | "Glowing" or anchor icon on target date |
| **Click to plan** | Click any show to plan a Trail Segment |
| **Placeholder support** | Drop in moments like "heat-up promo" or "pull-apart brawl" |

### Visual Cue System

| Icon | Meaning |
|------|---------|
| 🔴 | Planned segment exists |
| 🟡 | Placeholder (needs detail) |
| 🟢 | Locked and confirmed booking |
| ⚪ | Open slot |

---

## Connected Mechanics

- [[Trail Milestones]] - the beats placed during planning
- [[Trail Templates]] - pre-built structures to start from
- [[Road Agent Suggestions]] - AI assistance during planning

---

## Open Questions

- Can trails be cloned/duplicated for similar storylines?
- Undo/revision history for trail edits?

---

## Implementation Notes

```json
{
  "trail_id": "tr_001",
  "destination": {
    "match_type": "singles_title",
    "participants": ["w_001", "w_002"],
    "target_show": "show_mania_2025",
    "emotional_tone": "redemption"
  },
  "planning_window_weeks": 12,
  "created_date": "2025-01-15",
  "status": "active"
}
```
