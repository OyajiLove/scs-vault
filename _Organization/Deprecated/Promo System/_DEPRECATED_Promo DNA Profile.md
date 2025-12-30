# Promo DNA Profile System

📛 **MECHANIC:** Promo DNA Profile
🔗 **PARENT SYSTEM:** Promo System
🧭 **CATEGORY:** Worker Character / AI Generation
🔑 **KEYWORDS:** promo, character voice, tone, cadence, vocabulary, themes, LLM, AI generation
📌 **ORIGIN:** Vol 1 Extraction #211, #245
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Every worker needs a **Promo DNA Profile**: a structured template that captures their unique speaking style, themes, vocabulary, and emotional patterns. This enables consistent AI-generated promos that sound authentically like the character.

---

## Core Components

### Profile Structure (~5-7KB per worker)

| Component | Description | Example (Stone Cold) |
|-----------|-------------|----------------------|
| **Tone** | Emotional register | Aggressive, defiant, blue-collar rage |
| **Cadence** | Speech rhythm | Staccato bursts, dramatic pauses |
| **Vocabulary** | Word choice patterns | "What?", "son of a bitch", "bottom line" |
| **Themes** | Recurring subjects | Anti-authority, working man, self-reliance |
| **Catchphrases** | Signature lines | "And that's the bottom line...", "Austin 3:16" |
| **Targets** | Who they attack | Authority figures, corporate types, hypocrites |
| **Heat Generators** | What gets crowd going | Stunners, beer, middle fingers |
| **Weaknesses** | Promo blind spots | Sometimes rambles when not focused |

---

## Sample Profiles

### Stone Cold Steve Austin (Locked Reference)

```json
{
  "worker_id": "austin_1998",
  "promo_dna": {
    "tone": ["aggressive", "defiant", "blue_collar", "anti_authority"],
    "cadence": {
      "style": "staccato",
      "pause_frequency": "frequent",
      "intensity_curve": "builds_to_explosion"
    },
    "vocabulary": {
      "signature_words": ["bottom line", "what", "son of a bitch", "whoop your ass"],
      "avoid_words": ["please", "sorry", "respectfully"],
      "profanity_level": "high"
    },
    "themes": [
      "anti_authority",
      "self_made_man",
      "trust_no_one",
      "fighting_the_system"
    ],
    "catchphrases": [
      "And that's the bottom line, cause Stone Cold said so.",
      "Austin 3:16 says I just whipped your ass.",
      "What?",
      "Oh hell yeah!"
    ],
    "targets": {
      "preferred": ["authority_figures", "corporate_types", "hypocrites"],
      "avoid": ["sympathetic_faces", "kids"]
    },
    "heat_generators": ["stunner", "beer_bash", "middle_finger", "truck_destruction"],
    "promo_length_preference": "medium",
    "crowd_interaction": "high"
  }
}
```

### Eric Embry Promo Example (#245)

Vol 1 includes a full Eric Embry promo generation example demonstrating how the DNA Profile creates authentic territory-era heel promos:

**DNA Elements Used:**
- Southern heel vocabulary
- Arrogant condescension
- Territory-specific references
- Heat-seeking insults
- Building to call-to-action

---

## LLM Integration

### Generation Prompts

When generating promos, the LLM receives:

1. Worker's Promo DNA Profile
2. Current storyline context
3. Target opponent's profile
4. Crowd type (smart, casual, regional)
5. Segment length/placement
6. Era restrictions (what language/references fit)

### Quality Controls

| Control | Purpose |
|---------|---------|
| **Era Filter** | Prevents anachronistic references |
| **Character Consistency** | Maintains voice across promos |
| **Escalation Logic** | Promo intensity matches feud heat |
| **Catchphrase Frequency** | Prevents overuse or underuse |
| **Crowd Response Modeling** | Adjusts to expected reactions |

---

## Profile Complexity Tiers

| Tier | Profile Size | Worker Type |
|------|--------------|-------------|
| **Full** | 5-7KB | Main eventers, promo-heavy workers |
| **Standard** | 2-3KB | Midcarders with speaking roles |
| **Basic** | 0.5-1KB | Occasional speakers, managers handle promos |
| **Silent** | Minimal | No promo capability, all action |

---

## Connected Mechanics

- [[Booking_Engine_P1-3]] - Segment/Promo Engine
- [[Gimmick System/_Gimmick System Index|Gimmick System]] - Character identity
- [[Tags_System]] - Promo-related tags
- [[Crowd_Memory]] - Catchphrase memory, callback potential

---

## Open Questions

- Exact token budget for profile storage?
- How do profiles evolve with character changes?
- Manager promo profiles for workers they speak for?
- Cross-language promo generation (Japanese, Spanish)?

---

**Document Status:** Concept Locked, Implementation TBD
**Last Updated:** 2024-12-23
