# Promo Response

📛 **MECHANIC:** Promo Response
🔗 **PARENT SYSTEM:** [[_Segment Promo Index|Segment & Promo System]]
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** promo response, derailing, what chants, crowd hijack, smart crowd, casual crowd
📌 **ORIGIN:** Vol 7 (Promo Response System with derailing mechanics)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2-3 | 🔒 LOCKED |
| 2.0 | Vol 7 | 🔒 LOCKED |

---

## Overview

How crowds react to promos, including the risk of crowd hijacking. Integrates with [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] for era-locked behaviors. Smart crowds and casual crowds respond differently.

---

## Response Types

| Response | Description | Effect |
|----------|-------------|--------|
| **Engaged** | Crowd listening, reacting appropriately | Promo succeeds |
| **Hot** | Crowd intensely invested, big reactions | Promo excels |
| **Polite** | Listening but not invested | Promo neutral |
| **Bored** | Restless, quiet, side conversations | Promo failing |
| **Hostile** | Active rejection, boos, competing chants | Promo bombed |
| **Hijacked** | Crowd takes over, ignores performer | Promo derailed |

---

## Era-Locked Behaviors

Certain crowd behaviors only exist in certain eras:

| Behavior | Era | Region | Trigger |
|----------|-----|--------|---------|
| **"What?" chants** | 2001+ | US primarily | Pauses in promo, slow delivery |
| **"Boring!" chants** | All eras | US/UK | Long promos, poor content |
| **"You suck!" rhythmic** | 2000+ | US | Heel entrance, Kurt Angle style |
| **Silent treatment** | All eras | Japan | Disrespect or disappointment |
| **"We want [X]!" chants** | 1990+ | US/UK | Wrong person in segment |
| **Beach ball chants** | 2010+ | US | Complete disengagement |

See [[Crowd Signals/Region Era Profiles|Region Era Profiles]] for full era matrix.

---

## Smart Crowd vs Casual Crowd

| Crowd Type | Behavior | Risk |
|------------|----------|------|
| **Smart/Smark** | Analyzes booking, cheers workrate, ironic chants | High hijack risk |
| **Casual** | Reacts to face/heel, follows story | Low hijack risk |
| **Mixed** | Unpredictable, split chants | Medium hijack risk |
| **Hostile Smart** | Actively rejects pushed talent, meta-commentary | Very high hijack risk |

---

## Derailing Mechanics

When derailing risk exceeds threshold:

| Phase | Description |
|-------|-------------|
| **Warning Signs** | Scattered competing chants, restlessness |
| **Partial Derail** | Chants drowning out portions of promo |
| **Full Derail** | Crowd completely ignores performer, runs own show |
| **Hostile Takeover** | Crowd actively mocking performer |

---

## Derailing Triggers

| Trigger | Risk Increase |
|---------|---------------|
| **Long pauses** | Invites "What?" chants |
| **Slow pacing** | Crowd gets bored |
| **Weak content** | Nothing to react to |
| **Wrong worker for moment** | Crowd wants someone else |
| **Heel being too cool** | Ironic cheers, see [[Crowd Signals/Heat vs Hate|Heat vs Hate]] |
| **Repeated beats** | "We've heard this before" |
| **Ignoring crowd energy** | Fighting against natural reaction |

---

## Recovery Options

See [[Derailing Recovery]] for full details. Quick reference:

| Option | Risk | Reward |
|--------|------|--------|
| **Lean into it** | Low | Turns crowd ally |
| **Acknowledge and pivot** | Medium | Can save segment |
| **Fight the crowd** | High | Can escalate or backfire |
| **Walk off** | Low | Loses the moment |
| **Bring in help** | Medium | Shifts focus, may save |

---

## Regional Response Patterns

| Region | Tendency |
|--------|----------|
| **US (Smart markets)** | Quick to hijack, meta-aware |
| **US (Casual markets)** | More forgiving, face/heel reactive |
| **Japan** | Respectful silence until earned, devastating when disappointed |
| **UK** | Football chant culture, communal singalongs |
| **Mexico** | Passionate but traditional, rudo/técnico binary |

---

## Commentary Integration

Commentary adapts to crowd response:

| Response | Commentary Tone |
|----------|-----------------|
| Engaged | Sells the promo content |
| Derailing | Acknowledges crowd, tries to redirect |
| Hijacked | May break kayfabe slightly, damage control |
| Hostile | Sells heel heat (if heel) or concern (if face) |

---

## Connected Mechanics

- [[Promo Evaluation]] - quality determines response
- [[Derailing Recovery]] - options when derailed
- [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] - chant mechanics
- [[Crowd Signals/Region Era Profiles|Region Era Profiles]] - regional patterns

---

## Open Questions

- Exact derailing threshold formula
- Cross-regional crowd composition handling
- Social media era amplification of derails

---

## Implementation Notes

```json
{
  "promo_response": {
    "segment_id": "seg_001",
    "response_type": "partial_derail",
    "crowd_composition": {
      "smart": 0.6,
      "casual": 0.3,
      "hostile": 0.1
    },
    "era": "2010s",
    "region": "us_northeast",
    "derail_triggers": ["slow_pacing", "wrong_worker"],
    "active_chants": ["we_want_[worker_x]", "boring"],
    "recovery_attempted": "acknowledge_and_pivot",
    "recovery_success": true,
    "final_response": "polite"
  }
}
```
