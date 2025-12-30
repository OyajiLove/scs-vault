# Fanbase False Mythology Wars

📛 **NAME:** Fanbase False Mythology Wars  
🧭 **CATEGORY:** Fan Reaction System / Conflict  
🔑 **KEYWORDS:** false mythology, war, faction, authenticist, revisionist, memory, clash, nostalgia  
📝 **SUMMARY:** Models when fans clash violently over rewritten wrestling history. False Golden Eras emerging, corporate nostalgia campaigns, generational drift, and historian vs romanticist conflicts all trigger factional wars. Dominant narratives shift based on which faction wins the discourse war, affecting how promotions and workers are remembered.

⚙️ **LOGIC OVERVIEW:**
- 4 causes (false eras emerging, corporate campaigns, generational drift, historian clashes)
- 3 war types (Authenticists vs Revisionists, Corporate vs Purists, Cynics vs Nostalgists)
- Factional splitting mechanics
- Narrative shaping tugs-of-war
- Promotion risk from taking sides
- Rediscovery events can shock narrative equilibrium

🔬 **LLM INTEGRATION:** High (LLM could generate faction arguments, mythology war discourse, forum debates, podcast discussions)

📌 **ORIGIN:** Vol 5 lines 630-633 (locked)

📎 **CONNECTED SYSTEMS:**
- [[False_Golden_Era_Phenomenon]] - What's being fought over
- [[Cultural_Civil_Wars_Preservation]] - Related memory conflicts
- [[Fan_Subculture_Evolution]] - Faction dynamics
- [[World_Memory_Drift]] - Narrative outcomes
- [[Rediscovery_Cultural_Rehabilitation]] - Evidence bombs

❓ **OPEN QUESTIONS:**
- Faction victory conditions
- Cross-platform war coordination
- Media outlet faction alignment
- Long-term narrative stabilization

✅ **STATUS:** Locked

---

## 1. WAR CAUSES (4 TRIGGERS)

| Cause | Description | Conflict Intensity |
|-------|-------------|-------------------|
| **False Golden Eras Emerging** | Eras once despised become mythologized by younger fans, clashing with older lived-experience fanbases | HIGH |
| **Corporate Nostalgia Campaigns** | Promotions reframe bad eras for branding, inflaming resentment from authenticists | MEDIUM-HIGH |
| **Generational Emotional Drift** | Younger fans prioritize different emotional needs, reinterpret chaotic eras as honest rebellion, freedom, or charm | MEDIUM |
| **Historian vs Romanticist Clashes** | Independent analysts exposing real flaws (scandals, creative failures) vs fans insisting on emotional memory over harsh truths | HIGH |

---

## 2. WAR TYPES (3 CONFLICTS)

| Fan War Type | Emotional Axis | Resolution Likelihood |
|--------------|----------------|----------------------|
| **Authenticists vs Revisionists** | "It was a nightmare" vs "It was a misunderstood Golden Era" | LOW (generational divide) |
| **Corporate Loyalists vs Purists** | Defending brand rewrites vs preserving emotional truth | MEDIUM (depends on evidence) |
| **Cynics vs Nostalgists** | "Nothing was ever pure" vs "We lost something real and we must cherish it" | LOW (philosophical divide) |

### Conflict Intensity Scale

| Intensity | Manifestations |
|-----------|----------------|
| **Mild** | Disagreement threads, polite debates |
| **Moderate** | Hostile discourse, faction formation |
| **High** | Active campaigns, block lists, show boycotts |
| **Extreme** | Community schisms, harassment, platform migrations |

---

## 3. SIMULATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Factional Splitting** | Fanbases fracture into factions based on emotional memory allegiances |
| **Narrative Shaping Tugs-of-War** | Historical events, workers, and promotions drift based on which faction dominates media, documentaries, forums |
| **Promotion Risk Factors** | Promotions aligning too heavily with false myths risk alienating older loyalists but may capture younger fans if done smoothly |
| **Rediscovery Event Shocks** | Rediscovered scandals or matches can tilt narrative wars sharply, causing myth collapses or myth reinforcements |

### Narrative Dominance Calculation

```
Faction_Power = (Community_Size × 0.25) + (Media_Access × 0.25) + 
                (Evidence_Strength × 0.20) + (Emotional_Intensity × 0.20) + 
                (Cultural_Timing × 0.10)

Dominant_Narrative = Faction with highest power
IF Power_Gap < 15: CONTESTED (ongoing war)
IF Power_Gap > 30: HEGEMONIC (one side dominates)
```

### Rediscovery Shock Effects

| Discovery Type | Shock Effect |
|----------------|--------------|
| **Scandal Revealed** | -20 to -40 for positive myth faction |
| **Hidden Gem Found** | +15 to +30 for positive myth faction |
| **Worker Interview** | Variable, depends on content |
| **Documentary Release** | +/- 25-40 depending on framing |

---

## 4. HISTORICAL MODELS

| Event | Fanbase Conflict |
|-------|------------------|
| **Late WCW Memory** | Older fans remember death spiral; younger fans remember crazy chaos fondly. Cultural war over legacy ongoing. |
| **Inokiism NJPW** | Divided puroresu fans: ruinous betrayal vs misunderstood visionary era. Small but intense factions. |
| **WWECW Memory** | Mocked by many at the time, but younger fans now reinterpret it as "fun trash" compared to sterile modern eras. Ironic faction growing. |
| **Attitude Era Reassessment** | Nostalgists vs revisionists over sexism, racism, and excess. Ongoing generational battle. |
| **Benoit Legacy** | Permanent irreconcilable war. Separatists vs Erasers vs Contextualists. No resolution possible. |

### Inokiism Case Study

**Era:** NJPW early 2000s (Inoki's MMA obsession)

**Original Perception:**
- Disaster for traditional puroresu
- Injuries, failed experiments
- Talent exodus
- Business decline

**False Myth Formation:**
- "At least he took risks"
- "Modern NJPW is too safe"
- "Inokiism was ahead of its time"

**Current War:**
- **Authenticists:** "He nearly killed the company"
- **Revisionists:** "He was a visionary"
- **Historians:** "Complex legacy with mostly negative outcomes"

**War Status:** MODERATE INTENSITY, Authenticists currently dominant but Revisionists persistent

---

## 5. PROMOTION RISK MATRIX

| Promotion Action | Younger Fan Effect | Older Fan Effect | Net Risk |
|------------------|-------------------|------------------|----------|
| **Embrace False Myth** | +20-30 loyalty | -25-40 loyalty | HIGH |
| **Reject False Myth** | -15-25 loyalty | +20-30 loyalty | MEDIUM |
| **Balanced Approach** | +5-15 loyalty | +5-15 loyalty | LOW |
| **Ignore War** | 0 | 0 | NONE (but misses opportunity) |

---

## 6. IMPLEMENTATION NOTES

```json
{
  "mythology_war": {
    "subject": "LATE_WCW",
    "war_type": "AUTHENTICISTS_VS_REVISIONISTS",
    "intensity": "MODERATE",
    "factions": [
      {
        "name": "AUTHENTICISTS",
        "position": "DISASTER_ERA",
        "power": 55,
        "demographics": "OLDER_FANS"
      },
      {
        "name": "REVISIONISTS",
        "position": "MISUNDERSTOOD_GOLDEN",
        "power": 35,
        "demographics": "YOUNGER_FANS"
      },
      {
        "name": "IRONISTS",
        "position": "FUN_TRASH",
        "power": 10,
        "demographics": "MIXED"
      }
    ],
    "dominant_narrative": "CONTESTED",
    "power_gap": 20,
    "recent_shocks": [
      {
        "event": "DARK_SIDE_OF_RING_EPISODE",
        "effect": "AUTHENTICIST_BOOST",
        "magnitude": 10
      }
    ]
  }
}
```

---

## 7. PHILOSOPHY

> "History isn't settled. It's fought over. Every generation rewrites the past to serve their present needs. The fans who lived through disaster remember disaster. The fans who discovered it on YouTube see freedom and chaos and think 'at least it wasn't boring.' Neither side is entirely wrong. Neither side is entirely right. The war over memory is the war over what wrestling means. And that war never ends."

False mythology wars are inevitable. SCS models them as ongoing discourse battles that shape how wrestling history is transmitted.

---

## 8. RELATED SYSTEMS

- [[False_Golden_Era_Phenomenon]] - What's being fought over
- [[Cultural_Civil_Wars_Preservation]] - Related memory conflicts
- [[Fan_Subculture_Evolution]] - Faction dynamics
- [[World_Memory_Drift]] - Narrative outcomes
- [[Rediscovery_Cultural_Rehabilitation]] - Evidence bombs

---

**Document Status:** Locked  
**Source:** Vol 5 lines 630-633  
**Next Review:** Integration with fan community simulation
