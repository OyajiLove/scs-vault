# HYBRID WORKER SYSTEM

📛 **NAME:** Hybrid Worker System  
🧭 **CATEGORY:** Worker Classification, Career Mechanics  
🔑 **KEYWORDS:** hybrid, multi-archetype, career phase, evolution, crossover, archetype blending  
📝 **SUMMARY:** System for workers who don't lock into one archetype cleanly. The greatest or most interesting workers blur lines between archetypes and subtypes. This system allows primary archetype + secondary traits/tags, career phase transitions between archetypes, and multi-archetype compatibility for complex worker profiles.

⚙️ **LOGIC OVERVIEW:**

- Workers can have Primary Archetype and Secondary Traits/Tags
- Career phases can shift archetype alignment
- Hybrid Warriors operate across two archetypes without penalty
- Phase transitions model real career evolution
- Tags track hybrid capability and crossover potential

🔬 **LLM INTEGRATION:** Yes. LLM generates career arc narratives, archetype transition moments, hybrid identity descriptions.

📌 **ORIGIN:** Vol. 2 (developed from Benoit/Dynamite/Oba Femi classification discussion)

📎 **CONNECTED SYSTEMS:** [[Worker_Skills]], [[Tags_System]], [[Archetypes/_Archetypes_Index|All Archetypes]], [[Career System/_Career System Index|Career System]]

❓ **OPEN QUESTIONS:**

- Maximum number of secondary archetypes?
- Hybrid penalty thresholds for incompatible archetype combinations?
- Career phase transition triggers (age-based? event-based? booking-based?)

✅ **STATUS:** Exploratory (Vol 2)

---

## CORE CONCEPT

Wrestling isn't clean-cut. Many workers blend multiple archetype identities:
- **Early career:** Junior Puroresu style
- **Prime:** Transitions to Fighting Spirit or King's Road heavyweight
- **Late career:** Territory Lifer or Senior Circuit Hero

The Hybrid Worker System models this reality.

---

## WORKER ARCHETYPE STRUCTURE

### Standard Worker

```
Primary Archetype: [One archetype]
Subtype: [One subtype within that archetype]
Tags: [Various tags]
```

### Hybrid Worker

```
Primary Archetype: [Dominant archetype]
Secondary Archetype: [Blended archetype, partial influence]
Subtype: [From primary, or hybrid subtype]
Tags: [Includes Hybrid Warrior or similar crossover tags]
```

---

## HYBRID CLASSIFICATION EXAMPLES

### Dynamite Kid

| Career Phase | Primary Archetype | Secondary | Subtype |
|--------------|-------------------|-----------|---------|
| Young (1980s) | Junior Puroresu | Brawler | Tiger Style Junior / Lucharesu Hybrid |
| Prime (mid-80s) | Fighting Spirit | Junior Puroresu | Shooter Spirit |

**Notes:** Started as explosive junior but psychology was heavier than pure junior work. Transitioned to Fighting Spirit with strong-style violence as career progressed.

### Chris Benoit

| Career Phase | Primary Archetype | Secondary | Subtype |
|--------------|-------------------|-----------|---------|
| Young (Japan) | Junior Puroresu | Brawler | Junior Bruiser (violent, not flashy) |
| Prime (WWF/WCW) | Fighting Spirit | King's Road | Crashing Avalanche or Shooter Spirit |

**Notes:** Junior Puroresu body type but heavyweight psychology and violence. Heavy King's Road and NJPW influence. The UWFi stiffness adds Shooter Spirit flavor.

### Oba Femi

| Career Phase | Primary Archetype | Secondary | Subtype |
|--------------|-------------------|-----------|---------|
| Current | Powerhouse | Monster | Freak Athlete |
| Potential | Showman (hybrid) | Powerhouse | Athletic Entertainer with Freak Athlete upside |

**Notes:** Scary hybrid who's freakishly quick AND freakishly strong. Monster aura but athletic entertainer presentation in NXT context.

### Mick Foley / Cactus Jack

| Career Phase | Primary Archetype | Secondary | Subtype |
|--------------|-------------------|-----------|---------|
| Early | Brawler | Hardcore | Psychotic Brawler |
| Peak | Brawler | Showman | Hardcore Brawler + Emotional Performer blend |
| Late | Showman | Brawler | Emotional Performer (Mankind pathos era) |

**Notes:** Hardcore brawler core but Emotional Performer aspects made him transcendent. Career arc shows archetype weight shifting over time.

---

## CAREER PHASE TRANSITIONS

### Transition Triggers

| Trigger | Description |
|---------|-------------|
| **Age-Based** | Natural progression (junior → heavyweight, prime → veteran) |
| **Injury-Based** | Forced style change due to physical limitations |
| **Booking-Based** | Promotion pushes worker into new role |
| **Event-Based** | Major storyline moment (betrayal, title win, faction change) |
| **Weight Change** | Junior heavyweight → heavyweight division move |

### Common Transition Paths

| From | To | Example |
|------|----|---------| 
| Junior Puroresu | Fighting Spirit | Benoit, Dynamite, KENTA |
| Junior Puroresu | King's Road | Marufuji heavyweight era |
| Fighting Spirit | Territory Lifer | Aging NJPW veterans |
| King's Road | Senior Circuit Hero | Rusher Kimura, late-career legends |
| Showman | Brawler | Jeff Hardy late career shift |
| Monster | Showman | Kane comedy era, Big Show transitions |
| Powerhouse | Showman | Batista Hollywood transition |

---

## HYBRID TAGS

| Tag | Meaning |
|-----|---------|
| **Hybrid Warrior** | Can operate across two archetypes without major penalty |
| **Phase Shifter** | Transitions between archetype phases smoothly over career |
| **Style Chameleon** | Adapts match style to opponent's archetype effectively |
| **Crossover Specialist** | Excels in cross-promotion/cross-style matches |
| **Explosive Technician** | Bonus for dynamic, high-impact technical sequences (Junior→Fighting Spirit types) |

---

## ARCHETYPE COMPATIBILITY MATRIX

### High Compatibility (Natural Blends)

| Archetype A | Archetype B | Notes |
|-------------|-------------|-------|
| Junior Puroresu | Fighting Spirit | Common career progression |
| Fighting Spirit | King's Road | Puroresu ecosystem crossover |
| Brawler | Hardcore | Violence spectrum |
| Showman | Heel Ace | Entertainment heel territory |
| Monster | Powerhouse | Size-based intimidation |
| Dark Weaver | Showman | Broken Entertainer crossover |

### Low Compatibility (Tension/Penalty)

| Archetype A | Archetype B | Notes |
|-------------|-------------|-------|
| Technician | Hardcore | Opposite philosophies |
| Showman | Muga | Entertainment vs purity |
| Monster | Good Hand | Conflicting roles |
| Luchador | King's Road | Speed vs endurance |

---

## IMPLEMENTATION NOTES

### Data Structure (Conceptual)

```json
{
  "worker_id": "benoit_chris",
  "career_phases": [
    {
      "phase": "early",
      "years": "1985-1990",
      "primary_archetype": "junior_puroresu",
      "secondary_archetype": "brawler",
      "subtype": "junior_bruiser"
    },
    {
      "phase": "prime",
      "years": "1994-2004",
      "primary_archetype": "fighting_spirit",
      "secondary_archetype": "kings_road",
      "subtype": "crashing_avalanche"
    }
  ],
  "hybrid_tags": ["hybrid_warrior", "explosive_technician"]
}
```

### Career Arc Generation

For simulated workers, the system could:
1. Assign initial archetype based on training background
2. Track career events that might trigger transitions
3. Calculate hybrid compatibility for natural evolution
4. Generate narrative moments for archetype shifts

---

## FLAVOR TEXT

"The road of a wrestler is not a straight line. The burning junior becomes the grizzled heavyweight. The monster learns to make them laugh. The showman discovers violence. Every great career is a story of transformation: and the system must track every chapter."

---

## RELATED SYSTEMS

- [[Archetypes/_Archetypes_Index|All Archetypes]]: Source of primary/secondary assignments
- [[Tags_System]]: Hybrid tags implementation
- [[Career System/_Career System Index|Career System]]: Phase transition integration
- [[Worker_Skills]]: Skill evolution across phases

---

**Document Status:** Exploratory (Vol 2 Chunk 02 extraction)  
**Last Updated:** 2025-12-25  
**Next Review:** Compatibility matrix refinement, transition trigger formulas
