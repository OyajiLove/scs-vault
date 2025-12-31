# Make or Break Moments

📛 **NAME:** Make or Break Moments
🧭 **CATEGORY:** Push System / Pivotal Events
🔑 **KEYWORDS:** make or break, coronation, breakthrough, crowd acceptance, pivotal match, prove yourself
📝 **SUMMARY:** When a worker in False Popularity state is booked into a major event main event, that match becomes a Make or Break Moment. The crowd is actively waiting to see if the worker can justify their push. Success = breakthrough and acceptance. Failure = worsening state and forced recovery.

📌 **ORIGIN:** External feedback from Mike Ferguson (December 2025), building on Roman Reigns/Shota Umino analysis

---

## Concept

The Make or Break Moment is the **coronation match**: the crowd is either going to accept the king or reject them.

When an overpushed worker gets their big showcase match, everything crystallizes. The crowd isn't passively watching, they're actively judging: "Can you actually deliver?"

---

## Trigger Conditions

Make or Break Match activates when **ALL** are true:

| Condition | Requirement |
|-----------|-------------|
| **Worker State** | Has "Manufactured Star" tag OR Push Gap ≥ 15 |
| **Event Tier** | Major event (PPV, supercard, Dome show, WrestleMania-level) |
| **Stakes Level** | Stakes Multiplier ≥ 1.5 (title match, blowoff, career stakes) |
| **Card Position** | Main event or semi-main event |

---

## Success Factors

The outcome depends on:

| Factor | Weight | Description |
|--------|--------|-------------|
| **Match Quality** | 40% | Did they deliver in-ring? |
| **Crowd Engagement** | 30% | Did the crowd get invested despite resistance? |
| **Storytelling** | 20% | Did the match tell a compelling narrative? |
| **Finish Execution** | 10% | Was the win satisfying, earned, believable? |

---

## Outcome Table

| Match Quality | Crowd Response | Outcome | Effect |
|---------------|----------------|---------|--------|
| 85+ | Engaged, buying in | **BREAKTHROUGH** | Gap closes 50-75%, tag removed, momentum spike |
| 70-84 | Neutral, mixed | **ADEQUATE** | Gap closes 10-20%, still on probation |
| 50-69 | Apathetic | **DISAPPOINTING** | Gap widens 10-15%, "Failed Coronation" tag added |
| <50 | Hostile, rejecting | **DISASTER** | Gap widens 20-30%, immediate crisis |

---

## BREAKTHROUGH: "They Won Me Over"

When overpushed worker **delivers** at Make or Break:

### Immediate Effects
- Push Gap reduced by 50-75%
- "Manufactured Star" tag removed
- "Proved the Doubters Wrong" tag applied (temporary positive modifier)
- Momentum spike: +25 to +40
- Crowd memory anchor: "Remember when they delivered at [Event]?"

### Long-term Effects
- Organic popularity growth resumes at normal rate
- Future booking has reduced resistance
- Can be pointed to as "the match that proved it"
- Worker has **earned** their spot (for now)

### Examples
- Roman vs Brock (WM31) was *working* before Seth's interference
- The match quality was good, crowd was starting to accept
- (Ironically, the cash-in may have prevented a true Breakthrough)

---

## FAILURE: "They Blew It"

When overpushed worker **fails** at Make or Break:

### Immediate Effects
- Push Gap widens by 10-30 points
- Momentum crash: -30 to -50
- "Failed Coronation" tag applied
- Crowd memory anchor: "Remember when they flopped at [Event]?"

### Long-term Effects
- Next Make or Break will be even harder (compounding difficulty)
- Crowd enters "told you so" mode
- Company must choose: recovery action or double down
- Worker enters [[Failed_Coronation]] state

### Examples
- Roman vs HHH (WM32): Bad match, crowd rejected, Failed Coronation #1
- Roman vs Undertaker (WM33): Even worse, "this is my yard" flopped, Failed Coronation #2
- Shota vs ZSJ (Wrestle Kingdom): Underwhelming, fans stopped caring

---

## ADEQUATE: "Still on Probation"

When the match is decent but not convincing:

### Effects
- Push Gap closes slightly (10-20%)
- Tags remain
- Worker gets another chance
- Not a failure, but not a success either

### Situation
- Crowd is still skeptical
- Company can try another Make or Break
- Or pivot to recovery action
- Clock is ticking

---

## Skill Factor (Open Question)

Should worker skill affect Make or Break threshold?

**Argument For:** Great workers are more likely to deliver a good match, so they should have easier threshold.

**Argument Against:** The crowd doesn't care about workrate if they don't believe in the character. Shota is a good worker but still failed.

**Current Implementation:** Match quality is a factor, so skilled workers have natural advantage, but it's not automatic.

---

## Compounding Difficulty

Each Make or Break failure makes the next one harder:

| Failure Count | Next Make or Break Threshold |
|---------------|------------------------------|
| 0 (first attempt) | Standard (85+ for Breakthrough) |
| 1 failure | Elevated (88+ for Breakthrough) |
| 2 failures | High (92+ for Breakthrough) |
| 3+ failures | Near impossible (95+ for Breakthrough) |

**Why:** Crowd's "told you so" mentality means they're actively looking for reasons to reject, not accept.

---

## Implementation Data

```json
{
  "make_or_break_event": {
    "worker_id": "string",
    "event_name": "string",
    "event_tier": "MAJOR | SUPERCARD | WRESTLEMANIA_TIER",
    "opponent_id": "string",
    "match_type": "string",
    "stakes_multiplier": float,
    "card_position": "MAIN_EVENT | SEMI_MAIN",
    "pre_match_gap": integer,
    "failure_count": integer,
    "match_result": {
      "quality_score": 0-100,
      "crowd_engagement": 0-100,
      "storytelling_score": 0-100,
      "finish_quality": 0-100
    },
    "outcome": "BREAKTHROUGH | ADEQUATE | DISAPPOINTING | DISASTER",
    "post_match_gap": integer,
    "tags_applied": ["string"],
    "tags_removed": ["string"],
    "memory_anchor_created": boolean
  }
}
```

---

## Connected Mechanics

- [[False_Popularity]] - State that triggers Make or Break
- [[Failed_Coronation]] - State after failure
- [[Push_Gap]] - Gap calculation
- [[Recovery_Protocols]] - Options after failure
- [[Predictability_Stakes]] - Stakes multipliers

---

**Document Status:** NEW (December 2025)
**Attribution:** Concept developed from Mike Ferguson feedback
**Last Updated:** 2025-12-30
