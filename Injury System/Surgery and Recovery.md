# Surgery and Recovery

📛 **MECHANIC:** Surgery and Recovery System
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** surgery, recovery, healthcare, insurance, financial aid, surgical success, rehabilitation
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Surgery decisions shape lives forever. Whether a worker gets surgery depends on promotion support, personal wealth, national healthcare systems, personality traits, and desperation. Top stars see the best surgeons; jobbers may launch crowdfunding campaigns.

---

## Surgery Decision Factors

| Factor | Influence |
|--------|-----------|
| **Promotion Support** | Does the company cover surgery? (Rare in U.S. indies, more common in Japan, Mexico) |
| **Wealth/Salary** | Top stars can afford private care (Austin flying to Dr. Youngblood). Jobbers can't. |
| **National Healthcare** | Workers in Canada, Japan, UK, Australia have universal healthcare: easier access, slower timelines. |
| **Hidden Personality** | Drive, Ego, Future Planning, Morality influence decision to risk further damage or delay. |
| **Desperation Tags** | "Can't Lose My Spot" makes workers hide injuries, work hurt, rush back early. |
| **Financial Aid Requests** | Workers can ask promotion owners for help: success depends on Owner Personality. |
| **Crowdfunding** | Low-card workers may create campaigns if desperate: success depends on popularity and sympathy. |

---

## Healthcare Access by Region

| Region | System Type | Access Speed | Quality | Cost to Worker |
|--------|-------------|--------------|---------|----------------|
| **USA (Private)** | Insurance-based | Fast (if covered) | Top-tier available | High without coverage |
| **USA (Indie)** | None/Self-pay | Depends on funds | Variable | Catastrophic |
| **Japan** | Universal + Private | Moderate | High | Low-Moderate |
| **Mexico** | Mixed | Variable | Mixed | Low-Moderate |
| **UK/Canada** | Universal | Slow (waitlists) | Good | None |
| **Australia** | Universal + Private | Moderate | Good | None-Moderate |

### U.S. Healthcare Reality
- Major promotions may cover surgery (WWE, AEW)
- Indies almost never cover anything
- Workers classified as "independent contractors" often have no insurance
- Out-of-pocket costs can be $50,000+ for major surgeries

### Canadian Healthcare Example
Worker tears ACL in Canada:
- Surgery timeline: 9-12 month wait if using public system
- Cannot afford U.S. private care out-of-pocket
- May request financial aid from major company (denied if owner is Cheap personality)
- May launch crowdfunding campaign
- Recovery delayed; compensatory injuries possible

---

## Owner Personality and Financial Aid

When workers request help paying for surgery:

| Owner Personality | Response |
|-------------------|----------|
| **Generous** | Likely to cover or subsidize |
| **Image-Obsessed** | Covers if worker is public-facing star |
| **Ruthless** | Denies unless worker is irreplaceable |
| **Cheap** | Almost always denies |
| **Family Protector** | Covers if worker is "family" |
| **Cold Calculator** | Cost-benefit analysis determines response |

---

## Crowdfunding Campaigns

When workers can't afford surgery and promotion won't help:

| Factor | Effect on Success |
|--------|-------------------|
| **Worker Popularity** | High = more donations |
| **Fan Sympathy** | Underdog/beloved workers do better |
| **Public Image** | Scandal history reduces success |
| **Promotion Rep** | Fans may boycott promotion for abandoning worker |
| **Era** | Modern era = easier crowdfunding, more visibility |

**Generic Crowdfunding Platform:** FundTogether (or era-appropriate equivalent)

---

## Recovery Timeframes

Realistic timelines based on injury type:

| Injury | Recovery Time | Surgery Required |
|--------|---------------|------------------|
| **ACL Tear** | 8-12 months | Yes |
| **Shoulder Tear** | 6 months | Usually |
| **Broken Bones** | 2-4 months | Sometimes |
| **Neck Fusion** | 12-18 months | Yes |
| **Minor Herniation** | 2-4 months | Sometimes |
| **Concussion (Moderate)** | 4-8 weeks | No |
| **Meniscus Repair** | 3-6 months | Yes |

---

## Surgical Success Rates

Not all surgeries go well:

| Outcome | Likelihood | Effect |
|---------|------------|--------|
| **Full Recovery** | Common (modern medicine) | Return to previous level |
| **Partial Recovery** | Moderate | Permanent stat reduction |
| **Complications** | Uncommon | Extended recovery, additional surgery |
| **Botched Surgery** | Rare | Career-altering, permanent damage |
| **Scar Tissue Buildup** | Moderate over multiple surgeries | Reduced flexibility, chronic pain |

### Surgical Success Factors
- Quality of surgeon (top stars access best)
- Age of worker (younger = better healing)
- Worker's physical baseline (Athleticism, Durability)
- Previous surgeries on same area (each one harder)
- Post-surgery rehabilitation compliance

---

## Delayed Surgery Risks

Workers who refuse or delay surgery face:

| Risk | Description |
|------|-------------|
| **Increased Future Injury Risk** | Damaged area more vulnerable |
| **Permanent Stat Loss** | Durability, Stamina, Mobility degradation |
| **Chronic Pain** | Ongoing morale and performance penalty |
| **Catastrophic Failure** | Working through injury leads to worse break |
| **Compensatory Damage** | Protecting one area damages another |

---

## Surgery Decision Mechanics

```
Surgery Decision = f(Financial Access, Personality, Booking Pressure, Severity)

If Financial Access = True AND Severity >= Moderate:
  → Surgery recommended
  
If Financial Access = False:
  → Crowdfund, Request Aid, or Work Through It
  
Hidden Personality Modifiers:
- High Drive: More likely to work through injury
- High Future Planning: More likely to get surgery
- High Ego: May refuse surgery to not look weak
- Can't Lose My Spot tag: Delays surgery, rushes return
```

---

## Example Scenario

**Worker:** Indie midcarder, Canadian, tears ACL

1. Surgery timeline in Canada: 9-12 month wait (public system)
2. Cannot afford U.S. private care out-of-pocket
3. Requests financial aid from major company: **Denied** (Owner is Cheap personality)
4. Launches FundTogether campaign: **Semi-successful** (fans respect workrate)
5. Recovery delayed; re-injures meniscus compensating during return
6. **Emotional arc:** Pain, resilience, forgotten dream... or tragic burnout

*These forks are real storytelling moments. Not fake pop-ups. Lives happen for real.*

---

## Connected Mechanics

- [[Injury Types]] - Determines what surgery is needed
- [[Contract System]] - Promotion support based on contract type
- [[Financial System]] - Surgery costs, worker wealth
- [[Hidden Personality]] - Decision-making factors
- [[Addiction Risk System]] - Working through injury increases painkiller use

---

## Open Questions

- [ ] Exact cost tables for surgeries by region and era
- [ ] Crowdfunding success probability formulas
- [ ] Surgeon quality tiers and availability
- [ ] Post-surgery rehabilitation mechanics
- [ ] Insurance mechanics for promotion-covered workers

---

## Implementation Notes

```json
{
  "surgery_event": {
    "worker_id": "worker_001",
    "injury_id": "inj_001",
    "surgery_type": "acl_repair",
    "date": "1985-08-20",
    "location": "usa_private",
    "surgeon_quality": "elite",
    "funding_source": "promotion_covered",
    "cost": 45000,
    "outcome": "full_recovery",
    "recovery_weeks": 38,
    "complications": [],
    "return_date": "1986-05-15",
    "permanent_impact": {
      "mobility_penalty": 0,
      "reinjury_risk_modifier": 1.2
    }
  }
}
```
