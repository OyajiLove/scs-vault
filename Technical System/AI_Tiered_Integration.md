# AI TIERED INTEGRATION SYSTEM

📛 **NAME:** AI Tiered Integration System  
🧭 **CATEGORY:** Technical Architecture, AI Integration, Hardware Scaling  
🔑 **KEYWORDS:** AI, LLM, hardware, tiers, potato, scaling, local, cloud, graceful degradation, templates  
📝 **SUMMARY:**

SCS is designed to run across wildly different hardware configurations, from potato laptops to high-end gaming PCs. The AI Tiered Integration system ensures the game remains fully playable at every level while scaling up AI-powered features (promo generation, emergent events, booking AI) based on available compute. Core simulation logic remains deterministic; AI adds texture and surprise without being load-bearing.

⚙️ **LOGIC OVERVIEW:**

- Three hardware tiers: Potato (no GPU), Mid (6-12GB VRAM), High (12GB+ VRAM)
- AI features degrade gracefully: High → full generation, Mid → constrained generation, Potato → templates
- Core game loop never requires AI; simulation is deterministic
- AI makes decisions that the game then renders (separation of concerns)
- Users can manually override tier detection and choose their experience
- Architecture allows swapping models as ecosystem improves

🔬 **LLM INTEGRATION:** This IS the LLM integration architecture document

📌 **ORIGIN:** Conversation thread (December 2024), discussing hardware flexibility for SCS users

📎 **CONNECTED SYSTEMS:** [[Promo_DNA]], [[Angle_DNA]], Booking Engine, Emergent Events System, all content generation systems

❓ **OPEN QUESTIONS:**

- Exact VRAM thresholds for tier detection
- Recommended models per tier (will change rapidly)
- Cloud API fallback: offer as option for potato users?
- Performance benchmarking methodology
- Mobile tier considerations (iOS/Android)

✅ **STATUS:** Exploratory (December 2024 conversation, architectural planning)

---

## VERSION HISTORY

**Version 0.1 (December 2024 Conversation)**

- Transcript: https://claude.ai/share/4bb953d9-44fb-4759-9950-862697c769f1
- Established three-tier framework (Potato/Mid/High)
- Defined graceful degradation principle
- Separated AI texture from core simulation logic
- Identified key use cases: booking, promos, angles, emergent events

---

## DESIGN PRINCIPLES

1. **AI Adds Texture, Not Structure:** The simulation works without AI; AI makes it richer
2. **Graceful Degradation:** Every feature has a non-AI fallback
3. **Player Choice:** Users can override detected tier or disable AI entirely
4. **Future-Proof:** Architecture allows model swaps as technology improves
5. **No Cloud Dependency:** Local-first design, cloud as optional enhancement

---

## HARDWARE TIERS

### Tier 1: Potato (No Dedicated GPU)

**Hardware Profile:**
- Integrated graphics or very old GPU
- < 4GB usable VRAM
- Typical: Older laptops, budget PCs, some tablets

**AI Capabilities:**
- No local LLM inference
- Template-based content generation
- Rules-based decision making
- Optional: Cloud API if user provides key

**Experience:**
- Fully playable, all features functional
- Content generation feels more formulaic
- Less emergence in world events
- Faster performance (no AI overhead)

### Tier 2: Mid (6-12GB VRAM)

**Hardware Profile:**
- GTX 1060 6GB through RTX 3060 12GB
- Can run quantized 7B-13B models
- Typical: Mid-range gaming PCs, newer laptops with discrete GPU

**AI Capabilities:**
- Local inference with smaller models (7B-13B quantized)
- DNA-constrained generation (heavy guardrails)
- AI booking decisions with personality modeling
- Basic emergent event generation

**Experience:**
- Good variety in generated content
- Character voices recognizable but occasional drift
- Meaningful emergence in world simulation
- Moderate performance impact

### Tier 3: High (12GB+ VRAM)

**Hardware Profile:**
- RTX 3080+ or equivalent
- 24GB ideal (RTX 3090, 4090)
- Can run 30B-70B models
- Typical: High-end gaming PCs, workstations

**AI Capabilities:**
- Full local inference with large models
- Minimal-constraint generation
- Complex personality modeling for booking AI
- Rich emergent event synthesis
- Multi-character interaction generation

**Experience:**
- Surprising, creative content generation
- Strong character voice consistency
- Deep emergence (events that feel authored but weren't)
- Higher performance overhead, but manageable

---

## USE CASE BREAKDOWN

### Promo Generation

| Tier | Approach | Quality |
|------|----------|---------|
| Potato | Template + DNA variable injection | Functional, recognizable character |
| Mid | 7B model with heavy DNA constraints | Good variety, mostly on-voice |
| High | 70B model with DNA as profile | Creative, occasionally brilliant |

### Angle/Segment Generation

| Tier | Approach | Quality |
|------|----------|---------|
| Potato | Action templates from Angle DNA | Appropriate actions, basic descriptions |
| Mid | Model selects actions within DNA bounds | Varied, character-appropriate |
| High | Full scene generation | Cinematic, surprising |

### Booking AI (NPC Promoters)

| Tier | Approach | Quality |
|------|----------|---------|
| Potato | Rules-based with personality weights | Logical but predictable |
| Mid | Model reasoning with constraints | Has "opinions," makes interesting choices |
| High | Full personality simulation | Feels like competing against real bookers |

### Emergent Events

| Tier | Approach | Quality |
|------|----------|---------|
| Potato | Weighted random from event tables | Events happen, feel somewhat random |
| Mid | Model evaluates character states, selects fitting events | Events feel motivated |
| High | Model synthesizes novel events from character interactions | "Holy shit" moments |

---

## ARCHITECTURE

### Separation of Concerns:

```
┌─────────────────────────────────────────────────┐
│                 PRESENTATION                     │
│         (UI, text output, graphics)              │
└─────────────────────────────────────────────────┘
                        ▲
                        │
┌─────────────────────────────────────────────────┐
│              AI TEXTURE LAYER                    │
│  (Promo gen, angle gen, emergent events)         │
│  [OPTIONAL - degrades gracefully]                │
└─────────────────────────────────────────────────┘
                        ▲
                        │
┌─────────────────────────────────────────────────┐
│            CORE SIMULATION                       │
│  (Ratings, stats, progression, deterministic)    │
│  [REQUIRED - always runs, no AI dependency]      │
└─────────────────────────────────────────────────┘
                        ▲
                        │
┌─────────────────────────────────────────────────┐
│                 DATA LAYER                       │
│      (Workers, shows, history, DNA)              │
└─────────────────────────────────────────────────┘
```

### Key Point:

The AI Texture Layer makes **decisions** that the Core Simulation then **processes**. AI never directly modifies game state; it provides inputs that the deterministic engine handles.

Example:
1. AI decides "Worker X should have a backstage altercation with Worker Y"
2. Core Simulation processes: relationship change, potential injury roll, morale impact
3. AI generates text description of what happened
4. Presentation shows the event to player

---

## TIER DETECTION

### Auto-Detection (Default):

```python
def detect_tier():
    vram = get_available_vram()
    
    if vram < 4:
        return "potato"
    elif vram < 12:
        return "mid"
    else:
        return "high"
```

### Manual Override:

Players can force any tier:
- Potato users with cloud API key can enable Mid/High features
- High users who want faster performance can force Potato
- Settings persist across sessions

### Per-Feature Control:

Advanced settings allow per-feature tier selection:
- Promos: High (wants quality)
- Emergent events: Potato (wants speed)
- Booking AI: Mid (balance)

---

## MODEL RECOMMENDATIONS (As of December 2024)

**Note:** This section will need regular updates as models improve.

### Mid Tier:
- Llama 3.1 8B (Q4 quantized): Good balance
- Mistral 7B: Fast, decent quality
- Qwen 2.5 7B: Strong instruction following

### High Tier:
- Llama 3.1 70B (Q4 quantized): Excellent quality
- Qwen 2.5 72B: Strong reasoning
- Mixtral 8x7B: Good speed/quality balance

### Cloud Fallback (Optional):
- Claude API: Highest quality, costs money
- GPT-4 API: High quality, costs money
- Local preference strongly encouraged

---

## TEMPLATE SYSTEM (Potato Tier)

For potato tier, robust template libraries are essential:

### Template Categories:
- Promo templates by type (challenge, revenge, celebration, etc.)
- Angle templates by type (attack, confrontation, alliance, etc.)
- Event templates by category (scandal, injury, debut, etc.)
- News item templates

### Template + DNA Example:

**Template:**
```
{worker_name} stepped up to the microphone, {emotional_state}. 
"{opening_catchphrase}" {pronoun} began. "{body_statement} 
And {opponent_name}, {direct_address}. {closing_statement}"
```

**DNA Variables Injected:**
```
worker_name: "Ash Morrow"
emotional_state: "jaw tight, voice low" (from pacing.baseline)
opening_catchphrase: "" (none in DNA)
body_statement: generated from context + vocabulary tier
opponent_name: "Jack Thornton"
direct_address: generated from emotional_range
closing_statement: generated from pacing.builds_to
```

**Output:**
```
Ash Morrow stepped up to the microphone, jaw tight, voice low.
"" he began. "You think what you did last week goes unanswered?
And Jack Thornton, I'm coming for you. There's nowhere to hide."
```

---

## PERFORMANCE CONSIDERATIONS

### Memory Management:
- Load models once at game start
- Keep in memory during session
- Unload during save/load operations

### Inference Batching:
- Queue multiple generation requests
- Process during "advance time" operations
- Pre-generate content during downtime

### Fallback Triggers:
- If inference takes > 30 seconds, offer to fall back to lower tier
- If model crashes, graceful degradation to templates
- Always save before heavy inference operations

---

## FUTURE CONSIDERATIONS

### Mobile Tier (iOS/Android):
- Likely Potato-equivalent at launch
- May support on-device inference as mobile AI chips improve
- Cloud API option for mobile users who want quality

### Model Ecosystem Evolution:
- Architecture allows hot-swapping models
- User can choose preferred model
- Community can recommend models per use case

### Hybrid Approaches:
- Run small model locally for speed
- Send complex requests to cloud for quality
- User controls the balance

---

## RELATED SYSTEMS

- [[Promo_DNA]]: Primary consumer of promo generation tier
- [[Angle_DNA]]: Primary consumer of angle generation tier
- Booking Engine: Uses booking AI tier
- Emergent Events: Uses event generation tier
- All content generation systems depend on this architecture

---

**Document Status:** Exploratory, architectural planning  
**Next Review:** Revisit model recommendations quarterly, performance testing needed
