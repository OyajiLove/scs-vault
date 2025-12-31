# Failed Coronation

📛 **NAME:** Failed Coronation
🧭 **CATEGORY:** Push System / Worker State
🔑 **KEYWORDS:** failed coronation, failed push, crowd rejection, recovery required, compounding failure
📝 **SUMMARY:** Failed Coronation is the state a worker enters after failing a Make or Break moment. The crowd is now actively skeptical, waiting to reject again. The worker has a limited window to attempt recovery before degrading to the terminal Floundering state.

---

## Entry Conditions

A worker enters Failed Coronation state after:
- 1+ Make or Break failures (DISAPPOINTING or DISASTER outcome)
- OR sustained False Popularity (6+ months) without breakthrough

---

## Effects

### Crowd Disposition
- **Skeptical:** Waiting to reject again
- **"Prove it" mentality:** But with very low expectations
- **"Told you so" ready:** Any stumble reinforces narrative

### Booking Challenges
- Normal booking doesn't move the needle
- Worker needs recovery action OR another Make or Break attempt
- Continuing same push = diminishing returns
- Each failure compounds difficulty

### Tags Applied
- "Failed Coronation"
- Previous "Manufactured Star" tag persists
- May gain "Flop Myth" tag if failure was spectacular

---

## Failure Count Tracking

Each additional failure in Failed Coronation state makes recovery harder:

| Failure Count | Crowd Resistance | Recovery Difficulty | Notes |
|---------------|------------------|---------------------|-------|
| 1st failure | Skeptical | Standard | All recovery options viable |
| 2nd failure | Hostile | Elevated | Heel turn or step back recommended |
| 3rd failure | Resigned | High | Only major changes work |
| 4th+ failures | Apathetic | Extreme | Complete reinvention or release |

---

## Recovery Window

Worker has **3-6 months** to attempt recovery action before degrading to [[Floundering_State]].

### Timeline
- **Month 1-2:** Decision point, recovery action should begin
- **Month 3-4:** Recovery in progress, results uncertain
- **Month 5-6:** Final window, success or degradation
- **Month 7+:** Without action, degrades to Floundering

### What Resets the Clock
- Beginning a recovery action (turn, step back, etc.)
- Another Make or Break attempt (success or failure)
- Time off (pauses clock, doesn't reset)

---

## Available Recovery Actions

| Recovery Type | Success Rate | Time Required | Best For |
|---------------|--------------|---------------|----------|
| **Heel Turn** | 70-80% | 1-3 months | Workers crowd wants to hate |
| **Step Back** | 50-60% | 6-12 months | Workers who need to rebuild |
| **Gimmick Tweak** | 40-50% | 3-6 months | Minor adjustments needed |
| **Complete Reinvention** | 60-70% | 6-18 months | Severe damage, fresh start needed |
| **Time Off + Return** | 50-70% | 3-12 months | Creates absence demand |
| **Push Through** | 10-20% | Years | Almost never works |

See [[Recovery_Protocols]] for detailed mechanics.

---

## Warning Signs

System should flag when worker is in danger:

| Warning | Trigger |
|---------|---------|
| "Recovery Recommended" | 2 months in Failed Coronation, no action |
| "Recovery Required" | 4 months in Failed Coronation, no action |
| "Floundering Imminent" | 6 months in Failed Coronation, no action |

---

## The Roman Example

**Roman Reigns Failure Chain:**

| Event | Match | Outcome | State |
|-------|-------|---------|-------|
| WM32 | vs HHH | Stinker | Failed Coronation #1 |
| WM33 | vs Undertaker | Disaster | Failed Coronation #2 |
| WM34 | vs Brock | Crowd checked out | Failed Coronation #3 |
| 2018-2019 | Various | Apathy | Floundering |
| 2020 | Tribal Chief | Complete reinvention | Recovery (finally) |

**Total Time in Failed States:** 5 years
**Recovery Method:** Complete reinvention + heel turn + time off + new faction

---

## Exit Paths

### Positive Exits

| Exit | Requirement | Result |
|------|-------------|--------|
| **Breakthrough** | Win next Make or Break (harder threshold) | Returns to Healthy Push |
| **Successful Recovery** | Complete recovery action | Returns to Healthy or Warning Zone |

### Negative Exits

| Exit | Requirement | Result |
|------|-------------|--------|
| **Degradation** | No recovery action for 6 months | Enters [[Floundering_State]] |
| **Release** | Company gives up | Career elsewhere |
| **Permanent Midcard** | Accepted lower position | Career continues at reduced level |

---

## LLM Integration

AI can:
- Generate crowd sentiment descriptions ("The fans haven't forgotten WrestleMania...")
- Suggest recovery options ranked by success probability
- Narrate the stakes of upcoming Make or Break attempts
- Flag when worker is approaching Floundering

---

## Implementation Data

```json
{
  "failed_coronation_state": {
    "worker_id": "string",
    "entry_date": "date",
    "entry_reason": "MAKE_OR_BREAK_FAILURE | SUSTAINED_FALSE_POP",
    "failure_count": integer,
    "months_in_state": integer,
    "recovery_action": {
      "type": "NONE | HEEL_TURN | STEP_BACK | GIMMICK_TWEAK | REINVENTION | TIME_OFF",
      "start_date": "date | null",
      "status": "NOT_STARTED | IN_PROGRESS | COMPLETED | FAILED"
    },
    "make_or_break_history": [
      {
        "event": "string",
        "outcome": "string",
        "date": "date"
      }
    ],
    "floundering_risk": "LOW | MEDIUM | HIGH | IMMINENT"
  }
}
```

---

## Connected Mechanics

- [[Make_or_Break]] - How workers enter this state
- [[Floundering_State]] - Where they go if no recovery
- [[Recovery_Protocols]] - How to escape
- [[False_Popularity]] - Previous state

---

**Document Status:** NEW (December 2025)
**Last Updated:** 2025-12-30
