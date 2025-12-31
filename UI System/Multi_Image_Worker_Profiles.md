# Multi-Image Worker Profiles

📛 **NAME:** Multi-Image Worker Profiles
🧭 **CATEGORY:** UI System, Visual Identity
🔑 **KEYWORDS:** renders, portraits, entrance, ring gear, alt looks, image gallery
📝 **SUMMARY:** Optional extended render system allowing workers to have multiple visual representations (entrance, ring gear, legacy), navigable via arrows or swipes in their full profile.

📌 **ORIGIN:** Vol 7 (Lines 195-198)
✅ **STATUS:** Locked (Provisional) — pending fine-tuning

---

## Overview

Each worker can have **multiple assigned renders**, viewable via arrow tabs or swipes in their full profile.

This is especially valuable for characters with elaborate presentations or evolving personas (e.g., Kuchisake Onna whose mask/veil only appears for entrances).

---

## Image Types

| Type | Description | Use Case |
|------|-------------|----------|
| **Default Portrait** | Used for hover pop-ups, aligned to autocrop standards (face near top center) | Quick reference, match cards |
| **Entrance Attire** | Stylized render emphasizing grandeur, accessories, attitude | Veil, mask, cloak, ornate robes |
| **Ring Gear** | Tighter, functional gear render showing in-ring presence | Actual wrestling attire |
| **Legacy Look / Alt Gimmick** | Great for retired legends or workers who drastically change over time | Career timeline, gimmick changes |

---

## Technical Notes

- **No hardcoded order** — but labeling in UI ("Entrance," "Ring Gear," etc.) is helpful if assigned
- **Stored locally** in worker profile data — no need for image IDs or online syncing
- **Default render** still drives facial pop-up previews (autocrop logic applies only to this one)
- **Navigation UI:** left/right arrows, swipe gesture, or thumbnail strip depending on platform

---

## Why This Matters

**For characters like Kuchisake Onna:**
- Mask and veil look might only appear for entrances or promos
- Actual ring gear might show scars, weapons, or reveal the "truth" of the gimmick
- Having one render limits ability to show both without awkward compromises

**For characters like Don Sangre:**
- In-ring look (no shirt, oxblood tights)
- Entrance look (blood shroud towel)
- Different visual identity for different contexts

---

## Fine-Tuning Needed Before Full Commit

1. **Tagging system** — naming logic for extra renders ("default", "entrance", "ring", "legacy")
2. **Contextual use** — whether render switching is purely cosmetic or if some views are used in specific game contexts (news, entrances, match cards)
3. **Pipeline integration** — Ringstate-style render generation could queue multiple prompts at once during worker creation

---

## Implementation Notes

```
worker_renders: {
  default: "filename_default.png",     // Required
  entrance: "filename_entrance.png",   // Optional
  ring_gear: "filename_ring.png",      // Optional
  legacy: "filename_legacy.png"        // Optional
}
```

---

## Related Systems

- [[Newgen_Portrait_System]] — Render generation pipeline
- [[Worker_Profile_UI]] — Profile display system

---

**Document Status:** Locked (Provisional)
**Next Review:** Fine-tune tagging system, contextual use decisions
