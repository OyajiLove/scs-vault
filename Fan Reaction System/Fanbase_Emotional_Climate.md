# Fanbase Emotional Climate System (FEC)

📛 **NAME:** Fanbase Emotional Climate System (FEC)  
🧭 **CATEGORY:** Fan Reaction / LMC Subsystem  
🔑 **KEYWORDS:** fanbase, crowd, emotional, macro, micro, climate, drift, burnout, hope, rebellion, nostalgia  
📝 **SUMMARY:** Two-layer system tracking both world-level emotional atmosphere (Macro) and live show audience state (Micro). Macro affects booking philosophies and fan patience over years. Micro affects night-to-night show structure, detecting when crowds burn out or crave specific emotional payoffs. Road Agents use FEC to advise audibles.

⚙️ **LOGIC OVERVIEW:**
- Macro Climate: World emotional mood lasting years (Hopeful, Irony, Rebellion, Collapse, Nostalgia, Healing)
- Micro Climate: Live audience state updating per segment (Burnt, Violence-craving, Hope-starved, Joyful, Shell-shocked, Restless)
- Both layers active simultaneously
- Drift mechanics track how events shift climate states
- Road Agents warn when Micro Climate makes planned booking risky

🔬 **LLM INTEGRATION:** High (LLM can generate climate-aware booking suggestions, detect drift patterns, write crowd reaction descriptions)

📌 **ORIGIN:** Vol 5 lines 789-810

📎 **CONNECTED SYSTEMS:**
- [[Living_Match_Context_System]] - FEC is primary input
- [[Road_Agent_Layer_System]] - agents use FEC for warnings
- [[Emotional_Show_Flow]] - Micro Climate affects show pacing
- [[World_Memory_Drift]] - major events trigger Macro shifts
- [[Crowd_Memory]] - climate affects memory formation

❓ **OPEN QUESTIONS:**
- Exact duration of Macro Climate states
- Micro Climate decay/recovery rates per segment
- How regional variation affects climate
- Player ability to read/predict climate shifts

✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5 | 🔒 LOCKED |

---

## Two-Layer Architecture

| Layer | Scope | Duration | Updates |
|-------|-------|----------|---------|
| **Macro Climate** | World/industry-wide | Years | Major events (betrayals, scandals, tragedies, booms) |
| **Micro Climate** | Live audience at show | Per segment | Match results, promos, injuries, swerves |

✅ Both matter simultaneously.  
✅ Road Agents must recognize Micro moment and advise properly.  
✅ Worker history adds subtle flavor (scar tissue, emotional exhaustion, psychological trauma).

---

## Macro Emotional Climate ✅ LOCKED

The world's wrestling emotional mood at large scale:

| Climate | Description | Booking/Fan Behavior |
|---------|-------------|---------------------|
| **Hopeful Era** | Boom periods, beloved champions, uplifting stories | Fans patient with slow burns, big payoffs expected |
| **Irony Era** | Post-betrayal exhaustion, fans cynical, mockery high | Fans reject sincerity, pop for chaos and meme moments |
| **Rebellion Era** | Betrayed fanbases craving underdog victories | Fans crave upsets, rebellion arcs, corruption being shattered |
| **Collapse Era** | Promotions crumbling emotionally, trust loss | Fans fickle, desperate, angry, unpredictable reactions |
| **Nostalgia Era** | World clinging to past legends | Fans crave tributes, callbacks, returns, legacy matches |
| **Healing Era** | After collapse or tragedy, fans tender, emotional | Fans respond to sincerity, redemption arcs, forgiveness themes |

**Triggers:** World events (major betrayals, scandals, tragedies, golden eras ending) trigger shifts.  
**Duration:** These states last years unless massive emotional shocks accelerate transition.

---

## Micro Emotional Climate ✅ LOCKED

The crowd's mood right now, based on the show itself:

| Climate | Description | Booking Reaction Needed |
|---------|-------------|------------------------|
| **Emotionally Burnt** | Crowd exhausted after long matches, heavy emotion | Need sprints, chaos, humor, shock to re-ignite |
| **Violence Craving** | Crowd demanding blood, brutality, catharsis | Need hardcore matches, brawls, wild finishes |
| **Hope Starved** | Crowd desperate for underdog to finally break through | Need meaningful, credible triumphs. Avoid hollow victories. |
| **Joyful** | Crowd playful, ironic, in good spirits | Comedy matches, spotfests, wild characters thrive |
| **Shell-Shocked** | Crowd emotionally shattered by betrayals, injuries, deaths | Need careful emotional pacing. Avoid overloading. |
| **Anxious/Restless** | Crowd bored, anxious for something big to happen | Need major angle, turn, title change, shock moment |

**Updates:** Micro Climate updates live across the show based on matches, promos, injuries, swerves.  
**Road Agents:** Can warn if Micro Climate is drifting dangerously.

---

## FEC Drift Mechanics ✅ LOCKED

| Trigger | Macro or Micro? | Effect |
|---------|-----------------|--------|
| Huge betrayal storyline | Macro | Shifts world toward Rebellion or Collapse |
| Main event betrayal turn | Micro | Spikes audience anger, risks burnout if not managed |
| Workrate boom era | Macro | Fans tolerate longer technical matches, grow less patient with soap opera |
| Comedy match bombed earlier in show | Micro | Fans more cynical about lighthearted matches for next few segments |
| Brutal bloodbath early in show | Micro | Fans may become numb, need emotional recharging |
| Major tragedy (death, scandal) | Macro | Shifts toward Healing or Collapse depending on handling |
| Underdog finally wins big | Micro | Hope Starved → Joyful transition, catharsis achieved |

---

## FEC Inputs Summary

| Input Type | Examples |
|------------|----------|
| **Booking trends** | Match structures, finishes, pacing, promotion styles |
| **Worker arcs** | Betrayals, retirements, tragic deaths, inspirational rises |
| **Industry-wide events** | Company closures, booms, scandals, wars |
| **Show pacing** | How a single night is built emotionally |
| **Crowd reaction events** | Live crowd fatigue, anger, catharsis bursts |

---

## Practical Example

**Planned Match:** Epic 30-minute title match

**Micro Climate Reality:** Crowd is already emotionally drained after two major blood feuds earlier on the card.

**Road Agent Warning:**
```
📜 Crowd Emotional Alert:
- Crowd visibly burnt out after two heavy emotional matches.
- Planned 30-min Epic risks killing momentum and damaging crowd loyalty.
- Recommend audible to a shorter, sprint-paced war match with clean escalation to final hope spot.
- Optional: Worker A visible scar tissue could be exploited with a safe hardway near fall to re-ignite sympathy surge.
```

**Philosophy:** Road Agenting becomes an artform, not just a checklist. Booking becomes living, not mechanical.

---

## Connected Mechanics

- [[Living_Match_Context_System]] - FEC feeds into LMC
- [[Road_Agent_Layer_System]] - agents use FEC warnings
- [[Emotional_Show_Flow]] - Micro Climate affects pacing
- [[Crowd_Memory]] - climate affects memory formation
- [[World_Memory_Drift]] - major events trigger Macro shifts

---

## Implementation Notes

```json
{
  "fanbase_emotional_climate": {
    "macro_climate": {
      "current_state": "REBELLION_ERA",
      "duration_years": 2,
      "trigger_event": "WWE_PIPE_BOMB_2011",
      "fan_behavior": {
        "patience": "low",
        "underdog_craving": "high",
        "cynicism": "medium"
      }
    },
    "micro_climate": {
      "current_state": "HOPE_STARVED",
      "segments_in_state": 3,
      "previous_state": "EMOTIONALLY_BURNT",
      "recommended_booking": "meaningful_underdog_triumph"
    }
  }
}
```

---

**Document Status:** Locked  
**Source:** Vol 5 lines 789-810  
**Next Review:** Integration with Road Agent warning system
