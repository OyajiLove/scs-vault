# Match Consequences

📛 **MECHANIC:** Match Consequences
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Match Simulation / Core Gameplay
🔑 **KEYWORDS:** match consequences, match rating, momentum, popularity, morale, memory, scandal
📌 **ORIGIN:** Vol 1-2 (Booking Engine Phase 1)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-2 | 🔒 LOCKED |

---

## Overview

What happens after [[Match Processing]] completes. Match quality and context generate effects across multiple systems: ratings, momentum, popularity, morale, memory, and scandal risk.

---

## Consequence Categories

| Outcome | System Affected | Description |
|---------|-----------------|-------------|
| **Match Rating** | Reputation | Fan/observer perception |
| **Momentum Change** | [[Buzz System/_Buzz System Index\|Buzz]] | Short-term heat |
| **Popularity Adjustment** | [[Popularity_System\|Popularity]] | Long-term foundation |
| **Fanbase Reaction** | Crowd | Cheers, boos, silence, split |
| **Morale Shift** | Workers | Happiness from booking treatment |
| **Memory Retention** | [[Crowd_Memory\|Crowd Memory]] | What fans remember |
| **Scandal Risk** | [[Scandal System\|Scandal]] | Tasteless content triggers |

---

## Match Report Philosophy (#51)

**Core Law:** "The struggle must be felt, not just told."

| Principle | Implementation |
|-----------|----------------|
| **Struggle felt** | Describe exhaustion, willpower, agony, survival |
| **Emotional arcs** | Body language, facial expressions, small moments |
| **Losers gain glory** | Show heart even in losses |
| **Told in silence** | Near-kickouts, crawling to ropes, refusing to give up |

**Small Touches That Matter:**
- Fans standing for gutsy survivors even if they lose
- Stunned silences after sudden KO
- Commentators crying out at impossible kickouts
- Workers crawling, shaking heads, refusing to give up
- Blood dripping, sweat pouring, bodies trembling

---

## Match Rating

| Rating | Description | Effect |
|--------|-------------|--------|
| **5-Star+** | Legendary, classic | Massive reputation boost |
| **4.5-5** | Excellent, MOTY candidate | Strong reputation boost |
| **4-4.5** | Great, memorable | Positive reputation |
| **3-4** | Good, solid | Maintains reputation |
| **2-3** | Average, forgettable | Neutral |
| **1-2** | Bad, disappointing | Negative reputation |
| **0-1** | Disaster, trainwreck | Major reputation damage |

**Rating sources:**
- Fan perception (crowd reaction)
- Observer/newsletter scores (workrate focus)
- Promotion internal evaluation

---

## Momentum Change

From [[Buzz System/_Buzz System Index|Buzz System]]:

| Outcome | Buzz Effect |
|---------|-------------|
| **Great match, won clean** | Major Buzz gain |
| **Great match, lost protected** | Moderate Buzz gain |
| **Great match, won dirty** | Buzz + heat |
| **Bad match, won** | Minimal Buzz, may lose |
| **Bad match, lost** | Buzz loss |
| **Squash win** | Buzz for winner only |
| **Squash loss** | Momentum killer |

**Note:** Momentum ≠ winning. Great loss can build more Buzz than bad win.

---

## Popularity Adjustment

From [[Popularity_System|Popularity]]:

| Factor | Effect |
|--------|--------|
| **Match quality** | High quality = slow pop growth |
| **Crowd engagement** | Hot crowd = faster pop growth |
| **Booking context** | Push with buy-in = growth; false popularity = backlash |
| **Regional variation** | Home region gains faster |
| **Stakes level** | Higher stakes = bigger pop swings |

**False Popularity Trigger:** (Push Level - Organic Pop) ≥ 20 → Backlash

---

## Fanbase Reaction

| Reaction | Meaning | Next Show Effect |
|----------|---------|------------------|
| **Cheers** | Approval, investment | Positive anticipation |
| **Boos** | Heel heat (good) or rejection (bad) | Context dependent |
| **Silence** | Apathy, worst outcome | Need to rebuild |
| **Split** | Divided crowd | Potential for story |
| **Hostile** | Active rejection | Damage control needed |

---

## Morale Shift

| Scenario | Worker Morale |
|----------|---------------|
| **Great match, treated well** | Major boost |
| **Great match, buried** | Frustration |
| **Bad match, own fault** | Self-doubt |
| **Bad match, booking fault** | Resentment |
| **Protected loss** | Maintained |
| **Embarrassing loss** | Major hit |

**Affected parties:**
- Participants directly
- Observers (locker room watching)
- Veterans (may resent young talent push)
- Allies/rivals (faction dynamics)

---

## Memory Retention

From [[Crowd_Memory|Crowd Memory]]:

| Match Quality | Memory Duration |
|---------------|-----------------|
| **Legendary** | Permanent anchor |
| **Excellent** | Years |
| **Great** | Months |
| **Good** | Weeks |
| **Average** | Days |
| **Bad** | Forgotten (unless spectacularly bad) |

**Memory Anchors created by:**
- Career-defining moments
- Shocking finishes
- Betrayals
- Title changes
- Returns in match

---

## Scandal Risk

| Trigger | Risk Level |
|---------|------------|
| **Tasteless content** | High |
| **Blood overuse** | Medium |
| **Visible shoot moment** | High |
| **Unsafe work, injury** | Very High |
| **Offensive content** | Very High |
| **Worked shoot gone wrong** | High |

**Consequences:** Promotion reputation damage, worker discipline, potential firing

---

## Consequence Propagation

| System | Immediate Effect | Ripple Effect |
|--------|------------------|---------------|
| **Buzz** | Same-week spike/drop | Affects next booking options |
| **Pop** | Gradual change | Affects drawing power |
| **Morale** | Immediate | Affects future performance |
| **Memory** | Stored | Callbacks, future feuds |
| **Feud** | Intensity change | Next match anticipation |
| **Title** | Prestige change | Championship value |

---

## Connected Mechanics

- [[Match Processing]] - generates consequences
- [[Buzz System/_Buzz System Index|Buzz System]] - momentum effects
- [[Popularity_System|Popularity]] - long-term effects
- [[Crowd_Memory|Crowd Memory]] - retention
- [[Feud_Memory|Feud Memory]] - rivalry tracking

---

## Open Questions

- Exact consequence formulas
- Cascade effects (how one consequence triggers others)
- Diminishing returns on repeated great matches

---

## Implementation Notes

```json
{
  "match_consequences": {
    "match_id": "m_001",
    "quality_score": 84,
    "effects": {
      "rating": {
        "fan_perception": 4.25,
        "observer_rating": 4.5,
        "promotion_internal": 4.0
      },
      "buzz_change": {
        "w_001": 5,
        "w_002": 12
      },
      "pop_change": {
        "w_001": 1,
        "w_002": 3
      },
      "fanbase_reaction": "cheers",
      "morale_change": {
        "w_001": 2,
        "w_002": 8
      },
      "memory_created": {
        "duration": "months",
        "anchor": false
      },
      "scandal_risk": 0
    }
  }
}
```
