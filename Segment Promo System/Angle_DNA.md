# ANGLE DNA SYSTEM

📛 **NAME:** Angle DNA System  
🧭 **CATEGORY:** Worker Identity, Content Generation, Segment Execution  
🔑 **KEYWORDS:** angle, DNA, attack, violence, weapons, escalation, aftermath, segment, beatdown, ambush  
📝 **SUMMARY:**

Angle DNA encodes how a worker behaves in non-match segments: attacks, confrontations, backstage brawls, and dramatic moments. Just as Promo DNA defines voice, Angle DNA defines physical storytelling instincts. A Terry Funk attack segment looks nothing like a Miz attack segment, even with identical booking instructions. The system ensures character consistency in physical actions while mutating through career experiences.

⚙️ **LOGIC OVERVIEW:**

- Every worker has an Angle DNA profile defining their physical segment behavior
- DNA contains violence comfort, weapon preferences, escalation style, aftermath behavior
- Personality traits (Morals, Ego) constrain which actions are available
- Anchors and career events modify DNA over time
- System generates stage directions and action descriptions
- Works across hardware tiers like Promo DNA

🔬 **LLM INTEGRATION:** Yes (tiered)
- **High tier:** Full narrative segment generation with character-accurate actions
- **Mid tier:** Action selection with DNA constraints, templated descriptions
- **Potato tier:** Action templates pulled from DNA fields

📌 **ORIGIN:** Conversation thread (December 2024), discussing Terry Funk vs Miz attack segment differences

📎 **CONNECTED SYSTEMS:** [[Promo_DNA]], [[Hidden_Personality]], [[Tags_System]], [[Feud_Memory]], Segment Promo System, Match Engine

❓ **OPEN QUESTIONS:**

- How do tag team angles combine DNA from both members?
- Manager interference: uses manager's DNA or worker's?
- Injury risk calculations from violence_comfort levels
- Regional modifiers (Japan tolerance vs US tolerance for certain actions)

✅ **STATUS:** Exploratory (December 2024 conversation)

---

## VERSION HISTORY

**Version 0.1 (December 2024 Conversation)**

- Transcript: https://claude.ai/share/4bb953d9-44fb-4759-9950-862697c769f1
- Initial concept from Terry Funk vs Miz comparison
- Established core fields: violence_comfort, weapon_preferences, escalation_style, aftermath_behavior
- Linked to Hidden Personality (Morals, Ego constrain options)

---

## DESIGN PRINCIPLES

1. **Same Event, Different Output:** "Heel attacks babyface" produces wildly different scenes based on DNA
2. **Personality Constrains Options:** High-morals worker won't do certain actions regardless of booking
3. **Mutation Through Violence:** Hardcore matches, blood feuds change DNA over time
4. **Consistent Character:** Actions should feel "right" for who this person is

---

## DNA SCHEMA

### Core Fields:

```json
{
  "worker_id": "worker_terry_funk",
  "angle_dna": {
    "violence_comfort": 0.95,
    "weapon_preferences": [
      { "type": "found_objects", "affinity": 0.9 },
      { "type": "chairs", "affinity": 0.7 },
      { "type": "exotic", "affinity": 0.8, "examples": ["branding_iron", "plastic_bag", "pen"] }
    ],
    "escalation_style": {
      "pattern": "keeps_going",
      "restraint": 0.1,
      "needs_pulloff": true
    },
    "attack_demeanor": {
      "baseline": "feral",
      "personal_vendetta": "unhinged",
      "business_heel": "still_feral"
    },
    "aftermath_behavior": {
      "lingers": true,
      "cuts_promo_over_body": true,
      "emotional_display": "might_cry_while_hurting_you",
      "exit_style": "dragged_away"
    },
    "taboos": [],
    "signature_spots": [
      "piledriver_on_concrete",
      "branding",
      "suffocation"
    ]
  }
}
```

### Contrasting Example (The Miz):

```json
{
  "worker_id": "worker_the_miz",
  "angle_dna": {
    "violence_comfort": 0.5,
    "weapon_preferences": [
      { "type": "chairs", "affinity": 0.7 },
      { "type": "kendo_stick", "affinity": 0.5 }
    ],
    "escalation_style": {
      "pattern": "calculated",
      "restraint": 0.7,
      "needs_pulloff": false
    },
    "attack_demeanor": {
      "baseline": "performative",
      "personal_vendetta": "still_controlled",
      "business_heel": "smug"
    },
    "aftermath_behavior": {
      "lingers": false,
      "cuts_promo_over_body": true,
      "emotional_display": "smirking_to_camera",
      "exit_style": "walks_away_clean"
    },
    "taboos": [
      "no_blood",
      "no_permanent_damage_imagery"
    ],
    "signature_spots": [
      "skull_crushing_finale_on_object"
    ]
  }
}
```

---

## FIELD DEFINITIONS

| Field | Description | Range/Type |
|-------|-------------|------------|
| **violence_comfort** | How far this worker will go | 0.0 - 1.0 |
| **weapon_preferences** | Objects they gravitate toward | Array with affinity scores |
| **escalation_style.pattern** | How violence progresses | "one_and_done", "calculated", "keeps_going" |
| **escalation_style.restraint** | Likelihood of stopping naturally | 0.0 - 1.0 |
| **escalation_style.needs_pulloff** | Requires intervention to stop | Boolean |
| **attack_demeanor** | Emotional state during attacks | Object with context variations |
| **aftermath_behavior** | What happens after the attack | Object with multiple fields |
| **taboos** | Things this worker won't do | Array of strings |
| **signature_spots** | Iconic attack moments they return to | Array of strings |

---

## PERSONALITY CONSTRAINTS

Hidden Personality traits constrain Angle DNA options:

| Trait | Constraint |
|-------|------------|
| **Morals: High** | violence_comfort capped at 0.5, certain weapons unavailable |
| **Morals: Low** | No restrictions, can unlock extreme spots |
| **Ego: High** | More likely to linger, pose, claim credit |
| **Ego: Low** | More likely to exit quickly, avoid spotlight |
| **Loyalty: High** | Won't attack certain relationships regardless of booking |
| **Temperament: Volatile** | escalation_style.restraint lowered |

---

## MUTATION MECHANICS

### Anchor-Triggered Mutations:

| Anchor Type | DNA Effect |
|-------------|------------|
| **First blood match** | violence_comfort += 0.1 |
| **Brutal betrayal** | May unlock new weapon preferences, demeanor shifts |
| **Injures someone (kayfabe)** | Can add to signature_spots if crowd reacted |
| **Gets brutalized** | May increase or decrease violence_comfort (fight or flight) |
| **Deathmatch phase** | Major violence_comfort increase, exotic weapons unlock |
| **Babyface redemption arc** | May add taboos, lower violence_comfort |

### Working Style Influence:

Extended feuds with violent workers can shift DNA:
- 6-month feud with a brawler → violence_comfort trends up
- Working under strict promotion → taboos may be added

---

## GENERATION OUTPUT EXAMPLES

### Input:
```
Booking: "Heel attacks babyface after match"
Heel: Terry Funk DNA
Context: Heated personal feud, week 8
```

### Output (High Tier):
```
[Funk doesn't wait for the bell to finish ringing. He's already 
sliding a chair into the ring, but ignores it—grabs a pen from 
the timekeeper instead. The look in his eyes says this isn't 
business.

He drops onto the fallen babyface, pen raised. The crowd screams. 
Security floods the ring but Funk fights them off with his free 
hand, still trying to get at his opponent's face.

It takes six men to drag him away. He's crying. He's laughing. 
He's trying to explain something to the camera but it's just 
animal sounds.

The babyface hasn't moved.]
```

### Same Input with Miz DNA:

### Output (High Tier):
```
[Miz waits. Lets the moment breathe. The babyface struggles to 
their feet—that's when he strikes. Skull Crushing Finale onto 
the steel chair he'd positioned earlier.

He stands over the body, adjusts his hair, looks directly into 
the camera.

"This is what happens when you don't stay in your lane."

Clean exit through the ropes. Security doesn't need to intervene. 
He's already done what he came to do.]
```

---

## TIER IMPLEMENTATION

### Tier 1: Potato (No LLM)

**Process:**
1. Load attacker's Angle DNA
2. Select action template based on context + violence_comfort
3. Fill weapon from weapon_preferences
4. Apply aftermath_behavior template
5. Output stage directions

**Quality:** Functional, character-appropriate, limited narrative flair

### Tier 2: Mid (7B-13B Local)

**Process:**
1. Load Angle DNA as constraints
2. Provide feud context, recent events
3. Model selects actions within DNA boundaries
4. Generate prose description
5. Post-process for consistency

**Quality:** Good variety, maintains character, some narrative surprise

### Tier 3: High (30B+ Local or Cloud)

**Process:**
1. Full DNA profile as character
2. Complete feud history injection
3. Model generates full scene
4. Minimal constraints beyond DNA fields

**Quality:** Cinematic, surprising, character-perfect

---

## PLAYER INVOLVEMENT

Like Promo DNA, players choose involvement:

| Mode | Player Does | System Does |
|------|-------------|-------------|
| **Full AI** | Specifies "heel attacks face" | Generates full scene |
| **Key Beats** | "Use chair, target knee, security pulls off" | Writes around those beats |
| **Detailed Outline** | Writes action sequence | Adds description flavor |
| **Manual** | Writes full scene | Validates against DNA, flags OOC actions |
| **Skip** | Nothing | Updates storyline flags, no text |

---

## TAG INTEGRATION

Tags modify Angle DNA expression:

| Tag | Effect |
|-----|--------|
| **Innovator of Violence** | Unlocks creative weapon combinations |
| **Stone Cold Killer** | Removes emotional display from aftermath |
| **Protective (of X)** | Will intervene in attacks on protected worker |
| **Coward** | violence_comfort hard-capped, flees confrontations |
| **Hardcore Legend** | violence_comfort floor raised, can't go soft |

---

## RELATED SYSTEMS

- [[Promo_DNA]]: Same architecture for verbal expression
- [[Hidden_Personality]]: Morals, Ego, Temperament constrain options
- [[Tags_System]]: Tags modify DNA expression
- [[Feud_Memory]]: Feud intensity affects which DNA ranges activate
- Injury System: violence_comfort correlates with injury risk

---

**Document Status:** Exploratory, needs integration with existing Segment system docs  
**Next Review:** Cross-reference with Segment Types.md, validate against Vol materials
