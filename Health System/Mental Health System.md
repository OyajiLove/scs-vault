# Worker Mental Health System

📛 **SYSTEM:** Worker Mental Health
🧭 **CATEGORY:** Worker Simulation / Psychological State
🔑 **KEYWORDS:** mental health, morale, burnout, depression, trauma, recovery, sabbatical, cumulative damage
📝 **SUMMARY:** Models both short-term morale (week-to-week happiness) and long-term mental health (cumulative psychological resilience/collapse). Mental Health is not just "he mad at booking," it's what happens when the dream eats itself.

⚙️ **LOGIC OVERVIEW:**
- Morale = short-term, reactive, booking-related
- Mental Health = long-term, cumulative, based on career-wide events
- Both systems interact but track different timescales
- Mental health degradation has cascading effects on performance, scandal risk, and career trajectory

🔬 **LLM INTEGRATION:** Minimal

📌 **ORIGIN:** Vol 2 Chunk 09

📎 **CONNECTED SYSTEMS:**
- [[Hidden_Personality]] - Drive and Ego interact with mental state
- [[Contract System]] - Contract satisfaction feeds morale
- [[_Injury System Index|Injury System]] - Injuries affect mental state
- [[_Scandal System Index|Scandal System]] - Scandals damage mental health; poor mental health increases scandal risk
- [[Backstage Politics System/_Backstage Politics System Index|Backstage Politics]] - Political losses affect morale

❓ **OPEN QUESTIONS:**
- Exact formulas for degradation/recovery
- Threshold values for burnout triggers
- How visible is mental health to players?

✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 09 | 🔒 LOCKED (Concept) |

---

## Core Distinction: Morale vs Mental Health

| Aspect | Morale (Short-Term) | Mental Health (Long-Term) |
|--------|---------------------|---------------------------|
| **Timescale** | Week-to-week | Career-wide, cumulative |
| **Triggered By** | Current booking, pushes, backstage environment | Betrayals, injuries, scandals, political fights, family tragedies, public failures |
| **Effects** | Threatens to leave, slacks off, angry promos | Increased injury risk, scandal risk, substance abuse, sloppy performances, burnout |
| **Recovery** | Quick with good booking | Slow, requires rest, sabbaticals, career wins, positive environment |
| **Decay Rate** | Fast | Slow but persistent |

---

## Morale System (Short-Term)

### What Affects Morale

| Factor | Positive Effect | Negative Effect |
|--------|----------------|-----------------|
| **Booking Position** | Consistent push | Jobbing out, 50/50 booking |
| **Contract Status** | Fair pay, respect | Underpaid, feeling used |
| **Locker Room** | Positive environment, friends | Toxic politics, isolation |
| **Creative Input** | Voice in angles | Ideas ignored |
| **Match Quality** | Good matches | Botch-filled disasters |

### Low Morale Consequences

- Threatens to leave when contract expires
- Slacks off in matches (effort penalty)
- Goes into business for himself (shoot promos, worked shoots)
- Causes backstage friction
- Becomes flight risk for rival promotions

---

## Mental Health System (Long-Term)

### What Degrades Mental Health

| Trigger | Severity | Notes |
|---------|----------|-------|
| **Severe injury recovery** | Minor to Major | Emotional scarring from career-threatening injuries |
| **Public scandal fallout** | Severe | Shame, media harassment, loss of friends |
| **Locker room toxicity** | Gradual | Slow burn-down over months/years |
| **Repeated betrayals** | Moderate | Backstage screwings build long-term bitterness |
| **Media/public harassment** | Heavy | Post-scandal pile-on, online abuse |
| **Family tragedies** | Sharp drop (rare event) | Deaths, divorces, custody battles |
| **Career plateau** | Moderate | Feeling stuck, passed over |
| **Substance abuse** | Self-reinforcing | Damages health which damages mood which increases abuse |

### Mental Health Degradation Signs

| Sign | Gameplay Effect |
|------|-----------------|
| **Increased injury risk** | Depression lowers physical resilience |
| **Higher scandal risk** | Self-destructive behaviors |
| **Substance abuse spikes** | Health and scandal interactions |
| **Sloppy performances** | Match quality penalties |
| **Burnout possible** | Extended leave needed |
| **Extreme cases** | Retirement, scandal blowouts, even death in worst collapse spirals |

---

## Mental Health Recovery

### What Helps Recovery

| Recovery Path | Effect | Time Required |
|---------------|--------|---------------|
| **Rest periods** | Major healing chance | Weeks to months |
| **Sabbaticals** | Significant recovery | Months |
| **Therapist/trainer support** | Gradual improvement (if promotion offers) | Ongoing |
| **Big career wins** | Emotional recharge (title runs, redemption arcs) | Varies |
| **Positive locker room** | Slower degradation, some healing | Ongoing |
| **Stable personal life** | Baseline support | Ongoing |

### Recovery Barriers

- Continuing to work through problems
- Toxic locker room environment
- Ongoing media scrutiny
- Financial pressure to keep working
- Addiction cycles

---

## State Thresholds

| Mental Health Level | State | Behavior |
|--------------------|-------|----------|
| 80-100 | Healthy | Normal function, resilient |
| 60-79 | Strained | Minor performance dips, increased irritability |
| 40-59 | Struggling | Noticeable decline, rest needed |
| 20-39 | Crisis | Burnout imminent, sabbatical recommended |
| 0-19 | Collapse | Career threatened, extreme intervention needed |

---

## Interactions with Other Systems

### Scandal System

```
if mental_health < 40:
    scandal_risk_modifier += 0.25  # More likely to make bad decisions
    
if scandal_exposed:
    mental_health -= 15  # Scandal damages mental health
```

### Injury System

```
if mental_health < 50:
    injury_recovery_modifier -= 0.15  # Slower healing when depressed
    
if major_injury_occurs:
    mental_health -= 10  # Injury trauma
```

### Hidden Personality

```
# High Drive workers push through mental health issues
if drive_tag == "high" and mental_health < 50:
    burnout_risk += 0.20  # They keep going until they break
    
# High Ego workers spiral harder from public failures
if ego_tag == "high" and scandal_exposed:
    mental_health -= additional_10
```

---

## Historical Examples

| Worker | Mental Health Factor | Result |
|--------|---------------------|--------|
| Jake Roberts | Cumulative trauma + addiction | Decades of struggle, eventual recovery |
| Benoit | Long-term damage + isolation | Catastrophic collapse |
| Scott Hall | Trauma + addiction + enabling environment | Spiral before late-life recovery |
| Diamond Dallas Page | Built recovery systems | Helped others recover |
| Mick Foley | Accumulated damage + positive family life | Managed decline gracefully |

---

## Implementation Notes

```json
{
  "worker_id": "worker_001",
  "morale": {
    "current": 72,
    "trend": "stable",
    "recent_factors": ["pushed_on_tv", "lost_title_feud"]
  },
  "mental_health": {
    "current": 65,
    "lifetime_low": 45,
    "current_state": "strained",
    "degradation_factors": ["old_injury_memory", "toxic_locker_room_2019"],
    "recovery_factors": ["stable_contract", "positive_family"]
  }
}
```

---

## Connected Mechanics

- [[Hidden_Personality]] - Personality affects mental health response
- [[_Injury System Index|Injury System]] - Physical and mental health interact
- [[_Scandal System Index|Scandal System]] - Bidirectional relationship
- [[Contract System]] - Financial security affects mental state
- [[Burnout Collapse States]] - Extreme mental health failure modes
- [[Redemption Arcs]] - Recovery storylines

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-26
**Next Review:** Define exact formulas, thresholds, and recovery rates
