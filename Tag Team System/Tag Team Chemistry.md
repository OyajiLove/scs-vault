# Tag Team Chemistry System

📛 **MECHANIC:** Partner Synergy & Team Quality
🔗 **PARENT SYSTEM:** Tag Team System
🧭 **CATEGORY:** Match Performance / Team Dynamics
🔑 **KEYWORDS:** tag team, chemistry, synergy, team skill, partner compatibility
📌 **ORIGIN:** Vol 1 Extraction #106
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 Extraction #106 | 🔒 LOCKED |

---

## Overview

Tag teams need more than just two good singles workers. Chemistry, timing, and team-specific skills determine whether a pairing succeeds or fails. Some workers have natural synergy; others are disasters together regardless of individual talent.

---

## CHEMISTRY LEVELS (#106)

| Chemistry Level | Match Quality Modifier | Description |
|-----------------|----------------------|-------------|
| **Dream Team** | +25% | Perfect synergy, innovative double teams, telepathic timing |
| **Good Chemistry** | +10% | Solid partnership, reliable coordination |
| **Professional** | Baseline | Competent but unremarkable teaming |
| **Awkward** | -10% | Visible disconnect, mistimed spots |
| **Disaster** | -25% | Should not be teamed, actively harmful |

**Example Applications:**
- Dream Team: Road Warriors, Steiner Brothers at peak
- Good Chemistry: Most functional tag teams
- Professional: Thrown-together teams, serviceable
- Awkward: Mismatched styles or personalities
- Disaster: Oil and water, active friction visible in ring

---

## TAG TEAM SKILL

Separate skill stat measuring tag-specific abilities:

| Component | Description |
|-----------|-------------|
| **Timing** | Synchronization on saves, double teams |
| **Communication** | Reading partner's position and needs |
| **Team Moves** | Double team execution quality |
| **Save Instinct** | Breaking up pins at the right moment |
| **Hot Tag Rhythm** | Building to and delivering hot tags |

### Tag Team Skill Range

| Level | Description |
|-------|-------------|
| 1-5 | Singles specialist, awkward in teams |
| 6-10 | Functional tag worker |
| 11-15 | Good tag team skills |
| 16-18 | Tag team specialist |
| 19-20 | Elite tag team worker |

---

## TEAM HISTORY & SYNERGY BUILDING

Long-term teams develop synergy over time:

| Time Together | Synergy Bonus |
|---------------|---------------|
| 0-3 months | No bonus |
| 3-6 months | +2% chemistry |
| 6-12 months | +5% chemistry |
| 1-2 years | +8% chemistry |
| 2-5 years | +10% chemistry |
| 5+ years | +12% chemistry (cap) |

**Chemistry Cap:** Even long-term teams can't exceed their base chemistry potential.
- Disaster teams can improve to Awkward at best
- Awkward teams can reach Professional
- Professional teams can become Good Chemistry
- Good Chemistry teams can become Dream Teams (rare)

---

## CHEMISTRY COMPATIBILITY FACTORS

### Positive Factors

| Factor | Chemistry Boost |
|--------|-----------------|
| **Similar Style** | +5-10% |
| **Complementary Styles** (power + speed) | +10-15% |
| **Same Training Background** | +5% |
| **Personal Friendship** (backstage) | +10% |
| **Shared Philosophy** | +5% |

### Negative Factors

| Factor | Chemistry Penalty |
|--------|-------------------|
| **Ego Clash** | -10-20% |
| **Style Conflict** | -5-15% |
| **Personal Animosity** | -15-25% |
| **Communication Issues** | -10% |
| **One Refusing to Sell** | -20% |

---

## ICONIC TEAM ARCHETYPES

### The Matched Pair
Both workers similar style, mirrored offense.
- Examples: Hart Foundation (original), British Bulldogs
- Chemistry: High baseline

### The Powerhouse/Cruiser
Classic big man + speedster combo.
- Examples: Owen & Yoko, Luger & Sting
- Chemistry: Moderate baseline, can go high

### The Odd Couple
Contrasting personalities, unexpected synergy.
- Examples: Edge & Christian (early), Beer Money
- Chemistry: Variable, either great or disaster

### The Natural Team
Trained together, career-long partnership.
- Examples: Road Warriors, Steiners
- Chemistry: Very high ceiling

---

## CONNECTED MECHANICS

- [[Package Deal System]] - Inseparable team dynamics
- [[Relationship System]] - Backstage chemistry affects in-ring
- [[Match Engine/Tag Match Types|Tag Match Types]] - Match structure for teams
- [[Morale System]] - Team success/failure affects morale

---

## IMPLEMENTATION NOTES

```json
{
  "tag_team": {
    "team_id": "team_001",
    "members": ["worker_001", "worker_002"],
    "name": "The Dream Duo",
    "formation_date": "1985-03-15",
    "chemistry": {
      "base_level": "good_chemistry",
      "modifier": 0.10,
      "synergy_bonus": 0.05,
      "total_modifier": 0.15
    },
    "team_skill_average": 14,
    "signature_moves": ["double_suplex", "doomsday_device"],
    "time_together_months": 8,
    "matches_as_team": 47
  }
}
```

---

## OPEN QUESTIONS

- [ ] Exact chemistry calculation formula
- [ ] Can chemistry degrade from poor booking?
- [ ] Three-man team chemistry mechanics
- [ ] Freebird Rule effects on chemistry
- [ ] How does manager affect team chemistry?

---

**Document Status:** Locked
**Last Updated:** 2025-12-25
