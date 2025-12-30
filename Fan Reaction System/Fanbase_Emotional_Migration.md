# Fanbase Emotional Migration System

📛 **NAME:** Fanbase Emotional Migration System  
🧭 **CATEGORY:** Fan Reaction System / Crowd Dynamics  
🔑 **KEYWORDS:** migration, fanbase, exodus, drift, loyalty, worker anchor, promotion identity  
📝 **SUMMARY:** Models how fanbases emotionally drift between promotions after collapses, worker exodus, cultural shifts, or new movement emergence. Different fan archetypes migrate differently: purists seek prestige, crash TV fans chase chaos, cult loyalists stay until catastrophic betrayal.

⚙️ **LOGIC OVERVIEW:**
- 5 triggers cause fan migration (Golden Era collapse, worker exodus, cultural drift, new movements, world shifts)
- 5 fan archetypes with distinct migration behaviors
- Worker Anchor Effect: fans follow beloved workers to new homes
- Promotion Identity Resonance: clear emotional identity attracts drifting fans faster
- Migration is gradual, not instantaneous (demographic weighting)

🔬 **LLM INTEGRATION:** Minimal (deterministic migration tracking; LLM could generate fan discourse, migration narratives)

📌 **ORIGIN:** Vol 5 lines 412-415 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Fanbase_Emotional_Exodus]] - Exodus triggers migration
- [[Golden_Era_Collapse_Memory]] - Collapse drives fans out
- [[Worker_Loyalty_Drift]] - Worker movements pull fans
- [[New_Movement_Birth]] - New promotions catch migrants
- [[Fanbase_Cultural_Mutation]] - Migration changes fan culture

❓ **OPEN QUESTIONS:**
- Exact migration velocity calculations
- Worker anchor strength thresholds
- Cross-regional migration patterns
- How long migration waves last

✅ **STATUS:** Locked

---

## 1. MIGRATION TRIGGERS (5 CAUSES)

| Trigger | Description |
|---------|-------------|
| **Golden Era Collapse** | Collapse of emotional trust after betrayal, decay, or booking drift |
| **Worker Exodus** | Stars fans loved move elsewhere: loyalty drifts to where emotional anchors land |
| **Promotion Cultural Drift** | Home promotion no longer represents their emotional needs (too corporate, too ironic, too stagnant) |
| **New Movement Emerges** | Indie booms, splinter promotions, exile movements start emotionally "catching" displaced fans |
| **World Cultural Shifts** | Political, economic, social changes alter what fans want emotionally from wrestling |

---

## 2. FAN ARCHETYPE MIGRATION BEHAVIORS (5 TYPES)

| Archetype | Migration Behavior |
|-----------|-------------------|
| **Purists** | Drift toward promotions emphasizing serious storytelling, in-ring prestige, emotional arcs |
| **Crash TV Fans** | Drift toward wild, spectacle-driven promotions when emotional chaos feels honest |
| **Cynical Ironists** | Drift toward promotions blending irony, shock, realism, and self-awareness |
| **Workrate Fetishists** | Drift to ultra-match quality promotions: technical excellence over narratives |
| **Cult Loyalists** | Stay emotionally attached to old home until catastrophic betrayal or collapse |

### Migration Speed by Archetype

| Archetype | Speed | Notes |
|-----------|-------|-------|
| **Purists** | Medium | Thoughtful migration, seek quality |
| **Crash TV Fans** | Fast | Chase heat and buzz |
| **Cynical Ironists** | Fast | Quick to abandon, quick to adopt |
| **Workrate Fetishists** | Medium | Follow match quality metrics |
| **Cult Loyalists** | Very Slow | Only move after total betrayal |

---

## 3. SIMULATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Fan Demographic Migration Weighting** | Fans don't all leave at once: emotional strength and demographics affect migration speed |
| **Worker Anchor Effect** | If beloved workers jump to new promotions, fan segments follow them naturally |
| **Promotion Identity Resonance** | Promotions with clear emotional identity (e.g., AEW 2019-2020, NOAH 2000-2002) attract drifting fans faster |
| **External World Drift Matching** | Promotions that match new world cultural mood catch migrating fans automatically |

### Worker Anchor Strength

| Worker Tier | Fan Migration Pull |
|-------------|-------------------|
| **Immortal Icon** | 40-60% of their fan segment follows |
| **Era Star** | 25-40% follows |
| **Beloved Pillar** | 15-25% follows |
| **Master Technician** | 10-15% follows |
| **Average Worker** | Minimal pull |

### Identity Resonance Bonus

| Identity Clarity | Migration Attraction Bonus |
|------------------|---------------------------|
| **Crystal Clear** (ECW rebellion, NOAH purism) | +30% migration speed |
| **Strong** (AEW alternative) | +20% |
| **Moderate** | +10% |
| **Confused/Mixed** | No bonus |
| **Identity Crisis** | -20% (repels migrants) |

---

## 4. HISTORICAL MODELS

| Event | Migration Outcome |
|-------|-------------------|
| **WCW to WWF (2000-2001)** | Fans abandoned WCW en masse as loyalty and trust collapsed: migrated to Attitude Era WWF |
| **AJPW to NOAH (2000)** | King's Road purists emotionally migrated almost overnight with Misawa and crew |
| **WWE PG Shift (Mid-2000s)** | Purists, crash TV loyalists drifted to ROH, NJPW, and indies |
| **AEW Fan Fractures (2022-Present)** | Early Elite purists vs Punk realists vs Swerve/Hangman emotional movement fans |

### NOAH Migration Case Study

**Trigger:** Misawa led exodus from AJPW after Baba death political crisis.

**Worker Anchors:** Misawa (Immortal Icon), Kobashi (Era Star), Taue, Akiyama (Beloved Pillars).

**Fan Migration:** Near-total purist migration. AJPW left with skeleton fanbase.

**Speed:** Almost overnight for hardcore purists. Casual fans followed over 6-12 months.

**Identity Resonance:** NOAH positioned as "true King's Road spirit" = maximum resonance bonus.

---

## 5. IMPLEMENTATION NOTES

```json
{
  "migration_event": {
    "source_promotion": "ajpw",
    "destination_promotion": "noah",
    "trigger": "WORKER_EXODUS",
    "year": 2000,
    "worker_anchors": ["misawa", "kobashi", "taue", "akiyama"],
    "fan_segments_migrated": {
      "purists": 0.85,
      "cult_loyalists": 0.60,
      "casual": 0.40
    },
    "migration_duration_months": 12,
    "source_fanbase_remaining": 0.25,
    "destination_identity_resonance": "CRYSTAL_CLEAR"
  }
}
```

---

## 6. RELATED SYSTEMS

- [[Fanbase_Emotional_Exodus]] - Triggers migration
- [[Golden_Era_Collapse_Memory]] - Collapse context
- [[Worker_Loyalty_Drift]] - Worker movements
- [[New_Movement_Birth]] - New homes for migrants
- [[Exiled_Faction_Formation]] - Exile movements attract fans
- [[Survivor_Promotion_Mechanics]] - What's left behind

---

**Document Status:** Locked  
**Source:** Vol 5 lines 412-415  
**Next Review:** Integration with regional migration patterns
