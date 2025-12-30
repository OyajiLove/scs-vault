# Injury Types

📛 **MECHANIC:** Injury Classification System
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** acute injury, chronic injury, concussion, ligament, fracture, severity, body systems
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Injuries are grouped by body system realistically, with serious depth where needed. Not all concussions are the same, nor all ligament injuries. Severity scaling applies to every injury type.

---

## Injury Categories by Body System

| System | Injury Examples |
|--------|-----------------|
| **Concussions** | Light (1-2 weeks), Moderate (longer, reoccurrence risk), Severe (chronic symptoms, retirement trigger) |
| **Neck/Spine** | Whiplash, minor herniations, nerve impingement, major fractures (Austin, Edge) |
| **Shoulder** | Rotator cuff tear, AC joint sprain, dislocation, labrum tear |
| **Knee** | ACL/MCL/PCL tears, meniscus damage, chronic joint deterioration (Tanahashi) |
| **Back** | Disc herniations, sciatica, fractured vertebrae |
| **Arms/Hands** | Broken fingers, wrists, forearm fractures, tendon ruptures (Liger) |
| **Legs/Feet** | Ankle sprains, shin fractures, Achilles rupture (Edge), foot arch collapse |
| **Soft Tissue** | Muscle tears (quads, hamstrings), contusions, deep tissue bruising |
| **Organ Trauma** | Internal bleeding (hardcore/deathmatch risk), ruptured spleens, punctured lungs |
| **Skin/Facial** | Lacerations (accidental/hardway), orbital fractures (Shibata), cauliflower ear buildup |
| **Blood/Immune** | Blood loss risks (deathmatches), infection from foreign objects, sepsis (Foley ear incident) |

---

## Severity Grades

Every injury has severity scaling:

| Grade | Description | Recovery | Career Impact |
|-------|-------------|----------|---------------|
| **Minor** | Week off, minimal long-term impact | 1-2 weeks | None |
| **Moderate** | Months off, risk of re-injury | 1-6 months | Possible chronic issues |
| **Major** | Career altering, significant time out | 6-12+ months | Permanent limitations likely |
| **Catastrophic** | Career ending or life-threatening | Variable/permanent | Forced retirement possible |

---

## Acute vs Chronic Injuries

### Acute Injuries
Sudden, visible injuries triggered by:
- Match intensity
- Bump severity
- Botch chances
- Skill gaps between workers

**Examples:** Broken bones, torn muscles, concussions, lacerations

### Chronic Injuries
Damage accumulates until something gives out:
- Builds from [[Wear and Tear System]] thresholds
- Often hidden until sudden failure
- May require ongoing management rather than cure

**Examples:** Ric Flair's back, Tanahashi's knees, Dynamite Kid's spine

---

## Hidden Injury Possibility

Workers may hide injuries due to:
- Booking pressure ("can't lose my spot")
- Loyalty to promotion
- Pride and tough guy culture
- Financial need to keep working

**Consequences of Hidden Injuries:**
- Worsened long-term outcomes
- Higher re-injury risk
- Sudden catastrophic failure
- Accelerated chronic condition development

---

## Forced Retirement Triggers

Some injuries can end careers immediately:

| Injury Type | Retirement Trigger Conditions |
|-------------|------------------------------|
| **Concussions** | Repeated moderate+ concussions, severe single event |
| **Neck Fractures** | Compound fractures, nerve damage |
| **Spinal Injuries** | Paralysis risk, major disc damage |
| **Compound Fractures** | Bones that won't heal properly |
| **Nerve Damage** | Permanent loss of function |

---

## Injury Probability Factors

What increases injury likelihood:

| Factor | Effect on Risk |
|--------|----------------|
| **High Wear Counters** | Increased chronic injury trigger |
| **Match Intensity** | Higher intensity = higher acute risk |
| **Bump Severity** | Dangerous spots multiply risk |
| **Worker Chemistry** | Poor chemistry = more botches = more injuries |
| **Skill Gaps** | Less skilled workers more dangerous |
| **Fatigue** | Tired workers make mistakes |
| **Style** | High-risk styles have higher baselines |
| **Age** | Older workers heal slower, break easier |

---

## Injury-Specific Details

### Concussions
| Severity | Recovery | Re-Injury Risk | Long-Term Risk |
|----------|----------|----------------|----------------|
| Light | 1-2 weeks | Low | Minimal |
| Moderate | 4-8 weeks | Medium | CTE accumulation |
| Severe | 3-6 months | High | Chronic symptoms, retirement |

### Knee Injuries
| Type | Recovery | Surgery Required | Permanent Impact |
|------|----------|------------------|------------------|
| ACL Tear | 8-12 months | Yes | Mobility reduction |
| MCL Sprain | 4-8 weeks | Sometimes | Usually full recovery |
| Meniscus Tear | 3-6 months | Usually | Chronic deterioration |
| Chronic Deterioration | Ongoing | Management only | Style change required |

### Neck/Spine
| Type | Recovery | Risk Level | Career Impact |
|------|----------|------------|---------------|
| Whiplash | 2-4 weeks | Low | Minimal |
| Minor Herniation | 2-4 months | Medium | Recurring pain |
| Nerve Impingement | Variable | High | May require fusion |
| Major Fracture | 6-18 months | Critical | Often career-ending |

---

## Risk of Complication Layer

Every injury carries complication risks:

| Complication | Description |
|--------------|-------------|
| **Re-injury** | Same injury recurs, often worse |
| **Compromised Mobility** | Permanent loss of movement quality |
| **Chronic Pain Memory** | Body part never fully heals, ongoing pain |
| **Surgical Complications** | Botched surgery, infection, scar tissue |
| **Compensatory Injuries** | Protecting one injury causes another |

---

## Connected Mechanics

- [[Wear and Tear System]] - Accumulated damage triggers chronic injuries
- [[Surgery and Recovery]] - Treatment options and timelines
- [[Addiction Risk System]] - Pain management for injuries
- [[Style Adaptation]] - Changing style to protect damaged areas
- [[Hidden Personality]] - Drive, Ego affect hiding vs. reporting injuries

---

## Open Questions

- [ ] Exact probability tables for each injury type by match conditions
- [ ] Concussion protocol mechanics (modern era vs. territory era)
- [ ] How hidden injuries are revealed (if ever) to player
- [ ] Genetic predisposition modifiers (some workers more injury-prone)

---

## Implementation Notes

```json
{
  "injury": {
    "injury_id": "inj_001",
    "worker_id": "worker_001",
    "type": "acl_tear",
    "body_system": "knee",
    "severity": "major",
    "date_occurred": "1985-06-15",
    "cause": "match_bump",
    "match_id": "match_045",
    "hidden": false,
    "recovery_timeline": {
      "estimated_weeks": 40,
      "actual_weeks": null,
      "surgery_required": true
    },
    "complications": [],
    "permanent_impact": {
      "mobility_penalty": -5,
      "chronic_pain": true,
      "style_limitation": ["high_flying"]
    }
  }
}
```
