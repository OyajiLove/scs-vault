# Hot Potato Risk

📛 **MECHANIC:** Frequent Title Change Penalties
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Promotion
🔑 **KEYWORDS:** hot potato, title changes, short reigns, prestige damage, credibility
📌 **ORIGIN:** Vol 1-4 (Hot Potato Risk, Overprotection Penalty)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Hot potato booking (frequent title changes) rapidly destroys championship prestige. When titles change hands too often, fans stop believing the belt matters. The system tracks title change frequency and applies escalating penalties to prestige and match importance.

---

## Hot Potato Threshold

| Title Changes (Per Year) | Status | Prestige Effect |
|--------------------------|--------|-----------------|
| 1-2 | **Healthy** | No penalty |
| 3-4 | **Elevated** | -5 prestige per extra change |
| 5-6 | **High Risk** | -10 prestige per extra change |
| 7+ | **Hot Potato** | -15 prestige per change; fan faith collapse |

---

## Hot Potato Counter

System tracks:

| Metric | Description |
|--------|-------------|
| **Changes in Last 12 Months** | Rolling window of title changes |
| **Average Reign Length** | Mean days per champion |
| **Short Reign Count** | Reigns under 30 days |
| **Transitional Champion Count** | Obvious placeholder reigns |

### Hot Potato Trigger
```
If Changes_12_Months >= 5:
  Hot_Potato_Status = True
  Prestige_Penalty = (Changes - 4) × 15
  Fan_Faith_Modifier = -0.2 per extra change
```

---

## Consequences of Hot Potato Booking

| Consequence | Description |
|-------------|-------------|
| **Prestige Collapse** | Title becomes meaningless |
| **Match Rating Penalty** | Title matches feel less important |
| **Fan Apathy** | Crowds stop caring about title |
| **Worker Devaluation** | Champions seem interchangeable |
| **Storyline Damage** | Hard to build meaningful feuds |
| **Recovery Difficulty** | Takes months to rebuild credibility |

---

## Short Reign Classifications

| Reign Length | Classification | Effect |
|--------------|----------------|--------|
| 1-7 days | **Transitional** | Major prestige hit unless planned shock |
| 8-30 days | **Short** | Minor prestige hit |
| 31-90 days | **Standard** | No penalty |
| 91-180 days | **Solid** | Slight prestige boost |
| 180+ days | **Long** | Strong prestige boost (if maintained) |

---

## Acceptable Short Reigns

Some short reigns don't trigger hot potato penalties:

| Scenario | Penalty Applied? |
|----------|------------------|
| **Planned transitional** (announced) | Reduced penalty |
| **Injury forces change** | No penalty |
| **Worker leaves promotion** | No penalty |
| **Scandal forces strip** | Penalty to worker, not booking |
| **Shock cash-in** (MITB style) | Penalty depends on follow-up |

---

## Hot Potato Recovery

Rebuilding after hot potato damage:

| Method | Effect | Time Required |
|--------|--------|---------------|
| **Long reign (6+ months)** | +10 to +20 prestige | 6+ months |
| **Tournament for title** | +5 to +10 immediate | Immediate |
| **No changes for 6 months** | Reset hot potato counter | 6 months |
| **Classic title match** | +5 per match | Ongoing |
| **New championship design** | +5 temporary | Immediate, fades |

---

## Era Differences

| Era | Hot Potato Tolerance |
|-----|---------------------|
| **Territory** | Very low: titles sacred, changes rare |
| **80s National** | Low: still respected championship booking |
| **Attitude Era** | Moderate: more changes accepted |
| **Modern WWE** | High: frequent changes normalized |
| **AEW/Modern Indies** | Low-Moderate: trying to rebuild prestige |

---

## Opposite Problem: Overprotection

Too few title changes also causes issues:

| Scenario | Effect |
|----------|--------|
| **Champion never challenged credibly** | Fans lose interest |
| **Same champion 2+ years** | Staleness unless dynasty-level quality |
| **No near-falls ever** | Matches become predictable |
| **Burial of challengers** | Roster looks weak |

### Balance Point
Optimal title booking creates anticipation for possible change while making actual changes feel earned and significant.

---

## Historical Examples

| Promotion/Era | Hot Potato Situation | Outcome |
|---------------|---------------------|---------|
| **WCW 2000** | Constant title changes | Complete prestige collapse |
| **WWF 1999** | Russo hot-shotting | Title devalued but company hot |
| **NJPW Okada Era** | Long reigns with quality | Peak prestige |
| **WWE 24/7 Title** | Designed as hot potato | Joke title from day one |
| **AEW World Title** | Careful changes | Built credibility early |

---

## Connected Mechanics

- [[Title Prestige]] - Hot potato destroys prestige
- [[Title Run Dynamics]] - Short reigns prevent dynasty building
- [[Crowd Memory]] - Fans remember booking patterns
- [[Booking Engine]] - Tracks booking habits

---

## Open Questions

- [ ] Exact prestige penalty formulas
- [ ] How vacancies affect hot potato counter
- [ ] Multi-person match title changes (different rules?)
- [ ] Interim title handling
- [ ] "Paper champion" mechanics (champion who never defends)

---

## Implementation Notes

```json
{
  "hot_potato_tracker": {
    "title_id": "title_001",
    "changes_last_12_months": 3,
    "average_reign_days": 95,
    "short_reigns_count": 1,
    "hot_potato_status": false,
    "prestige_penalty_active": 0,
    "fan_faith_modifier": 1.0,
    "recovery_mode": false,
    "months_since_change": 4,
    "last_changes": [
      { "date": "1985-03-15", "reign_length": 120 },
      { "date": "1985-07-15", "reign_length": 90 },
      { "date": "1985-10-15", "reign_length": null }
    ]
  }
}
```
