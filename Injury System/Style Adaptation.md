# Style Adaptation

📛 **MECHANIC:** Style Adaptation and Late Career Shift
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** style shift, late career, survival, adaptation, aging, refusal consequences
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Style isn't just about what looks cool: it's about survival. Once body wear crosses threshold, smart workers adapt (shifting to matwork, emotional selling, charisma-first styles). Prideful workers who don't adjust fall faster, get injured worse, and lose fan patience.

---

## Style Shifting Triggers

Workers may need to adapt when:

| Trigger | Description |
|---------|-------------|
| **Wear Threshold Crossed** | Body part wear counters exceed 70%+ |
| **Major Injury Recovery** | Post-surgery, can't do old moves safely |
| **Age-Related Decline** | Athleticism drops, speed decreases |
| **Chronic Condition** | Ongoing issue requires permanent adjustment |
| **Doctor Recommendation** | Medical advice to change approach |

---

## Adaptation Options

| Original Style | Adaptation Path | Examples |
|----------------|-----------------|----------|
| **High-Flyer** | Technical base, psychology-first, charisma | Tanahashi (knees), Rey Mysterio |
| **Strong Style** | Matwork, emotional selling, slower pace | Nagata, KENTA (post-injury) |
| **Power/Hoss** | Brawling, strategic striking, manager work | Vader (late career), Kane |
| **Deathmatch** | Hardcore psychology, slower violence, manager | Foley (shift to character work) |
| **Technical** | Pure psychology, mentorship, charisma | Bret Hart (later years) |

---

## Adaptation Factors

What determines successful adaptation:

| Factor | Effect |
|--------|--------|
| **High Intelligence** | Better at learning new approaches |
| **High Drive** | Willing to put in work to change |
| **Low Ego** | Accepts need to change, doesn't fight it |
| **High Adaptability Tag** | Natural chameleon ability |
| **Strong Psychology** | Can make slower work compelling |
| **Charisma/Entertainment** | Can compensate with presence |

### Adaptation Success Probability
```
Adaptation Success = (Intelligence + Drive + Psychology) - Ego

If Success Score > 40: Smooth transition
If Success Score 25-40: Rough transition, temporary dip
If Success Score < 25: Failed adaptation, continued decline
```

---

## Refusal to Adapt

### Why Workers Refuse
| Reason | Description |
|--------|-------------|
| **High Ego** | "I don't need to change" |
| **Identity Crisis** | Style is who they are, can't imagine change |
| **Fear of Irrelevance** | Worry new style won't get over |
| **Denial** | Refuse to accept physical decline |
| **Short-Term Thinking** | Prioritize now over longevity |

### Consequences of Refusal
| Consequence | Description |
|-------------|-------------|
| **Accelerated Injury** | Continue doing moves body can't handle |
| **Worse Injury Severity** | When injuries happen, they're more severe |
| **Fan Patience Loss** | Audience sees someone past their prime struggling |
| **Tragic Legacy Arc** | Remembered for sad decline rather than graceful exit |
| **Earlier Retirement** | Forced out rather than choosing to adapt |

---

## Late Career Archetypes

| Archetype | Description | Examples |
|-----------|-------------|----------|
| **Ageless Warrior** | Adapted wisely, seems to defy time | Minoru Suzuki, Tanahashi (current) |
| **Graceful Transition** | Moved to psychology/charisma before breakdown | Ric Flair (80s-90s), Regal |
| **Broken Body Walking** | Didn't adapt, became shell of themselves | Dynamite Kid, Ultimate Warrior |
| **Last Match Legend** | Retired at right time, preserved legacy | Shawn Michaels (first retirement) |
| **Can't Let Go** | Keeps wrestling past when they should stop | Terry Funk (endless retirements) |

---

## Adaptation Timeline

| Career Phase | Recommended Action |
|--------------|--------------------|
| **Early 30s** | Begin assessing wear, consider minor adjustments |
| **Mid 30s** | Active style evaluation, protect damaged areas |
| **Late 30s** | Major adaptation likely needed for most styles |
| **40s** | Survival mode: charisma/psychology primary |
| **50s** | Limited schedule, special attraction status |

---

## Fan Response to Adaptation

| Adaptation Quality | Fan Response |
|-------------------|--------------|
| **Seamless** | Fans don't notice, respect maintained |
| **Visible but Effective** | Fans appreciate wisdom, may increase respect |
| **Rough Transition** | Temporary rejection, can recover |
| **Failed Adaptation** | Fans lose patience, "time to retire" sentiment |
| **Refusal Visible** | Pity, frustration, legacy erosion |

---

## Special Cases

### Comeback After Major Injury
Workers returning from career-threatening injuries often need forced adaptation:
- Edge (neck): Returned with modified moveset, more psychology
- Undertaker (hips): Transitioned to limited schedule, spectacle matches
- Christian (concussions): Brief return, careful style

### Era-Forced Adaptation
Some workers must adapt due to era changes, not just body damage:
- Technical specialists in entertainment-first era
- Hardcore specialists post-PG era
- High-flyers as aerial moves become common

---

## Connected Mechanics

- [[Wear and Tear System]] - Triggers need for adaptation
- [[Injury Types]] - Specific injuries require specific adaptations
- [[Hidden Personality]] - Ego, Drive affect adaptation willingness
- [[Worker Skills]] - Psychology, Charisma enable successful transitions
- [[Crowd Memory]] - Fans remember workers who aged gracefully vs. tragically

---

## Open Questions

- [ ] Exact wear threshold values triggering adaptation recommendation
- [ ] How system suggests adaptation to player (hints vs. explicit)
- [ ] Training mechanics for learning new styles mid-career
- [ ] Fan memory impact of successful vs. failed adaptations

---

## Implementation Notes

```json
{
  "style_adaptation": {
    "worker_id": "worker_001",
    "original_style": "high_flyer",
    "current_style": "psychology_first",
    "adaptation_status": "complete",
    "trigger": "knee_deterioration",
    "adaptation_date": "1988-06-15",
    "transition_quality": "seamless",
    "protected_areas": ["knees", "lower_back"],
    "abandoned_moves": ["moonsault", "shooting_star_press", "top_rope_dives"],
    "new_strengths": ["emotional_selling", "technical_base", "storytelling"],
    "fan_response": "increased_respect"
  }
}
```
