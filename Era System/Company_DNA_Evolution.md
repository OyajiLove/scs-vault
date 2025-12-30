# COMPANY DNA EVOLUTION SYSTEM

📛 **NAME:** Company DNA Evolution System  
🧭 **CATEGORY:** Federation Management / Identity  
🔑 **KEYWORDS:** DNA, tone, style drift, product identity, creative evolution, promotion personality  
📝 **SUMMARY:**

The deep layer underneath Federation Identity. Tracks how your promotion's product *feels*, presents, and evolves over time, even if you didn't consciously direct it. Your booking choices accumulate into an emergent identity that affects every system in the game.

⚙️ **LOGIC OVERVIEW:**

- DNA consists of 7 core layers defining your product style
- DNA shifts passively based on booking choices, events, and external pressure
- Misalignment between DNA and audience expectations causes systemic problems
- Every 6 months in-game, receive a creative trajectory report
- You don't pick your DNA. You *become* it.

🔬 **LLM INTEGRATION:** High (narrative feedback, trajectory analysis, era naming)

📌 **ORIGIN:** Vol 3 lines 293-310

📎 **CONNECTED SYSTEMS:**
- [[Era Markers & Legacy Milestones]] - Names your creative periods
- [[Major Event Inflection System]] - Sudden DNA resets
- [[Sponsor Alignment System]] - Sponsors react to DNA
- [[Worker Foundation/Hidden Personality Traits]] - Workers may clash with fed DNA
- [[Crowd Memory]] - Fans remember and react to DNA drift

❓ **OPEN QUESTIONS:**
- Exact thresholds for DNA shift triggers
- How quickly can DNA change intentionally?
- Can you deliberately steer DNA or only react?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 293-310 | 🔒 LOCKED |

---

## CORE DNA LAYERS

Your promotion's product style exists on 7 spectrums:

| Layer | Spectrum |
|-------|----------|
| **Tone** | Wholesome ←→ Edgy ←→ Nihilistic |
| **Structure** | Classic Escalation ←→ Hybrid Chaos |
| **Booking Focus** | Workrate ←→ Character ←→ Pop Culture |
| **Pacing** | Deliberate ←→ Breathless ←→ Incoherent |
| **Reality Level** | Sportslike ←→ Cinematic ←→ Surreal |
| **Emotional Rhythm** | Earnest ←→ Spiteful ←→ Hopeless |
| **Push Logic** | Meritocratic ←→ Heat Machine ←→ Clique Warfare |

---

## DNA SHIFT TRIGGERS

| Trigger | Effect |
|---------|--------|
| Long-running push of specific style/champion | Gradual tonal change (e.g., deathmatch champ = violence normalization) |
| Sponsor mandates | Edge pulled off, diversity spotlighted, tone adjusted |
| TV network demands | More stories per hour, less technical wrestling |
| Unionization | Focus on safety = fewer risky spots, more emotion-driven booking |
| Cultural moments | #MeToo → no more creepy angles; global crises → hope arcs emerge |
| Fan revolt | "This is too slick" → shift to rawer presentation |
| Scandals or tragedies | Change tone permanently (e.g., Benoit, Hana Kimura, Owen Hart) |
| New booker or top agent takes power | Massive tone recalibration |

---

## REAL WORLD EXAMPLES OF DNA DRIFT

| Federation | DNA Evolution |
|------------|---------------|
| 1980s AJPW | → King's Road → Death and Honor |
| 2000s WWE | → Ruthless Aggression → Edgy Popcorn Violence |
| AEW 2021 | → Hybrid Escalation → Emotional Workrate |
| AAA 2023 | → TV Chaos → Meme Deathmatch Comedy |

---

## DNA FEEDBACK SYSTEM

Every 6 months in-game, you receive a **creative trajectory report**:

**Example Reports:**
- "Your product is trending toward breathless pacing and chaotic emotion. Fans are starting to fatigue."
- "You've accidentally created a hope-core promotion. Sponsors love it. Edgy fans are tuning out."
- "You've normalized cruelty. And the locker room has noticed."

---

## DNA VS AUDIENCE EXPECTATION

When your DNA and audience expectation drift apart:

| Result | Effect |
|--------|--------|
| **Fans feel betrayed** | Heat dies. Even good matches feel cold. |
| **Sponsors get confused** | Pressure to "find your voice again" |
| **Workers misaligned** | Morale drops: "This isn't what I signed up for" |
| **Agents suggest change** | May offer pushback: "This ain't the fed we built." |

---

## IMPLEMENTATION NOTES

### DNA Profile Structure

```json
{
  "fed_id": "promotion_001",
  "dna_profile": {
    "tone": 0.7,           // 0=Wholesome, 0.5=Edgy, 1=Nihilistic
    "structure": 0.3,      // 0=Classic, 0.5=Hybrid, 1=Chaos
    "booking_focus": 0.5,  // 0=Workrate, 0.5=Character, 1=Pop Culture
    "pacing": 0.4,         // 0=Deliberate, 0.5=Breathless, 1=Incoherent
    "reality_level": 0.6,  // 0=Sportslike, 0.5=Cinematic, 1=Surreal
    "emotional_rhythm": 0.3, // 0=Earnest, 0.5=Spiteful, 1=Hopeless
    "push_logic": 0.2      // 0=Meritocratic, 0.5=Heat Machine, 1=Clique Warfare
  },
  "drift_velocity": {
    "tone": +0.02,         // Currently trending more edgy
    "pacing": -0.01        // Slowing down slightly
  },
  "last_trajectory_report": "2027-06-01"
}
```

---

## RELATED SYSTEMS

- **[[Era Markers & Legacy Milestones]]:** DNA drift creates new era markers
- **[[Major Event Inflection System]]:** Sudden events can hard-reset DNA
- **[[Sponsor Alignment System]]:** Sponsors evaluate DNA fit
- **[[Booker Memory Engine]]:** Your patterns shape DNA over time

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Integration with Sponsor system
