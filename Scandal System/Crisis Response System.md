# Crisis Response System

📛 **MECHANIC:** Scandal Management Player Decisions  
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]  
🧭 **CATEGORY:** Management / Crisis Management  
🔑 **KEYWORDS:** crisis, scandal response, locker room, briefing, PR, player decision, management  
📌 **ORIGIN:** Vol 2 Chunk 06 (Scandal Shielding discussion)  
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 06 | 🔒 LOCKED |

---

## Overview

When a scandal hits, management must respond. Players (if Owner/Booker) choose how to handle it. AI management responds based on [[Management Behaviour Tags]].

**Core Truth:** You can't fully control human souls, only try to herd them and manage the consequences.

---

## Scandal Response Flow

| Phase | What Happens |
|-------|--------------|
| 1. **Internal Awareness** | Management finds out (police call, social media post, whisper network) |
| 2. **Emergency Meeting** | Management gathers key locker room leaders (top stars, trusted vets) |
| 3. **Company Line Established** | Management sets "expected reaction": Stay Silent, Defend, Distance, Apologize, No Comment |
| 4. **Worker Decision Point** | Each worker decides internally whether to follow line based on traits |
| 5. **Media Explosion** | Reporters swarm locker room and social media; workers stay on script or go off-book |
| 6. **Fallout Begins** | Locker room fractures, media narrative forms, fans take sides |

---

## Crisis Reaction Stances (Player Options)

When briefing the locker room, management can choose:

| Stance | Description | Short-Term Effect | Long-Term Effect |
|--------|-------------|-------------------|------------------|
| **Stay Silent** | "No comment" across entire locker room | Shields short-term, risks scandal escalation if seen as cowardly | Chain Risk increases if scandal resurfaces |
| **Defend** | Publicly defend the accused figure | Can cause massive backlash if figure proven guilty | Loyal workers love it; principled workers hate it |
| **Distance Softly** | "I can't comment, but I stand for respect and safety" | Safe political stance; neutral media reaction | Neither gains nor loses trust |
| **Be Honest** | Allow workers to say what they feel | Creates immediate chaos, potential heroism | Authentic but unpredictable; may heal faster |
| **Internal Loyalty, External Silence** | Stay loyal inside locker room, silent publicly | Maintains internal unity short-term | Erodes if scandal proves true |

---

## Worker Response to Crisis Briefing

Workers don't automatically follow the company line. Each rolls based on their traits:

### Factors Affecting Worker Compliance

| Factor | Effect |
|--------|--------|
| **Loyalty Tags** | Dirty Loyalty, Company Man = follow the line |
| **Morality Rating** | High morality = may break ranks if scandal is severe |
| **Political Tags** | Political Assassin = follow whichever helps their career |
| **Relationship to Accused** | Friends defend; enemies leak |
| **Whistleblower Tag** | Likely to leak regardless of briefing |
| **Fear of Retaliation** | Union Buster management = workers stay silent out of fear |

### Worker Response Types

| Response Type | Behavior | Consequence |
|---------------|----------|-------------|
| **Compliant** | Follows company line exactly | Maintains unity |
| **Nervous Compliance** | Follows line but clearly uncomfortable | Media notices cracks |
| **Silent Resistance** | Follows line publicly, leaks privately | Chain Risk increases |
| **Open Defiance** | Goes off-script publicly | Immediate crisis within crisis |
| **Hero Move** | Speaks truth, accepts consequences | May become beloved or blacklisted |

---

## Media Response Mechanics

Once workers are briefed and media starts asking:

| Media Scenario | Trigger | Consequence |
|----------------|---------|-------------|
| **United Front** | All workers stay on message | Media suspicious but moves on |
| **Cracks Appear** | Some workers uncomfortable, evasive | Media digs harder |
| **Breaking Ranks** | Worker contradicts company line | Major story, chain event risk |
| **Whistleblower Goes Public** | Worker provides evidence to media | Shield collapse, chain cascade |

---

## Soundbite Dynamics

Management can advise, but workers will respond based on personality:

| Worker Type | Likely Soundbite |
|-------------|------------------|
| **Company Man** | "I trust the company to handle this appropriately" |
| **Dirty Loyalty** | "I've known [accused] for years, this doesn't sound like them" |
| **Principled** | "Everyone deserves due process, but victims deserve to be heard" |
| **Political Assassin** | Whatever damages their rivals most |
| **Whistleblower** | "I've seen things. We need to talk" |
| **Scared Rookie** | "No comment" (visibly nervous) |

---

## Player Agency in Crisis

| Role | Control Level |
|------|---------------|
| **Player is Owner + Booker** | Full control: Choose response stance, brief locker room, make firing decisions |
| **Player is Booker Only** | Partial control: Advise management, handle booking around scandal |
| **AI Management** | Responds based on Management Behaviour Tags |

### Owner + Booker Decision Tree

1. **Scandal breaks internally** (not public yet)
2. **Player chooses:** Fire immediately? Shield? Investigate?
3. **If shielding:** Player briefs locker room with chosen stance
4. **Workers roll response**
5. **Media hits:** Player handles public statements
6. **Fallout calculated**

---

## Consequences by Response Choice

| Choice | If Scandal Proves False | If Scandal Proves True |
|--------|------------------------|------------------------|
| **Fired Immediately** | Wrongful termination backlash; possible lawsuit | Clean break; company credibility intact |
| **Defended Publicly** | Vindication; loyalty cemented | Company branded as enablers; chain risk high |
| **Silent Stance** | Minor suspicion lingers | "You knew and did nothing" narrative |
| **Be Honest** | Chaos but truth wins | Chaos but authenticity respected |
| **Soft Distance** | Neutral outcome | Seen as cowardly fence-sitting |

---

## Locker Room Political Fractures

Scandal responses create faction splits:

| Faction Type | Composition | Behavior |
|--------------|-------------|----------|
| **Defenders** | Friends, allies, beneficiaries of accused | Rally around accused; attack accusers |
| **Accusers** | Victims, enemies, principled workers | Demand action; may leak information |
| **Fence-Sitters** | Most of locker room | Wait to see how wind blows; follow power |
| **Opportunists** | Political workers | Use crisis to advance own position |

---

## Historical Examples

| Case | Management Response | Outcome |
|------|---------------------|---------|
| **Vince/Snuka 1983** | Full cover-up, threats | Decades of silence, eventual exposure |
| **SpeakingOut 2020** | Varied responses by promotion | Quick firings = survived; slow response = damaged |
| **Punk/Cabana 2014** | Silence, legal threats | Podcast goes nuclear, narrative shifts |
| **WWF Steroid Trial** | Deny, deflect, survive | Won legally, reputation damaged permanently |

---

## Connected Systems

- [[Management Behaviour Tags]] - Tags determine AI management response
- [[Scandal Chain Events]] - Crisis response affects chain risk
- [[Star Protection System]] - Shielding mechanics
- [[Fan Loyalty Resistance]] - Fan response to crisis handling
- [[Toxic Worker Consequences]] - What happens if you keep the worker

---

## Implementation Notes

```json
{
  "crisis_response": {
    "scandal_id": "scan_001",
    "management_response": {
      "stance_chosen": "defend",
      "locker_room_briefed": true,
      "worker_compliance": {
        "compliant": 0.45,
        "nervous_compliance": 0.30,
        "silent_resistance": 0.15,
        "open_defiance": 0.05,
        "hero_move": 0.05
      }
    },
    "media_response": "cracks_appear",
    "chain_risk_modifier": 1.25,
    "faction_splits": {
      "defenders": ["worker_001", "worker_002"],
      "accusers": ["worker_003"],
      "fence_sitters": ["worker_004", "worker_005"],
      "opportunists": ["worker_006"]
    }
  }
}
```

---

## Open Questions

- [ ] Exact compliance roll formulas
- [ ] Multiple scandal simultaneous handling?
- [ ] Media relationship mechanics (can you influence coverage?)
- [ ] Worker relationship damage from defending wrong person

---

**Document Status:** Locked (Vol 2 Chunk 06)  
**Last Updated:** 2025-12-26  
**Next Review:** Integrate with Political System faction mechanics
