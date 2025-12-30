# Exodus Template

📛 **MECHANIC:** Mass Departure Events
🔗 **PARENT SYSTEM:** [[_Backstage Politics System Index|Backstage Politics System]]
🧭 **CATEGORY:** Major Events
🔑 **KEYWORDS:** exodus, mass departure, schism, split, defection, NOAH, walkout
📌 **ORIGIN:** Vol 4 (AJPW exodus template created)
✅ **STATUS:** Template Exists (AJPW model), General mechanics conceptual

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED (AJPW template) |

---

## Overview

An Exodus is a mass departure event where multiple workers leave a promotion together, often to form or join a competitor. These are watershed moments that can cripple promotions and reshape the industry. The AJPW Exodus (Misawa leading workers to form NOAH) serves as the primary template.

---

## AJPW Exodus Template (Vol 4, Locked)

### Historical Context: Giant Baba's Death (1999)

| Phase | Event | Mechanic |
|-------|-------|----------|
| **Trigger** | Giant Baba dies | Founder death → Succession crisis |
| **Power Vacuum** | Motoko Baba (widow) takes control | Non-worker owner → Legitimacy crisis |
| **Faction Formation** | Misawa faction vs. Kawada/management | Ideological split on future direction |
| **Escalation** | Creative control disputes | Booking committee deadlock |
| **Breaking Point** | Misawa demands, rejected | Failed negotiation → Exit decision |
| **Cascade** | Workers choose sides | Loyalty test → Mass departure |
| **Exodus** | Misawa + 24 workers form NOAH | New promotion founded |

### Mechanics Demonstrated

**Succession Crisis:**
- Owner/booker death or departure creates vacuum
- Successor legitimacy questioned
- Workers loyal to predecessor, not successor

**Loyalty Cascade:**
- Key figure (Misawa) declares intention
- Workers with high loyalty to leader follow
- Workers with high promotion loyalty stay
- Undecided workers weigh options

**Who Follows Whom:**
```
Follow Probability = 
  (Loyalty to Leader × 0.4) +
  (Dissatisfaction with Management × 0.3) +
  (Career Calculation × 0.2) +
  (Personal Bonds × 0.1)
```

**Stayers vs. Leavers:**

| Profile | Likely Action |
|---------|---------------|
| **High loyalty to leader** | Follow |
| **High promotion loyalty** | Stay |
| **Career peak past** | May stay (stability) |
| **Career rising** | Follow leader (opportunity) |
| **Family ties to region** | Stay |
| **Personal grudge with leader** | Stay |
| **Personal bond with leader** | Follow |

---

## Exodus Trigger Conditions

| Trigger Type | Probability |
|--------------|-------------|
| **Founder death** | High (if no clear successor) |
| **Hostile takeover** | Very High |
| **Ideology shift** | Medium-High |
| **Failed contract negotiations (key talent)** | Medium |
| **Regime change (new booker antagonizes)** | Medium |
| **Sustained burial of faction** | Low-Medium |
| **External offer (competing promotion)** | Variable |

### Required Conditions

For an exodus to occur:
1. **Leadership figure** willing to leave and lead exodus
2. **Critical mass** of workers willing to follow (5+ typically)
3. **Destination** (new promotion, competitor, or founding capital)
4. **Catalyst event** (final straw that triggers departure)

---

## Exodus Phases

### Phase 1: Tension Building

| Element | Description |
|---------|-------------|
| **Grievances accumulate** | Multiple political defeats |
| **Faction crystallizes** | Workers align with leader |
| **Management rigidity** | Demands rejected |
| **External awareness** | Other promotions notice instability |

### Phase 2: Breaking Point

| Element | Description |
|---------|-------------|
| **Ultimatum** | Leader demands, management refuses |
| **Decision made** | Leader decides to leave |
| **Secret planning** | Departure organized quietly |
| **Contract review** | Legal options assessed |

### Phase 3: Cascade

| Element | Description |
|---------|-------------|
| **Loyalty tests** | Leader approaches potential followers |
| **Word spreads** | Rumor mill activates |
| **Pressure intensifies** | Workers must choose sides |
| **Counter-offers** | Management tries to retain key talent |

### Phase 4: Exodus

| Element | Description |
|---------|-------------|
| **Departure announcements** | Workers give notice |
| **Contract disputes** | Legal battles possible |
| **Media coverage** | Public attention |
| **New entity** | Promotion formed or workers absorbed |

### Phase 5: Aftermath

| Element | Description |
|---------|-------------|
| **Roster devastation** | Original promotion weakened |
| **Talent scramble** | Both sides recruit |
| **Industry realignment** | Power balance shifts |
| **Long-term grudges** | Relationships permanently damaged |

---

## Exodus Effects

### On Original Promotion

| Impact | Severity |
|--------|----------|
| **Roster depletion** | Critical (may lose 30-70% of stars) |
| **Crowd confusion** | High (favorites gone) |
| **Revenue drop** | Severe (short-term) |
| **Prestige damage** | High |
| **Opportunity** | Space for new talent to rise |

### On New Entity

| Impact | Description |
|--------|-------------|
| **Instant credibility** | Established stars carry weight |
| **Crowd carry-over** | Fans follow favorites |
| **Financial challenge** | Startup costs, no infrastructure |
| **Political baggage** | Exodus politics continue |
| **Roster holes** | May lack depth, youth |

### On Workers

| Who | Effect |
|-----|--------|
| **Exodus Leader** | Career-defining, high risk/reward |
| **Followers** | Tied to new entity's success |
| **Stayers** | Opportunity for advancement, or sinking ship |
| **Undecided** | May be blacklisted by both sides |

---

## Historical Examples

| Exodus | Year | Leader | From → To | Scale |
|--------|------|--------|-----------|-------|
| **AJPW → NOAH** | 2000 | Misawa | AJPW | 24 workers |
| **WWF → WCW** | 1994-96 | Various | WWF | Key individuals |
| **ECW → WWF/WCW** | 1997-99 | Various | ECW | Gradual drain |
| **AJPW → WAR** | 1990 | Tenryu | AJPW | 12 workers |
| **AWA → Various** | 1984-87 | Various | AWA | Slow collapse |

---

## Ringstate Exodus Considerations

In the Ringstate world, exodus has additional dimensions:

| Factor | Effect |
|--------|--------|
| **Faction alignment** | Leaving CCA for GWA = ideological defection |
| **Blacklisting** | Some factions blacklist defectors |
| **Political asylum** | Blade Underground accepts anyone |
| **State involvement** | PWU defections trigger government response |
| **Cultural consequences** | CFPW departures affect community standing |

---

## Connected Mechanics

- [[Power Struggle Events]] - Tier 4 struggles trigger exodus
- [[Clique Formation]] - Cliques form exodus core
- [[Influence Mechanics]] - Leader needs high influence |
- [[Regime Change]] - Regime change can trigger exodus
- [[_Contract System Index|Contract System]] - Contract status affects departure

---

## Open Questions

- [ ] Exact loyalty cascade formulas
- [ ] How to simulate "secret planning" phase?
- [ ] Counter-offer effectiveness calculation
- [ ] Multi-promotion destination selection
- [ ] Legal dispute simulation (no-compete clauses)

---

## Implementation Notes

```json
{
  "exodus_event": {
    "event_id": "EXODUS_2000_001",
    "origin_promotion": "AJPW",
    "destination": "NOAH_NEW",
    "leader_id": "WORKER_MISAWA",
    "trigger": "succession_crisis",
    "catalyst": "creative_control_rejection",
    "followers": ["WORKER_001", "WORKER_002", "..."],
    "stayers": ["WORKER_KAWADA", "..."],
    "total_departed": 24,
    "roster_percentage_lost": 0.65,
    "date": "2000-06-16"
  }
}
```

---

**Document Status:** Template Exists (AJPW), General Mechanics Conceptual
**Last Updated:** 2025-12-21
**Next Review:** Design loyalty cascade algorithms
