# NWA Governing Body System

📛 **MECHANIC:** NWA Governing Body / Political Capital
🔗 **PARENT SYSTEM:** [[_Backstage Politics System Index|Backstage Politics System]]
🧭 **CATEGORY:** Inter-Promotion Politics
🔑 **KEYWORDS:** NWA, governing body, board of directors, political capital, arguments, alliances
📌 **ORIGIN:** Vol 1 Extraction #101-102, #107-108, #166-168
✅ **STATUS:** Locked (Concept), Open (Formulas)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept and structure) |

---

## Overview

The NWA (and similar governing bodies) function as political arenas where member promotions jockey for influence, titles, and talent access. This creates emergent drama, territorial conflicts, and power struggles that shape the wrestling landscape.

---

## Core Concepts

### Board of Directors

Governing bodies have a **Board of Directors** consisting of major member promotions:

| Role | Description |
|------|-------------|
| **President** | Tiebreaker vote, sets agenda, represents org publicly |
| **Board Members** | Each major promotion gets a vote |
| **Associate Members** | Minor promotions with limited voice |
| **Outlaw Promotions** | Not members, can be targets or rivals |

### Political Capital

Each promotion accumulates **Political Capital** through:

| Action | Capital Gained |
|--------|----------------|
| Hosting successful NWA title defenses | +5-15 |
| Providing talent for cross-territorial shows | +3-8 |
| Winning arguments at board meetings | +10-20 |
| Long-term membership in good standing | +1-3/year |
| Backing winning faction in power struggle | +15-25 |

**Spending Political Capital:**

| Action | Capital Cost |
|--------|--------------|
| Requesting NWA champion appearance | 10-30 |
| Blocking another promotion's proposal | 15-25 |
| Pushing your worker for NWA title shot | 20-40 |
| Forcing policy change | 30-50 |
| Removing a board member | 50+ |

---

## Argument System (#101)

Board meetings include formal **Arguments** where promotions debate policy:

### Argument Types

| Type | Stakes |
|------|--------|
| **Title Holder Dispute** | Who should hold world title next? |
| **Talent Sharing** | Which promotions get access to which workers? |
| **Territory Boundaries** | Who books which regions? |
| **Dues/Fees** | Financial obligations of members |
| **New Member Admission** | Should X promotion join? |
| **Expulsion** | Should X promotion be kicked out? |

### Argument Resolution

Arguments are resolved through:

1. **Debate Phase:** Promotions present cases
2. **Alliance Check:** Who supports whom?
3. **Vote:** Majority or supermajority depending on issue
4. **Political Capital Adjustment:** Winners gain, losers spend

---

## Promotion Exploitation Dynamics (#107)

Larger promotions can exploit smaller ones within governing body structures:

| Exploitation Type | Mechanism |
|-------------------|-----------|
| **Talent Drain** | Big promotions poach stars from small territories |
| **Title Favoritism** | Champions defend more often in big markets |
| **Booking Pressure** | Small promotions forced to job their talent to visitors |
| **Financial Leverage** | Dues structured to favor wealthy promotions |

### Unequal Partnership

| Partner Size | Power Dynamic |
|--------------|---------------|
| Major + Major | Equals, negotiate fairly |
| Major + Minor | Major dominates terms |
| Minor + Minor | True partnership, mutual benefit |

### Resistance Options

Smaller promotions can:
- Form alliances with other small promotions
- Go outlaw (leave governing body)
- Build political capital through loyalty
- Leverage unique talent/territory value

---

## Argument Personality Dynamics (#108)

Different promoter personalities respond differently to arguments:

| Personality Type | Reaction to Arguments |
|-----------------|----------------------|
| **Paranoid/Selfish** | Resist proposals that don't benefit them directly |
| **Pragmatic** | Can be won over with logic or cash |
| **Old School** | May favour bloodlines, tradition, legacy |
| **Cutthroat** | Will nod yes then immediately start sabotaging later |

### Argument Examples

| Argument Type | Example |
|---------------|--------|
| **Talent Value** | "Terry Funk can represent our brand with toughness and realism!" |
| **Business Case** | "Funk draws houses across the South and Japan." |
| **Financial Backing** | "We pledge to front travel costs." |
| **Legacy Appeal** | "Funk Family has history, prestige, loyalty." |

---

## Buyout Mechanics (#108) (LOCKED)

Big promotions can slowly buy up other members' influence:

### Hostile Takeover Process

| Phase | Description |
|-------|-------------|
| **Accumulation** | Buy stake in smaller promotions, acquire their debt |
| **Political Pressure** | Use board votes to squeeze targets |
| **Critical Mass** | When major promotion controls enough votes/capital |
| **Reorganization** | Federation collapses or reorganizes under new leadership |

**Example:** "You are no longer the NWA... you are now World Championship Wrestling."

### Buyout Triggers

| Condition | Vulnerability |
|-----------|---------------|
| Financial distress | High |
| Leadership vacuum | High |
| Political isolation | Medium |
| Talent exodus | Medium |
| Low political capital | Low-Medium |

---

## Performance Expectations (#108)

When you push your candidate for a title, results matter:

| Outcome | Political Effect |
|---------|------------------|
| **Your guy wins and draws badly** | Board forces quick title drop, you lose 20-40 political capital |
| **Your guy wins and performs as expected** | Neutral, maintain position |
| **Your guy overperforms** | Massive political capital gain (+30-50), may dictate multiple title runs |
| **Your guy causes scandal** | Emergency vote possible, major capital loss |

---

## Scandal Cover-Up Logic (#109)

Governing bodies help member promotions manage scandals:

| Scandal Severity | Board Response |
|------------------|----------------|
| **Minor** (kayfabe break) | Swept under rug, small fine |
| **Moderate** (backstage fight) | Private discipline, no public action |
| **Major** (criminal activity) | Public distancing, possible expulsion vote |
| **Catastrophic** (death, major crime) | Emergency session, damage control |

### Era Sensitivity

| Era | Cover-Up Tolerance |
|-----|-------------------|
| 1950s-1970s | Very high, almost anything hidden |
| 1980s | Declining, media more intrusive |
| 1990s-2000s | Limited, internet exposes quickly |
| 2010s+ | Minimal, social media prevents cover-ups |

---

## Alliance Networks

Promotions form alliances for mutual benefit:

### Alliance Types

| Type | Description |
|------|-------------|
| **Talent Sharing Pact** | Workers move freely between promotions |
| **Booking Alliance** | Joint shows, cross-promotional feuds |
| **Political Bloc** | Vote together on board issues |
| **Exclusive Partnership** | One promotion has first rights to another's talent |

### Alliance Stress

Alliances can break under pressure:
- One partner poaches key talent
- Voting against ally on important issue
- Financial disputes
- Personality clashes between owners

---

## Connected Mechanics

- [[Clique Formation]] - How backstage factions work
- [[Power Struggle Events]] - When control of promotion changes
- [[Exodus Template]] - Mass talent departures
- [[Territory System/_Territory System Index|Territory System]] - Geographic booking rights

---

## Implementation Notes

```json
{
  "governing_body_id": "nwa_1985",
  "name": "National Wrestling Alliance",
  "member_promotions": [
    {
      "promotion_id": "crockett",
      "status": "board_member",
      "political_capital": 85,
      "votes": 1
    },
    {
      "promotion_id": "wwf",
      "status": "former_member",
      "political_capital": 0,
      "notes": "Left 1983"
    }
  ],
  "pending_arguments": [
    {
      "type": "title_holder_dispute",
      "proposer": "crockett",
      "subject": "Who challenges Flair next?",
      "votes_for": ["crockett", "stl"],
      "votes_against": ["florida"]
    }
  ]
}
```

---

## Open Questions

- Exact Political Capital formulas?
- How does NWA champion booking work mechanically?
- Voting threshold for different decision types?
- How do outlaw promotions affect NWA dynamics?

---

**Document Status:** Concept Locked, Details Open
**Last Updated:** 2025-12-25
