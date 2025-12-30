# Immortal Feud Templates

📛 **MECHANIC:** Immortal Feud Templates
🔗 **PARENT SYSTEM:** [[_Gimmick System Index|Gimmick System]]
🧭 **CATEGORY:** Worker Identity / Presentation
🔑 **KEYWORDS:** immortal feuds, legend booking, torch passing, nostalgia feud
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

Special booking patterns for feuds involving [[Cultural Immortality|Cultural Immortals]] or high-tier [[Iconic Lock]] workers. These feuds follow different rules than normal booking due to the protected status of participants.

---

## Template Types

| Template | Purpose |
|----------|---------|
| **Torch Pass** | Legend elevates young star through defeat |
| **Final Chapter** | Retirement feud, definitive ending |
| **Nostalgia Collision** | Two legends meet (possibly for first/last time) |
| **Generation War** | Old guard vs new guard, meta-commentary |
| **Dream Match** | Fan fantasy booking made real |
| **Redemption Close** | Legend addresses past failure/controversy |

---

## Torch Pass Template

**Goal:** Elevate a younger worker by having them defeat or earn respect from an immortal.

| Beat | Function |
|------|----------|
| Legend dismisses challenger | Establish hierarchy |
| Challenger earns respect through persistence | Build credibility |
| Near-fall on legend | "Holy shit, they almost did it" |
| Clean victory OR mutual respect draw | Transfer of legitimacy |
| Post-match moment | Handshake, raise hand, symbolic gesture |

**Examples:** Flair/HHH, Hogan/Rock, Undertaker/Reigns

---

## Final Chapter Template

**Goal:** Give a legend a proper sendoff.

| Beat | Function |
|------|----------|
| Retirement announcement | Begin countdown |
| Career retrospective | Emotional investment |
| Final opponent selection | Must be meaningful |
| The match itself | Quality matters less than emotion |
| Post-match ceremony | Closure for fans and worker |

**Examples:** Ric Flair WM24, Shawn Michaels WM26, Undertaker Final Farewell

---

## Nostalgia Collision Template

**Goal:** Fantasy booking come to life, two legends who rarely/never faced each other.

| Beat | Function |
|------|----------|
| Unexpected encounter | Surprise pop |
| Verbal confrontation | Let them talk |
| Physical tease | Will they actually fight? |
| The match (if it happens) | Manage expectations carefully |
| Aftermath | Mutual respect or continued tension |

**Examples:** Hogan/Warrior II, Goldberg returns, Sting/Undertaker (never happened, always teased)

---

## Booking Rules for Immortals

| Rule | Reasoning |
|------|-----------|
| **Never bury** | Damages your product, not them |
| **Limit appearances** | Preserve specialness |
| **Protect finishes** | Clean losses must mean something |
| **Manage expectations** | In-ring work may be limited |
| **Prioritize moments** | One great moment > one great match |

---

## Connected Mechanics

- [[Cultural Immortality]] - who qualifies for these templates
- [[Iconic Lock]] - near-immortals use modified versions
- [[Trail Templates]] - these are specialized trail structures
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - immortal feuds create permanent snapshots

---

## Open Questions

- Immortal vs Immortal booking rules (who goes over?)
- Failed torch pass recovery (what if crowd rejects new star?)
- Posthumous immortal tributes (memorial feuds?)

---

## Implementation Notes

```json
{
  "feud_id": "fd_immortal_001",
  "template": "torch_pass",
  "immortal_participant": "w_undertaker",
  "challenger": "w_reigns",
  "destination_match": "wrestlemania_33",
  "planned_outcome": "clean_loss_immortal",
  "torch_pass_success_probability": 0.75,
  "memory_impact": "permanent_snapshot"
}
```
