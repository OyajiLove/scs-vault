# HOF Voter Types

📛 **MECHANIC:** HOF Voter Types
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy & Recognition
🔑 **KEYWORDS:** voters, fan vote, veteran committee, critics, journalists
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Overview

Different voter groups have different priorities when selecting Hall of Fame inductees. Understanding voter types helps predict induction likelihood and explains why some candidates get snubbed.

---

## Voter Categories

| Voter Type | Weight | Priorities |
|------------|--------|------------|
| **Fans** | 25-40% | Popularity, memorable moments, nostalgia |
| **Veterans** | 20-30% | In-ring work, locker room respect, professionalism |
| **Critics/Journalists** | 15-25% | Match quality, historical significance, innovation |
| **Management** | 15-25% | Business impact, loyalty, company legacy |

---

## Fan Voters

**What they prioritize:**
- Memorable moments and catchphrases
- Peak popularity periods
- Nostalgia factor
- Mainstream crossover

**What they overlook:**
- Technical in-ring ability
- Backstage contributions
- Workrate consistency

**Bias:** Recency and spectacle over sustained excellence

---

## Veteran Voters

**What they prioritize:**
- Locker room leadership
- Safe worker reputation
- Willingness to put others over
- Professionalism and reliability

**What they overlook:**
- Mainstream popularity
- Gimmick quality
- Drawing power

**Bias:** "One of us" mentality, old-school values

---

## Critic/Journalist Voters

**What they prioritize:**
- Match quality and star ratings
- Historical significance
- Innovation and influence
- Career arc and storytelling

**What they overlook:**
- Business success
- Popularity with casual fans
- Backstage politics

**Bias:** Workrate, Japanese wrestling, "smart" favorites

---

## Management Voters

**What they prioritize:**
- Business impact (gates, ratings, merch)
- Company loyalty
- Brand ambassadorship
- Ease of relationship

**What they overlook:**
- In-ring excellence (if it didn't draw)
- Critical acclaim
- Historical significance outside their company

**Bias:** Money, loyalty, corporate image

---

## Connected Mechanics

- [[HOF Voting and Selection]] - Where voter types participate
- [[HOF Eligibility]] - Different voters may value different criteria
- [[Fan Memory Engine/_Fan Memory Index|Fan Memory]] - Fan voters influenced by memory

---

## Open Questions

- Voter manipulation mechanics
- Changing voter weights over time
- Regional voter differences

---

## Implementation Notes

```json
{
  "voter_weights": {
    "promotion": "major_fed_001",
    "fans": 0.30,
    "veterans": 0.25,
    "critics": 0.20,
    "management": 0.25
  },
  "candidate_scores": {
    "w_001": {
      "fans": 92,
      "veterans": 78,
      "critics": 85,
      "management": 88,
      "weighted_total": 86.1
    }
  }
}
```
