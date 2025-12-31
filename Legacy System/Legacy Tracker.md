# Legacy Tracker

📛 **SYSTEM:** Legacy Tracker
🔗 **PARENT:** [[_Legacy System Index|Legacy System]]
🧭 **CATEGORY:** Career & Long-Term Simulation
🔑 **KEYWORDS:** legacy score, career imprint, hall of fame, retirement, legend
📌 **ORIGIN:** Vol 6
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 6 | 🔒 LOCKED |

---

## Overview

The Legacy Tracker simulates a worker's career imprint as perceived by fans, bookers, media, and peers, blending fact, memory, and emotion.

This determines:
- Hall of Fame induction
- Retirement pop
- Last-run respect
- Posthumous legend status
- Documentary praise or burial

---

## Legacy Score: 1-100 (Non-linear Scale)

- Visible only in HOF or legacy-related screens
- Driven by Fan Memory Snapshots, Title Reigns, Buzz Peaks, Feuds, and Match Quality
- Modified by Time, Scandal, Death, and Promotion Politics

| Score Range | Label | Meaning |
|-------------|-------|---------|
| 90-100 | **Immortal** | Legendary across generations, referenced constantly |
| 75-89 | **Iconic** | National hero, genre-defining reigns, or myth-making feuds |
| 50-74 | **Respected Veteran** | Career longevity, key matches, remembered regionally |
| 30-49 | **Cult Figure** | Underground following, specific match or scandal fans won't forget |
| 10-29 | **Forgotten Workhorse** | Good hand, few moments that stuck |
| 0-9 | **Erased / Disgraced** | Scandals, vanishing, or complete cultural loss |

---

## Legacy Builders

| Source | Influence |
|--------|-----------|
| 📸 **Fan Memory Snapshots** | Strongest driver; 1 memory alone can lift a legacy |
| 🏆 **Title Prestige + Length** | Great runs elevate; cold or hot potato reigns do little |
| 🎭 **Emotional Arcs** | Redemption, tragedy, betrayal, perseverance all boost legacy |
| 🔥 **Buzz Peaks (Repeated)** | Sustained moments across years = deeper legacy |
| ⏳ **Career Length** | Longevity matters, with quality moments to anchor it |
| 🏟 **Big Match Setting** | Dome shows, Mania, Budokan, Arena Mexico etc. amplify imprint |
| 📺 **Commentary Reinforcement** | Bookers and announcers can preserve or bury legacies via language over time |

---

## Legacy Modifiers (Positive + Negative)

| Event | Legacy Impact |
|-------|---------------|
| 🎤 **Final Farewell Promo** | +Legacy (especially if emotionally earned) |
| 💀 **Death (if respected)** | +10 to +15 Legacy spike, often permanent |
| 🚫 **Death (if disgraced)** | May freeze legacy or split fanbase |
| 🧨 **Scandal** (DUI, abuse, public meltdowns) | -10 to -40 depending on severity + timing |
| 🛑 **Career Ending Injury** | Can elevate legacy if timing is poetic |
| 🧠 **Reinvention Arc** | "Rebuilt from the ashes" legacies = strong boost |
| 🐍 **Political Manipulator Tag** | Slows legacy growth, especially post-career |

---

## Uses of Legacy Score in Simulation

| System | Role |
|--------|------|
| 🏅 **Hall of Fame Voting** | Minimum Legacy threshold + story arcs required |
| 🎤 **AI Promos** | "A legend in this business..." lines tied to score |
| 💼 **AI Booker Logic** | May keep cold legends around for mentorship or HOF setup |
| 😊 **Worker Morale** | High legacy = morale boost in retirement, or resentment if overlooked |
| 🗞 **Media / Fan Chatter** | Year-end lists, online revisionism, feuds over legacy |
| ⚰️ **Death Tributes** | The higher the Legacy, the louder the eulogy |
| 🧬 **Generational Feuds** | Younger stars cutting promos to surpass a 93-Legacy figure ("Your time is over.") |

---

## System Integration Recap

| Source System | Contribution to Legacy |
|---------------|------------------------|
| [[Buzz System/_Buzz System Index\|Buzz System]] | Short-term peaks, crowd memory |
| [[Fan Memory Engine/_Fan Memory Index\|Fan Memory Engine]] | Snapshot permanence, distortion over time |
| [[Emotional_Show_Flow\|Show Flow + Emotional Tags]] | Emotional weight of arcs |
| [[Title Logic]] | Prestige of reigns, big-match resonance |
| [[Booking Trails System/_Booking_Trails_Index\|Booking Trails]] | Long-term narrative arcs, especially tragedy/redemption |
| [[Hidden_Personality]] | Drive and Morality can influence who seeks legacy or sabotages it |

---

## Open Questions

- Exact formula for Legacy Score calculation
- How often Legacy recalculates (per show? per month? per year?)
- Regional vs Global Legacy tracking
- Tag team shared Legacy mechanics

---

## Implementation Notes

```json
{
  "legacy_tracker": {
    "worker_id": "w_001",
    "legacy_score": 72,
    "legacy_tier": "respected_veteran",
    "builders": {
      "memory_snapshots": 3,
      "title_reigns": 2,
      "emotional_arcs": ["redemption", "perseverance"],
      "buzz_peaks": 5,
      "career_length_years": 18,
      "big_match_count": 4
    },
    "modifiers": {
      "farewell_promo": true,
      "scandal_active": false,
      "political_manipulator": false
    },
    "hof_eligible": true,
    "legend_status": "none"
  }
}
```
