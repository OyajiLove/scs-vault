# Health System

📛 **SYSTEM ID:** HEALTH-001
🧭 **CATEGORY:** Worker Longevity / Career Management
🔑 **KEYWORDS:** injury, health, wear and tear, recovery, lifestyle, aging, medical, stamina
📝 **SUMMARY:** 

The Health System governs worker physical condition over time, including injury risk, recovery rates, cumulative wear and tear, and lifestyle factors that affect career longevity. It connects to match booking, training, aging, and retirement systems.

⚙️ **LOGIC OVERVIEW:**
- Workers accumulate damage from matches (acute injuries and cumulative wear)
- Recovery rates vary by worker attributes and rest time
- Lifestyle choices affect aging curves and injury susceptibility
- Medical exams can reveal hidden damage
- Era affects injury handling (kayfabe era swept under rug, modern era transparency)
- Certain match types and styles accelerate wear

🔬 **LLM INTEGRATION:** Minimal (numeric tracking), but LLM can generate injury descriptions and recovery narratives

📌 **ORIGIN:** Vol 1 Extraction #45, #163-176, Vol 4 (Scandal System injury tie-ins)

📎 **CONNECTED SYSTEMS:**
- [[Worker_Skills]] - Stats affected by injuries
- [[Booking_Engine_P1-3]] - Cumulative Fatigue System
- [[Training System/_Training System Index|Training System]] - Recovery and rehabilitation
- [[Aging System]] - Long-term health effects
- [[Scandal System/_Scandal System Index|Scandal System]] - Injury cover-ups, working hurt

❓ **OPEN QUESTIONS:**
- Exact injury probability formulas per match type
- Recovery time calculations
- Long-term stat degradation formulas
- Concussion protocol mechanics

✅ **STATUS:** Conceptual (formulas pending)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Injury Mechanics]] | Acute injury types, probability, effects | 📝 Conceptual |
| [[Wear and Tear System]] | Cumulative damage tracking | 📝 Conceptual |
| [[Lifestyle Tracker]] | Lifestyle factors affecting health | 🔒 Locked (concept) |
| [[Recovery System]] | Healing rates and rehabilitation | 📝 Conceptual |
| [[Medical Exams]] | Hidden damage detection | 📝 Conceptual |

---

## Design Philosophy

Health isn't just "injury prone" as a hidden stat. It's a dynamic system where:

1. **Booking Choices Matter:** Stiff matches, deathmatches, and tournaments take real tolls
2. **Style Affects Longevity:** High flyers break down differently than technicians
3. **Lifestyle Is Consequential:** Hard living shows on the body over time
4. **Recovery Isn't Magic:** Rushed comebacks risk further damage
5. **Era Context:** Older eras ignored injuries; modern era has protocols

---

## Implementation Priority

**Phase 1 (MVP):** Basic injury probability, recovery timers
**Phase 2:** Cumulative wear tracking, lifestyle modifiers
**Phase 3:** Full dynamic health simulation with career-ending injuries

---

**Document Status:** Index Created
**Last Updated:** 2024-12-23
