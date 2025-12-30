# Shared Titles and Governing Bodies

📛 **MECHANIC:** NWA-Style Title Politics
🔗 **PARENT SYSTEM:** [[_Title System Index|Title System]]
🧭 **CATEGORY:** Booking / Promotion / Politics
🔑 **KEYWORDS:** NWA, governing body, shared title, board vote, political capital, territory politics
📌 **ORIGIN:** Vol 1-4 (Shared Titles and Governing Body Politics)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Some championships are jointly owned by federations of promotions, not individual companies. Winning the title for your guy feels like a revolution, not just a booking note. This system models the political warfare, board votes, and power dynamics of organizations like the NWA.

---

## Governing Body System

Promotions can join federations (alliances):

| Component | Description |
|-----------|-------------|
| **Federation Membership** | Promotions join organizations (NWA, early WWWF alliances) |
| **Shared Belts** | Some belts (World, Tag) jointly owned by federation |
| **Board of Directors** | Representatives vote on title decisions |
| **Voting Weight** | Based on promotion size, prestige, financial contribution |
| **Political Capital** | Resource spent on influence, favors, arguments |

---

## Board of Directors Mechanics

### Voting Weight Factors

| Factor | Weight Contribution |
|--------|---------------------|
| **Promotion Size** | Larger = more votes |
| **Prestige/History** | Legendary promotions carry weight |
| **Financial Contribution** | Pay more, vote more |
| **Political Leverage** | Favors owed, alliances built |
| **Champion Performance** | Past champions drawing well = credibility |

### Board Personality Types

| Personality | Behavior |
|-------------|----------|
| **Paranoid/Selfish** | Resists others' candidates; protects own interests |
| **Pragmatic** | Can be won with logic, data, or cash |
| **Old School** | Favors bloodlines, tradition, loyalty |
| **Cutthroat** | Nods yes, immediately plots sabotage |
| **Neutral** | Swings with strongest argument |

---

## Political Capital System

Every promoter has a Political Capital pool:

### Earning Political Capital

| Method | Capital Gained |
|--------|----------------|
| **Champion draws well** | +10 to +20 |
| **Hosting successful shows** | +5 per major event |
| **Supporting others' candidates** | +3 to +5 (building alliances) |
| **Financial contributions** | +5 to +10 |
| **Staying neutral in conflicts** | +2 to +3 |

### Spending Political Capital

| Action | Capital Cost |
|--------|--------------|
| **Push candidate for title** | -10 to -30 depending on opposition |
| **Block someone's candidate** | -5 to -15 |
| **Force short reign** | -20 |
| **Secure defense location** | -5 |
| **Call in favor** | Variable |

### Losing Political Capital

| Event | Capital Lost |
|-------|--------------|
| **Champion flops** | -15 to -25 |
| **Making enemies** | -5 to -10 per enemy |
| **Breaking promises** | -10 to -20 |
| **Scandal involving your guy** | -10 to -30 |
| **Losing internal vote badly** | -5 |

---

## The Argument System

Before major title decisions, players present arguments to the board:

| Argument Type | Description |
|---------------|-------------|
| **Talent Value** | "Terry Funk represents toughness and realism!" |
| **Business Case** | "Funk draws houses across the South and Japan." |
| **Financial Backing** | "We'll front travel costs." |
| **Legacy Appeal** | "Funk Family has history, prestige, loyalty." |
| **Political Alliance** | "The Southwest territories support our candidate." |

### Argument Success Factors

| Factor | Effect |
|--------|--------|
| **Promoter Charisma** | Smooth talkers (Eddie Graham) do better |
| **Data Support** | Actual drawing power matters |
| **Alliances** | Pre-arranged support helps |
| **Board Composition** | Some boards favor certain argument types |
| **Timing** | Recent successes or failures matter |

---

## Performance Expectations

### Champion Success

| Outcome | Effect |
|---------|--------|
| **Champion draws well** | Massive political capital gain |
| **Can dictate future title runs** | Multiple reigns possible |
| **Board trusts your judgment** | Future candidates easier |

### Champion Failure

| Outcome | Effect |
|---------|--------|
| **Champion draws poorly** | Board forces quick drop |
| **Lose political capital** | -15 to -25 |
| **Harder to get future candidates** | Need to rebuild trust |
| **May be pressured to pay costs** | Financial penalty |

---

## Buyouts and Hostile Takeovers

Big promotions can attempt to control federations:

| Method | Description |
|--------|-------------|
| **Buy Up Influence** | Slowly acquire voting weight |
| **Poach Members** | Convince promotions to leave or align |
| **Financial Pressure** | Outspend smaller members |
| **Critical Mass** | When dominant, federation reorganizes |

### Historical Example: NWA to WCW
Crockett (later Turner) slowly bought up influence until NWA effectively became WCW.

---

## Travelling Champion Mechanics

Shared title holders travel:

| Aspect | Details |
|--------|---------|
| **Defense Schedule** | Board determines where champion defends |
| **Travel Costs** | May be split or covered by requesting promotion |
| **Local Enhancement** | Champion elevates local faces |
| **Territory Rotation** | Champion moves to prevent staleness |
| **Escape Wins** | Close matches where champion retains |

### Travelling Champion Tags

| Tag | Description |
|-----|-------------|
| **Travelling Heel Champion** | Elite worker trusted to elevate faces while protecting title |
| **Travelling Heel Monster** | Brute who wrecks roster, builds for face toppling |

---

## Federation Collapse Triggers

What destroys governing bodies:

| Trigger | Description |
|---------|-------------|
| **Dominant Member Leaves** | Power vacuum, scramble for control |
| **Hostile Takeover Complete** | Federation absorbed by one promotion |
| **Member Rebellion** | Multiple promotions leave |
| **Financial Collapse** | Can't sustain organization |
| **Political Warfare** | Internal fighting destroys cooperation |

---

## Connected Mechanics

- [[Title Prestige]] - Shared titles have federation prestige |
- [[Promotion Dynamics]] | Inter-promotion relationships |
- [[Territory System]] | Regional politics |
- [[Contract System]] | Travelling champion logistics |

---

## Open Questions

- [ ] Exact voting weight formulas
- [ ] How new federations form
- [ ] Shared title creation mechanics
- [ ] Board meeting frequency
- [ ] Emergency title situations (injury, scandal)

---

## Implementation Notes

```json
{
  "governing_body": {
    "body_id": "nwa_001",
    "name": "National Wrestling Alliance",
    "member_promotions": ["promo_001", "promo_002", "promo_003"],
    "shared_titles": ["title_world_001", "title_tag_001"],
    "board": [
      { "promotion_id": "promo_001", "voting_weight": 25, "personality": "pragmatic" },
      { "promotion_id": "promo_002", "voting_weight": 20, "personality": "old_school" },
      { "promotion_id": "promo_003", "voting_weight": 15, "personality": "cutthroat" }
    ],
    "political_capital": {
      "promo_001": 45,
      "promo_002": 30,
      "promo_003": 25
    },
    "current_champion": {
      "title_id": "title_world_001",
      "champion_id": "worker_001",
      "sponsoring_promotion": "promo_001",
      "defense_schedule": []
    }
  }
}
```
