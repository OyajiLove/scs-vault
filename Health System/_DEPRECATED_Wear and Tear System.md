# Wear and Tear System

📛 **MECHANIC:** Wear and Tear Evolution / Cumulative Damage
🔗 **PARENT SYSTEM:** [[_Health System Index|Health System]]
🧭 **CATEGORY:** Career Longevity / Injury Tracking
🔑 **KEYWORDS:** wear, tear, cumulative damage, body parts, chronic injury, career ending
📌 **ORIGIN:** Vol 1 Extraction #163-176
✅ **STATUS:** Conceptual

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 📝 Conceptual |

---

## Overview

Beyond acute injuries (broken bones, torn muscles), workers accumulate invisible damage over their careers. The Wear and Tear System tracks this cumulative damage by body region, eventually leading to chronic conditions, style changes, and career-ending situations.

---

## Body Region Tracking

### Tracked Regions

| Region | Common Damage Sources |
|--------|----------------------|
| **Head/Neck** | Bumps, strikes, piledrivers, chairshots |
| **Back** | Bumps, power moves, lifting |
| **Knees** | Running, jumping, submissions |
| **Shoulders** | Bumps, arm work, throws |
| **Hips** | Bumps, age, power moves |
| **Elbows** | Strikes, hyperextension |
| **Ankles** | Running, top rope, submissions |
| **Hands/Wrists** | Strikes, catches |

### Damage Accumulation

| Activity | Damage Added |
|----------|--------------|
| Standard match (10-15 min) | +1-2 to relevant regions |
| Long match (20+ min) | +3-5 to relevant regions |
| Stiff match | +2-4 additional |
| Deathmatch | +5-10 to multiple regions |
| High spot heavy | +3-5 to back/knees |
| Submission heavy | +2-3 to targeted limbs |

---

## Damage Thresholds

### Per Body Region (0-100 scale)

| Range | Status | Effect |
|-------|--------|--------|
| 0-20 | Healthy | No effect |
| 21-40 | Minor Wear | Occasional discomfort flag |
| 41-60 | Moderate Wear | Style limitations emerging |
| 61-80 | Significant Wear | Chronic issues, stat penalties |
| 81-90 | Severe Wear | Major style changes required |
| 91-100 | Critical | Career-threatening, surgery needed |

---

## Wear Effects on Wrestling

### Style Adaptation Requirements

| Region Damaged | Forced Changes |
|----------------|----------------|
| Knees (60+) | Reduce aerial moves, running |
| Back (60+) | Avoid power moves, limit bumps |
| Neck (60+) | No piledrivers, careful bumps |
| Shoulders (60+) | Modify throws, protect arm |

### Stat Degradation

| Region | Stats Affected |
|--------|----------------|
| Knees | Agility, Aerial, Speed |
| Back | Power, Stamina, Bumping |
| Neck | All (severe cases), Psychology |
| Shoulders | Power, Technical |
| Head | Focus, Consistency, Psychology |

---

## Medical Exam Triggers (#163)

### Automatic Triggers

| Event | Exam Type |
|-------|-----------|
| Post-major injury | Mandatory recovery check |
| Pre-contract signing | Physical evaluation |
| Post-tournament | Cumulative damage assessment |
| Worker request | On-demand evaluation |
| Visible deterioration | Promotion-initiated |

### Exam Results

| Finding | Action |
|---------|--------|
| Clean | Clear to work |
| Minor Issues | Warnings, suggested rest |
| Moderate Issues | Limited schedule recommended |
| Serious Issues | Mandatory time off |
| Career-Threatening | Retirement discussion |

---

## Hidden Damage (#175)

Some damage is invisible until detected:

| Type | Detection |
|------|-----------|
| Concussion history | Only via medical exam |
| Spinal compression | Only via medical exam |
| Early arthritis | Only via medical exam |
| Heart issues | Only via medical exam |

### Health Status Visibility (#176)

| Level | What Player Sees |
|-------|-----------------|
| **Public** | Major injuries, surgery announcements |
| **Promotion** | Medical exam results, recovery timelines |
| **Hidden** | Cumulative damage percentages, hidden conditions |

---

## Era-Specific Handling

### Territory/Kayfabe Era

- Injuries often hidden from public
- Workers work hurt constantly
- No concussion protocols
- "Shake it off" culture
- Career-ending injuries more common

### Modern Era

- Mandatory concussion protocols
- Public injury announcements
- Fans aware of recovery timelines
- Worker wellness programs
- Insurance/liability concerns

---

## Recovery and Repair

### Rest Recovery

| Rest Duration | Recovery Rate |
|---------------|---------------|
| 1 week | -2 to -5 wear per region |
| 1 month | -10 to -20 wear per region |
| 3 months | -30 to -50 wear per region |

### Surgery

| Surgery Type | Effect |
|--------------|--------|
| Minor (scope) | Reset to 40 wear, 2-3 month recovery |
| Major (reconstruction) | Reset to 20 wear, 6-12 month recovery |
| Experimental | Variable results |

### Permanent Damage

Some wear cannot be fully repaired:

| Threshold | Permanent Effect |
|-----------|-----------------|
| Region hit 90+ | Minimum 30 wear permanently |
| Region hit 100 | Minimum 50 wear permanently |
| Multiple surgeries | Diminishing returns |

---

## Implementation Notes

```json
{
  "worker_id": "mick_foley",
  "wear_and_tear": {
    "head": 85,
    "neck": 75,
    "back": 80,
    "knees": 70,
    "shoulders": 65,
    "hips": 60,
    "elbows": 55,
    "ankles": 50
  },
  "chronic_conditions": ["memory_issues", "chronic_pain"],
  "surgeries": ["knee_1998", "hip_2002"],
  "style_restrictions": ["no_chair_shots", "limited_bumps"]
}
```

---

## Connected Mechanics

- [[Lifestyle Tracker]] - Accelerates/decelerates wear
- [[Booking_Engine_P1-3]] - Cumulative Fatigue feeds into wear
- [[Worker_Skills]] - Stats degraded by wear
- Aging System - Wear compounds with age

---

## Open Questions

- Exact wear accumulation formulas per move type?
- Surgery success rate calculations?
- How does wear affect match quality rating?
- Concussion protocol specifics?

---

**Document Status:** Conceptual
**Last Updated:** 2024-12-23
