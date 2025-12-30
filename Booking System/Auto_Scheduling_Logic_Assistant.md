# AUTO-SCHEDULING LOGIC ASSISTANT

📛 **NAME:** Auto-Scheduling Logic Assistant
🧭 **CATEGORY:** Booking System / Planning Tools
🔑 **KEYWORDS:** scheduling, title defence, contracts, obligations, TV, network, rhythm, pacing
📝 **SUMMARY:** A smart assistant layer that helps track TV deal demands, title defence schedules, push pacing, and contractual obligations without taking over the player's booking style. Not a full AutoBooker, but a rhythm management tool.

⚙️ **LOGIC OVERVIEW:**
- Tracks weekly rhythm (build, peak, fallout, go-home, cooldown)
- Reminds when title defences are overdue
- Alerts on contract obligation deadlines
- Warns when story arcs are stagnating
- Integrates network notes if tied to broadcast partner
- Three behaviour modes: Soft Guidance, Active Planning, Hands-Off

🔬 **LLM INTEGRATION:** Minimal (agent message generation)

📌 **ORIGIN:** Vol 3, lines 596-602

📎 **CONNECTED SYSTEMS:**
- [[Calendar_UI_System]] - Visual interface for reminders
- [[Contract_System]] - Obligation tracking
- [[AutoBooker_System]] - Can receive rules from scheduler
- [[Tour_Load_Balance_System]] - Multi-show pacing
- [[Booker_Memory_Engine]] - Learns player's natural pacing

❓ **OPEN QUESTIONS:**
- How "firm" can network notes get before consequences?
- Specific thresholds for "story stagnation" warnings
- Integration with house show vs TV show distinction

✅ **STATUS:** Locked (Vol 3)

---

## CORE FEATURES

| Feature | Description |
|---------|-------------|
| Weekly Rhythm Planner | Shows each show's function (build, peak, fallout, go-home, cooldown) |
| Title Defence Reminder | "TV Title hasn't been defended in 3 weeks — network may notice." |
| Contract Obligation Alerts | "Shinobu needs one more singles match this month to fulfil their deal." |
| Story Progression Pacing | "Your main arc is stagnating — fans may start losing interest by next taping." |
| Network Notes | If tied to broadcast partner: "Viewership was high last title match. Can we build to another in 2 weeks?" |

---

## BEHAVIOUR MODES

| Mode | Result |
|------|--------|
| Soft Guidance (Default) | Sticky note reminders, agent whispers, emails |
| Active Planning Mode | Auto-fills tentative skeletons of next month's shows — you edit |
| Hands-Off | You do everything manually — no reminders unless crisis triggers |

---

## EXAMPLE MESSAGES

> "Gedo-style build detected: slow tension. Crowd may want a major payoff on your 4th show."

> "You haven't defended the secondary belt on TV in 5 weeks. That's a red flag for fan engagement."

> "X has a clause requiring 1 promo segment per tour. They've said nothing all month."

---

## SYSTEM INTERACTIONS

| System | Effect |
|--------|--------|
| AutoBooker | Can be given rules based on TV and title expectations |
| Contract Module | Wrestler demands for spotlight become gameplay constraints |
| Tour Visualizer | Integrates with show blocks to forecast pressure points |
| Booker Memory Engine | Learns your natural pacing, adjusts what it flags over time |

---

## RELATED SYSTEMS

- [[Calendar_UI_System]] - Where reminders appear
- [[Tour_Load_Balance_System]] - Macro-level pacing
- [[Contract_System]] - Obligation source
- [[Title_Lineage_System]] - Defence tracking

---

**Document Status:** Locked
**Version:** 1.0 (Vol 3)
**Next Review:** Network pressure escalation mechanics
