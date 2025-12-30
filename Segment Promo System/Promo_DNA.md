# PROMO DNA SYSTEM

📛 **NAME:** Promo DNA System  
🧭 **CATEGORY:** Worker Identity, Content Generation, AI Integration  
🔑 **KEYWORDS:** promo, DNA, voice, character, catchphrase, pacing, vocabulary, mutation, emergence, templates  
📝 **SUMMARY:**

Promo DNA encodes a worker's unique voice and promo style as structured data that can generate infinite variations while maintaining character consistency. Unlike static bios, DNA mutates through play: anchors, career events, and influences reshape how a worker speaks over time. The system scales across hardware tiers, from template-based generation on potato machines to full AI synthesis on high-end systems.

⚙️ **LOGIC OVERVIEW:**

- Every worker has a Promo DNA profile defining their verbal identity
- DNA contains vocabulary tier, emotional range, pacing patterns, catchphrases, influences, and taboos
- Greenhorns start with generic templates; DNA develops through career events
- Anchors (major life events) trigger DNA mutations
- Working with veterans can add "influences" that shift speech patterns
- Heel/face turns unlock new emotional ranges
- System outputs promo scripts, but player can write their own or give bullet points

🔬 **LLM INTEGRATION:** Yes (tiered)
- **High tier (70B+ local or cloud):** Full generative promos from DNA + context
- **Mid tier (7B-13B local):** DNA provides heavy guardrails, model fills variables
- **Potato tier (no LLM):** Pure template system, DNA drives mad-libs style generation

📌 **ORIGIN:** Conversation thread (December 2024), synthesizing Vol 2-3 promo concepts with AI integration planning

📎 **CONNECTED SYSTEMS:** [[Angle_DNA]], [[Hidden_Personality]], [[Tags_System]], [[Crowd_Memory]], [[Feud_Memory]], Segment Promo System, AI Tiered Integration

❓ **OPEN QUESTIONS:**

- Exact mutation triggers and magnitudes for each anchor type
- How many "influence slots" can a worker have?
- Decay rate for influences (do old influences fade?)
- Template library size needed for potato-tier viability
- How does regional context modify DNA expression?

✅ **STATUS:** Exploratory (December 2024 conversation, needs Vol integration check)

---

## VERSION HISTORY

**Version 0.1 (December 2024 Conversation)**

- Transcript: https://claude.ai/share/4bb953d9-44fb-4759-9950-862697c769f1
- Initial concept developed through discussion of Eric Embry promos
- Distinguished from "promo bio" (static) to "promo DNA" (dynamic, generative)
- Established tiered AI integration approach
- Defined core DNA fields: vocabulary, pacing, emotional range, catchphrases, influences, taboos, mannerisms

---

## DESIGN PRINCIPLES

1. **DNA Not Bio:** This isn't static backstory; it's generative code that produces output
2. **Mutation Through Play:** Characters become themselves through what happens to them
3. **Hardware Agnostic:** System works on potato to powerhouse, just with different fidelity
4. **Player Agency Spectrum:** Full AI generation ↔ Bullet points ↔ Manual writing

---

## DNA SCHEMA

### Core Fields:

```json
{
  "worker_id": "worker_ash_morrow",
  "promo_dna": {
    "base_template": "grizzled_veteran",
    "vocabulary": {
      "tier": 2,
      "regional_flavor": "southern_territory",
      "educated_words": false,
      "profanity_level": "moderate",
      "signature_phrases": []
    },
    "pacing": {
      "baseline": "measured",
      "builds_to": "explosive",
      "pause_frequency": "high",
      "sentence_length": "varied"
    },
    "emotional_range": {
      "floor": 0.2,
      "ceiling": 0.9,
      "default_start": 0.3,
      "escalation_speed": "slow_burn"
    },
    "catchphrases": [],
    "influences": [],
    "taboos": [
      "never mentions past directly",
      "avoids self-aggrandizing"
    ],
    "mannerisms": [
      {
        "trigger": "building_intensity",
        "action": "voice drops lower before explosion",
        "frequency": "common"
      }
    ]
  }
}
```

### Field Definitions:

| Field | Description | Mutation Source |
|-------|-------------|-----------------|
| **base_template** | Starting archetype (greenhorn_generic, veteran, manager, etc.) | Set at creation |
| **vocabulary.tier** | 1-5 scale of verbal sophistication | Education anchors, age |
| **vocabulary.regional_flavor** | Speech patterns by region | Territory history |
| **pacing.baseline** | Default speech rhythm | Personality, training |
| **pacing.builds_to** | Where promos escalate to | Emotional events, anchors |
| **emotional_range.floor/ceiling** | Minimum and maximum intensity | Anchors unlock new ranges |
| **catchphrases** | Signature lines that get repeated | Emerge from successful promos |
| **influences** | Other workers whose style bleeds in | Working relationships |
| **taboos** | Things this character would never say | Personality, backstory |
| **mannerisms** | Physical/vocal habits during promos | Observation, anchors |

---

## MUTATION MECHANICS

### Anchor-Triggered Mutations:

| Anchor Type | DNA Effect |
|-------------|------------|
| **Breakout moment** | emotional_range.ceiling += 0.15 |
| **Betrayal (victim)** | Unlocks "bitter" vocabulary, taboo on trust language |
| **Betrayal (perpetrator)** | Unlocks "justification" patterns |
| **Title win** | confidence markers increase, may add catchphrase |
| **Devastating loss** | emotional_range.floor may lower (vulnerability) |
| **Long feud** | Opponent's name becomes trigger word |
| **Mentor relationship** | Add mentor to influences array |
| **Traumatic injury return** | New mannerisms, pacing changes |

### Influence Bleeding:

When Worker A spends significant time (6+ months) working with Worker B:
- Worker A's DNA gains `influences.push(worker_b_id)`
- Generation can pull speech patterns from Worker B's DNA
- Creates organic "learning from veterans" feel

### Heel/Face Turn Effects:

- **Face → Heel:** Unlocks sarcasm, cruelty vocabulary; ceiling increases
- **Heel → Face:** Unlocks vulnerability; floor may lower; removes certain taboos

---

## GENERATION TIERS

### Tier 1: Potato (No LLM)

**Process:**
1. Load worker's Promo DNA
2. Select template based on context (challenge promo, revenge promo, etc.)
3. Fill template variables from DNA fields
4. Apply pacing markers as stage directions
5. Output formatted script

**Quality:** Functional, recognizable character voice, limited variation

### Tier 2: Mid (7B-13B Local)

**Process:**
1. Load worker's Promo DNA
2. Construct prompt with DNA as strict constraints
3. Provide context (opponent, storyline state, recent events)
4. Model generates within guardrails
5. Post-process for format consistency

**Quality:** Good variation, character voice maintained, occasional drift

### Tier 3: High (30B+ Local or Cloud)

**Process:**
1. Load worker's Promo DNA as character profile
2. Inject full context (feud history, recent matches, crowd state)
3. Model generates freely within voice constraints
4. Minimal post-processing needed

**Quality:** Surprising, emergent, occasionally brilliant

---

## PLAYER ENGAGEMENT SPECTRUM

Players choose their involvement level:

| Mode | Player Does | System Does |
|------|-------------|-------------|
| **Full AI** | Clicks "generate" | Everything |
| **Bullet Points** | Provides key beats ("mention the ladder match, challenge for title, stay calm until the end") | Writes the promo hitting those beats |
| **Outline** | Writes structure and key lines | Fills in transitions and flavor |
| **Manual** | Writes entire promo | Provides suggestions, checks character consistency |
| **Skip** | Nothing | Updates heat/storyline flags, no text generated |

---

## EXAMPLE: ERIC EMBRY DNA

Based on conversation analysis:

```json
{
  "worker_id": "eric_embry_1988",
  "promo_dna": {
    "base_template": "territory_heel_fire",
    "vocabulary": {
      "tier": 3,
      "regional_flavor": "memphis_southern",
      "educated_words": false,
      "profanity_level": "moderate",
      "signature_phrases": ["I'll tell you what"]
    },
    "pacing": {
      "baseline": "calm_controlled",
      "builds_to": "unhinged_screaming",
      "pause_frequency": "strategic",
      "sentence_length": "starts_long_gets_choppy"
    },
    "emotional_range": {
      "floor": 0.3,
      "ceiling": 1.0,
      "default_start": 0.4,
      "escalation_speed": "slow_then_explosive"
    },
    "catchphrases": [],
    "influences": ["memphis_territory_style"],
    "taboos": [],
    "mannerisms": [
      {
        "trigger": "internal_conflict",
        "action": "wrists together, hands raised in pleading gesture",
        "frequency": "signature"
      },
      {
        "trigger": "peak_intensity",
        "action": "eyes widen, veins visible",
        "frequency": "common"
      }
    ]
  }
}
```

---

## GREENHORN EVOLUTION EXAMPLE

**Start (Age 19):**
```json
{
  "base_template": "greenhorn_generic",
  "vocabulary": { "tier": 1 },
  "emotional_range": { "floor": 0.3, "ceiling": 0.5 },
  "catchphrases": [],
  "influences": [],
  "mannerisms": []
}
```

**After 2 years + working with veteran:**
```json
{
  "base_template": "developing_babyface",
  "vocabulary": { "tier": 2 },
  "emotional_range": { "floor": 0.2, "ceiling": 0.6 },
  "catchphrases": ["One day at a time"],
  "influences": ["veteran_mentor_id"],
  "mannerisms": [{ "trigger": "fired_up", "action": "points at crowd" }]
}
```

**After 5 years + heel turn + title win:**
```json
{
  "base_template": "cocky_champion",
  "vocabulary": { "tier": 3, "profanity_level": "high" },
  "emotional_range": { "floor": 0.4, "ceiling": 0.95 },
  "catchphrases": ["One day at a time", "Your time is UP"],
  "influences": ["veteran_mentor_id", "heel_manager_id"],
  "mannerisms": [
    { "trigger": "fired_up", "action": "points at crowd" },
    { "trigger": "dismissive", "action": "waves hand, turns back" }
  ]
}
```

---

## PROFILE COMPLEXITY TIERS (Vol 1 Merge)

Not every worker needs full DNA profiles:

| Tier | Profile Size | Worker Type | Use Case |
|------|--------------|-------------|----------|
| **Full** | 5-7KB | Main eventers, promo-heavy workers | Weekly TV, PPV promos |
| **Standard** | 2-3KB | Midcarders with speaking roles | Occasional promos |
| **Basic** | 0.5-1KB | Occasional speakers, managers handle promos | Rare speaking spots |
| **Silent** | Minimal | No promo capability, all action | Manager speaks, or pure in-ring |

---

## STONE COLD STEVE AUSTIN REFERENCE PROFILE (Vol 1 Merge)

Canonical example of a fully-developed main event promo DNA:

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

---

## LLM QUALITY CONTROLS (Vol 1 Merge)

When generating promos, apply these filters:

| Control | Purpose |
|---------|---------|
| **Era Filter** | Prevents anachronistic references |
| **Character Consistency** | Maintains voice across promos |
| **Escalation Logic** | Promo intensity matches feud heat |
| **Catchphrase Frequency** | Prevents overuse or underuse |
| **Crowd Response Modeling** | Adjusts to expected reactions |

### Generation Prompt Structure

When generating promos, the LLM receives:
1. Worker's Promo DNA Profile
2. Current storyline context
3. Target opponent's profile
4. Crowd type (smart, casual, regional)
5. Segment length/placement
6. Era restrictions (what language/references fit)

---

## RELATED SYSTEMS

- [[Angle_DNA]]: Same architecture for attack segments and physical storytelling
- [[Hidden_Personality]]: Drive, Ego, Morals affect which DNA mutations can occur
- [[Tags_System]]: Tags can unlock/restrict certain vocabulary or mannerisms
- [[Feud_Memory]]: Feud history provides context injection for generation
- [[Crowd_Memory]]: Crowd reactions can trigger catchphrase emergence

---

**Document Status:** Exploratory, needs Vol integration review  
**Next Review:** Cross-reference with Vol 7 promo systems, validate schema against existing Segment Promo mechanics
