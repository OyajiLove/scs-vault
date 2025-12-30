# Faction Stability

📛 **MECHANIC:** Internal Faction Health Tracking
🔗 **PARENT SYSTEM:** [[_Faction System Index|Faction System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** stability, friction, goals, internal conflict, faction health
📌 **ORIGIN:** Vol 1-4 (Faction Logic, Stability Score, Friction Meter)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Every faction has an internal stability score that tracks how healthy the group is. Friction builds from jealousy, uneven push, failed goals, and personality conflicts. When stability drops too low, the faction becomes vulnerable to implosion, betrayal, or collapse.

---

## Faction Stability Score

| Range | Status | Behavior |
|-------|--------|----------|
| 90-100 | **Ironclad** | Unified, peak chemistry, dominant |
| 75-89 | **Stable** | Healthy group, minor tensions manageable |
| 50-74 | **Strained** | Visible cracks, friction events possible |
| 25-49 | **Unstable** | High betrayal risk, internal conflict |
| 0-24 | **Collapse Imminent** | Faction likely to implode soon |

---

## Stability Factors

### What Builds Stability

| Factor | Effect |
|--------|--------|
| **Achieving Goals** | +10 to +20 per major goal |
| **Title Victories** | +5 to +10 per title win |
| **Successful Feuds** | +5 per feud won together |
| **Even Push** | +2 to +5 per month if balanced |
| **Strong Leadership** | +3 to +5 base bonus |
| **Backstage Harmony** | +1 to +3 ongoing |
| **Shared Hardship** | +5 to +15 (overcome together) |

### What Damages Stability

| Factor | Effect |
|--------|--------|
| **Failed Goals** | -10 to -20 per major failure |
| **Uneven Push** | -3 to -8 per month |
| **Internal Jealousy** | -5 to -15 per incident |
| **Leader Ego Outgrows** | -10 to -20 |
| **Member Buried** | -5 to -10 |
| **Backstage Conflict** | -5 to -15 |
| **Outside Temptation** | -3 to -10 if workers tempted |
| **Loss Streak** | -2 per consecutive loss |

---

## Internal Friction Meter

Separate from stability, friction tracks active tensions:

| Friction Level | Description |
|----------------|-------------|
| 0-15 | **Minimal** | Normal minor disagreements |
| 16-35 | **Simmering** | Tensions noticeable, need addressing |
| 36-55 | **Active** | Conflicts affecting performance |
| 56-75 | **Dangerous** | Betrayal or split highly likely |
| 76-100 | **Critical** | Explosion imminent |

### Friction Sources

| Source | Friction Added |
|--------|----------------|
| **Momentum Imbalance** | +5 per month if one member much hotter |
| **Suppressed Members** | +8 per buried midcarder |
| **Ego Clashes** | +10 to +20 between high-ego members |
| **Romantic Entanglements** | +5 to +15 if involving members |
| **Financial Disputes** | +5 to +10 (merch split, pay gaps) |
| **Creative Differences** | +3 to +8 |

### Friction Resolution

| Method | Friction Reduced |
|--------|------------------|
| **Spotlight Rotation** | -5 to -10 |
| **Clear Leadership** | -3 to -5 ongoing |
| **Shared Victory** | -5 to -10 |
| **Booker Intervention** | -5 to -15 (if successful) |
| **Internal Match** | Variable (can increase or decrease) |

---

## Faction Goals Tracking

Factions have implicit or explicit goals:

| Goal Status | Effect on Stability |
|-------------|---------------------|
| **Progressing** | +2 per month |
| **Achieved** | +10 to +20 spike |
| **Stalled** | -2 per month |
| **Failed** | -10 to -20 immediate |
| **Abandoned** | -5, goal removed |

### Goal Types

| Goal | Success Condition |
|------|-------------------|
| **Title Domination** | Hold target titles |
| **Feud Victory** | Defeat rival faction/worker |
| **Leader Protection** | Leader avoids losses/damage |
| **Territory Control** | Dominate division |
| **Revolution** | Change promotion direction |

---

## Collapse Triggers

What causes faction implosion:

| Trigger | Description |
|---------|-------------|
| **Leader Ego Outgrows** | Leader prioritizes self over group |
| **Suppressed Member Revolt** | Buried midcarder turns |
| **Failed Title Quest** | Repeated failures decay loyalty |
| **Outside Offer** | Member tempted away |
| **Public Betrayal** | Trust destroyed instantly |
| **Scandal** | Member scandal taints group |

---

## Stability Warnings

System alerts booker:

| Warning | Trigger |
|---------|---------|
| "Faction showing internal tension" | Stability < 75 |
| "Friction between [X] and [Y]" | Friction > 35 |
| "[Member] feels underutilized" | Push imbalance detected |
| "Faction goals stalling" | No progress 2+ months |
| "Betrayal risk elevated" | Stability < 50 + high friction |

---

## Connected Mechanics

- [[Faction Formation]] - Starting stability based on formation type
- [[Faction Loyalty]] - Individual loyalty affects stability
- [[Betrayal and Breakup]] - What happens when stability fails
- [[Hidden Personality]] - Ego, Paranoia create friction sources

---

## Open Questions

- [ ] Exact stability calculation formula
- [ ] How faction size affects stability thresholds
- [ ] Booker intervention success rates
- [ ] How injuries affect stability
- [ ] Multiple faction goals priority system

---

## Implementation Notes

```json
{
  "faction_health": {
    "faction_id": "faction_001",
    "stability_score": 68,
    "friction_meter": 28,
    "goals": [
      { "type": "title_domination", "target": "tag_titles", "progress": 60, "status": "progressing" }
    ],
    "internal_tensions": [
      { "worker_a": "worker_002", "worker_b": "worker_003", "type": "momentum_imbalance", "severity": 15 }
    ],
    "warnings_active": ["friction_simmering"],
    "months_since_goal_progress": 1,
    "betrayal_risk": "moderate"
  }
}
```
