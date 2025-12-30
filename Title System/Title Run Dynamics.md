# Title Run Dynamics

📛 **MECHANIC:** Champion Run and Chase Mechanics
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Promotion
🔑 **KEYWORDS:** title run, chase, reign, decay curve, champion maintenance, Okada run
📌 **ORIGIN:** Vol 1-4 (Title Reigns vs Chases, Natural Title Run Decay Curve)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

The chase is always easier than the reign. Babyface champions naturally struggle to stay hot, while heel champions decay slower (they're easier to hate). Title runs have a natural decay curve that must be actively fought through fresh challengers, memorable defenses, and evolving storylines.

---

## Chase vs. Reign Dynamics

| Phase | Dynamics |
|-------|----------|
| **The Chase** | Momentum builds naturally; every close call increases investment; underdog narrative is easy to maintain |
| **The Win** | Peak emotional moment; massive buzz spike |
| **Early Reign** | Honeymoon period; fans excited for defenses |
| **Mid Reign** | Decay begins unless fresh challengers emerge |
| **Late Reign** | Staleness risk; need character evolution or hot feud |
| **End of Reign** | Can be glorious (passing torch) or flat (cold loss) |

### Chase Momentum Buffs
```
Chase Phase: +10 momentum bonus per gutsy close loss
Win Moment: +25 immediate buzz spike
```

### Reign Decay (Babyface)
```
Months 1-3: Minimal decay (honeymoon)
Months 4-6: -2 momentum per month unless fresh challenger
Months 7-12: -4 momentum per month unless classic defense
Year 2+: -6 momentum per month unless dynasty-level booking
```

### Reign Decay (Heel)
```
Months 1-6: Minimal decay (easy heat)
Months 7-12: -2 momentum per month unless face threat rises
Year 2+: -4 momentum per month unless character evolution
```

---

## Title Run Maintenance

To fight decay, bookers must:

| Strategy | Effect |
|----------|--------|
| **Fresh Challengers** | New credible threats reset decay clock |
| **Classic Defenses** | MOTY-candidate matches boost prestige |
| **Character Evolution** | Champion grows/changes during reign |
| **Escalating Stakes** | Each defense feels bigger than the last |
| **Near Falls** | Teasing title change without delivering |
| **Special Stipulations** | Cage, ladder, etc. for variety |

---

## Worker Fatigue During Title Runs

Champions get worn down:

| Factor | Effect |
|--------|--------|
| **Match Frequency** | More defenses = more physical toll |
| **Travel Schedule** | Champions often work more dates |
| **Mental Pressure** | Pressure to deliver every night |
| **Creative Burden** | Must maintain character freshness |

### Booking Warnings
System should alert booker:
- "The crowd loves [Champion], but they're starting to crave something new."
- "[Champion]'s reign is in danger of going stale without a fresh challenge."
- "[Champion] is showing signs of fatigue. Consider lighter schedule or title change."

---

## Dynasty Runs

If decay is fought successfully (like Okada 2016-18), dynasty runs create:

| Effect | Description |
|--------|-------------|
| **Prestige Explosion** | Title becomes promotion's crown jewel |
| **Champion Elevation** | Worker becomes all-time legend |
| **Challenger Elevation** | Anyone who challenges gains credibility |
| **Memory Anchors** | Multiple classic defenses become historic |

### Dynasty Requirements
- 12+ month reign
- 5+ quality defenses
- 2+ MOTY-candidate matches
- No prestige drops below starting point
- Consistent character maintenance

---

## Title Run Types

| Run Type | Length | Strategy |
|----------|--------|----------|
| **Transitional** | Days to weeks | Bridge between longer reigns |
| **Short Reign** | 1-3 months | Statement win, immediate challenge |
| **Standard Reign** | 3-6 months | Solid run with 2-3 defenses |
| **Long Reign** | 6-12 months | Requires careful maintenance |
| **Dynasty** | 12+ months | Legendary difficulty to maintain |

---

## Champion Personality Effects

Hidden personality affects reign success:

| Trait | Effect |
|-------|--------|
| **High Drive** | Fights decay harder; motivated to stay on top |
| **Low Drive** | Coasts once champion; accelerated decay |
| **High Ego** | Demands protection; may resist losing |
| **Title Belt Hoarder Tag** | Clings to reign; backstage politics |
| **Chase Greatness Goal** | Motivated champion; good reign likely |
| **Enjoy Life Goal** | May not care about title; flat reign |

---

## Heel vs. Face Champion Differences

| Aspect | Babyface Champion | Heel Champion |
|--------|-------------------|---------------|
| **Decay Speed** | Faster | Slower |
| **Storytelling** | Harder (who to root for?) | Easier (root against) |
| **Match Finishes** | Need clean wins | Can escape/cheat |
| **Challenger Pool** | Need credible heels | Anyone can challenge |
| **Fan Fatigue** | Higher risk | Lower risk |

---

## The "Mail It In" Problem

Workers mentally check out after success (Drive decay):

| Symptom | Effect |
|---------|--------|
| **Shorter Matches** | Worker stops going long |
| **Safer Work** | Fewer big spots, less risk |
| **Lazy Promos** | Character becomes stale |
| **Fan Detection** | Crowds notice laziness |

### Nakamura Example
1. Wins top title
2. Drive naturally declines
3. Matches become shorter, safer, lazier
4. Fans slowly feel it
5. Unless booker intervenes, coasts and fades

---

## Connected Mechanics

- [[Title Prestige]] - Reign quality affects prestige
- [[Hot Potato Risk]] - Short reigns damage prestige
- [[Hidden Personality]] - Drive, Ego affect reign quality
- [[Worker Skills]] - Psychology needed for great defenses
- [[Crowd Memory]] - Classic defenses become anchors

---

## Open Questions

- [ ] Exact decay formulas by reign length
- [ ] How injury during reign affects decay
- [ ] Interim title mechanics
- [ ] Remote champion (touring elsewhere) effects
- [ ] Multiple title holder complications

---

## Implementation Notes

```json
{
  "title_run": {
    "title_id": "title_001",
    "champion_id": "worker_001",
    "start_date": "1985-03-15",
    "current_length_months": 8,
    "defenses": 6,
    "quality_defenses": 4,
    "moty_candidates": 1,
    "decay_status": {
      "current_decay_rate": -2,
      "honeymoon_expired": true,
      "last_fresh_challenger": "1985-09-01"
    },
    "maintenance_alerts": [
      "Reign entering staleness risk zone",
      "Consider fresh challenger"
    ],
    "dynasty_progress": 45
  }
}
```
