# Betrayal Memory for Formative Promotion Desertions

📛 **NAME:** Betrayal Memory for Formative Promotion Desertions  
🧭 **CATEGORY:** Contract System / Emotional Consequences  
🔑 **KEYWORDS:** betrayal, desertion, formative, no-show, exit, scar, memory, loyalty, rehabilitation  
📝 **SUMMARY:** Models how forced abandonment of a worker's emotional home creates lasting career scars. Forced no-shows, disrespectful exits, public denouncements, and careerist jumping all trigger betrayal memory flags that damage fanbase loyalty, worker emotional stability, career arc potential, and historical legacy unless rehabilitated.

⚙️ **LOGIC OVERVIEW:**
- 4 betrayal triggers (forced no-show, disrespectful exit, denouncement, careerist jumping)
- 4 effect areas (fanbase damage, emotional stability, career mutation, historical scarring)
- Loyalty decay rolls after betrayal events
- Fanbase migration patterns from betrayed workers
- Long-term world memory flags unless redemption overwrites

🔬 **LLM INTEGRATION:** Moderate (LLM could generate betrayal narratives, fan discourse, worker internal conflict, redemption arc scripts)

📌 **ORIGIN:** Vol 5 lines 515-517 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Worker_Formative_Loyalty]] - What's being betrayed
- [[Worker_Prioritization_Multi_Promotion]] - Priority decisions that trigger betrayal
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Individual memory tracking
- [[Fanbase_Emotional_Migration]] - How fans react to betrayal
- [[Redemption_Arcs]] - How betrayal can be healed

❓ **OPEN QUESTIONS:**
- Exact betrayal severity calculation
- Minimum time before rehabilitation possible
- Regional variation in betrayal perception
- Multiple betrayal stacking effects

✅ **STATUS:** Locked

---

## 1. BETRAYAL TRIGGERS (4 CAUSES)

| Trigger | Description | Severity |
|---------|-------------|----------|
| **Forced No-Show** | Worker misses a major formative promotion event (anniversary, title defense, emotional arc payoff) without mutual agreement | HIGH |
| **Disrespectful Exit** | Worker exits formative promotion without farewell matches, story closure, or loyalty acknowledgment | MEDIUM-HIGH |
| **Public Denouncement** | Worker speaks negatively about formative promotion post-departure, accelerates betrayal memory triggers | HIGH |
| **Careerist Jumping** | Worker visibly prioritizes bigger money or prestige despite formative emotional ties, creates fanbase resentment | MEDIUM |

### Trigger Severity Modifiers

| Factor | Effect on Severity |
|--------|-------------------|
| **Event Importance** | Anniversary/PPV = +20%, regular show = base |
| **Public Visibility** | High-profile = +15%, quiet = base |
| **Worker Status** | Main eventer = +10%, midcarder = base |
| **Promotion Health** | Struggling fed = +25%, healthy = base |
| **Fan Attachment** | High emotional investment = +20% |

---

## 2. EFFECT AREAS (4 CONSEQUENCES)

| Area | Impact | Duration |
|------|--------|----------|
| **Fanbase Loyalty Damage** | Fans emotionally tied to formative promotion partially or fully abandon the worker. Affects face reactions, merchandise sales, online narrative control. | 2-10 years |
| **Worker Emotional Stability Hit** | Internal loyalty, morale, and consistency ratings take small penalties reflecting guilt, cognitive dissonance, or backlash stress. | 1-5 years |
| **Career Arc Mutation** | Workers may find it harder to become universal babyfaces post-betrayal without hard redemption arcs later. Heel turns easier. | Until rehabilitated |
| **Historical Memory Scarring** | Decades later, betrayal scars remain part of historical writeups unless repaired or rewritten through emotional rehabilitation. | Permanent unless healed |

### Damage Severity Scale

| Betrayal Level | Fanbase Loss | Stability Hit | Arc Restriction | Memory Flag |
|----------------|--------------|---------------|-----------------|-------------|
| **Minor** | 5-15% | -5 | Slight difficulty | Footnote |
| **Moderate** | 15-30% | -10 | Notable difficulty | Mentioned |
| **Severe** | 30-50% | -20 | Major restriction | Prominent |
| **Catastrophic** | 50-75% | -35 | Near-impossible | Defining |

---

## 3. SIMULATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Loyalty Decay Roll** | After betrayal trigger, worker loyalty toward original promotion collapses sharply unless repaired by later respectful reconciliation events |
| **Fanbase Migration** | Betrayed fans either abandon worker entirely or emotionally "reassign" them to rival promotions (sometimes bitterly) |
| **Long-Term World Memory Flag** | Workers who betray formative homes are tagged in world history with emotional scars (unless redemption arcs overwrite) |
| **Rehabilitation Threshold** | Minimum time/actions required before betrayal can be healed |

### Loyalty Decay Amounts

| Trigger Type | Immediate Decay | Long-Term Decay |
|--------------|-----------------|-----------------|
| **Forced No-Show** | -25 to -40 | -10 to -20 |
| **Disrespectful Exit** | -20 to -35 | -15 to -25 |
| **Public Denouncement** | -30 to -50 | -20 to -30 |
| **Careerist Jumping** | -15 to -30 | -10 to -15 |

### Rehabilitation Requirements

| Betrayal Level | Minimum Time | Required Actions |
|----------------|--------------|------------------|
| **Minor** | 1 year | Public acknowledgment, one respectful appearance |
| **Moderate** | 2-3 years | Farewell tour, public apology, storyline closure |
| **Severe** | 5+ years | Extended redemption arc, major emotional moment |
| **Catastrophic** | 10+ years or never | Extraordinary circumstances, death of grudge-holders |

---

## 4. HISTORICAL MODELS

| Worker | Betrayal Memory |
|--------|-----------------|
| **Kawada/Misawa Complexity** | Depending on perspective, either could be seen as betrayer. Kawada loyalists see him as samurai who stayed. Misawa loyalists see him as savior who left. Emotional fracture, not simple betrayal. |
| **Ric Flair (1991-92 WWF Jump)** | Early NWA/Crockett fans viewed jump with mixed emotions despite logical career move. Big Gold Belt in WWF felt like kayfabe trauma. Partial rehabilitation through later returns. |
| **Cody Rhodes (Post-WWE Departure)** | Early emotional betrayal perceptions flipped into emotional rebirth narrative later. Successful rehabilitation rare but possible. AEW years rehabilitated, then WWE return created new complexity. |
| **Bret Hart (1997 WWF Exit)** | Montreal Screwjob created permanent betrayal memory, but victim status rather than betrayer. Complex case where company betrayed worker. |

### Cody Rhodes Rehabilitation Case Study

**Initial Betrayal:** Left WWE (formative promotion where he was built as legacy star).

**Perception:** Some fans saw as careerist jumping, others as principled departure.

**Rehabilitation Path:**
- AEW founding (created new formative loyalty)
- Emotional storytelling (Dusty tribute, authentic promos)
- Years of dedication to new project
- WWE return framed as homecoming, not betrayal of AEW

**Outcome:** Successful double rehabilitation. Rare case of healing betrayal perceptions at two different promotions.

---

## 5. IMPLEMENTATION NOTES

```json
{
  "betrayal_memory": {
    "worker_id": "ric_flair",
    "formative_promotion": "nwa_crockett",
    "betrayal_year": 1991,
    "trigger_type": "CAREERIST_JUMPING",
    "severity": "MODERATE",
    "effects": {
      "fanbase_damage": 0.25,
      "stability_hit": -10,
      "career_mutation": "HEEL_LEAN",
      "memory_flag": "MENTIONED"
    },
    "rehabilitation": {
      "status": "PARTIAL",
      "years_to_heal": 5,
      "healing_events": ["WCW_RETURN_1993", "FOUR_HORSEMEN_REVIVAL"]
    },
    "current_memory": "COMPLEX_LEGACY"
  }
}
```

---

## 6. PHILOSOPHY

> "Betrayal isn't just leaving. It's how you leave. A worker can move on with their head held high if they honor what came before. But abandon your home without respect, and the scar follows you forever, whispered in every crowd reaction, written into every retrospective, felt in every return that could have been a homecoming but becomes an apology tour instead."

Betrayal memory creates lasting consequences that make career decisions feel meaningful. It's not just about contracts: it's about emotional debts.

---

## 7. RELATED SYSTEMS

- [[Worker_Formative_Loyalty]] - What's being betrayed
- [[Worker_Prioritization_Multi_Promotion]] - Priority decisions that trigger betrayal
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Individual memory tracking
- [[Fanbase_Emotional_Migration]] - How fans react to betrayal
- [[Redemption_Arcs]] - How betrayal can be healed
- [[Historical_Betrayal_Fracture_Points]] - When betrayal memory splits

---

**Document Status:** Locked  
**Source:** Vol 5 lines 515-517  
**Next Review:** Integration with Redemption Arc system
