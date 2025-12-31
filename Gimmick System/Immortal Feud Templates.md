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

## Cultural Immortal Feud Templates (Vol 6)

Not every rivalry is about hate. Some are about legacy, reverence... or proving you belong.

These feuds operate differently from typical angles:
- No betrayals
- No "heat"
- No title chase

Instead, they're about **spiritual inheritance**, **respect**, or **shaking the heavens to test your soul**.

### Vol 6 Template 1: Prove Yourself Feud

| Element | Description |
|---------|-------------|
| **Setup** | Rising star openly challenges immortal. No heel heat, just ambition. |
| **Tone** | Reverent but assertive |
| **Stakes** | Not a title. Recognition. |
| **Match Outcome** | Usually respectful loss for challenger. Can end in draw or surprise win if star is fully ready. |
| **Post-Match** | If challenger impressed, immortal may acknowledge them. Memory anchor created. |

### Vol 6 Template 2: The Spiritual Succession

| Element | Description |
|---------|-------------|
| **Setup** | Immortal handpicks their successor. Not a feud, a blessing. |
| **Tone** | Sacred. "I see myself in you." |
| **Stakes** | The right to carry the legacy forward |
| **Match Outcome** | Symbolic, not competitive. May involve tag match, not singles. |
| **Post-Match** | Mask passed, move inherited, commentary calls them "the next." |

### Vol 6 Template 3: One Final Test

| Element | Description |
|---------|-------------|
| **Setup** | Immortal issues one last challenge: who can survive their final trial? |
| **Tone** | Epic, career-capping |
| **Stakes** | The right to say "I wrestled them at their end" |
| **Match Outcome** | Often a clean immortal win. But the young worker's effort is canonized. |
| **Post-Match** | Both elevated. Retirement window opens for immortal. |

### Vol 6 Template 4: The Challenge Denied

| Element | Description |
|---------|-------------|
| **Setup** | A disrespectful star demands a match. Immortal refuses. |
| **Tone** | Humiliation for the challenger. Silent power from the immortal. |
| **Stakes** | Will the challenge ever be accepted? |
| **Match Outcome** | May never happen. If it does, immortal wins clean. |
| **Post-Match** | Challenger either learns humility... or doubles down (heat with fans, not immortal). |

### Vol 6 Template 5: Passing of the Flame

| Element | Description |
|---------|-------------|
| **Setup** | Immortal loses to someone they approve of. Intentional. |
| **Tone** | Bittersweet. "It was always going to be you." |
| **Stakes** | Legitimacy transfer. The torch literally passes. |
| **Match Outcome** | Clean loss, immortal sells it like death. |
| **Post-Match** | Embrace, tears, commentary shifts narrative: "A new era begins tonight." |

---

## Usage Notes (Vol 6)

- These feuds are **rare**
- Cooldown timers apply: one Final Test per year max per promotion
- Immortals must **agree** (AI workers with high Ego or Traditionalism may refuse based on prior disrespect)
- Player-controlled Immortals can set **"Final Gate Conditions"**: who may challenge them and when

> They don't feud to win. They feud to pass on the flame.
> These are the moments that build legacies for two souls at once.

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
