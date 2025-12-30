# Shoot Fighting Ability

📛 **MECHANIC:** Backstage Physical Presence
🔗 **PARENT SYSTEM:** [[_Backstage Politics System Index|Backstage Politics System]]
🧭 **CATEGORY:** Hidden Stats / Locker Room Dynamics
🔑 **KEYWORDS:** shoot, fighting, backstage, respect, intimidation, brawl, toughness
📌 **ORIGIN:** Vol 1 Extraction #171
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

Shoot Fighting Ability is a separate backstage attribute distinct from kayfabe Physical stats. It represents a worker's actual fighting ability, not their in-ring performance. This affects locker room dynamics, backstage incidents, and the "no one messes with him" reputation that protects certain workers.

**Key Distinction:** Haku could rip your face off but wasn't a cardio machine in ring. Bart Gunn won Brawl for All but was nothing special in kayfabe.

---

## Backstage Physical Attributes

| Stat | What It Captures |
|------|------------------|
| **Shoot Fighting Ability** | Actual ability to scrap if chaos breaks out |
| **Locker Room Presence** | Level of respect/fear/admiration from peers |
| **Temperament** | Likelihood to start fights, hold grudges |
| **Professionalism** | Willingness to work safely, show up, play ball |

---

## Why It's Separate from Ring Stats

Ring work is performance. Backstage physicality is real:

| Scenario | Ring Stats Irrelevant |
|----------|----------------------|
| Bar fight breaks out | Stamina for 20-min match doesn't help |
| Worker tries to shoot in ring | Technical wrestling ≠ combat |
| Backstage confrontation | Charisma doesn't stop a punch |
| Hazing situation | High-flyer skills won't help |

---

## Shoot Fighting Triggers

When does this stat matter:

| Trigger | Effect |
|---------|--------|
| **Brawl for All type events** | Determines outcome of shoots |
| **Breaking up backstage fights** | Strong scrapper = stops faster |
| **"No one messes with him" rep** | Protects from bullying/burial |
| **Worker intimidation angles** | Real fear enhances stories |
| **Locker room disputes** | Affects resolution and consequences |
| **Hazing situations** | Targets and responders |

---

## Locker Room Protection

High shoot ability provides informal protection:

| Protection Level | Description |
|------------------|-------------|
| **Untouchable** | No one dares cross them (Haku, Meng) |
| **Respected** | Others think twice before starting conflict |
| **Normal** | Standard locker room dynamics apply |
| **Vulnerable** | May be targeted by bullies |
| **Easy Mark** | Likely to be hazed, politicked against |

---

## Temperament Interaction

| Temperament | Shoot Ability Impact |
|-------------|---------------------|
| **Hot-headed + High Shoot** | Dangerous, may cause incidents |
| **Hot-headed + Low Shoot** | Causes trouble but gets beaten |
| **Calm + High Shoot** | Respected peacekeeper |
| **Calm + Low Shoot** | Avoids conflict, manages politically |

---

## Historical Examples

| Worker | Shoot Rating | Notes |
|--------|--------------|-------|
| **Haku/Meng** | Legendary | Known for extreme real-life toughness |
| **Danny Hodge** | Legendary | Legitimate wrestler, could crush apples |
| **Ken Shamrock** | Very High | MMA background, legitimate fighter |
| **Bart Gunn** | High | Brawl for All winner, not main event |
| **Most workers** | Average | Can handle themselves, nothing special |
| **Brian Pillman** | Above Average | Scrappy, not afraid of anyone |
| **Shawn Michaels (early)** | Low | Got in trouble, couldn't back it up |

---

## The Brawl for All Problem

Shoot ability exposed in unworked situations:

| Reality Check | What We Learned |
|---------------|-----------------|
| Worked wrestling ≠ Fighting | Best workers not best fighters |
| Size matters less | Technique and toughness prevail |
| Legitimacy questions | "Tough guy" gimmicks tested |
| Career consequences | Butterbean vs. Bart Gunn |

---

## Connected Mechanics

- [[Hidden_Personality|Hidden Personality]] - Temperament affects when shoot matters
- [[Clique Formation]] - Tough guys protect each other
- [[Power Struggle Events]] - Physical intimidation as political tool
- [[Morale System]] - Fear/respect affects morale dynamics

---

## Open Questions

- [ ] How shoot ability is revealed to player
- [ ] Shoot ability decline with age
- [ ] Training options to improve shoot ability
- [ ] Era variations (territory toughness vs. modern professionalism)

---

## Implementation Notes

```json
{
  "backstage_physical": {
    "worker_id": "worker_haku",
    "shoot_fighting": 98,
    "locker_room_presence": 95,
    "temperament": "calm_dangerous",
    "professionalism": 75,
    "reputation_tags": ["untouchable", "peacekeeper"],
    "incident_history": [
      { "date": "1989-03-15", "type": "defended_colleague", "outcome": "decisive_victory" }
    ]
  }
}
```

---

**Document Status:** Locked (Vol 1)
**Last Updated:** 2025-12-24
**Next Review:** Design shoot ability visibility mechanics
