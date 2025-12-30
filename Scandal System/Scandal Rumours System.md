# Scandal Rumours System

📛 **SYSTEM:** Scandal Rumours
🧭 **CATEGORY:** Scandal System / Pre-Exposure Phase
🔑 **KEYWORDS:** rumours, whispers, gossip, blind items, locker room talk, unverified allegations, scandal shield erosion
📝 **SUMMARY:** Tracks unverified allegations, rumours, and whispers before official scandal exposure. Rumours can be true, exaggerated, or completely false. Simulates how the industry whispers first, and those whispers stain long before truth lands.

⚙️ **LOGIC OVERVIEW:**
- Scandals don't emerge fully formed, they build through whispers
- Rumours can rise, stall, fade, or explode
- False rumours exist (sabotage, misinterpretation, jealousy)
- Rumour saturation weakens scandal shields even without proof

🔬 **LLM INTEGRATION:** Yes (for generating realistic blind items, gossip narratives)

📌 **ORIGIN:** Vol 2 Chunk 09

📎 **CONNECTED SYSTEMS:**
- [[_Scandal System Index|Scandal System]] - Rumours precede full scandal exposure
- [[Star Protection System]] - Shields erode from rumour saturation
- [[Shield Wear Down Over Time]] - How repeated whispers crack protection
- [[Hidden_Personality]] - Loose Lips tag affects rumour spread
- [[_Backstage Politics System Index|Backstage Politics]] - Political enemies may spread rumours

❓ **OPEN QUESTIONS:**
- Exact probability tables for rumour spread
- How long rumours persist before fading
- False rumour detection mechanics

✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 09 | 🔒 LOCKED (Concept) |

---

## Core Concept

**You don't need proof to poison the air. You just need a whisper that doesn't go away.**

Scandals begin as whispers. Sometimes they're smoke before fire. Sometimes they're just smoke thrown by someone with a grudge. Either way, they affect:
- Worker careers
- Locker room dynamics
- Media behaviour
- Sponsor trust
- Fan belief and polarization
- Long-term Shield durability

---

## How Rumours Begin

| Trigger | Chance | Notes |
|---------|--------|-------|
| **Known Bad Behaviour (hidden tag)** | Gradual | Locker room gossip spreads over time |
| **Bad Reputation + High Profile** | Moderate | Media begins sniffing around, tabloid attention |
| **Worker With Loose Lips Tag** | Increased | Secrets leak, even unintentionally |
| **Backstage Heat + Resentment** | Varies | Someone may try to get a rival in trouble |
| **Scandals involving friends/associates** | Low-Moderate | Splashback: "If X did it, what about Y?" |
| **Old scandals with sealed history** | Rare | Occasionally dredged up during career rise or by rival promotions |

---

## Rumour Credibility Levels

| Level | Name | Description | Effects |
|-------|------|-------------|---------|
| **0** | Background Noise | Untracked or hidden history | No visible impact |
| **1** | Locker Room Whispers | Workers may reference it quietly | No public backlash yet |
| **2** | Dirtsheet Blind Items | "A major star in [company] allegedly..." | Appears in newsletters/forums |
| **3** | Industry Speculation | Workers distancing themselves | Some fans demanding action, company in damage control |
| **4** | Imminent Exposure | Journalists have sources | Worker may be suspended quietly, Shield heavily weakened |
| **5** | Public Scandal Hits | Truth or perception bursts into public | Full scandal system activates |

### Level Progression

```
Level 0 → 1: Internal pressure (locker room talk)
Level 1 → 2: Someone talks to media
Level 2 → 3: Multiple sources, pattern emerges
Level 3 → 4: Journalists investigating, sources going on record
Level 4 → 5: Story breaks publicly
```

### Level Regression

- Rumours can **stall** if no new evidence emerges
- Rumours can **fade** over time if not reinforced
- Worker changing companies may reset visibility (but not truth)

---

## Effects of Rumours by Level

| Effect Area | Level 1-2 | Level 3-4 | Level 5 |
|-------------|-----------|-----------|---------|
| **Locker Room Morale** | Tension, factionalism | Workers actively distancing | Chaos, picking sides |
| **Promotion Image** | Slight drop (smart fanbases) | Moderate damage | Depends on response |
| **Media Pressure** | Minimal | Journalists digging | Full coverage |
| **Sponsors** | None | May quietly pull back | Demand action or leave |
| **Fan Reaction** | Hardcore loyalists unaware | Divided, polarized | Full spectrum |
| **Scandal Shield** | Slight erosion | Heavy erosion | Tested at full damage |
| **Cascading Risk** | Low | Moderate (others may speak up) | High (floodgates open) |

---

## False Rumour Potential

**Not all rumours are true.**

### False Rumour Sources

| Source | Motivation | Detection Difficulty |
|--------|-----------|---------------------|
| **Sabotage** | Political enemy spreading lies | Moderate |
| **Misinterpretation** | Innocent action misconstrued | Low |
| **Mistaken identity** | Wrong person blamed | Low-Moderate |
| **Jealous workers** | Petty backstage grudges | Moderate |
| **Projection from past** | "They did it before, probably doing it now" | High |

### False Rumour Outcomes

| Outcome | Effect |
|---------|--------|
| **Dies Quietly** | Fans forget, slight reputational residue may linger |
| **Proven False Publicly** | Company gains sympathy boost, accused worker gets minor popularity spike or "Vindicated" tag |
| **Lingers Unconfirmed** | Ongoing reputation damage: "Where there's smoke..." |

### The Dark Truth

Sometimes the accused is guilty but the scandal **never breaks** and it stays as a whisper for years. Just like real life.

---

## Promotion Response Options

When rumours reach Level 3+:

| Response | Effect | Risk |
|----------|--------|------|
| **Ignore** | May fade, may explode | Looks bad if scandal breaks |
| **Internal Investigation** | Buys time, shows action | May confirm rumours |
| **Quiet Suspension** | Reduces visibility | Media notices |
| **Public Statement** | Controls narrative | Draws more attention |
| **Fire Worker** | Decisive, may end story | May be premature, legal risk |

### Promotion Tags Affecting Response

| Tag | Effect |
|-----|--------|
| **Dirty Cover-Up** | Company known for protecting stars, media more aggressive |
| **Whistleblower Friendly** | Workers feel safe speaking up, scandals surface faster |
| **Old Boys Club** | Rumours suppressed longer, but explode bigger when they break |

---

## Worker Tags Affecting Spread

| Tag | Effect on Rumour System |
|-----|------------------------|
| **Loose Lips** | Increases chance of rumours surfacing (unintentional exposure) |
| **Dirtsheet Gossip** | Deliberate leaks to media (targeted exposure) |
| **Trustworthy** | Less likely to be source of leaks |
| **Political Animal** | May weaponize rumours against rivals |

---

## Interactions with Other Systems

### Scandal Shield System

```
if rumour_level >= 2:
    shield_integrity -= 5 per month  # Erosion even without proof
    
if rumour_level >= 4:
    shield_integrity -= 15  # Heavy damage from imminent exposure
```

### Mental Health System

```
if target_worker.rumour_level >= 3:
    mental_health -= 5  # Stress of being under suspicion
    
if rumour_proven_false:
    mental_health += 3  # Relief, vindication
```

---

## Historical Examples

| Person | Rumour Level Reached | Outcome |
|--------|---------------------|---------|
| Jerry Lawler (pre-arrest) | Level 3-4 | Industry knew, fans suspected |
| Ric Flair (various) | Level 2-3 (multiple) | Stories circulated for decades |
| CM Punk (various beefs) | Level 3-4 | Dirtsheets covered extensively |
| Benoit (concussions) | Level 1-2 | Whispers about behavior before tragedy |

---

## Implementation Notes

```json
{
  "rumour_id": "rumour_001",
  "target_worker_id": "worker_045",
  "scandal_type": "substance_abuse",
  "credibility_level": 2,
  "sources": ["locker_room", "former_partner"],
  "true_or_false": "true",
  "months_active": 4,
  "shield_erosion_total": 12,
  "progression_blocked_by": null,
  "associated_events": []
}
```

---

## Connected Mechanics

- [[Scandal Types]] - What kinds of scandals start as rumours
- [[Star Protection System]] - How shields interact with rumours
- [[Shield Wear Down Over Time]] - Cumulative erosion mechanics
- [[Crisis Response System]] - How promotions handle rumour escalation
- [[Era-Based Response]] - Different eras handle rumours differently

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-26
**Next Review:** Define probability tables and timeline mechanics
