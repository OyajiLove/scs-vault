# Training Philosophy Types

📛 **MECHANIC:** Training Philosophy and Developmental Approach
🔗 **PARENT SYSTEM:** [[_Training System Index|Training System]]
🧭 **CATEGORY:** Worker Development
🔑 **KEYWORDS:** dojo, traditional, corporate, hybrid, training philosophy, development pipeline
📌 **ORIGIN:** Vol 4, Ringstate Atlas (promotion training descriptions)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4, Ringstate Atlas | 🔒 LOCKED |

---

## Overview

Training philosophy determines not just HOW workers are developed, but WHAT kind of workers they become. Traditional dojo systems produce technically sound, mentally tough workers who may struggle in entertainment-focused environments. Corporate pipelines create charismatic performers who may lack credibility in shoot-style contexts. The philosophy shapes the worker's entire career trajectory.

---

## Philosophy Types

### Traditional Dojo System

**Examples:** NJPW, AJPW, Miss Mitsuko's NSP women's division, FRF

**Characteristics:**
- 5 AM starts, grueling conditioning before technique
- No complaints tolerated, no days off for minor injuries
- Public humiliation for mistakes (running stairs while veterans watch)
- Hierarchical structure: young lions serve veterans
- Multi-year commitment before debut (2-4 years typical)
- Emphasis on fundamentals, psychology, selling

**Worker Outcomes:**
- High Durability, Stamina, Composure
- Strong Psychology and Selling foundation
- High Resilience (Hidden Personality)
- Potentially lower Entertainment stats (varies)
- Tags: "Dojo Product", "Trained to Suffer", "Fundamental Foundation"

**Philosophy Quote:** "Suffering builds legitimacy. Idol culture demands we package it sweetly." (Miss Mitsuko)

---

### Corporate Development Pipeline

**Examples:** GWA main, SWA men's division, 1990s WWF

**Characteristics:**
- 6-8 hour training days with proper rest
- Sports medicine approach, injury prevention priority
- Emphasis on looks, charisma, athleticism alongside ability
- Faster path to debut (6-18 months typical)
- Character development prioritized early
- Colorful gear, entrance training, promo coaching

**Worker Outcomes:**
- High Entertainment stats (Mic Skills, Character Work, Entrance)
- Good Speed, Agility (athletic emphasis)
- Potentially lower Psychology, Selling (unless specifically trained)
- Lower Resilience, higher expectations of comfort
- Tags: "Corporate Creation", "Pipeline Product", "Charisma-First"

**Criticism:** Traditional promotions see graduates as "sellouts" who chose corporate backing over dojo torture.

---

### Hybrid Approach

**Examples:** SWA (overall), modern NJPW, some UK promotions

**Characteristics:**
- Rigorous by Western standards, lighter than traditional Japanese
- Balance of fundamental training and entertainment development
- Mentorship without full young lion servitude
- Flexible timeline based on readiness
- Cross-training in multiple styles

**Worker Outcomes:**
- Balanced stat development
- Good adaptability (can work multiple styles)
- May lack extreme specialization
- Tags: "Well-Rounded", "Style Versatile"

---

### Shootstyle/Combat Focus

**Examples:** FRF, UWF lineage, some PWU promotions

**Characteristics:**
- Martial arts foundation required before wrestling training
- Emphasis on legitimate fighting ability
- Minimal entertainment training
- Short path to competition if combat credentials exist
- Constant sparring, conditioning matches

**Worker Outcomes:**
- Very high Technical, Striking, Submission
- High Composure (pressure tested)
- Often lower Entertainment stats
- High credibility, lower mainstream appeal
- Tags: "Shooter", "Combat Credentialed", "Legitimate"

**Philosophy Quote:** "Wrestling should hurt. Or it's just theatre." (Shiro Kenzaki, FRF)

---

### Backyard/Underground Path

**Examples:** Blade Underground, indie circuits, ECW originals

**Characteristics:**
- Self-taught or informal training
- Learning by doing (often painfully)
- No formal structure or timeline
- Sink-or-swim mentality
- May receive later formal training to fill gaps

**Worker Outcomes:**
- Highly variable: could be brilliant or dangerous
- Often high Risk-Taking (Hidden Personality)
- Strong performer instincts (survived without structure)
- Technical gaps common
- Tags: "Self-Trained", "Backyard Origins", "Crash Course Graduate"

---

## Philosophy Compatibility

| Home Philosophy | Adapts Well To | Struggles With |
|-----------------|----------------|----------------|
| Traditional Dojo | Any wrestling environment | Pure entertainment shows |
| Corporate | Entertainment-focused | Shootstyle, traditional credibility tests |
| Hybrid | Most environments | Extreme specialists may outshine |
| Shootstyle | MMA, shootstyle, strong style | Comedy, sports entertainment |
| Underground | Hardcore, indie, guerrilla | Corporate structure, traditional hierarchy |

---

## Training Philosophy by Alliance

| Alliance | Dominant Philosophy | Notes |
|----------|---------------------|-------|
| **CCA** | Traditional | Territory system roots, respect for craft |
| **GWA** | Corporate | Entertainment-first, global standardization |
| **PWU** | Hybrid/Shootstyle | Legitimacy emphasis, worker-controlled |
| **CFPW** | Traditional (Indigenous) | Ceremonial elements, community-based |
| **LGBTQW+** | Hybrid | Inclusive, varied backgrounds |
| **Blade** | Underground | Survival-based, self-taught |

---

## System Effects

### On Worker Generation
- Philosophy determines starting stat distribution
- Influences which tags are possible at debut
- Sets Hidden Personality trait ranges (e.g., dojo = high Resilience)

### On Career Development
- Philosophy compatibility affects adaptation when changing promotions
- Mismatch creates adjustment period, potential morale issues
- Some workers never adapt (philosophy-locked)

### On Crowd Perception
- Traditional background = credibility in serious contexts
- Corporate background = acceptance in entertainment contexts
- Philosophy known to smart fans, affects perception

---

## Connected Mechanics

- [[Skill Growth Mechanics]] - Philosophy affects growth rates
- [[Mentor System]] - Philosophy affects mentorship style
- [[_Training System Index]] - Parent system

---

## Implementation Notes

```json
{
  "training_philosophy": {
    "type": "traditional_dojo",
    "promotion": "NJPW",
    "years_in_training": 3,
    "stat_modifiers": {
      "durability": 1.2,
      "stamina": 1.15,
      "composure": 1.1,
      "mic_skills": 0.9
    },
    "personality_modifiers": {
      "resilience": "+3",
      "traditionalism": "+2",
      "ego": "-1"
    },
    "possible_starting_tags": [
      "Dojo Product",
      "Young Lion",
      "Fundamental Foundation"
    ]
  }
}
```

---

**Document Status:** Locked
**Last Updated:** 2025-12-21
