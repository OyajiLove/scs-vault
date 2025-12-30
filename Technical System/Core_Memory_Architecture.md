# Core Memory Architecture Map

📛 **NAME:** Core Memory Architecture Map  
🧭 **CATEGORY:** Technical System / Architecture  
🔑 **KEYWORDS:** memory, architecture, layer, flow, worker, promotion, fanbase, world, artifact, integration  
📝 **SUMMARY:** The foundational architecture showing how all memory systems in SCS interconnect. Five core memory layers (Worker, Promotion, Fanbase, World, Artifact) share emotional data through defined flows. Events ripple through layers creating emergent historical narratives. This is the "bloodstream" that makes SCS feel alive.

⚙️ **LOGIC OVERVIEW:**
- 5 core memory layers with distinct purposes
- Memory flows define how events ripple between layers
- All systems hook into shared emotional weight APIs
- Memory compression handles long-term save management
- Fractured memory by demographic creates organic historical debates

🔬 **LLM INTEGRATION:** High (LLM could access memory layers for narrative generation, historical context, character development)

📌 **ORIGIN:** Vol 5 lines 545-546 (locked)

📎 **CONNECTED SYSTEMS:**
- ALL memory-related systems connect through this architecture
- [[Career_Memory_Management_MDOD]] - Technical implementation
- [[World_Memory_Drift]] - World layer specifics
- [[Cultural_Artifact_Memory]] - Artifact layer specifics
- [[Worker_Loyalty_Drift]] - Worker layer specifics

❓ **OPEN QUESTIONS:**
- Exact API specifications for inter-layer communication
- Memory layer priority when conflicts arise
- Performance benchmarks for memory operations
- Serialization format for save files

✅ **STATUS:** Locked

---

## 1. THE FIVE MEMORY LAYERS

| Layer | What It Stores | Update Frequency |
|-------|----------------|------------------|
| **Worker Memory** | Betrayals, loyalty arcs, career-defining matches, emotional rises/falls, legacy drift. Hidden and visible career histories. | Per-event |
| **Promotion Memory** | Golden eras, collapses, philosophical betrayals, cultural shifts, scandals, resurgence arcs. Affects booking trust, fan loyalty, talent migrations. | Per-show/Per-event |
| **Fanbase Memory** | Emotional loyalty to workers, promotions, eras, titles, styles, fractured by betrayals and shifts. Drives emotional buy-in, rebellions, nostalgia waves. | Per-show |
| **World Memory** | Major global events (eras, scandals, rediscoveries, collapses). How generations remember wrestling history. Public perception. | Per-year/Per-major-event |
| **Artifact Memory** | Emotional weight of belts, arenas, logos, magazines, music, images. Carries nostalgia, betrayal scars, myth reinforcement. | Per-change/Per-event |

---

## 2. MEMORY FLOW DIAGRAM

```
┌─────────────────────────────────────────────────────────────────┐
│                        WORLD MEMORY                              │
│    (Generational perception, historical consensus, myths)        │
└─────────────────────────────────────────────────────────────────┘
        ▲                    ▲                    ▲
        │                    │                    │
        │         ┌─────────────────────┐        │
        │         │   FANBASE MEMORY    │        │
        │         │  (Loyalty, trust,   │        │
        │         │   emotional buy-in) │        │
        │         └─────────────────────┘        │
        │              ▲           ▲             │
        │              │           │             │
┌───────────────┐      │           │      ┌──────────────────┐
│ WORKER MEMORY │──────┘           └──────│ PROMOTION MEMORY │
│  (Careers,    │                         │  (Eras, scandals,│
│   betrayals)  │                         │   philosophy)    │
└───────────────┘                         └──────────────────┘
        ▲                                         ▲
        │                                         │
        └────────────┬───────────────────────────┘
                     │
              ┌──────────────────┐
              │ ARTIFACT MEMORY  │
              │ (Belts, arenas,  │
              │  logos, themes)  │
              └──────────────────┘
```

---

## 3. MEMORY FLOWS (DETAILED)

| From | To | Trigger | Example |
|------|-----|---------|---------|
| **Worker Actions** | Worker → Promotion → Fanbase → World | Betrayals, loyalty shifts, emotional arcs | Worker betrays home fed → Promotion trust damaged → Fans split → World remembers as historical event |
| **Promotion Actions** | Promotion → Fanbase → World | Booking decisions, collapse, scandals | Promotion collapses → Fans traumatized → World memory of era crystallizes |
| **Fan Reactions** | Fanbase → Worker and Promotion | Migration, loyalty decay, rebellion | Fans migrate to new fed → Worker popularity shifts → Promotion loses audience |
| **Artifact Events** | Artifact → Fanbase → World | Belts retired, arenas demolished, logos changed | Classic belt retired → Fans upset → Historical significance elevated |
| **Rediscovery** | World → Worker/Promotion/Artifact | Hidden classics revived, myths collapse | Documentary exposes truth → Worker reputation re-evaluated → Artifacts gain new meaning |

---

## 4. SHARED EMOTIONAL WEIGHT SYSTEM

All memory layers use a shared emotional weight scoring system:

| Weight Level | Score Range | Persistence | Example |
|--------------|-------------|-------------|---------|
| **Trivial** | 0-10 | Auto-decay (1 year) | Random undercard match |
| **Minor** | 11-30 | Slow decay (5 years) | Mid-card title change |
| **Significant** | 31-60 | Long persistence (20 years) | Main event at major show |
| **Major** | 61-85 | Very long (50+ years) | Championship classic, betrayal |
| **Legendary** | 86-100 | Permanent | Career-defining, era-defining |

### Emotional Weight Modifiers

| Modifier | Effect |
|----------|--------|
| **Worker Tier** | Immortal Icon events +30, Jobber events -20 |
| **Event Importance** | PPV main event +20, dark match -15 |
| **Emotional Stakes** | Betrayal/redemption +25, routine defense +0 |
| **Fan Investment** | High crowd engagement +15, dead crowd -10 |
| **Historical Context** | First/last occurrence +20, repetition -5 |

---

## 5. INTER-LAYER COMMUNICATION API

### Event Propagation

When an event occurs, it propagates through layers:

```json
{
  "event": {
    "type": "BETRAYAL",
    "source_layer": "WORKER",
    "primary_subject": "worker_123",
    "secondary_subjects": ["promotion_456", "worker_789"],
    "emotional_weight": 75,
    "propagation": [
      {"target": "PROMOTION_MEMORY", "weight_modifier": 0.8},
      {"target": "FANBASE_MEMORY", "weight_modifier": 1.0},
      {"target": "WORLD_MEMORY", "weight_modifier": 0.6, "delay": "5_YEARS"}
    ]
  }
}
```

### Memory Query

Systems can query across layers:

```json
{
  "query": {
    "subject": "worker_123",
    "layers": ["WORKER", "FANBASE", "WORLD"],
    "time_range": {"start": 1990, "end": 2000},
    "event_types": ["BETRAYAL", "TITLE_WIN", "LEGENDARY_MATCH"],
    "min_weight": 50
  }
}
```

---

## 6. MEMORY COMPRESSION AND DECAY

### Automatic Compression Rules

| Memory Age | Compression Level |
|------------|-------------------|
| 0-5 years | Full detail |
| 5-15 years | Summarized (key moments preserved) |
| 15-30 years | Highlights only (legendary events) |
| 30+ years | Mythologized (simplified narratives) |

### Decay Exceptions

| Condition | Effect |
|-----------|--------|
| **Emotional Weight > 80** | Never decays |
| **Active Reference** | Decay paused while referenced |
| **Rediscovery Event** | Compressed memory re-expanded |
| **Player Pinned** | Never decays |

---

## 7. FRACTURED MEMORY BY DEMOGRAPHIC

Different fan groups remember the same events differently:

| Demographic | Memory Bias |
|-------------|-------------|
| **Hardcore Fans** | Preserve nuance, resist simplification |
| **Casual Fans** | Accept mainstream narrative |
| **Regional Fans** | Emphasize local/regional events |
| **Generational Fans** | Mythologize their formative era |
| **Cynical Fans** | Emphasize scandals, betrayals |

### Memory Consensus Calculation

```
World_Consensus = (Hardcore × 0.15) + (Casual × 0.50) + 
                  (Regional × 0.10) + (Generational × 0.15) + 
                  (Cynical × 0.10)
```

---

## 8. IMPLEMENTATION PRIORITIES

| Step | Action | Priority |
|------|--------|----------|
| **1. Core Memory System** | World + Worker + Promotion + Artifact defined cleanly | CRITICAL |
| **2. Emotional Event Hooks** | Betrayals, scandals, title wins trigger shifts automatically | CRITICAL |
| **3. Memory Decay/Rediscovery** | Light pruning, powerful rediscovery events | HIGH |
| **4. Player UX Layer** | Natural history display without micromanagement | HIGH |
| **5. Modular Expansion** | New systems plug into existing flows | MEDIUM |

---

## 9. PHILOSOPHY

> "Memory is the bloodstream. Every system breathes memory — every betrayal scars it. Every rediscovery heals it. Every fanbase, worker, title, and promotion lives and dies inside it."

This architecture ensures SCS doesn't feel like disconnected mechanics. Everything is connected through shared emotional truth. Events ripple naturally. History emerges organically. The world feels alive because it remembers.

---

## 10. RELATED SYSTEMS

- [[Career_Memory_Management_MDOD]] - Technical memory storage
- [[World_Memory_Drift]] - World layer mechanics
- [[Cultural_Artifact_Memory]] - Artifact layer mechanics
- [[Worker_Loyalty_Drift]] - Worker layer mechanics
- [[Fanbase_Cultural_Mutation]] - Fanbase layer mechanics
- [[Historical_Betrayal_Fracture_Points]] - Memory fracturing

---

**Document Status:** Locked  
**Source:** Vol 5 lines 545-546  
**Next Review:** Implementation specification phase
