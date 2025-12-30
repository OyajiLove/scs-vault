# HOF Special Categories

📛 **MECHANIC:** HOF Special Categories
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy & Recognition
🔑 **KEYWORDS:** special categories, tag teams, managers, announcers, contributor
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

Not all Hall of Fame inductees are solo wrestlers. Special categories recognize tag teams, managers, announcers, and other contributors to the industry.

---

## Category Types

| Category | Description |
|----------|-------------|
| **Main/Individual** | Standard solo wrestler induction |
| **Tag Team** | Team inducted as a unit |
| **Manager/Valet** | Non-wrestling performers |
| **Announcer/Commentary** | Broadcast talent |
| **Contributor** | Promoters, trainers, referees, etc. |
| **Celebrity Wing** | Non-wrestling celebrities with wrestling ties |
| **Legacy** | Posthumous or historical figures |

---

## Tag Team Inductions

**Requirements:**
- Team must have achieved success as a unit
- Both members must meet minimum individual thresholds
- Team legacy score calculated separately from individuals

**Edge Cases:**
- Can individual members be inducted separately later? (Yes)
- What if one member is controversial? (Case by case)
- Breakup feuds don't disqualify team legacy

---

## Manager/Valet Inductions

**Eligibility factors:**
- Number of stars managed
- Promo/character contribution
- Cultural impact
- Career longevity

**Examples:** Bobby Heenan, Paul Bearer, Miss Elizabeth, Paul Heyman

---

## Announcer Inductions

**Eligibility factors:**
- Years behind the desk
- Iconic calls
- Era association
- Cross-generational recognition

**Examples:** Jim Ross, Gordon Solie, Howard Finkel

---

## Contributor Category

Catch-all for industry builders:

| Type | Examples |
|------|----------|
| Promoters | Vince McMahon Sr., Antonio Inoki |
| Trainers | Stu Hart, Killer Kowalski |
| Referees | Earl Hebner, Red Shoes |
| Innovators | Paul Heyman (ECW), Gabe Sapolsky |

---

## Celebrity Wing

Non-wrestlers with significant wrestling involvement:

| Criteria | Examples |
|----------|----------|
| Multiple appearances | Mr. T, Lawrence Taylor |
| Cultural crossover | Andy Kaufman |
| Significant storyline role | Mike Tyson |

---

## Connected Mechanics

- [[HOF Eligibility]] - Different thresholds for different categories
- [[HOF Voting and Selection]] - Categories may have different voting weights
- [[Legend Status Effects]] - Effects vary by category

---

## Open Questions

- Can one person be in multiple categories?
- Tag team + individual dual induction timing
- Celebrity Wing credibility concerns

---

## Implementation Notes

```json
{
  "special_induction": {
    "inductee_type": "tag_team",
    "members": ["w_001", "w_002"],
    "team_name": "The Road Warriors",
    "team_legacy_score": 88,
    "individual_eligibility": {
      "w_001": true,
      "w_002": true
    },
    "category": "tag_team",
    "future_individual_eligible": true
  }
}
```
