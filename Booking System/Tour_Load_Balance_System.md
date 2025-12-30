# TOUR LOAD BALANCE SYSTEM

📛 **NAME:** Tour Load Balance System
🧭 **CATEGORY:** Booking System / Tour Management
🔑 **KEYWORDS:** tour, workload, burnout, pacing, multi-show, fatigue, agent feedback
📝 **SUMMARY:** A macro-level planning system that visualizes worker usage, match type overlap, and emotional pacing across multiple shows. Helps prevent burnout while maintaining narrative momentum.

⚙️ **LOGIC OVERVIEW:**
- Shows worker usage frequency across tour dates
- Flags match type repetition (e.g., "fourth cage match this tour")
- Displays emotional weight distribution (too many blowoffs, no cooldowns)
- Agent tour reports identify physical/emotional drain risks
- Story tracker flags stagnating or overexposed feuds
- Crowd flow forecast predicts cold periods

🔬 **LLM INTEGRATION:** Minimal (agent feedback text generation, crowd forecast narrative)

📌 **ORIGIN:** Vol 3, lines 509-511

📎 **CONNECTED SYSTEMS:**
- [[Emotional_Show_Flow]] - Show-level emotional pacing
- [[AutoBooker_System]] - Can receive tour-level rules
- [[Agent_System]] - Generates tour feedback
- [[Injury_System]] - Burnout risk calculations
- [[Worker_Morale_System]] - Workload fairness impact

❓ **OPEN QUESTIONS:**
- Exact formula for "injury risk prevention" through pacing
- How many shows constitute a "tour" (player-defined or preset?)
- Integration with contract "required appearances" system

✅ **STATUS:** Locked (Vol 3)

---

## CORE TOOLS

| Tool | Function |
|------|----------|
| Worker Usage Map | "You've booked Konishi in 5 of the next 7 shows. 3 singles, 2 tags." |
| Match Type Overlap Flag | "That's your fourth cage match this tour. Crowd fatigue likely." |
| Heat Map View | Emotional weight of each show: too many blowoffs? No cooldowns? |
| Agent Tour Reports | "Week 2 has six guys who wrestle three nights in a row. Your call." |
| Story Tracker | Flags feuds that aren't progressing, or are overexposed |
| Crowd Flow Forecast | "The second weekend will feel cold unless you juice these undercard stories." |
| "Let AutoSpace" Button | Lets assistant offer reshuffled show structure for pacing |

---

## EXAMPLE IN PRACTICE

Opening Tour Manager shows:

```
Night 1 (Osaka)
- Konishi vs Tsukasa (Main Event)
- Steel & Wildfire vs Velocity (Tag Semi)

Night 2 (Nagoya)
- Tsukasa vs Raven
- Konishi post-match interview

Night 3 (Tokyo)
- Konishi vs Steel (Semi-Main)
- Raven promo on Tsukasa
```

Agent note slides in:
> "Konishi's taking lead on three straight shows. Just flagging the physical and emotional drain." – Riku

Player options:
- Shift one match to a tag
- Delay the big blowoff
- Use an off-night promo to rest the body but push the arc

---

## SYSTEM IMPACTS

| System | Effect |
|--------|--------|
| Injury Risk | Preventable with better show pacing |
| Worker Morale | Rises when workload feels fair and story feels meaningful |
| Fan Trust | Avoids overexposure, gives emotional highs time to land |
| Agent Relationships | Better spacing = more respectful booking = loyalty |
| Booking Reputation | "That tour was tight, emotional, and clean." vs. "They looked dead by week two." |

---

## RELATED SYSTEMS

- [[Calendar_UI_System]] - Visual interface for tour planning
- [[Segment_Emotional_Weight_System]] - Per-segment emotional tracking
- [[AutoBooker_System]] - House show mode integration

---

**Document Status:** Locked
**Version:** 1.0 (Vol 3)
**Next Review:** Integration with contract obligation tracking
