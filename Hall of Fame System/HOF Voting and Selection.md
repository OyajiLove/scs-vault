# HOF Voting and Selection

📛 **MECHANIC:** How Hall of Fame Inductees Are Chosen
🔗 **PARENT SYSTEM:** [[_Hall of Fame Index|Hall of Fame System]]
🧭 **CATEGORY:** Legacy
🔑 **KEYWORDS:** voting, selection, committee, politics, induction class
📌 **ORIGIN:** Vol 1-4 (HOF voting/eligibility)
✅ **STATUS:** Locked

---

## Overview

Eligibility doesn't guarantee induction. Selection involves politics, timing, company relationships, and strategic considerations. Some eligible workers wait decades; others are fast-tracked. The selection process varies by promotion and can be influenced by player decisions.

---

## Selection Methods

| Method | Description | Example |
|--------|-------------|---------|
| **Owner Decision** | One person decides | WWE (Vince era) |
| **Committee Vote** | Panel selects | Observer HOF |
| **Fan Vote** | Public selection | Some fan categories |
| **Automatic** | Criteria-based trigger | Career milestones |
| **Political** | Relationships matter | Most real HOFs |

---

## Selection Factors

### Promotion Considerations

| Factor | Weight |
|--------|--------|
| **Company loyalty** | Very High |
| **Current relationship** | High |
| **PR value** | High |
| **Timing (anniversary, etc.)** | Moderate |
| **Class composition** | Moderate |
| **Fan demand** | Moderate |
| **Available for ceremony** | High |

### Timing Considerations

| Factor | Effect |
|--------|--------|
| **Major anniversary** | Fast-tracks eligible workers |
| **Recent death** | Often triggers posthumous |
| **Reconciliation** | Opens previously closed doors |
| **PR need** | Company may rush to positive news |
| **Class balance** | Mix of eras, styles, roles |

---

## Political Factors

| Factor | Description |
|--------|-------------|
| **Owner grudge** | Can block indefinitely |
| **Bad exit** | Delays consideration |
| **Competitor ties** | May cause hesitation |
| **Backstage enemies** | Lobbying against |
| **Champions in corner** | Lobbying for |
| **Public pressure** | Fan campaigns |

### Historical Examples

| Worker | Political Factor | Result |
|--------|------------------|--------|
| **Bruno Sammartino** | McMahon feud | Delayed 20+ years |
| **Macho Man** | Vince grudge | Posthumous only |
| **Ultimate Warrior** | Burned bridges | Required reconciliation |
| **Bret Hart** | Montreal Screwjob | Eventually reconciled |

---

## Induction Class Composition

Typical class structure:

| Category | Typical Slots |
|----------|---------------|
| **Headliner(s)** | 1-2 main event legends |
| **Supporting legends** | 2-3 solid careers |
| **Tag team/faction** | 0-1 group |
| **Legacy/builder** | 1-2 non-wrestlers |
| **Celebrity** | 0-1 crossover name |
| **Posthumous** | As needed |

---

## Annual Selection Process

| Phase | Description |
|-------|-------------|
| **Eligible pool review** | All qualified workers assessed |
| **Company priority list** | Key targets identified |
| **Outreach** | Contact candidates |
| **Negotiation** | Terms, attendance, speech |
| **Announcement** | Public reveal (often staged) |
| **Ceremony prep** | Video packages, introductions |

---

## Player Influence (If Running Promotion)

| Action | Effect |
|--------|--------|
| **Nominate worker** | Adds to consideration |
| **Block worker** | Removes from pool |
| **Rush induction** | Skip waiting period |
| **Posthumous decision** | Induct after death |
| **Reconciliation angle** | Repair relationship first |

---

## Refusal and Complications

| Scenario | Outcome |
|----------|---------|
| **Worker refuses** | Not inducted (Owen Hart family) |
| **Health prevents attendance** | Inducted anyway |
| **Death before ceremony** | Posthumous conversion |
| **Public embarrassment risk** | May delay |
| **Active scandal breaks** | May cancel |

---

## Regional Considerations

| Promotion Type | Selection Style |
|----------------|-----------------|
| **National (WWE)** | Political, company-focused |
| **Critical (Observer)** | Merit-based, worldwide |
| **Regional** | Local significance weighted |
| **Japanese** | Respect, longevity valued |
| **Indie** | Counter-culture credibility |

---

## Snub Mechanics

Candidates who don't make it:

- Remain in eligibility pool
- "Years on ballot" tracked
- Fan resentment builds for repeated snubs
- Eventually may trigger Veteran's Committee path
- Snubs can become storylines

---

## Connected Mechanics

- [[HOF Eligibility]] - Who qualifies for selection
- [[HOF Voter Types]] - Who votes and their priorities
- [[Legacy Score]] - Influences selection priority
- [[Scandal System/_Scandal System Index|Scandal System]] - Blocks or delays selection
- [[Hidden Personality]] - Ego affects refusal likelihood

---

## Open Questions

- [ ] How fan campaigns affect selection
- [ ] Committee composition and voting weights
- [ ] Multi-promotion workers: which hall first?
- [ ] How to handle rejected inductees
- [ ] Controversy during ceremony handling

---

## Implementation Notes

```json
{
  "selection_process": {
    "year": 1995,
    "promotion": "promo_001",
    "eligible_pool": ["worker_001", "worker_002", "worker_003", "..."],
    "company_priorities": ["worker_001"],
    "political_blocks": ["worker_042"],
    "selected_class": [
      { "worker_id": "worker_001", "category": "headliner" },
      { "worker_id": "worker_015", "category": "supporting" },
      { "worker_id": "tag_team_001", "category": "tag_team" }
    ],
    "refusals": [],
    "ceremony_date": "1995-03-15"
  }
}
```
