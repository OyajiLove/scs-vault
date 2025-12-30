# Manager Types

📛 **MECHANIC:** Manager Role Classifications
🔗 **PARENT SYSTEM:** [[_Manager System Index|Manager System]]
🧭 **CATEGORY:** Booking / Roster
🔑 **KEYWORDS:** mouthpiece, valet, heat magnet, advocate, stable leader
📌 **ORIGIN:** Vol 1-4 (Manager Tags, Non-Wrestler Roles)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Managers serve different functions depending on their skills, personality, and the needs of their clients. Some are pure mouthpieces covering for non-talkers, others generate heat through their own performance, and some lead entire stables as strategic masterminds. Understanding manager types helps match them to appropriate clients.

---

## Primary Manager Types

### Mouthpiece

| Aspect | Description |
|--------|-------------|
| **Function** | Speaks for wrestlers who lack promo ability |
| **Key Skill** | Microphone, Charisma |
| **Client Type** | Strong workers, weak talkers |
| **Example** | Jimmy Hart, Paul Ellering |
| **Era Usage** | All eras, essential role |

### Heat Magnet

| Aspect | Description |
|--------|-------------|
| **Function** | Draws heel heat, takes bumps, gets comeuppance |
| **Key Skill** | Entertainment, Selling, Charisma |
| **Client Type** | Heel workers needing extra heat |
| **Example** | Bobby Heenan, Jim Cornette |
| **Era Usage** | Territory through Attitude, declining modern |

### Valet

| Aspect | Description |
|--------|-------------|
| **Function** | Adds visual appeal, distraction spots |
| **Key Skill** | Looks, Presence, Character |
| **Client Type** | Singles or tag teams needing presentation boost |
| **Example** | Miss Elizabeth, Sunny, Lana |
| **Era Usage** | All eras, presentation varies |

### Stable Leader

| Aspect | Description |
|--------|-------------|
| **Function** | Leads faction, strategic mastermind |
| **Key Skill** | Promo, Psychology, Booking Mind |
| **Client Type** | Multiple workers in faction |
| **Example** | Paul Heyman (ECW), Raven (Flock) |
| **Era Usage** | 90s peak, still viable |

### Advocate

| Aspect | Description |
|--------|-------------|
| **Function** | Speaks for special attraction, elevates aura |
| **Key Skill** | Microphone, Presence, Credibility |
| **Client Type** | Part-time stars, special attractions |
| **Example** | Heyman for Lesnar, DiBiase for Virgil |
| **Era Usage** | Modern, sporadic appearances |

### Cornerman/Second

| Aspect | Description |
|--------|-------------|
| **Function** | Minimal speaking, physical presence, backup |
| **Key Skill** | Intimidation, Loyalty, Interference |
| **Client Type** | Workers who can talk but need backup |
| **Example** | Various unnamed seconds |
| **Era Usage** | Territory, Japan, MMA-influenced |

---

## Secondary Manager Roles

| Role | Description | Example |
|------|-------------|---------|
| **Translator** | Speaks for foreign talent | Various throughout history |
| **Authority Proxy** | Represents ownership on screen | Shane McMahon (early) |
| **Mentor Figure** | Wise elder guiding young talent | Various |
| **Cheerleader** | Enthusiastic supporter, minimal interference | Some valets |
| **Heel Valet** | Interferes, distracts, betrays | Sherri, Francine |

---

## Manager Skill Set

| Skill | Description | Importance |
|-------|-------------|------------|
| **Microphone** | Speaking ability | Critical for mouthpieces |
| **Charisma** | Natural magnetism | Universal importance |
| **Heat Generation** | Ability to draw boos | Key for heel managers |
| **Interference** | Match manipulation skill | For active managers |
| **Psychology** | Understanding story beats | For stable leaders |
| **Bump Taking** | Willingness to take hits | For heat magnets |
| **Presence** | Commanding attention | For advocates |

---

## Manager Type by Era

| Era | Dominant Types | Notes |
|-----|----------------|-------|
| **Territory** | Mouthpiece, Heat Magnet | Managers essential, lots of bumping |
| **80s National** | All types flourished | Golden age of managers |
| **Attitude Era** | Stable Leader, Authority | Faction-heavy, less traditional |
| **Ruthless Aggression** | Declining usage | Writers replaced need |
| **Modern** | Advocate, occasional Mouthpiece | Limited but high-profile |

---

## Type Combinations

Managers can embody multiple types:

| Combination | Description | Example |
|-------------|-------------|---------|
| **Mouthpiece + Heat Magnet** | Talks AND bumps | Bobby Heenan |
| **Valet + Heat Magnet** | Attractive AND generates heat | Sherri |
| **Stable Leader + Advocate** | Leads group AND speaks | Heyman |
| **Cornerman + Mouthpiece** | Physical AND verbal | Rare combo |

---

## Type Effectiveness

| Type | Best For |
|------|----------|
| **Mouthpiece** | Great workers who can't talk |
| **Heat Magnet** | Monsters who need interaction |
| **Valet** | Presentation-focused acts |
| **Stable Leader** | Multi-person groups |
| **Advocate** | Part-timers, special attractions |
| **Cornerman** | MMA-style, realistic presentation |

---

## Connected Mechanics

- [[Manager-Client Relationships]] - How types affect bonding
- [[Manager Match Impact]] - Type determines interference style
- [[Promo System]] - Mouthpiece mechanics
- [[Faction System]] - Stable Leader integration

---

## Open Questions

- [ ] How to quantify type effectiveness
- [ ] Type evolution during career
- [ ] Multiple manager types for one client
- [ ] Manager type impact on match rating

---

## Implementation Notes

```json
{
  "manager_type": {
    "manager_id": "manager_001",
    "primary_type": "heat_magnet",
    "secondary_type": "mouthpiece",
    "skills": {
      "microphone": 92,
      "charisma": 88,
      "heat_generation": 95,
      "interference": 80,
      "bump_taking": 75
    },
    "effectiveness_by_client_type": {
      "monster_heel": 0.95,
      "technical_face": 0.60,
      "tag_team": 0.85
    }
  }
}
```
