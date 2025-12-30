# Contract Types

📛 **MECHANIC:** Contract Types
🔗 **PARENT SYSTEM:** [[_Contract System Index|Contract System]]
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** handshake, per-appearance, written, guaranteed, sliding scale, unionized, CBA
📌 **ORIGIN:** Vol 4 (locked at line 70402)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Six base contract types reflecting the historical evolution of wrestling labour relations, from informal territory handshakes to modern guaranteed deals and hypothetical union contracts.

---

## Base Contract Types

| Type | Description | Use Case |
|------|-------------|----------|
| **Handshake** | Pay per appearance. No formal protection. | Classic territory model, non-TV indies |
| **Per-Appearance** | Worker paid set rate for each show | Flexible, cheap; risky for push consistency |
| **Written (Time-Locked)** | Standard term (30, 90, 365 days, etc.) | Major TV feds; includes default creative clauses |
| **Guaranteed** | Paid whether booked or not | 90s WCW disaster fuel. High cost, high trust |
| **Sliding Scale** | Base rate + bonus per match or crowd draw | Indie and rising star bridges |
| **Unionized Written** | Bound by CBA. Termination requires just cause + grievance review | No more carny firings |

---

## Type Details

### Handshake Deal
- **Protection Level:** None
- **Termination:** Immediate, no notice required
- **Historical Model:** Territory era, CMLL culture
- **Risk:** Worker can leave anytime; promotion can fire anytime
- **Era Availability:** All eras (common pre-1990s, rare post-2000s)

### Per-Appearance Contract
- **Protection Level:** Minimal
- **Termination:** Simply stop booking
- **Use Case:** Testing new talent, fill-in wrestlers, part-timers
- **Risk:** No guarantee of consistent work or push
- **Era Availability:** All eras

### Written Contract (Time-Locked)
- **Protection Level:** Moderate
- **Termination:** Breach or buyout required
- **Standard Terms:** 30-day, 90-day, 1-year, multi-year
- **Default Clauses:** Exclusivity, dates minimum, creative direction
- **Era Availability:** Post-1980s TV era standard

### Guaranteed Contract
- **Protection Level:** High
- **Termination:** Full payout owed (or negotiated settlement)
- **Historical Model:** WCW's bloated roster 1996-2001
- **Risk:** Can destroy promotion finances if workers aren't used
- **Era Availability:** Rare; primarily 1990s-present major promotions

### Sliding Scale Contract
- **Protection Level:** Variable
- **Structure:** Base rate + performance bonuses
- **Bonus Triggers:** Per match, per crowd size, per merch sales
- **Use Case:** Rising stars proving themselves, indie-to-TV transitions
- **Era Availability:** All eras (increasingly common modern era)

### Unionized Written Contract
- **Protection Level:** Maximum
- **Termination:** Just cause required + grievance review process
- **CBA Features:** Tiered pay scales, contract minimums, benefits
- **Historical Model:** Never existed in wrestling (Ventura tried, Hogan snitched)
- **Era Availability:** Only if union successfully forms in simulation

---

## Contract Duration Standards

| Term | Typical Use |
|------|-------------|
| 30 days | Try-out periods, short-term fill-ins |
| 90 days | Standard TV developmental deal |
| 1 year | Standard full roster contract |
| 2-3 years | Established stars, title holders |
| 5+ years | Rare; usually includes guaranteed money |

---

## Era-Based Contract Norms

| Era | Dominant Type | Rare Type |
|-----|---------------|-----------|
| Territory (1950s-1980s) | Handshake | Written |
| National TV (1980s-1990s) | Written (Time-Locked) | Guaranteed |
| Monday Night Wars (1996-2001) | Guaranteed | Sliding Scale |
| Post-Attitude (2002-2010s) | Written (Time-Locked) | Guaranteed |
| Modern (2010s-Present) | Mixed (Written + Guaranteed) | Unionized |

---

## Connected Mechanics

- [[Negotiation Clauses]] - Additional features added to base types
- [[Merch Cut System]] - Compensation clause affecting contract value
- [[Firing System]] - Termination rules vary by contract type
- [[Loyalty System]] - Contract satisfaction affects loyalty scores

---

## Open Questions

- [ ] Exact percentage distribution of contract types by promotion tier
- [ ] Contract type influence on worker morale baseline
- [ ] Multi-promotion contract rules (exclusive vs. non-exclusive)

---

## Implementation Notes

```json
{
  "contract_type": {
    "id": "written_time_locked",
    "name": "Written Contract (Time-Locked)",
    "protection_level": "moderate",
    "termination_rules": {
      "requires_buyout": true,
      "notice_period_days": 30,
      "just_cause_required": false
    },
    "era_availability": {
      "territory": "rare",
      "national_tv": "common",
      "monday_night_wars": "common",
      "modern": "standard"
    }
  }
}
```
