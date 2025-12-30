# Manager-Client Relationships

📛 **MECHANIC:** Loyalty, Bonds, and Package Deals
🔗 **PARENT SYSTEM:** [[_Manager System Index|Manager System]]
🧭 **CATEGORY:** Booking / Relationships
🔑 **KEYWORDS:** loyalty, package deal, bond, separation, morale
📌 **ORIGIN:** Vol 1-4 (Manager Loyalty Tree, Package Deals, Cornette example)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 🔒 LOCKED |

---

## Overview

Manager-client relationships are dynamic bonds that affect morale, booking, and career trajectory. Some pairings become inseparable package deals (Cornette and the Midnights), while others are temporary business arrangements. The loyalty tree tracks who managers protect, who they might sabotage, and what happens when bonds break.

---

## Relationship Types

| Type | Description | Example |
|------|-------------|---------|
| **Package Deal** | Inseparable, travel together | Cornette/Midnights |
| **Career Partnership** | Long-term, deep loyalty | Heyman/Lesnar |
| **Business Arrangement** | Professional, limited attachment | Various |
| **Convenience** | Temporary, easily dissolved | Short-term pairings |
| **Forced Pairing** | Booker-assigned, may not gel | Various |

---

## Loyalty Tree

Every manager has a loyalty tree:

| Category | Description |
|----------|-------------|
| **Protects** | Workers the manager actively supports |
| **Neutral** | No special investment |
| **Sabotages** | Workers the manager undermines |
| **Former Clients** | Past relationships, may be positive or negative |

### Loyalty Strength

| Level | Description |
|-------|-------------|
| **Absolute** | Would never betray, career-defining bond |
| **Strong** | Very loyal, would need major provocation |
| **Moderate** | Professional, can be swayed |
| **Weak** | Easily broken, business-focused |
| **Hostile** | Actively working against |

---

## Package Deals

Iconic pairings that demand joint booking:

| Feature | Description |
|---------|-------------|
| **Joint Contracts** | Must be signed together |
| **Joint Booking** | Appear together or not at all |
| **Morale Link** | One unhappy = both unhappy |
| **Separation Risk** | Breaking deal causes major fallout |

### Historical Package Deals

| Manager | Client(s) | Strength |
|---------|-----------|----------|
| **Jim Cornette** | Midnight Express | Absolute |
| **Paul Ellering** | Road Warriors | Strong |
| **Jimmy Hart** | Various (rotates) | Moderate |
| **Heyman** | ECW originals | Strong |

---

## Bond Formation

How relationships strengthen:

| Activity | Bond Increase |
|----------|---------------|
| **Successful promos** | +3 to +5 |
| **Title wins together** | +10 to +15 |
| **Feud victories** | +5 to +8 |
| **Manager takes bump** | +5 to +10 |
| **Time together** | +1 per month |
| **Shared hardship** | +10 to +15 |

### Bond Weakening

| Event | Bond Decrease |
|-------|---------------|
| **Booker separates them** | -10 to -20 |
| **Manager assigned elsewhere** | -5 to -15 |
| **Client loses faith** | -5 to -10 |
| **Backstage conflict** | -10 to -20 |
| **Manager sabotages** | -30 to -50 |

---

## Separation Consequences

When manager-client bonds break:

| Consequence | Description |
|-------------|-------------|
| **Morale Drop** | Both parties lose morale |
| **Stability Hit** | Faction stability decreases |
| **Promo Vacuum** | Client loses speaking support |
| **Heat Loss** | Less interference, less heat |
| **Career Impact** | Some workers flounder solo |

### Separation Types

| Type | Impact |
|------|--------|
| **Mutual Agreement** | Minimal damage |
| **Booker Decision** | Resentment possible |
| **Betrayal by Manager** | Major fallout, feud potential |
| **Betrayal by Client** | Manager becomes enemy |
| **Contract Issues** | Business-based, moderate impact |

---

## Manager Loyalty Factors

What affects manager loyalty:

| Factor | Effect |
|--------|--------|
| **Payment** | Money influences business-minded |
| **Success** | Winning builds loyalty |
| **Respect** | Being valued matters |
| **Creative Freedom** | Micromanagement hurts |
| **Client Attitude** | Bad clients lose managers |
| **Booker Treatment** | How promotion treats them |

---

## Multiple Clients

Managers with multiple clients:

| Scenario | Consideration |
|----------|---------------|
| **Stable Management** | Natural, all get attention |
| **Multiple Singles** | Must balance, jealousy risk |
| **Conflicting Feuds** | Can't manage both sides |
| **Priority Hierarchy** | Some clients more important |

---

## Betrayal Mechanics

Manager betrayal dynamics:

| Setup | Description |
|-------|-------------|
| **Heel Turn** | Manager turns on face client |
| **Better Offer** | Jumps to higher-profile client |
| **Revenge** | Client mistreated, manager retaliates |
| **Booking** | Scripted betrayal for story |
| **Shoot** | Real falling out |

---

## Connected Mechanics

- [[Manager Types]] - Type affects relationship style
- [[Faction System]] - Manager role in stables
- [[Contract System]] - Package deal contracts
- [[Morale System]] - Separation effects

---

## Open Questions

- [ ] Exact loyalty score thresholds
- [ ] How to model jealousy between clients
- [ ] Manager retirement from active managing
- [ ] Multi-promotion manager relationships

---

## Implementation Notes

```json
{
  "manager_relationship": {
    "manager_id": "manager_001",
    "clients": [
      {
        "worker_id": "worker_001",
        "relationship_type": "package_deal",
        "loyalty_strength": 95,
        "bond_start_date": "1985-01-01",
        "bond_history": [
          { "event": "title_win", "date": "1985-06-15", "change": +12 }
        ]
      }
    ],
    "loyalty_tree": {
      "protects": ["worker_001", "worker_002"],
      "neutral": ["worker_003"],
      "sabotages": [],
      "former_clients": ["worker_042"]
    },
    "package_deals": ["midnight_express"],
    "morale_link_active": true
  }
}
```
