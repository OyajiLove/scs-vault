# Trail Templates

📛 **MECHANIC:** Trail Templates
🔗 **PARENT SYSTEM:** [[_Booking Trails Index|Booking Trails]]
🧭 **CATEGORY:** Booking & Simulation / Long-Term Planning
🔑 **KEYWORDS:** templates, arc structures, heel turn, redemption, title chase, tag split
📌 **ORIGIN:** Vol 5, Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5, Vol 6 | 🔒 LOCKED |

---

## Overview

Pre-built arc structures for quick booking or AI use. Templates provide the emotional skeleton; player fills in the specific workers and segments.

---

## Heel Turn Arc

Build trust → moment of doubt → betrayal → aftermath

| Beat | Emotional Function |
|------|-------------------|
| Ally victory together | Establish trust |
| Friction hint (missed tag, stolen pin) | Plant seed |
| Near-betrayal swerve (saved at last second) | False relief |
| Full betrayal | Catharsis/shock |
| Aftermath promo | Define new dynamic |

---

## Redemption Arc

Fall from grace → struggle → test → triumph

| Beat | Emotional Function |
|------|-------------------|
| Major loss or humiliation | Starting point |
| Withdrawal/doubt period | Emotional low |
| Mentor or rival challenges them | Inciting incident |
| Failed attempt | Stakes raised |
| Final triumph | Catharsis |

---

## Title Chase

Establish contender → obstacles → near-miss → victory/defeat

| Beat | Emotional Function |
|------|-------------------|
| Impressive win over gatekeeper | Prove worthy |
| #1 contender match/tournament | Earn shot |
| Champion attacks/undermines | Build heat |
| Near-win (DQ, time limit, interference) | So close |
| Blow-off match | Resolution |

---

## Tag Split

Tension hints → blow-up → singles feud

| Beat | Emotional Function |
|------|-------------------|
| Miscommunication costs match | Seed planted |
| Argument backstage | Tension escalates |
| One partner succeeds solo | Jealousy trigger |
| In-ring confrontation | Breaking point |
| First singles match | New chapter |

---

## Injury Return Arc

Absence → tease → return pop → revenge match

| Beat | Emotional Function |
|------|-------------------|
| Injury angle (heel attack) | Create absence |
| Video packages during recovery | Maintain memory |
| Surprise return | Pop spike |
| Revenge promo | Set destination |
| Blow-off match | Catharsis |

---

## Retirement Run

Announcement → tribute matches → final opponent → farewell

| Beat | Emotional Function |
|------|-------------------|
| Retirement announcement | Begin countdown |
| Tribute match vs old rival | Nostalgia |
| Torch-pass match vs young star | Legacy |
| Final match | Closure |
| Ceremony segment | Emotional farewell |

---

## Passing the Torch

Legend tests protégé → protégé fails → grows → succeeds

| Beat | Emotional Function |
|------|-------------------|
| Legend acknowledges potential | Establish dynamic |
| First test (loss or disappointment) | Not ready yet |
| Growth period | Character development |
| Second test (near-victory) | Almost there |
| Final confrontation | Torch passed |

---

## Connected Mechanics

- [[Trail Planning]] - templates applied during planning
- [[Trail Milestones]] - templates are milestone sequences
- [[Road Agent Suggestions]] - AI can recommend templates

---

## Open Questions

- Custom template creation by player?
- Template success rate tracking?

---

## Implementation Notes

```json
{
  "template_id": "tmpl_heel_turn",
  "name": "Heel Turn Arc",
  "beats": [
    {"order": 1, "type": "trust_build", "description": "Ally victory together"},
    {"order": 2, "type": "doubt_seed", "description": "Friction hint"},
    {"order": 3, "type": "false_relief", "description": "Near-betrayal swerve"},
    {"order": 4, "type": "climax", "description": "Full betrayal"},
    {"order": 5, "type": "aftermath", "description": "Aftermath promo"}
  ],
  "recommended_length_weeks": 6
}
```
