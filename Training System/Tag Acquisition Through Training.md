# Tag Acquisition Through Training

📛 **MECHANIC:** Learning Style Tags via Development
🔗 **PARENT SYSTEM:** [[_Training System Index|Training System]]
🧭 **CATEGORY:** Worker Specialization
🔑 **KEYWORDS:** tag acquisition, style tags, training focus, specialization, learning
📌 **ORIGIN:** Vol 3 (Tags System), Vol 4 (training concepts)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3-4 | 🔒 LOCKED |

---

## Overview

While some tags are earned through career events (betrayals, title wins, scandals), many style and specialization tags can be **acquired through focused training**. This allows workers to expand their repertoire, learn new styles, or deepen existing specializations.

---

## Trainable Tag Categories

### Fully Trainable (Through Development)

| Category | Examples | Training Time |
|----------|----------|---------------|
| **Style Specialization** | "Submission Specialist", "Power Style", "High Flyer" | 6-18 months |
| **Technical Skills** | "Mat Wizard", "Chain Wrestling", "Catch Wrestling" | 12-24 months |
| **Combat Style** | "Strong Style", "Lucha Libre", "Puroresu" | 18-36 months |
| **Match Type Specialty** | "Cage Specialist", "Ladder Match Expert" | 6-12 months |
| **Performance** | "Safe Worker", "Seller Extraordinaire" | 12-24 months |

### Partially Trainable (Requires Aptitude + Training)

| Category | Examples | Requirements |
|----------|----------|--------------|
| **Elite Specialization** | "Psychology Monster", "Ring General" | High base Psychology + years of experience |
| **Physical Specialty** | "Cardio Machine", "Ironman Specialist" | High base Stamina + training |
| **Hybrid Styles** | "Lucha Strong Style", "Technical Brawler" | Existing base in both |

### Non-Trainable (Earned Only)

| Category | Examples | Acquisition |
|----------|----------|-------------|
| **Legacy Tags** | "Legend", "Hall of Famer" | Career achievement |
| **Behavior Tags** | "Locker Room Leader", "Politician" | Emergent behavior |
| **Event Tags** | "Screwjob Survivor", "Retirement Match" | Specific events |
| **Anchor-Adjacent** | "Innovator of Violence", "Deathmatch Poet" | Historic achievement |

---

## Training Requirements

### Style Tags

| Tag | Stat Prerequisites | Training Time | Mentor Needed? |
|-----|-------------------|---------------|----------------|
| **Submission Specialist** | Technical 12+, Submission 14+ | 12 months | Recommended |
| **High Flyer** | Aerial 14+, Speed 14+ | 6 months | Optional |
| **Power Style** | Strength 14+, Power 14+ | 6 months | Optional |
| **Strong Style** | Striking 14+, Durability 14+ | 18 months | Required |
| **Lucha Libre** | Aerial 12+, Speed 12+, Agility 12+ | 24 months | Required |
| **King's Road** | Technical 14+, Psychology 16+, Durability 14+ | 36 months | Required |
| **Catch Wrestling** | Technical 14+, Submission 16+ | 18 months | Required |
| **Chain Wrestling** | Technical 16+, Psychology 14+ | 12 months | Recommended |

### Performance Tags

| Tag | Stat Prerequisites | Training Time | Notes |
|-----|-------------------|---------------|-------|
| **Safe Worker** | Technical 12+, Composure 14+ | 12 months | Reduces injury infliction |
| **Seller Extraordinaire** | Selling 16+, Psychology 14+ | 18 months | Must demonstrate consistently |
| **Bump Machine** | Durability 16+, Selling 14+ | 12 months | Requires injury tolerance |
| **Stiff Worker** | Striking 14+ | 6 months | Increases injury infliction |

---

## Training Process

### Focus Declaration
- Worker declares training focus (one primary tag target)
- Training time begins counting
- Stats must meet prerequisites throughout

### Progress Tracking
- Progress measured in months
- Match experience in related style accelerates (+10-20%)
- Mentor in that style accelerates (+25-50%)
- Injuries pause progress

### Completion
- When training time complete AND stats maintained
- Tag is acquired and active
- Worker can begin training new tag

---

## Tag Stacking Rules

### Compatible Stacks
- "Technical" + "Submission Specialist" (deepens specialty)
- "High Flyer" + "Lucha Libre" (style combination)
- "Safe Worker" + any style tag (professional modifier)

### Incompatible (Cannot Coexist)
- "Safe Worker" + "Stiff Worker" (contradictory)
- "Style Locked" + "Style Versatile" (contradictory)
- "High Flyer" + "Grounded Veteran" (mutually exclusive)

### Soft Limits
- Workers typically hold 3-5 style specialty tags
- More than 8 specialty tags = diluted identity
- System may auto-prune least-used tags over time

---

## Tag Decay & Loss

### Through Inactivity
- Style tags require occasional use to maintain
- 12+ months without using style = risk of decay
- "Rusty [Style]" transitional state before loss

### Through Injury
- Physical specialty tags may be lost to injury
- "Former High Flyer" anchor replaces lost "High Flyer" tag
- Some tags can be rebuilt through rehabilitation training

### Through Age
- Physical style tags (High Flyer, Speed Merchant) decay with age
- Technical style tags (Mat Wizard, Psychology Monster) persist
- Replacement tags may emerge ("Grounded Veteran", "Ring General")

---

## Connected Mechanics

- [[Training Philosophy Types]] - Philosophy affects tag availability
- [[Skill Growth Mechanics]] - Stats must meet prerequisites
- [[Mentor System]] - Mentors accelerate tag acquisition
- [[Tags System]] - Master tag list and categories

---

## Implementation Notes

```json
{
  "tag_training": {
    "worker_id": "WORK_12345",
    "current_focus": {
      "target_tag": "Strong Style",
      "months_trained": 8,
      "months_required": 18,
      "mentor_id": "WORK_67890",
      "mentor_bonus": 0.35
    },
    "tag_eligibility": {
      "submission_specialist": true,
      "high_flyer": true,
      "kings_road": false,
      "ineligibility_reason": "Psychology below 16"
    },
    "acquired_through_training": [
      "Technical Foundation",
      "Chain Wrestling"
    ]
  }
}
```

---

**Document Status:** Locked
**Last Updated:** 2025-12-21
