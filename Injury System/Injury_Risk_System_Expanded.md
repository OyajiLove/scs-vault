# Injury Risk System (Expanded)

📛 **NAME:** Injury Risk System (Expanded)
🧭 **CATEGORY:** Health System / Injury System
🔑 **KEYWORDS:** durability, bad luck, fatigue, wrestling style, promotion intensity, injury rolls, career health
📝 **SUMMARY:** Comprehensive injury probability system incorporating durability, bad luck tags, fatigue, wrestling style, promotion culture intensity, and substance abuse. Not just "who gets hurt" but "why careers break."

⚙️ **LOGIC OVERVIEW:**
- Every active worker rolls against injury thresholds quarterly/monthly
- Multiple modifiers stack to create final injury risk
- Durability stat provides base protection
- Bad Luck tag allows freak accidents regardless of other factors
- Wrestling style, promotion intensity, and lifestyle all contribute
- Injuries range from Minor (1-2 months) to Catastrophic (career-ending)

🔬 **LLM INTEGRATION:** Minimal (calculation system)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Worker Skills]] (Durability stat)
- [[Tags System]] (Bad Luck, lifestyle tags)
- [[Promotion Identity]] (intensity culture)
- [[Match Engine]] (style risk per match)
- [[Alt-History Mode]] (organic vs scripted injuries)

❓ **OPEN QUESTIONS:**
- Exact percentage values for each modifier need playtesting
- Should mental health affect injury risk? (depression → riskier behavior)
- How does aging interact with base injury chance?

✅ **STATUS:** Locked

---

## Core Injury Roll Flow

```
[Quarter/Month Begins]
       ↓
[Is Worker Actively Wrestling?]
       → No → Skip Roll (unless freak accident triggered)
       → Yes → Proceed
       ↓
[Calculate Base Injury Risk]
       ↓
[Apply All Modifiers]
       + Fatigue Multiplier
       + Wrestling Style Risk
       + Promotion Intensity Risk
       + Substance Abuse Risk
       - Durability Modifier
       + Bad Luck Modifier
       + Age Modifier
       ↓
[Final Injury Roll]
       ↓
[Roll Succeeds?]
       → Yes → Injury Severity Check
       → No → Continue (slight wear accumulation)
```

---

## Risk Modifiers

### Durability Stat

| Durability Level | Effect |
|------------------|--------|
| Very High (18-20) | -20% to -30% injury risk |
| High (14-17) | -10% to -15% injury risk |
| Medium (10-13) | No modifier |
| Low (6-9) | +10% to +15% injury risk |
| Very Low (1-5) | +20% to +30% injury risk |

### Bad Luck Tag ("Harbinger of Misfortune")

| Status | Effect |
|--------|--------|
| No Bad Luck | Normal risk only |
| Has Bad Luck | +Flat chance of freak accidents regardless of other factors |

**Philosophy:** Even if Durability is high, Bad Luck tag increases freak accident chance dramatically. It's not fair. It's not mechanical. It's life.

### Fatigue (Short-Term Burnout)

| Fatigue Level | Effect |
|---------------|--------|
| Well-Rested | -5% injury risk |
| Normal | No modifier |
| Fatigued | +10% to +15% injury risk |
| Overworked | +20% to +30% injury risk |
| Burnout | +30% to +40% injury risk |

### Wrestling Style Risk

| Style | Baseline Risk |
|-------|---------------|
| Safe/Protective (80s WWF main event style) | +0% to +5% |
| Technical/Mat-Based | +5% to +10% |
| Brawling/Hardcore | +15% to +20% |
| High-Flying/Lucha | +15% to +25% |
| Strong Style/King's Road | +20% to +30% |
| Deathmatch/Garbage | +25% to +40% |

### Promotion Intensity Culture

| Culture | Effect |
|---------|--------|
| Wellness/Protective (Modern WWE) | -10% to -20% injury risk |
| Standard (Most major promotions) | No modifier |
| Demanding (NJPW main event scene) | +10% to +15% injury risk |
| King's Road Era (90s AJPW) | +25% to +30% injury risk |
| Outlaw/No Regulation | +20% to +35% injury risk |

### Substance Abuse

| Level | Effect |
|-------|--------|
| Clean | No modifier |
| Recreational | +5% to +10% injury risk |
| Regular User | +15% to +20% injury risk |
| Heavy Abuse | +25% to +40% injury risk |
| Addiction Crisis | +40%+ injury risk, freak collapse possible |

### Age Modifier

| Age Range | Effect |
|-----------|--------|
| Under 25 | -5% (young resilience) |
| 25-30 | No modifier |
| 31-35 | +5% to +10% |
| 36-40 | +15% to +20% |
| 41-45 | +25% to +30% |
| 46+ | +35%+ (senior circuit risk) |

---

## Injury Severity Levels

| Level | Duration | Career Impact |
|-------|----------|---------------|
| Minor | 1-2 months | None |
| Moderate | 3-6 months | Slight decline possible |
| Major | 6-12 months | Career threatening, style change possible |
| Catastrophic | Career-ending | Forced retirement or severe limitation |

### Severity Roll Modifiers

- Bad Luck tag increases catastrophic injury chance
- High durability reduces severity even when injured
- Age increases severity outcomes
- Repeated injuries in same body part compound severity

---

## Real-World Examples

| Worker | Durability | Bad Luck | Factors | Outcome |
|--------|------------|----------|---------|---------|
| Stan Hansen | High | No | Brawling (safer than deathmatch) | Long career despite physicality |
| Kenta Kobashi | High | No | King's Road 90s intensity | Knees/back collapse, still long career |
| Hayabusa | Medium | Yes | High-risk high flyer | Severe early career injury (SSP botch) |
| Nick Gage | Low | No | Deathmatch + substance abuse | Brutal cumulative breakdowns |
| Dynamite Kid | Low | No | Insane bump schedule | Rapid collapse, wheelchair by early 90s |
| Magnum TA | High | Freak Event | Car crash (random) | Career-ending despite durability |

---

## Freak Accident System

Separate from regular injury rolls, workers with Bad Luck tag roll for rare catastrophic events:

| Event Type | Examples |
|------------|----------|
| Vehicle Accidents | Pillman, Magnum TA |
| Illness/Disease | Jumbo Tsuruta hepatitis |
| Overdose/Collapse | Various |
| In-Ring Freak Injury | Hayabusa SSP, Shibata headbutt |
| Backstage Accident | Falls, equipment failure |

These bypass normal durability protection.

---

## Implementation Notes

### Data Structure

```json
{
  "worker_id": "brian_pillman",
  "durability": 8,
  "bad_luck_tag": true,
  "current_fatigue": "fatigued",
  "wrestling_style_risk": 20,
  "promotion_intensity": 15,
  "substance_abuse_level": "regular_user",
  "age": 35,
  "accumulated_wear": 45
}
```

### Roll Calculation

```
base_risk = 10
fatigue_mod = fatigue_modifier_table[current_fatigue]
style_mod = wrestling_style_risk
promo_mod = promotion_intensity
substance_mod = substance_modifier_table[substance_abuse_level]
durability_mod = (10 - durability) * 2
age_mod = age_modifier_table[age_bracket]

total_risk = base_risk + fatigue_mod + style_mod + promo_mod + substance_mod + durability_mod + age_mod

roll = random(1, 100)
IF roll <= total_risk:
    determine_severity()
    apply_injury()
```

---

## RELATED SYSTEMS

- **[[Worker Skills]]:** Durability stat definition
- **[[Tags System]]:** Bad Luck and lifestyle tags
- **[[Promotion Identity]]:** Culture intensity
- **[[Alt-History Mode]]:** Organic vs scripted injuries
- **[[Aging System]]:** Age-related risk increases

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Playtest modifier percentages, balance freak accident frequency
