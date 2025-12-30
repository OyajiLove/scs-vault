# Road Agent Layer System

📛 **NAME:** Road Agent Layer System  
🧭 **CATEGORY:** Booking System / Match Planning  
🔑 **KEYWORDS:** road agent, match planning, agenting, instructions, emotional, story, finish, crowd, worker arc  
📝 **SUMMARY:** Models how road agents plan matches with emotional, career, and memory consequences. Unlike TEW's mechanical stat tweaking, SCS road agents architect emotional stories that leave scars, build legends, affect loyalty, and anchor world memory. Every match instruction has downstream effects on workers, crowds, promotions, and mythology.

⚙️ **LOGIC OVERVIEW:**
- 7 Core Pillars (outcome, emotional aim, worker focus, match structure, finish type, special triggers, crowd target)
- 4 New SCS categories (worker arc planning, crowd emotional target, promotion philosophy alignment, memory anchor chance)
- Road agent instructions affect worker memory, relationships, locker room culture, fanbase perception
- Matches aren't just "booked," they're emotionally architected

🔬 **LLM INTEGRATION:** High (LLM could generate agent notes, suggest emotional aims, evaluate philosophy alignment)

📌 **ORIGIN:** Vol 5 lines 736-758 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Match Flavors]] - flavor compatibility
- [[Match Type Categories]] - structural formats
- [[Booking_Engine_P1-3]] - booking inputs
- [[Emotional_Show_Flow]] - show pacing
- [[World_Memory_Drift]] - memory anchoring
- [[Worker_Morale]] - worker emotional response

❓ **OPEN QUESTIONS:**
- Agent personality types (specialists in different styles)
- Agent-worker relationship effects
- Agent reputation/trust mechanics
- Auto-suggestion algorithms

✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 5 | 🔒 LOCKED |

---

## The Problem with TEW Agenting

TEW treats road agents as mechanical stat tweakers:
- "Misawa almost got into a fight" → no emotional follow-up
- No loyalty drift, no career impact, no myth building
- Matches happen → file closed
- No living memory

**SCS Fix:** Every incident triggers downstream effects across Worker Memory, Relationship Drift, Locker Room Culture, Fanbase Perception, Promotion Trust, and Myth Evolution.

---

## SCS Road Agent Core Pillars (7)

| Pillar | Description |
|--------|-------------|
| **Outcome Planning** | Wins, losses, draws tied to career arcs, loyalty, morale, myth building |
| **Emotional Story Planning** | Match aims (Work Crowd, Tell Story, Create Chaos) tied to crowd memory, worker arc growth |
| **Worker Focus Orders** | Protect, Dominate, Keep Strong affecting worker pride, loyalty, backstage reputation |
| **Match Structure Emotion** | Scripted vs Called vs Open chaos affecting how authentic match feels to fans and workers |
| **Finish Emotional Resonance** | Clean Wins, Screwjobs, Distractions affecting crowd memory, worker mythology |
| **External Involvement Impact** | Interference, Bumps, Betrayals building fan memory of cowardice, bravery, injustice |
| **Special Emotional Triggers** | Mask Loss, Hair Loss, Bumps with emotional memory, career scars, crowd empathy |

---

## New SCS-Specific Categories (4)

| Category | Purpose |
|----------|---------|
| **Worker Emotional Arc Planning** | "This is part of X's redemption arc, must show struggle" / "This is X's pride collapse match" |
| **Crowd Emotional Target** | "Crowd must feel injustice" / "Crowd must feel bittersweet triumph" / "Crowd must erupt for rebellion" |
| **Promotion Philosophy Alignment** | Does this match uphold the promotion's soul (King's Road storytelling, Outlaw chaos, Strong Style realism)? |
| **Memory Anchor Chance** | Is this match planned with potential to become world memory moment? If yes, extra emotional weight triggers |

---

## Full Road Agent Instruction Menu

### 1. Outcome

| Instruction | Effect |
|-------------|--------|
| **Clean Win** | Winner gains credibility, loser loses some |
| **Protected Loss** | Loser maintains credibility despite losing |
| **Draw** | Both protected, builds rematch demand |
| **Controversial Finish** | Story advancement, both partially protected |
| **Squash** | Winner dominant, loser damaged |

### 2. Emotional Aim

| Instruction | Crowd Target |
|-------------|--------------|
| **Work the Crowd** | Build heat or pop through engagement |
| **Tell a Story** | Psychological arc, beginning-middle-end |
| **Calm the Crowd** | Bring energy down (before or after hot match) |
| **Create Mayhem** | Chaos, unpredictability, spectacle |
| **Build a Star** | One worker elevated, crowd investment increases |

### 3. Worker Focus

| Instruction | Effect on Worker |
|-------------|------------------|
| **Keep Strong** | Protected, credibility maintained |
| **Protect** | Minimal damage even in loss |
| **Dominate** | Look powerful, squash opponent |
| **Humble** | Lose credibility, knocked down a peg |
| **Humiliate** | Career-damaging loss, pride destroyed |
| **Heal** | Redemption arc advancement |
| **Harden** | Build through adversity, future payoff |

### 4. Match Structure

| Instruction | Feel |
|-------------|------|
| **Scripted** | Tight, professional, mechanical |
| **Called in Ring** | Authentic, organic, raw |
| **Open Chaos** | Unplanned feeling, volatile |
| **Hybrid** | Scripted spots with called transitions |

### 5. Finish Type

| Instruction | Emotional Resonance |
|-------------|---------------------|
| **Clean Pin** | Decisive, honorable |
| **Submission** | Technical dominance |
| **Cheap Win** | Heel heat, face sympathy |
| **Screwjob** | Injustice, controversy |
| **Interference** | Story advancement |
| **DQ** | Protects both, frustrates crowd if overused |
| **Countout** | Weak, protect both, can signal cowardice |
| **Time Limit Draw** | Builds epic rematch |
| **Ref Bump Finish** | Classic heel victory |
| **Rollup/Flash Pin** | Underdog victory or sneaky heel |

### 6. Special Triggers

| Instruction | Career Impact |
|-------------|---------------|
| **Heel Turn** | Massive memory anchor, changes career trajectory |
| **Face Turn** | Redemption arc, crowd re-evaluation |
| **Unmasking** | Career-defining moment (especially lucha) |
| **Hair Loss** | Humiliation, pride damage |
| **Blood** | Intensity escalation, polarizing |
| **Stretcher Spot** | Injury angle, sympathy generation |
| **Post-Match Attack** | Heat building, story continuation |

### 7. Crowd Emotional Target

| Instruction | Desired Feeling |
|-------------|-----------------|
| **Hope** | Babyface overcomes odds |
| **Anger** | Injustice, heel heat |
| **Sadness** | Tragedy, loss, retirement |
| **Rebellion** | Anti-authority, underdog uprising |
| **Nostalgia** | Tribute, legacy honoring |
| **Shock** | Unexpected turn, upset |
| **Catharsis** | Payoff of long build |

---

## Sample Road Agent Sheet

```yaml
📜 Road Agent Instructions:
🏆 Outcome: Worker A Wins
🎭 Emotional Aim: Redemption Match - Crowd must feel bittersweet triumph
🔨 Worker Focus: 
  - Worker A: Protected, show struggle before victory
  - Worker B: Protected but must show growing cracks in confidence
🎬 Match Structure: Called In Ring (emotional authenticity emphasized)
🎨 Match Flavor: Story with Technical elements
🏁 Finish Type: Clean Win - overcoming adversity
🎯 Special Trigger: Worker B teases heel turn post-match (emotional fracture)
😭 Crowd Target: Hope → Catharsis
💀 Memory Anchor Attempt: YES - if crowd emotional surge crosses threshold
🏛 Promotion Identity: King's Road - must maintain emotional escalation
```

---

## Downstream Effects

Every road agent decision ripples through:

| System | Effect |
|--------|--------|
| **Worker Memory** | "Misawa almost got into a fight" → reputation adjustment |
| **Relationship Drift** | Conflict/bonding affects future interactions |
| **Locker Room Culture** | How incident handled affects morale |
| **Fanbase Rumor Drift** | Leaks reframe worker perception |
| **Promotion Trust** | How leadership handles incidents affects worker loyalty |
| **Myth Drift** | Over time, incidents fold into legend or cautionary tale |

---

## Road Agent Dynamic Warnings ✅ LOCKED

Good road agents detect live crowd drift and advise audibles. These warnings fire based on show context.

### Warning Timing

| Timing | Trigger |
|--------|--------|
| **Pre-Match Check** | Right before match starts. Agent notices misalignment between planned match and crowd state. |
| **Pre-Segment Check** | Before major angles, interviews, or special appearances if crowd emotional needs are mismatched. |
| **Live Mid-Match Observation** | 🔨 PHASE 2: If live crowd drift simulation built, agents could warn about mid-match burnout. |

### Warning Categories (6 Types)

| Category | Description | Example |
|----------|-------------|--------|
| **Crowd Fatigue Warning** | Crowd emotionally exhausted, needs re-energizing | "Boss, the crowd's dying out there. This next epic might kill the vibe." |
| **Mismatch Warning** | Match flavor/length wrong for current crowd mood | "Might wanna rethink sending a 20-min grapplefest after that bloody street fight." |
| **Overload Warning** | Too many similar emotional beats stacking | "Another screwjob finish after what they just saw? Crowd might riot." |
| **Pacing Drift Warning** | Show flow unbalanced, too many fast/slow segments | "We've had three sprints in a row. Crowd might burn out without a breather." |
| **Worker Fatigue Warning** | Key worker visibly exhausted or injured | "Worker A's dragging a leg out there, boss. Maybe call an audible, shorten it." |
| **Micro-Climate Betrayal Risk** | Crowd about to turn if next segment flops | "They're restless, boss. One more misfire and we might lose them tonight." |

**Philosophy:** Warnings always contextual, human, short. Not just numeric popups. Good agents warn clearly. Bad agents might miss it or give misleading advice (see Agent Traits in Parking Lot).

### Warning Delivery Channels

| Channel | Description |
|---------|-------------|
| **Popup Agent Message** | Discrete textbox near booking flow: "Agent [Name]: 'Hey boss, the crowd's fading. Maybe send them something fast and wild?'" |
| **Sound Cue** | If Soul Sounds enabled, small voice line or audio clip tied to warning trigger |
| **Action Prompt** | Player can Acknowledge, Adjust Match, or Ignore the advice |

**No forced changes.** You decide how to react. Agents build trust reputation based on how often their advice proves correct. Workers remember if you blame them for things you ignored.

### Warning Severity Levels

| Severity | Description |
|----------|-------------|
| **Minor Alert** | Small emotional drift risk. Could course-correct naturally. Safe to gamble. |
| **Moderate Risk** | Noticeable drift. Serious booking adjustment advised. |
| **Critical Risk** | Emotional collapse incoming. Crowd loyalty, show prestige, worker morale could all take serious hits if ignored. |

---

## Worker Physical/Emotional Markers ✅ LOCKED

Road agents track visible worker state that affects crowd response:

| Physical Marker | Emotional Resonance |
|-----------------|--------------------|
| **Scar Tissue** | Crowd recognizes hard lives lived. Bigger pops for blood. |
| **Limping or Hesitation** | Crowd sees emotional or physical exhaustion. Bigger sympathy if done right. |
| **Facial Emotion Acting** | Workers trained in selling grief, fury, panic. Crowd buys in deeper. |

---

## Agent Awareness Requirements

Road Agents must be aware of:

1. **Match Type booked** (by booker)
2. **Flavor compatibility** (from [[Match Flavors]] chart)
3. **Worker specialties** (can they deliver this?)
4. **Promotion identity** (does this fit house style?)
5. **Show pacing** (where does this fit in flow?)
6. **Feud stage** (early build vs blowoff?)
7. **Crowd emotional state** (what came before?)

---

## TEW vs SCS Comparison

| Aspect | TEW | SCS |
|--------|-----|-----|
| **Match outcomes** | Stats change | Career arcs evolve |
| **Worker focus** | Stat modifiers | Pride, loyalty, morale affected |
| **Finish types** | Mechanical options | Emotional resonance tracked |
| **Memory** | None | World memory anchoring |
| **Promotion identity** | Ignored | Alignment checked |
| **Crowd** | Rating number | Emotional state tracked |
| **Long-term** | Nothing | Scars, legends, betrayals persist |

---

## Connected Mechanics

- [[Match Flavors]] - flavor compatibility for agenting
- [[Match Type Categories]] - structural constraints
- [[Booking_Engine_P1-3]] - booking layer inputs
- [[Emotional_Show_Flow]] - show pacing context
- [[World_Memory_Drift]] - memory anchoring
- [[Worker_Morale]] - worker response to treatment

---

## Implementation Notes

```json
{
  "road_agent_sheet": {
    "match_id": "match_001",
    "outcome": "CLEAN_WIN",
    "emotional_aim": "REDEMPTION",
    "worker_focus": {
      "worker_a": "PROTECTED_WINNER",
      "worker_b": "PROTECTED_LOSER"
    },
    "match_structure": "CALLED_IN_RING",
    "match_flavor": "STORY",
    "finish_type": "CLEAN_PIN",
    "special_triggers": ["HEEL_TURN_TEASE"],
    "crowd_target": "HOPE_TO_CATHARSIS",
    "memory_anchor_attempt": true,
    "promotion_alignment": "KINGS_ROAD",
    "downstream_effects": {
      "worker_a_morale": +15,
      "worker_b_confidence": -10,
      "crowd_satisfaction": 85,
      "memory_anchor_roll": 72
    }
  }
}
```

---

## Philosophy

> "Matches in SCS will not just 'happen.' They will leave scars, legends, betrayals, loyalty shifts, if agented right. Road agents aren't stat tweakers. They're emotional architects, building moments that echo through careers and generations."

---

**Document Status:** Locked  
**Source:** Vol 5 lines 736-758  
**Next Review:** Road Agent Personality Types
