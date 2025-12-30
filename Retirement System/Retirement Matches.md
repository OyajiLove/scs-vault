# Retirement Matches

📛 **MECHANIC:** Booking Career-Ending Matches and Angles
🔗 **PARENT SYSTEM:** [[_Retirement System Index|Retirement System]]
🧭 **CATEGORY:** Booking / Worker Lifecycle
🔑 **KEYWORDS:** farewell match, retirement ceremony, last ride, career vs career, loser retires
📌 **ORIGIN:** Vol 1-4 (Match Stakes, Emotional Show Flow, Onita retirement example)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Retirement matches are among the most emotionally charged in wrestling. Done right, they crystallize a legacy and create permanent memory anchors. Done poorly, they tarnish careers. The system handles various retirement match types, booking considerations, and the unique emotional dynamics involved.

---

## Retirement Match Types

| Type | Description | Example |
|------|-------------|---------|
| **Ceremonial Farewell** | Planned final match with ceremony | Flair (WM24), Undertaker (Final Farewell) |
| **Career vs. Career** | Loser must retire | Flair/Michaels |
| **Loser Retires** | One-sided stipulation | Common in territories |
| **Surprise Final** | Unannounced last match | Rarely intentional |
| **Injury Exit** | Final match before injury retirement | Edge (first), Paige |
| **Deathmatch Farewell** | Extreme violence as goodbye | Onita style |
| **Quiet Final** | Last match without ceremony | Many |

---

## Match Booking Considerations

### Opponent Selection

| Opponent Type | Effect |
|---------------|--------|
| **Career Rival** | Maximum emotional weight |
| **Passing Torch** | Rising star goes over |
| **Legend vs. Legend** | Dream match closure |
| **Protege** | Symbolic passing |
| **Chosen Successor** | Endorsement of next era |

### Match Result

| Result | Legacy Impact |
|--------|---------------|
| **Clean Loss to Rising Star** | +15% (graceful exit) |
| **Clean Loss to Rival** | +10% (closure) |
| **Victory** | +5% (went out on top) |
| **Controversial Finish** | -5% to +5% (depends) |
| **Injury During Match** | Variable |
| **Poor Performance** | -10% to -20% |

---

## Emotional Beat Structure

Retirement matches follow specific emotional patterns:

| Phase | Description |
|-------|-------------|
| **Entrance** | Extended, dramatic, acknowledgment |
| **Early Match** | Showcase signature offense |
| **Struggle** | Can still fight, but showing age |
| **Near Falls** | False hope moments |
| **Final Sequence** | Acceptance, fighting spirit |
| **Finish** | Clean, decisive, respectful |
| **Post-Match** | Ceremony, speech, tribute |

---

## Stakes Modifiers

| Factor | Match Rating Boost |
|--------|-------------------|
| **Retirement Stipulation** | +15% to +25% |
| **Career Rival Opponent** | +10% to +15% |
| **Main Event Placement** | +10% |
| **Major Event (WrestleMania)** | +15% to +20% |
| **Career vs. Career** | +20% to +30% |
| **Torch Passing Story** | +10% |

---

## Ceremony Elements

| Element | Memory Impact |
|---------|---------------|
| **Video Package** | +10% memory strength |
| **Locker Room Appearance** | +15% |
| **Family in Ring** | +10% |
| **Rival Acknowledgment** | +15% |
| **Tears/Emotion** | +10% to +20% |
| **Final Pose/Gesture** | +5% |
| **Commentary Tribute** | +5% |

---

## Risk Factors

| Risk | Description |
|------|-------------|
| **Physical Decline Visible** | Undermines memory if too obvious |
| **Match Too Long** | Exposes limitations |
| **Wrong Opponent** | Lacks emotional resonance |
| **Botched Finish** | Ruins the moment |
| **Overshadowed** | Other events steal focus |
| **Crowd Not Invested** | Falls flat |

---

## Historical Examples

| Match | Elements | Memory Impact |
|-------|----------|---------------|
| **Flair vs. Michaels (WM24)** | Career vs. Career, rival respect, emotion | Legendary |
| **Undertaker Final Farewell** | Ceremony, legacy tribute, symbol burial | Very High |
| **Michaels vs. Undertaker (WM26)** | Career stipulation, callback, perfection | Legendary |
| **Onita Retirement Deathmatch** | Exploding ring, melodrama, tears | Legendary (cult) |
| **Sting vs. Undertaker (WM31)** | Injury during, abrupt ending | Low (tragic) |

---

## Booking Recommendations

### Do

- Match opponent to story significance
- Keep match length appropriate to physical capability
- Build emotional peaks, not just wrestling peaks
- Allow post-match ceremony time
- Involve meaningful figures (rivals, students, family)
- Let worker have input on their exit

### Don't

- Expose physical decline unnecessarily
- Rush the ceremony
- Overshadow with other storylines
- Force clean victory if loss serves story
- Book another major angle immediately after
- Ignore worker's legacy in the booking

---

## Crowd Memory Impact

Retirement matches have amplified memory effects:

| Match Quality | Memory Strength |
|---------------|-----------------|
| **Legendary (95+)** | Permanent, defining |
| **Excellent (85-94)** | 10+ years strong |
| **Good (75-84)** | 5-10 years |
| **Average (65-74)** | 2-5 years |
| **Poor (Below 65)** | May hurt legacy |

---

## Connected Mechanics

- [[Retirement Types]] - Type affects match booking
- [[Crowd Memory]] - Retirement as memory anchor
- [[Emotional Show Flow]] - Peak placement critical
- [[Match Rating]] - Stakes modifiers apply
- [[Hall of Fame System]] - Good farewell helps eligibility

---

## Open Questions

- [ ] How "worked" retirement matches differ
- [ ] Multiple retirement match handling (returns)
- [ ] Tag team retirement matches
- [ ] Faction retirement ceremonies
- [ ] Death during retirement match (extremely rare edge case)

---

## Implementation Notes

```json
{
  "retirement_match": {
    "match_id": "match_001",
    "retiring_worker": "worker_001",
    "opponent": "worker_042",
    "match_type": "career_vs_career",
    "result": {
      "winner": "worker_042",
      "method": "pin",
      "clean": true
    },
    "ceremony": {
      "video_package": true,
      "locker_room_appearance": true,
      "family_present": true,
      "speech_given": true,
      "rival_acknowledgment": ["worker_015", "worker_023"]
    },
    "base_rating": 88,
    "stakes_modifier": 1.25,
    "final_rating": 94,
    "memory_impact": "legendary",
    "legacy_modifier": 0.18
  }
}
```
