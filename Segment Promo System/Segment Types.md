# Segment Types

📛 **MECHANIC:** Segment Types
🔗 **PARENT SYSTEM:** [[_Segment Promo Index|Segment & Promo System]]
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** segment types, promo, interview, ambush, contract signing, return, debut, retirement
📌 **ORIGIN:** Vol 2-3 (Booking Engine Phase 3)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2-3 | 🔒 LOCKED |

---

## Overview

Non-wrestling content that builds feuds and characters. Uses the same evaluation framework as matches: Intent, Tone, Placement, Fan Expectations, Execution Quality. Can be attached to matches or run standalone.

---

## Segment Categories

| Category | Purpose | Risk Level |
|----------|---------|------------|
| **Promo** | Character/feud development through speech | Medium |
| **Physical** | Action without official match | High |
| **Ceremony** | Ritual/emotional moments | Low-Medium |
| **Surprise** | Unexpected events | Variable |
| **Media** | Fourth-wall or press elements | Medium |

---

## Promo Segments

| Type | Description | Key Variables |
|------|-------------|---------------|
| **In-Ring Promo (Solo)** | Single worker addresses crowd | Mic skills, character work, crowd mood |
| **In-Ring Promo (Confrontation)** | Two+ workers face off verbally | Chemistry, heat, escalation potential |
| **Backstage Interview** | Controlled environment, interviewer present | Character consistency, soundbite potential |
| **Pre-Taped Promo** | Edited, produced content | Production value, authenticity feel |
| **Shoot-Style Promo** | Fourth-wall breaking, "real" feel | Risk/reward, crowd sophistication |

---

## Physical Segments

| Type | Description | Key Variables |
|------|-------------|---------------|
| **Ambush/Beatdown** | Surprise attack on worker | Timing, victim sympathy, attacker heat |
| **Brawl** | Mutual combat without match structure | Intensity, crowd investment |
| **Run-In** | Interference in ongoing segment | Surprise factor, logic of involvement |
| **Locker Room Fight** | Backstage violence | Chaos feel, injury risk |
| **Parking Lot Attack** | Outside venue violence | "Real" feel, serious tone |

---

## Ceremony Segments

| Type | Description | Key Variables |
|------|-------------|---------------|
| **Contract Signing** | Build tension before brawl | Inevitability, table spot timing |
| **Title Presentation** | New champion crowned | Prestige, crowd investment |
| **Retirement Speech** | Career send-off | [[Legacy Tracker/_Legacy Tracker Index|Legacy]], emotional resonance |
| **Hall of Fame Induction** | [[Hall of Fame/_Hall of Fame Index|HOF]] ceremony | Earned vs forced, speech quality |
| **Mask Retirement** | Lucha sacred ceremony | Cultural weight, tradition respect |
| **Wedding/Funeral** | Kayfabe life events | Soap opera risk, crowd patience |

---

## Surprise Segments

| Type | Description | Key Variables |
|------|-------------|---------------|
| **Return** | Worker back from absence | Absence length, pop potential |
| **Debut** | New worker introduction | Build/cold debut, presentation |
| **Invasion** | Outside promotion attacks | Shock value, roster implications |
| **Shock Turn** | Unexpected alignment change | Setup (or lack thereof), victim |
| **Title Change** | Unexpected belt switch | Stakes, believability |

---

## Media Segments

| Type | Description | Key Variables |
|------|-------------|---------------|
| **Press Conference** | Kayfabe media interaction | Shoot elements, controversy |
| **Talk Show** | In-ring interview segment | Host character, guest chemistry |
| **Documentary Style** | Produced biographical content | Authenticity, emotional depth |
| **Social Media** | Modern era digital content | Virality potential, era-locked |

---

## Segment Type → Best Skills Mapping (#136)

📌 **Source:** Vol 1 Extraction #136

| Type | Purpose | Best Skills |
|------|---------|-------------|
| **Challenge Promo** | Demand match, build heat | Charisma, Menace |
| **Emotional Promo** | Connect with fans, tell story | Believability, Resonance |
| **Comedy Segment** | Entertainment, character showcase | Charisma, Timing |
| **Interview** | Exposition, storyline advancement | Fluency, Poise |
| **Confrontation** | Physical + verbal, build stakes | Menace, Presence |
| **Contract Signing** | Tension building, table spot setup | Psychology |

### Segment Quality Formula (Conceptual)

```
Quality = (Skill Match × Gimmick Fit) + Stakes Bonus + Chemistry Modifier
```

---

## Segment Placement

| Placement | Effect |
|-----------|--------|
| **Show Open** | Sets tone, hooks audience |
| **Pre-Match** | Builds anticipation for match |
| **Post-Match** | Extends story, sets up future |
| **Mid-Show Break** | Palate cleanser or angle seed |
| **Main Event Slot** | Maximum attention, high stakes |
| **Dark Segment** | House show only, not aired |

---

## Segment Inputs

Same as match booking:

| Input | Description |
|-------|-------------|
| **Intent** | What should this accomplish? |
| **Tone** | Serious, comedic, chaotic, emotional? |
| **Placement** | Where in show? |
| **Fan Expectations** | What does crowd anticipate? |
| **Execution Quality** | How well was it performed? |

---

## Connected Mechanics

- [[Promo Evaluation]] - quality assessment
- [[Promo Response]] - crowd reaction mechanics
- [[Segment Outcomes]] - effects on systems
- [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] - chant integration

---

## Open Questions

- Segment length optimization
- Multiple segment chains (angle across show)
- Dark segment vs aired segment rules

---

## Implementation Notes

```json
{
  "segment": {
    "segment_id": "seg_001",
    "type": "in_ring_promo_confrontation",
    "category": "promo",
    "participants": ["w_001", "w_002"],
    "placement": "show_open",
    "intent": "feud_escalation",
    "tone": "heated",
    "duration_minutes": 8,
    "attached_to_match": null,
    "era": "2000s",
    "region": "us"
  }
}
```
