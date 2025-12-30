# MATCH DNA SYSTEM

📛 **NAME:** Match DNA System  
🧭 **CATEGORY:** Match Simulation, Worker Classification  
🔑 **KEYWORDS:** match dna, style clash, fighting spirit, king's road, lucha, sports entertainment, shoot style, match pacing  
📝 **SUMMARY:** Workers carry "Match DNA" that determines their natural match style, affecting pacing, finish likelihood, spot choices, injury probabilities, and crowd pop curves. When workers with different DNA face each other, their narratives clash and blend.

⚙️ **LOGIC OVERVIEW:**

- Every worker has a primary Match DNA type
- DNA affects all match simulation parameters
- Style clashes create interesting narrative tension
- DNA can evolve over career (e.g., young Tanahashi → mature Tanahashi)
- Promotions have "house style" DNA that influences booking expectations

🔬 **LLM INTEGRATION:** Yes. LLM references DNA type when generating match commentary, highlight moments, and narrative descriptions.

📌 **ORIGIN:** Vol. 2 (conceptual system)

📎 **CONNECTED SYSTEMS:** [[Match Engine/_Match Engine Index|Match Engine]], [[Fighting_Spirit_Archetype]], [[Kings_Road_Archetype]], [[Worker_Skills]], [[Match_Presentation]]

❓ **OPEN QUESTIONS:**

- How exactly do DNA types blend in cross-style matches?
- Can workers have secondary DNA types?
- How does DNA interact with match stipulations?
- DNA evolution mechanics over career?
- Promotion house style enforcement vs. worker DNA?

✅ **STATUS:** 🔨 EXPLORATORY (Concept defined, mechanics need development)

---

## VERSION HISTORY

**Version 1.0 (Vol 2) [EXPLORATORY]**
- Core DNA types defined
- Comparison tables established
- Integration points identified
- Detailed mechanics TBD

---

## MATCH DNA TYPES

### Fighting Spirit DNA (NJPW Style)

| Element | Implementation |
|---------|----------------|
| **Offensive Momentum System** | Fast shift momentum engine: dominant offense rewarded |
| **Submission Threat Level** | Submissions have live threat throughout match, not just wear-down |
| **Sudden Finish System** | Finishes can happen at any time (no guaranteed multi-kickout drama) |
| **Aggression Modifier** | Bonus to strike flurries, comeback flurries |
| **Spirit Bomb Tag** | Comebacks possible but dangerous |

**In gameplay terms:** Matches feel urgent, punishing, more like a fight than choreographed escalation.

---

### King's Road DNA (AJPW/NOAH Style)

| Element | Implementation |
|---------|----------------|
| **Structured Escalation Engine** | Matches have phases: base → heat → escalation → killshot |
| **Accumulated Damage Tracking** | System measures limb/body core injury over time |
| **Injury Risk Spike** | Big head drops and insane moves massively spike injury chance |
| **Crescendo Psychology** | Crowd heat builds steadily but explodes at escalation stage |
| **Last Stand Spirit Tag** | Huge final gasp comebacks at 80-90% injury |

**In gameplay terms:** Matches feel like building a tragedy. Fans anticipate, dread, and hope.

---

### Lucha DNA (Mexican Style)

| Element | Implementation |
|---------|----------------|
| **Aerial Sequence Priority** | High-flying sequences emphasized |
| **Tecnico/Rudo Psychology** | Clear face/heel dynamics |
| **Mask Importance** | Mask-based stipulations have extreme weight |
| **Multi-Fall Structure** | 2-of-3 falls common |
| **Trios Coordination** | Tag team coordination emphasized |

**In gameplay terms:** Spectacle, tradition, honor, and acrobatic drama.

---

### Sports Entertainment DNA (American Commercial Style)

| Element | Implementation |
|---------|----------------|
| **Promo-Match Integration** | Storyline beats matter more than match quality |
| **Finish Protection** | Certain finishers are protected |
| **Interference Tolerance** | Run-ins and cheating expected |
| **TV Timing** | Matches fit commercial breaks |
| **Character Work** | Persona matters as much as workrate |

**In gameplay terms:** Wrestling as entertainment spectacle, stories over matches.

---

### Shoot DNA (UWF/Pancrase Style)

| Element | Implementation |
|---------|----------------|
| **Submission Credibility** | All submissions are live threats |
| **Strike Damage** | Strikes do real damage |
| **Minimal High Spots** | Flashy moves rare |
| **Position-Based Advantage** | Ground control matters |
| **Realistic Selling** | No miraculous recoveries |

**In gameplay terms:** Matches feel like fights, not performances.

---

## DNA COMPARISON MATRIX

| Trait | Fighting Spirit | King's Road | Lucha | Sports Ent | Shoot |
|-------|-----------------|-------------|-------|------------|-------|
| **Sudden Death Threat** | ✓ | ✗ | Medium | Low | ✓ |
| **Structured Escalation** | ✗ | ✓ | Medium | Low | ✗ |
| **Active Submissions** | ✓ | Mid-stage | Low | Low | ✓ |
| **Head Drop Tolerance** | Lower | Very High | Low | Medium | Very Low |
| **Comeback Flurry** | Short, vicious | Long, defiant | Dramatic | Scripted | Rare |
| **Average Match Length** | Medium | Long | Medium | Short-Medium | Short |
| **Crowd Psychology** | Martial energy | Tragic investment | Celebratory | Entertainment | Tension |

---

## STYLE CLASH MECHANICS

When workers with different Match DNA face each other:

### Narrative Effect
- Creates "two narratives smashing together"
- LLM commentary reflects style tension
- Match quality can suffer OR create unique drama

### Mechanical Effect (Conceptual)
- Blend parameters from both DNA types
- Primary DNA of higher-billed worker may dominate
- Promotion house style may override both
- Special "clash" moments possible when styles directly conflict

### Examples

| Matchup | Effect |
|---------|--------|
| **Fighting Spirit vs King's Road** | Tension between quick finishes and slow escalation |
| **Lucha vs Shoot** | High-flying vs grounded realism clash |
| **Sports Ent vs Fighting Spirit** | Entertainment beats vs martial intensity |

---

## WORKER DNA ASSIGNMENT

### Primary DNA
Every worker has one primary DNA type based on:
- Training background
- Home promotion
- Peak career style
- Archetype (strongly correlated)

### DNA-Archetype Correlations

| Archetype | Typical DNA |
|-----------|-------------|
| Fighting Spirit | Fighting Spirit |
| King's Road | King's Road |
| Muga Technician | King's Road or Shoot |
| Luchador/Tecnico/Rudo | Lucha |
| Showman/Entertainer | Sports Entertainment |
| Shooter | Shoot |
| Indie Darling | Varies (often hybrid) |

### DNA Evolution

Workers may shift DNA over career:
- Young Tanahashi (Muga) → Prime Tanahashi (Fighting Spirit/Golden Boy)
- Moxley (Sports Ent) → Moxley (Fighting Spirit/Deathmatch hybrid)
- Nakamura (Fighting Spirit) → WWE Nakamura (Sports Ent)

---

## IMPLEMENTATION NOTES

### Data Structure (Conceptual)

```json
{
  "worker_id": "WORKER_12345",
  "match_dna": {
    "primary": "fighting_spirit",
    "secondary": null,
    "evolution_history": [
      {"era": "young_lion", "dna": "king's_road"},
      {"era": "prime", "dna": "fighting_spirit"}
    ]
  },
  "dna_modifiers": {
    "submission_threat": 0.8,
    "sudden_finish": 0.7,
    "escalation_tolerance": 0.4
  }
}
```

### Integration Points

- **Match Engine:** DNA affects all simulation parameters
- **Match Presentation:** DNA affects highlight generation and recap style
- **Booking System:** DNA compatibility warnings for mismatched styles
- **Commentary:** DNA-specific language and references

---

## RELATED SYSTEMS

- [[Match Engine/_Match Engine Index|Match Engine]]: Core simulation uses DNA
- [[Fighting_Spirit_Archetype]]: Fighting Spirit DNA details
- [[Kings_Road_Archetype]]: King's Road DNA details
- [[Match_Presentation]]: DNA affects output style
- [[Worker_Skills]]: Skills interact with DNA expression

---

**Document Status:** 🔨 Exploratory (Vol 2 concept, needs full mechanics)  
**Last Updated:** 2025-12-25  
**Next Review:** Define exact parameter values; style clash resolution mechanics
