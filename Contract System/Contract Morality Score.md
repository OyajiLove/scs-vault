# Contract Morality Score

📛 **MECHANIC:** Contract Morality Score
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** fairness, exploitation, labour ethics, reputation, trust, hidden scoring
📌 **ORIGIN:** Vol 4 (described in "BONUS: CONTRACT MORALITY SCORE" section)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

A hidden score attached to each contract measuring its ethical fairness. This isn't visible to players directly but influences worker morale, union trust, agent suggestions, and media commentary. Exploitative contracts have consequences; fair deals build loyalty.

---

## Morality Score Components

| Factor | Weight | Description |
|--------|--------|-------------|
| **Fairness vs. Push** | High | Pay relative to actual booking usage |
| **Clause Balance** | Medium | Worker protections vs. promotion control |
| **Pay vs. Tier** | Medium | Compensation compared to industry standard for tier |
| **Post-Signing Behavior** | High | How promotion treats worker after signing |
| **Merch Cut Fairness** | Medium | Revenue share relative to sales contribution |

---

## Score Ranges

| Range | Rating | Meaning |
|-------|--------|---------|
| 85-100 | Excellent | Worker treated exceptionally well |
| 70-84 | Good | Fair deal, no major complaints |
| 50-69 | Neutral | Standard contract, some minor issues |
| 30-49 | Poor | Worker getting squeezed |
| 0-29 | Exploitative | Carny bullshit, major morale/trust impact |

---

## Score Calculation

```
Base Score starts at 50 (neutral)

Modifiers:
+ Pay matches or exceeds tier standard: +10 to +20
+ Merch cut is 50%+: +5 to +15
+ Push promise kept: +10
+ Title opportunity honored: +10
+ Creative control respected: +10
- Pay below tier standard: -10 to -20
- Merch cut below 30%: -5 to -15
- Push promise broken: -15
- Buried creatively despite contract: -20
- Fired without cause (non-union): -25
- Public humiliation: -30
```

---

## What Morality Score Affects

### Worker Morale
Low morality score = faster morale decay, harder to maintain satisfaction

| Score Range | Morale Effect |
|-------------|---------------|
| 85-100 | +10 baseline morale |
| 70-84 | +5 baseline morale |
| 50-69 | No modifier |
| 30-49 | -10 baseline morale |
| 0-29 | -20 baseline morale, active resentment |

### Union Trust
If union exists, contract morality affects collective trust:

| Score Range | Union Trust Effect |
|-------------|-------------------|
| 85-100 | Union sees promotion as good-faith partner |
| 70-84 | Neutral relations |
| 50-69 | Union watchful, minor grievances |
| 30-49 | Union hostile, investigations likely |
| 0-29 | Union war, strikes possible, public campaigns |

### Agent Suggestions
Worker's agent (if any) reacts to contract morality:

| Score Range | Agent Behavior |
|-------------|----------------|
| 85-100 | Agent recommends loyalty, long-term deals |
| 70-84 | Agent neutral |
| 50-69 | Agent suggests renegotiation |
| 30-49 | Agent advises seeking other offers |
| 0-29 | Agent pushing for immediate exit |

### Media Commentary
Wrestling press and social media react:

| Score Range | Media Effect |
|-------------|--------------|
| 85-100 | Praise for worker treatment |
| 70-84 | No commentary |
| 50-69 | Occasional questions about fairness |
| 30-49 | "Reports of unhappy workers" leaks |
| 0-29 | Exposes, boycott calls, PR crisis |

---

## Tracking Over Time

Contract morality isn't static. It changes based on:

| Event | Score Change |
|-------|--------------|
| Promise kept | +5 to +10 |
| Promise broken | -10 to -20 |
| Raise given proactively | +10 |
| Raise denied despite success | -10 |
| Worker protected during scandal | +15 |
| Worker scapegoated | -25 |
| Clean exit handled well | +10 |
| Messy public firing | -20 |

---

## Hidden From Player

Players don't see exact morality scores, but they experience effects:
- Agent warns about "unhappy workers"
- Media reports on "backstage unrest"
- Union files grievances
- Workers' mood indicators shift
- Exit interviews reveal frustrations

This creates emergent storytelling: you may not know exactly why morale is low, forcing you to investigate your own practices.

---

## Connected Mechanics

- [[Morale System]] - Morality directly affects morale baseline
- [[Worker Resistance]] - Low morality triggers pushback
- [[Union System]] - Collective morality affects union relations
- [[Scandal System]] - Exploitation can become public scandal
- [[Hidden Personality]] - Morality trait affects worker's tolerance

---

## Open Questions

- [ ] Exact weight values for each morality component
- [ ] How long negative events affect score (decay over time?)
- [ ] Promotion-wide morality score vs. per-contract scores
- [ ] Player access to morality indicators (full hidden vs. hints)

---

## Implementation Notes

```json
{
  "contract_morality": {
    "contract_id": "contract_001",
    "base_score": 50,
    "current_score": 62,
    "components": {
      "pay_fairness": 8,
      "clause_balance": 5,
      "tier_comparison": 3,
      "post_signing_behavior": -4,
      "merch_cut_fairness": 0
    },
    "effects": {
      "morale_modifier": 0,
      "union_trust_modifier": 0,
      "agent_stance": "neutral",
      "media_risk": "low"
    },
    "history": [
      { "event": "push_promise_kept", "change": +10, "date": "1985-06-15" },
      { "event": "raise_denied", "change": -8, "date": "1985-09-01" }
    ]
  }
}
```
