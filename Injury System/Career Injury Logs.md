# Career Injury Logs

📛 **MECHANIC:** Historical Injury Records
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation / Save State
🔑 **KEYWORDS:** injury history, career logs, save state, historical data, wear accumulation
📌 **ORIGIN:** Vol 1 Extraction #172
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Every worker has a persistent historical record of injuries that affects their current save state. Starting a game in 1999 means Steve Austin's neck is already heavily compromised. Starting in 1996 means minimal damage, standard wear. This creates authentic career simulation where past damage matters.

---

## Log Structure

Each injury log entry contains:

| Field | Description | Example |
|-------|-------------|---------|
| **Date** | When injury occurred (Season/Year if exact unavailable) | Aug 1997 |
| **Type** | Body part affected | Neck |
| **Cause** | How injury happened | SummerSlam vs Owen Hart |
| **Severity** | Minor, Medium, Major, Career-Threatening | Severe |
| **Recovery Time** | How long worker was out | 6 months |
| **Permanent Impact** | Lasting effects | Chronic pain, reduced mobility |

---

## Save State Impact

Different start dates mean different injury histories:

| Save Year | Worker Example | Injury State |
|-----------|----------------|--------------|
| 1996 | Steve Austin | Minimal damage, standard wear |
| 1999 | Steve Austin | Neck heavily compromised |
| 2002 | Steve Austin | Severe neck + back collapse |

---

## Example Career Injury Log

### Steve Austin

```
1996 - Knee injuries begin (WCW) - Minor
Aug 1997 - Neck injury (SummerSlam vs Owen) - Severe
1999 - Multiple knee surgeries - Moderate
2001 - Back issues - Moderate
2002 - Severe Neck + Back Collapse - Career-Threatening
```

### Mick Foley

```
1983-1988 - Accumulated minor injuries (training, early career) - Minor
1992 - Concussion (WCW) - Moderate
1994 - Ear torn off (Germany) - Moderate
1996-1998 - Repeated concussions (ECW, WWF) - Cumulative Severe
1998 - HIAC damage (WWF) - Major
1999 - Repeated head trauma (WWF) - Career-Threatening
```

---

## Data Sources for Historical Workers

| Source Type | Reliability | Coverage |
|-------------|-------------|----------|
| **Observer archives** | High | Injuries reported in newsletters |
| **Wrestling wikis** | Moderate | "Injury" sections on profiles |
| **Shoot interviews** | Variable | Workers discussing past injuries |
| **Podcasts** | Variable | Casual injury mentions |
| **Autobiographies** | High | Detailed personal accounts |
| **Documentary footage** | High | Visual evidence of injuries |

---

## Auto-Generation for New Workers

Generated workers build injury logs dynamically:

| Career Stage | Expected Log Entries |
|--------------|---------------------|
| Rookie (0-2 years) | 0-2 minor entries |
| Young (3-5 years) | 1-4 entries, mostly minor |
| Established (6-10 years) | 3-8 entries, moderate mix |
| Veteran (11-15 years) | 5-12 entries, some major |
| Legend (16+ years) | 8-20 entries, cumulative damage |

---

## System Interactions

### With Wear and Tear
- Each logged injury adds to cumulative wear counters
- Severe injuries create permanent ceiling reductions

### With Style Adaptation
- Logged injuries inform what style adaptations are needed
- Workers with neck damage may need to reduce head bumps

### With Medical Exams
- Injury logs inform medical evaluation results
- Past injuries increase risk flags

### With Career Arcs
- Injury history affects peak timing
- Accumulated damage influences retirement timing

---

## Injury Culture by Era (#46)

📌 **Source:** Vol 1 Extraction #46

How injuries were handled varied dramatically by era:

| Era | Injury Culture |
|-----|----------------|
| **1970s** | Everyone works hurt, injuries hidden, no medical oversight |
| **1990s** | Car crash TV, lots of long-term injuries, some awareness emerging |
| **Modern** | Better rehab protocols, but more delicate bodies, wellness policies |

---

## Connected Mechanics

- [[Wear and Tear System]] - Logs feed cumulative damage
- [[Injury Types]] - Classification for log entries
- [[Style Adaptation]] - Logs inform adaptation needs
- [[_Aging System Index|Aging System]] - Career arc adjustments

---

## Open Questions

- [ ] How detailed should historical logs be for obscure workers?
- [ ] Automated log generation based on match history simulation?
- [ ] Fan-created log contributions for historical accuracy?
- [ ] Cross-referencing multiple sources for accuracy scores?

---

## Implementation Notes

```json
{
  "career_injury_log": {
    "worker_id": "austin_steve",
    "entries": [
      {
        "date": "1996-01-01",
        "type": "knee",
        "cause": "WCW accumulated damage",
        "severity": "minor",
        "recovery_weeks": 2,
        "permanent_impact": null
      },
      {
        "date": "1997-08-03",
        "type": "neck",
        "cause": "SummerSlam piledriver (Owen Hart)",
        "severity": "severe",
        "recovery_weeks": 26,
        "permanent_impact": {
          "mobility_reduction": -15,
          "chronic_pain": true,
          "style_limitation": ["head_bump_heavy"]
        }
      },
      {
        "date": "2002-03-01",
        "type": "neck",
        "cause": "Accumulated damage",
        "severity": "career_threatening",
        "recovery_weeks": null,
        "permanent_impact": {
          "forced_retirement_trigger": true
        }
      }
    ],
    "total_logged_injuries": 7,
    "cumulative_severity_score": 85
  }
}
```

---

**Document Status:** Locked (Vol 1)
**Last Updated:** 2025-12-24
**Next Review:** Build historical injury database for top 100 workers
