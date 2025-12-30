# Road Agent Reports

📛 **MECHANIC:** Post-Match Feedback System
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Backstage / Match Analysis
🔑 **KEYWORDS:** road agent, agent, feedback, match report, effort, chemistry, safety
📌 **ORIGIN:** Vol 1 Extraction #120
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Road agents provide behind-the-scenes feedback on match quality, worker effort, and areas for improvement. This system surfaces information players need to make booking decisions while adding realism to the backstage simulation.

---

## Report Types (#120)

| Report Type | Content |
|-------------|---------|
| **Match Quality** | Technical assessment of in-ring performance |
| **Effort Level** | How hard workers tried (mailing it in vs. going all out) |
| **Chemistry Notes** | How well they worked together |
| **Safety Concerns** | Any reckless moments, near-injuries |
| **Suggestions** | Ideas for future matches, style adjustments |

---

## Report Content Examples

### Positive Report
> "Great chemistry between [Worker A] and [Worker B]. Both worked hard, story was clear. Crowd was hot for the finish. Recommend running this again."

### Concerning Report
> "[Worker A] seemed distracted tonight, match felt shorter than planned. [Worker B] carried most of the psychology. May want to check if something's going on backstage."

### Safety Report
> "[Worker A] working stiff tonight, caught [Worker B] with a hard elbow. No injury, but concerning pattern. Recommend conversation about working style."

---

## Agent Skill Effects

| Agent Quality | Report Accuracy | Hidden Info Revealed |
|---------------|-----------------|---------------------|
| **Elite** | 95%+ | Notes hidden morale, backstage issues |
| **Good** | 80% | Catches major issues reliably |
| **Average** | 60% | Misses subtle problems |
| **Poor** | 40% | Often wrong, miss obvious issues |

### Agent Bias

| Bias Type | Effect |
|-----------|--------|
| **Politically Motivated** | Protects favorites, buries enemies |
| **Style Preference** | Overrates workers matching their style |
| **Era Bias** | Old school agents may not appreciate modern styles |
| **Neutral** | Fair assessment across roster |

---

## Report Triggers

| Trigger | Report Generated |
|---------|------------------|
| Every match | Basic quality report |
| Unusual outcome | Detailed analysis |
| Safety incident | Immediate alert |
| Worker conflict | Backstage addendum |
| Major show | Comprehensive review |

---

## Information Surfacing

Road agent reports are a key way players learn about:

| Information | How It Appears |
|-------------|----------------|
| **Coasting workers** | "Effort seemed reduced" |
| **Hidden injuries** | "Moving slower than usual" |
| **Chemistry issues** | "Awkward transitions, not clicking" |
| **Potential stars** | "Really stepped up tonight, consider push" |
| **Morale problems** | "Seemed distracted, locker room chatter" |

---

## Chemistry Assessment Scale (Backstage Politics Merge)

| Chemistry Rating | Description |
|------------------|-------------|
| **Excellent** | Natural partners, should book together often |
| **Good** | Work well together, reliable pairing |
| **Average** | Functional, nothing special |
| **Poor** | Struggle to connect, awkward timing |
| **Dangerous** | Safety concerns, avoid future pairings |

---

## Report Visibility (Backstage Politics Merge)

| Recipient | What They See |
|-----------|---------------|
| **Player/Booker** | Full report with agent's assessment |
| **Workers** | Summarized feedback (can request full) |
| **Other Agents** | May share insights informally |
| **Promotion Archives** | Stored for historical reference |

---

## Feedback Loop Effects (Backstage Politics Merge)

| Report Content | Potential Outcome |
|----------------|-------------------|
| **High chemistry noted** | More pairings, potential feud/tag team |
| **Safety issues flagged** | Worker counseled, style adjustment required |
| **Low effort noted** | Morale check, contract implications |
| **Excellent performance** | Push consideration, title opportunity |
| **Deteriorating quality** | Medical exam suggested, career review |

---

## Historical Examples (Backstage Politics Merge)

| Agent | Known For |
|-------|-----------|
| **Pat Patterson** | Legendary match architect, trusted feedback |
| **Arn Anderson** | Technical excellence, honest assessment |
| **Michael Hayes** | Politically connected, faction-minded |
| **Fit Finlay** | Safety-focused, technical precision |

---

## Connected Mechanics

- [[Match Processing]] - Quality assessment feeds reports
- [[Match Consequences]] - Reports affect booking decisions
- [[Hidden_Personality]] - Agent personality affects bias
- [[Backstage Politics System/_Backstage Politics System Index|Backstage Politics]] - Political agents play favorites

---

## Implementation Notes

```json
{
  "road_agent_report": {
    "match_id": "m_001",
    "agent_id": "agent_005",
    "agent_quality": "good",
    "agent_bias": "neutral",
    "report": {
      "match_quality": 78,
      "effort_assessment": {
        "worker_a": "full_effort",
        "worker_b": "reduced_effort"
      },
      "chemistry": "average",
      "safety_concerns": [],
      "suggestions": "Worker B may be dealing with something personal. Match was fine but [B] didn't go as hard as usual.",
      "hidden_notes": "Worker B overheard complaining about recent booking"
    }
  }
}
```

---

**Document Status:** Locked
**Last Updated:** 2025-12-25
