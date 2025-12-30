# Match Inputs

📛 **MECHANIC:** Match Inputs
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Match Simulation / Core Gameplay
🔑 **KEYWORDS:** match inputs, participants, match type, stakes, outcome, booking intent, agenting
📌 **ORIGIN:** Vol 1-2 (Booking Engine Phase 1)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-2 | 🔒 LOCKED |

---

## Overview

What the booker defines before a match runs. These inputs feed into [[Match Processing]] to generate quality and consequences. From [[Booking_Engine_P1-3|Booking Engine Phase 1]].

---

## Core Inputs

| Input | Description | Source |
|-------|-------------|--------|
| **Participants** | Workers, teams, managers, seconds, special refs | Roster database |
| **Match Type** | Singles, tag, ladder, cage, etc. | [[Match Types/Match Type Categories|Match Type Categories]] |
| **Card Placement** | Opener, midcard, semi-main, main, post-main | Show structure |
| **Stakes** | Title, grudge, tournament, retirement, pride, none | Booking decision |
| **Intended Outcome** | Who wins, how, clean vs dirty | Booking decision |
| **Booking Intent** | Why booked (elevate, cool down, test chemistry) | Booking philosophy |
| **Agenting/Flow** | Pacing notes, spots, interference | Match layout |

---

## Participants

| Field | Description |
|-------|-------------|
| **Workers** | 1-30+ (match type dependent) |
| **Teams** | Pre-formed or ad-hoc |
| **Managers** | Ringside presence, interference potential |
| **Seconds** | Support without manager role |
| **Special Referee** | Affects finish credibility |
| **Enforcer** | Outside interference agent |

---

## Card Placement

| Slot | Expectation | Risk |
|------|-------------|------|
| **Opener** | Hot start, wake crowd up | Wasted if crowd cold |
| **Early Midcard** | Building energy | Forgettable slot |
| **Midcard** | Story advancement | Can cool crowd |
| **Semi-Main** | High stakes, pre-main hype | Overshadowed by main |
| **Main Event** | Show peak, maximum attention | Highest scrutiny |
| **Post-Main** | Angle setup for next show | Crowd leaving risk |

---

## Stakes

From [[Predictability_Stakes|Predictability & Stakes]]:

| Stakes Type | Multiplier | Description |
|-------------|------------|-------------|
| **None (Filler)** | 0.5x | Nothing on the line |
| **Pride** | 1.0x | Personal glory |
| **Grudge** | 1.3x | Personal animosity |
| **Number One Contender** | 1.5x | Future title shot |
| **Title Match** | 1.8x | Championship on line |
| **Hair vs Hair** | 2.0x | Humiliation stakes |
| **Bloodline/Legacy** | 2.2x | Family honor |
| **Loser Leaves Town** | 2.5x | Career stakes |
| **Career vs Career** | 3.0x | Retirement match |
| **Mask vs Mask** | 3.5x | Sacred (lucha) |

---

## Intended Outcome

| Field | Options |
|-------|---------|
| **Winner** | Worker A, Worker B, Draw, No Contest |
| **Method** | Pin, Submission, Countout, DQ, KO |
| **Finish Style** | Clean, Dirty, Distraction, Roll-up, Interference |
| **Surprise Level** | Expected, Slight upset, Major upset, Shocking |

---

## Booking Intent

Why is this match happening?

| Intent | Description | Risk |
|--------|-------------|------|
| **Elevate talent** | Winner gains, loser protected | Obvious push |
| **Cool someone down** | Reduce overexposure | Crowd may reject |
| **Extend feud** | Build to bigger match | Repetition fatigue |
| **Payoff angle** | Blowoff match | Must deliver |
| **Test chemistry** | See if pairing works | Low stakes |
| **Send message** | Squash, burial, statement | Backfire risk |
| **Fill time** | Just need a match | Forgettable |

---

## Agenting/Flow Control

| Element | Description |
|---------|-------------|
| **Pace** | Fast, methodical, building |
| **Dominance balance** | Back-and-forth, one-sided, heel control |
| **Required spots** | Callbacks, signature moves, planned moments |
| **Avoid spots** | Injuries, overused moves, wrong crowd |
| **Interference timing** | Pre-planned run-ins |
| **Finish rehearsal** | How ending is executed |

---

## Promotion Philosophy Modifiers

From [[Booking_Engine_P1-3|Booking Engine]]:

| Setting | Effect on Inputs |
|---------|------------------|
| **Fan Engagement Target** | Who you're booking for |
| **Push Strategy** | How aggressively talent elevated |
| **Booking Tone** | Realism vs chaos vs comedy |
| **House Style Enforcement** | How strictly matches fit fed style |

---

## Connected Mechanics

- [[Match Processing]] - inputs feed processing
- [[Match Types/Match Type Categories|Match Types]] - type affects structure
- [[Booking_Engine_P1-3|Booking Engine]] - parent system
- [[Predictability_Stakes|Stakes]] - stakes multipliers

---

## Open Questions

- Automated vs manual agenting options
- Multi-match card optimization
- Emergency rebooking mid-show

---

## Implementation Notes

```json
{
  "match_input": {
    "match_id": "m_001",
    "participants": {
      "workers": ["w_001", "w_002"],
      "managers": ["w_003"],
      "special_ref": null
    },
    "match_type": "singles",
    "card_placement": "main_event",
    "stakes": {
      "type": "title_match",
      "title_id": "t_world_001",
      "multiplier": 1.8
    },
    "outcome": {
      "winner": "w_002",
      "method": "pin",
      "finish_style": "clean",
      "surprise_level": "slight_upset"
    },
    "booking_intent": "elevate_talent",
    "agenting": {
      "pace": "building",
      "dominance": "back_and_forth",
      "required_spots": ["signature_taunt", "callback_to_feud"],
      "interference": null
    }
  }
}
```
