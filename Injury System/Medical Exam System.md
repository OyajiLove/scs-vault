# Medical Exam System

📛 **MECHANIC:** Health Evaluation and Intervention
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation / Player Interface
🔑 **KEYWORDS:** medical exam, health visibility, intervention, worker reaction, career decision
📌 **ORIGIN:** Vol 1 Extraction #174, #175
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED |

---

## Overview

The Medical Exam System provides players with ways to assess worker health without breaking immersion. It governs how health information is surfaced, how workers react to medical intervention, and the dynamic consequences of health management decisions.

**Core Quote:** "You aren't just building matches, you're booking living bodies breaking down in real time."

---

## Wear and Tear Visibility Framework (#174)

### Design Principle

No hard numbers by default. Health information is conveyed through in-world cues that feel natural.

### Visibility Methods

| Method | Description | Example |
|--------|-------------|---------|
| **Worker Profile Status** | Natural language health descriptor | "Currently healthy" → "Minor lingering injuries" → "Significant accumulated damage" → "Severe long-term wear threatening career" |
| **Match Reports** | Road agent observations | "Worker X appeared visibly slower and favored his right knee" |
| **Backstage Reports** | Locker room gossip | "Road Agent notes Worker Y is struggling to recover between matches" |
| **Commentary Hints** | Announcers noting changes | "X has been limping lately" |
| **Optional Medical Exam** | Detailed assessment (player-initiated) | "Worker Z's back shows chronic degeneration. Risk of major injury within 6 months if schedule not adjusted" |

### Health Status Tiers

| Tier | Description | Visual Cue |
|------|-------------|-----------|
| **Healthy** | No concerns | Green status, no notes |
| **Minor Issues** | Some wear, nothing urgent | Yellow status, occasional notes |
| **Moderate Concern** | Accumulated damage showing | Orange status, regular notes |
| **Serious** | Career at risk without intervention | Red status, frequent warnings |
| **Critical** | Immediate retirement threat | Flashing red, urgent notifications |

---

## Medical Exam Trigger System (#175)

### Initiating an Exam

Player can send any worker for medical evaluation. This is a choice with consequences.

**Risks of Initiating:**
- Exposes issues that might have stayed hidden
- May upset the worker (personality-dependent)
- Creates expectation of action based on findings
- Worker may lose trust if findings are ignored

### Decision Flow

```
1. Player initiates exam
   ↓
2. Results returned (severity language varies)
   ↓
3. Player chooses: Private OR Share with worker
   ↓
4. Player decision: Force time off / Suggest reduced schedule / Ignore
   ↓
5. Worker reaction (based on personality tags)
   ↓
6. Dynamic world fallout (injuries, departures, addiction, reinvention)
```

### Result Phrasing

| Severity | Soft Phrasing | Heavy Phrasing |
|----------|---------------|----------------|
| Minor | "Some wear, nothing immediate" | "Early warning signs present" |
| Moderate | "Accumulated damage noted" | "Intervention recommended" |
| Major | "Significant risk if unchanged" | "Career in danger within 6-12 months" |
| Critical | "Immediate action required" | "Retirement may be necessary" |

---

## Worker Reaction System

### Reaction Based on Personality Tags

| Tag | Reaction to Intervention |
|-----|--------------------------|
| **Driven to Destruction** | Furious about being asked to slow down, may refuse, addiction risk |
| **Fragile/Lazy** | Accept easily, may exploit politically (milk injury) |
| **Loyalist** | Listen if respected, cooperate with reduced schedule |
| **Bitter** | Leak resentment, cause morale issues, potential no-show |

### Kurt Angle 2005 Example (Full Flow)

**Scenario:** WWE sends for evaluation

**Flow:**
1. Results: Severe neck flagged
2. Time off suggested
3. "Driven to Destruction" tag triggers fury
4. Threatens to leave
5. Builds painkiller addiction arc (see [[Addiction Risk System]])
6. Leaves for TNA
7. Rebuilds career in new arc
8. Legacy becomes tragic-heroic

**Design Quote:** "Wrestlers aren't just chess pieces. They are living dreams tied to broken bodies."

---

## Decision Outcomes

### Force Time Off

| Outcome Type | Description |
|--------------|-------------|
| **Positive** | Worker heals, returns refreshed, grateful |
| **Neutral** | Worker heals, resents time away, returns with chip on shoulder |
| **Negative** | Worker refuses, leaves for competitor, spreads resentment |

### Suggest Reduced Schedule

| Outcome Type | Description |
|--------------|-------------|
| **Positive** | Worker adjusts, career extended, appreciative |
| **Neutral** | Worker complies minimally, some resentment |
| **Negative** | Worker refuses "demotion," escalates conflict |

### Ignore Findings

| Outcome Type | Description |
|--------------|-------------|
| **Possible** | Nothing happens (luck) |
| **Likely** | Injury worsens, more severe breakdown later |
| **Worst Case** | Career-ending injury, addiction spiral, death |

---

## Player Information Balance

### What Players Can Always See

- General health status (tier, not numbers)
- Match report notes
- Backstage gossip

### What Requires Action to See

- Detailed medical assessment (must initiate exam)
- Specific body part damage levels
- Recovery timeline projections
- Risk calculations

### What Stays Hidden

- Exact wear meter values
- Precise injury probability
- Internal worker health calculations

---

## Connected Mechanics

- [[Wear and Tear System]] - Underlying damage tracked
- [[Career Injury Logs]] - Historical context for exams
- [[Addiction Risk System]] - Intervention can trigger or prevent addiction
- [[Style Adaptation]] - Recommendations may include style changes
- [[Retirement System/_Retirement System Index|Retirement System]] - Exam results can trigger retirement pressure
- [[Tags_System|Tags System]] - Medical reaction tags affect outcomes

---

## Open Questions

- [ ] How often can players initiate exams without it becoming routine?
- [ ] Cost/resource requirement for medical exams?
- [ ] Era-specific medical exam quality (1970s vs. modern)?
- [ ] Can workers refuse to participate in exams?
- [ ] How do exam results leak to other promotions?

---

## Implementation Notes

```json
{
  "medical_exam": {
    "exam_id": "exam_001",
    "worker_id": "worker_001",
    "date": "1985-06-15",
    "initiated_by": "player",
    "results": {
      "severity_level": "major",
      "affected_areas": ["neck", "back"],
      "recommendation": "reduced_schedule",
      "career_risk_window": "6-12 months",
      "detailed_notes": "Chronic degeneration in C4-C5 region. Continued heavy bump schedule will likely result in career-threatening injury within 6-12 months. Recommend reduced match count and elimination of high-impact finishing moves."
    },
    "player_action": "suggest_reduced",
    "worker_reaction": {
      "personality_tag": "driven_to_destruction",
      "initial_response": "refused",
      "morale_change": -15,
      "relationship_change": -10,
      "consequence_triggered": "addiction_risk_increase"
    },
    "follow_up_required": "1985-09-15"
  }
}
```

---

**Document Status:** Locked (Vol 1)
**Last Updated:** 2025-12-24
**Next Review:** Design exam cost/frequency mechanics
