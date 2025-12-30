# Match Processing

📛 **MECHANIC:** Match Processing
🔗 **PARENT SYSTEM:** [[_Match Engine Index|Match Engine]]
🧭 **CATEGORY:** Match Simulation / Core Gameplay
🔑 **KEYWORDS:** match processing, chemistry, execution, finish impact, card placement, narrative context
📌 **ORIGIN:** Vol 1-2 (Booking Engine Phase 1)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-2 | 🔒 LOCKED |

---

## Overview

The evaluation layer between [[Match Inputs]] and [[Match Consequences]]. Determines match quality by evaluating chemistry, execution, context, and finish. Feeds into [[Match Types/Match Quality Factors|Match Quality Factors]].

---

## Processing Layers

| Layer | Evaluates | Weight |
|-------|-----------|--------|
| **Worker Chemistry** | Style compatibility, history, tension | High |
| **Match Type Fit** | Are workers suited to this format? | Medium |
| **Card Placement** | Over/under-delivering for slot? | Medium |
| **Crowd Energy** | Entering energy level, stamina | High |
| **Execution Quality** | Psychology, pacing, botches, charisma | Highest |
| **Finish Impact** | Clean vs dirty, surprise, believability | High |
| **Narrative Context** | Does it advance or confuse story? | Medium |

---

## Worker Chemistry

| Factor | Effect |
|--------|--------|
| **Style compatibility** | Complementary styles mesh well |
| **Past matches** | Experience together improves chemistry |
| **Personal tension** | Real heat can enhance or hurt |
| **Communication skills** | Calling spots, adjustments |
| **Ego conflicts** | High ego workers may not cooperate |

**Chemistry Score:** Composite of above factors

| Chemistry | Result |
|-----------|--------|
| Excellent | Natural flow, easy storytelling |
| Good | Solid work, minor rough spots |
| Neutral | Professional, nothing special |
| Poor | Awkward, visible disconnects |
| Terrible | Trainwreck, botch-prone |

### Chemistry Tag System (#209)

| Tag | Effect |
|-----|--------|
| **Natural Chemistry** | +15% match quality together |
| **Proven Chemistry** | History of great matches, +10% |
| **Awkward Pairing** | -10% match quality |
| **Toxic Chemistry** | -20%, should be avoided |
| **Learning Curve** | First few matches rough, improves with repetition |
| **Carry Ability** | Can elevate weak partners |

**Application:** Most pairings are neutral; tags only for notable cases.

### Style Synergy Mechanics (#30)

| Pairing | Typical Result |
|---------|----------------|
| Technical vs Technical | Chess match, appreciated by purists |
| Brawler vs Brawler | Chaotic violence, crowd heat |
| High Flyer vs Monster | David vs Goliath drama |
| Shooter vs Technical | Mat-based clinic |
| Conflicting Styles | Requires adaptation or suffers |

**Application:** Chemistry tags flag known pairings; most matches default to "competent."

---

## Match Type Fit

From worker [[Tags_System|Tags]] and [[Worker_Skills|Skills]]:

| Scenario | Effect |
|----------|--------|
| **Specialist in type** | +15% quality ceiling |
| **Competent in type** | Normal quality range |
| **Uncomfortable in type** | -15% quality ceiling |
| **Wrong type entirely** | Risk of disaster |

Examples:
- High Flyer in Ironman = stamina issues
- Technical wrestler in Deathmatch = uncomfortable
- Brawler in Ladder match = may work, different flavor

---

## Card Placement Evaluation

| Scenario | Effect |
|----------|--------|
| **Match exceeds slot** | Pleasant surprise, bonus |
| **Match meets slot** | Expectations fulfilled |
| **Match below slot** | Disappointment penalty |
| **Main event underdelivers** | Major negative |
| **Opener overdelivers** | Sets high bar (risky for rest of card) |

---

## Crowd Energy (from [[Emotional_Show_Flow|Emotional Show Flow]])

| Crowd State | Effect |
|-------------|--------|
| **Hot** | Reactions amplified, moves land harder |
| **Neutral** | Standard evaluation |
| **Cool** | Need to work harder for reactions |
| **Burned out** | Even good work gets muted response |
| **Dead** | Major penalty, uphill battle |

**Crowd Stamina Modifier:** Same 4.5-star match gets lower rating if crowd exhausted

---

## Execution Quality

The biggest factor. Components:

| Component | Description |
|-----------|-------------|
| **Psychology** | In-match storytelling, see [[Match Types/Match Quality Factors|Match Quality Factors]] |
| **Pacing** | Rhythm, escalation, peaks |
| **Botches** | Mistakes, blown spots, safety issues |
| **Charisma** | Individual star quality |
| **Improvisation** | Adjusting to unexpected situations |
| **Fan Alignment** | Working with or against crowd mood |

**Psychology is the primary multiplier** (0.5x to 2.0x on base quality)

---

## Finish Impact

| Finish Type | Impact |
|-------------|--------|
| **Clean, decisive** | Positive, builds winner |
| **Protected loss** | Loser preserved |
| **Surprise upset** | Major bump if believable |
| **Dusty finish** | Crowd frustration risk |
| **Screwjob** | Story heat, credibility risk |
| **Interference** | Depends on story needs |
| **Botched finish** | Damages both workers |
| **Anti-climactic** | Crowd disappointment |

---

## Narrative Context

| Scenario | Effect |
|----------|--------|
| **Advances story** | Positive, feud progression |
| **Payoff moment** | Major positive if earned |
| **Confuses story** | Negative, crowd disengaged |
| **Contradicts continuity** | Major negative |
| **Creates new story** | Opportunity for future |

---

## Processing Flow

```
Match Inputs → Processing Layers → Quality Score → Consequences

1. Calculate base quality (worker skills average)
2. Apply chemistry modifier
3. Apply match type fit modifier
4. Apply card placement modifier
5. Apply crowd energy modifier
6. Apply execution quality multiplier
7. Apply finish impact modifier
8. Apply narrative context modifier
9. Final quality score (0-100)
```

---

## Connected Mechanics

- [[Match Inputs]] - feeds processing
- [[Match Consequences]] - output of processing
- [[Match Types/Match Quality Factors|Match Quality Factors]] - detailed quality criteria
- [[Emotional_Show_Flow|Emotional Show Flow]] - crowd context

---

## In-Match Momentum System (#190)

**Core Concept:** Momentum shifts during matches create drama.

| Momentum State | Visual/Narrative Cues |
|----------------|-----------------------|
| **Dominant** | Controlling pace, landing offense |
| **Neutral** | Back and forth, feeling out |
| **On Ropes** | Taking punishment, survival mode |
| **Fire Up** | Rally beginning, crowd sensing comeback |
| **Second Wind** | Desperation burst, everything they've got |

**Psychology Skill determines:** How well worker controls these shifts.  
**Selling Skill determines:** How believably they convey momentum states.

---

## Match Pace Categories (#214)

| Pace | Description | Best For |
|------|-------------|----------|
| **Methodical** | Slow build, holds, psychology | Technical, old school |
| **Standard** | Balanced offense and selling | Most workers |
| **Fast-Paced** | Quick exchanges, limited selling | High flyers, juniors |
| **Chaotic** | Weapon spots, brawling, no rules | Hardcore matches |
| **Sprint** | All action, minimal rest | Short TV matches |
| **Epic** | Multiple pace shifts, long-form | PPV main events |

**Worker Preference:** Some workers work better at certain paces.  
**Crowd Fatigue:** Fast pace + long duration = burnout.

---

## Botch System (#103)

| Botch Type | Cause | Effect |
|------------|-------|--------|
| **Minor** | Timing off, sloppy execution | Small rating dip |
| **Noticeable** | Clear mistake, crowd groans | Moderate rating hit |
| **Major** | Move completely fails | Significant rating drop |
| **Dangerous** | Nearly causes injury | Rating hit + backstage heat |
| **Catastrophic** | Causes actual injury | Match stops, major fallout |

**Recovery:** High psychology workers can work botches into story.  
**Cover Ability:** Some workers excellent at hiding mistakes (see Ring Generalship in [[Worker_Skills]]).

---

## Match Timing System (#105)

| Aspect | Description |
|--------|-------------|
| **Entrance Timing** | Knowing when to start/stop poses |
| **Spot Timing** | Executing moves at peak dramatic moment |
| **Finish Timing** | Ending match at emotional high point |
| **Commercial Timing** | TV workers know when to pause for breaks |
| **Recovery Timing** | How long between big spots |

**Who Masters It:** TV era veterans, psychology experts  
**Who Struggles:** Indie stars, deathmatch workers, green talent

---

## Open Questions

- Exact weights for each layer
- Chemistry calculation formula
- Botch frequency and impact scaling

---

## Implementation Notes

```json
{
  "match_processing": {
    "match_id": "m_001",
    "base_quality": 72,
    "modifiers": {
      "chemistry": 1.15,
      "match_type_fit": 1.0,
      "card_placement": 1.05,
      "crowd_energy": 0.95,
      "execution_quality": {
        "psychology": 1.3,
        "pacing": 1.1,
        "botches": -2,
        "charisma": 1.1
      },
      "finish_impact": 1.1,
      "narrative_context": 1.05
    },
    "final_quality": 84,
    "quality_tier": "great_match"
  }
}
```
