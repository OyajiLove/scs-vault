# Injury System

📛 **SYSTEM:** Worker Health and Injury Lifecycle
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** injury, health, wear, surgery, recovery, addiction, painkiller, style adaptation, retirement
📝 **SUMMARY:** Comprehensive system simulating the physical and psychological toll wrestling takes on workers. Covers accumulated wear, acute and chronic injuries, surgery decisions, addiction risks, and late-career style adaptation. Not "HP bars" but lived consequences.

⚙️ **LOGIC OVERVIEW:**
- Wear and tear accumulates silently even without visible injuries
- Acute injuries triggered by match intensity, bump severity, botch risk
- Chronic injuries emerge from accumulated damage crossing thresholds
- Surgery decisions shaped by finances, healthcare access, personality, booking pressure
- Painkiller usage creates addiction spiral risk
- Smart workers adapt styles to survive; prideful workers break down faster

🔬 **LLM INTEGRATION:** Minimal
- Injury narrative generation (optional)
- Medical report flavour text (optional)
- Comeback storyline suggestions based on injury history

📌 **ORIGIN:** Vol 4 (Double-L locked at line 5275)

---

## VERSION HISTORY

**Version 1.0 (Vol 4) [CURRENT - LOCKED]**
- Injury System fully formalized (Double-L document)
- Wear and Tear accumulation mechanics
- Acute vs chronic injury distinction
- Surgery decision-making system
- Painkiller and addiction risk mechanics
- Style adaptation for late career survival
- External accident triggers
- Historical context (Benoit, Edge, Dynamite Kid, Tanahashi)

---

📎 **CONNECTED SYSTEMS:**
- [[Hidden_Personality|Hidden Personality]] (Drive, Ego, Future Planning affect surgery decisions)
- [[Worker_Skills|Worker Skills]] (Durability, Athleticism affect recovery)
- [[Contract System/_Contract System Index|Contract System]] (Promotion support, healthcare coverage)
- [[Morale System]] (Injury affects mental state)
- [[Retirement System/_Retirement System Index|Retirement System]] (Career-ending injuries trigger forced retirement)
- [[Financial System]] (Surgery costs, healthcare access)
- [[Scandal System/_Scandal System Index|Scandal System]] (Addiction spirals can become public)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Wear and Tear System]] | Accumulated damage over time | Locked |
| [[Injury Types]] | Acute, chronic, severity grades, body systems | Locked |
| [[Surgery and Recovery]] | Healthcare access, decision-making, timelines | Locked |
| [[Addiction Risk System]] | Painkiller usage, addiction spirals, recovery | Locked |
| [[Style Adaptation]] | Late career survival, refusal consequences | Locked |
| [[External Accidents]] | Non-wrestling injuries (car crashes, etc.) | Locked |

---

## Design Philosophy

This is not "HP bars" or random injury pop-ups. We simulate life: the cost of wrestling on bodies, minds, and careers.

**Core truths this system captures:**
- Wrestling eats lives quietly through pills before fans notice
- Surgery decisions shape lives forever
- Not every injury shows on TV
- Some injuries destroy golden careers in an instant
- Pain management is not free
- Style isn't just about what looks cool: it's about survival

**The forge burns everyone differently, deeply.**

---

## What We Simulate

| Reality | How We Simulate |
|---------|-----------------|
| **Wear and Tear** | Accumulated damage over time even without "injuries." Not all pain is visible. |
| **Real Injuries** | Acute events (torn ACL, broken neck, concussions) impacting short- and long-term career arcs. |
| **Surgical Repair** | Optional or mandatory surgeries: wrestlers choose or delay based on Drive, Fear, Booking Pressure. |
| **Painkiller/Drug Risk** | Management choices lead to spirals: masking pain leads to breakdowns, addictions, deaths. |
| **Body Style Aging** | Different styles destroy different parts of body faster (deathmatch = blood loss, workrate = joints, strong style = spine). |
| **Late Career Style Shifts** | Smart workers shift styles to survive (Tanahashi, Nagata). |
| **Early Retirement** | Catastrophic injuries, mental burnout, drug spirals can cause early retirements. |
| **Tough Guy Myths** | Workers remembered for fighting through injuries: sometimes legendary, sometimes tragic. |

---

## Historical Context

Real-world injury dynamics inform this system:

- **Chris Benoit:** Accumulated brain damage, tragic end
- **Edge:** Multiple neck surgeries, forced retirement, eventual comeback
- **Dynamite Kid:** Style destruction, wheelchair by 50s
- **Tanahashi:** Knee destruction, successful style adaptation
- **Stone Cold:** Broken neck, worked through it, shortened career
- **Hayabusa:** Paralysis from broken neck on basic move

---

## Open Questions

- [ ] Exact bump counter thresholds for triggering chronic conditions
- [ ] Probability formulas for surgical success/failure
- [ ] Addiction threshold values and reset mechanics
- [ ] Era-specific injury likelihood modifiers
- [ ] Insurance/healthcare cost structures by region

---

## Implementation Notes

```json
{
  "worker_health": {
    "worker_id": "worker_001",
    "wear_and_tear": {
      "total_bumps": 4500,
      "high_impact_bumps": 890,
      "style_wear": {
        "knees": 72,
        "back": 45,
        "neck": 38
      }
    },
    "current_injuries": [],
    "chronic_conditions": [
      { "type": "knee_deterioration", "severity": "moderate" }
    ],
    "surgical_history": [
      { "type": "acl_repair", "date": "1983-06-15", "success": true }
    ],
    "painkiller_usage": {
      "current_level": 3,
      "addiction_threshold": 10,
      "history": []
    },
    "style_adapted": false,
    "recovery_efficiency": 0.85
  }
}
```

---

**Document Status:** Locked (Vol 4, Double-L)
**Last Updated:** 2025-12-20
**Next Review:** Integrate with Financial System for healthcare costs
