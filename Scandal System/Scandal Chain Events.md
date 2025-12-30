# Scandal Chain Events

📛 **MECHANIC:** Cascading Scandal Escalation  
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]  
🧭 **CATEGORY:** Scandal Response / Risk Management  
🔑 **KEYWORDS:** scandal chain, escalation, cover-up, whistleblower, cascade, exposure, fallout  
📌 **ORIGIN:** Vol 2 Chunk 06 (Scandal Shielding expansion)  
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 2 Chunk 06 | 🔒 LOCKED |

---

## Overview

When one scandal triggers a second, larger scandal, either because of botched cover-ups, whistleblowing, media investigation, or internal rot being exposed.

**Core Truth:** Scandals almost never stay isolated. They spiderweb, like Vince's 2022 scandals reactivating old lawsuits, or the Ring Boy scandal exposing layers of WWF corruption.

---

## How Scandal Chains Work

| Phase | What Happens |
|-------|--------------|
| 1. Initial Scandal Detected | Minor or Major scandal happens (DUI, abuse, grooming, financial scandal, etc.) |
| 2. Immediate Shield Attempt | Management tries to cover it up (based on Shield Strength system) |
| 3. Chain Risk Roll | Based on severity + Shield Success + Management Behaviour, roll for "Chain Risk" chance |
| 4. Chain Event Triggers | If Chain Risk hits, a NEW scandal event emerges (whistleblower, lawsuit exposure, new story) |
| 5. Chain Escalation | New scandal causes Shield Strength to plummet, Fan Loyalty to collapse faster, sponsors/media turn harder |

---

## Chain Risk Factors

| Factor | Effect on Chain Risk |
|--------|----------------------|
| **Severity of Original Scandal** | Higher severity = Higher Chain Risk |
| **Dirty Cover-Up Artist Tag** | Increases short-term shielding, DOUBLES long-term Chain Risk if exposed |
| **Whistleblower Friendly Tag** | Decreases Chain Risk (workers trust internal handling, don't leak) |
| **Era Sensitivity** | Modern eras (2000s onward) = massive increase in Chain Risk (internet, social media, leaks) |
| **Worker Political Leanings** | Workers tagged "Whistleblower" or "Worker First Culture" more likely to leak and trigger chains |
| **Number of Witnesses** | More people know = higher chain risk |
| **Time Since Original Scandal** | Older buried scandals have lower risk until new scandal activates them |

---

## Chain Risk Calculation

```
Chain Risk % = (Base Scandal Severity × 10%) 
             + (Era Modifier)
             + (Cover-Up Modifier if cover-up attempted)
             - (Whistleblower Friendly × 15%)
             + (Dirty Cover-Up Artist × 25%)
             + (Witness Count × 5%)
```

### Era Modifier for Chain Risk

| Era | Chain Risk Modifier |
|-----|---------------------|
| Pre-1984 Territory | +0% |
| 1984-1995 National Expansion | +5% |
| 1996-2005 Internet Emergence | +15% |
| 2006-2015 Social Media Rise | +25% |
| 2016+ Always Online | +40% |

---

## Chain Event Types

When a chain triggers, roll for what type of exposure:

| Chain Type | Description | Consequences |
|------------|-------------|--------------|
| **Whistleblower Leak** | Worker or staff leaks information to media/podcast | Original scandal exposed + management complicity |
| **Lawsuit Exposure** | Legal discovery reveals additional misconduct | Original + NEW scandals enter public record |
| **Media Investigation** | Journalists dig deeper, find pattern | Series exposé, multiple scandals connected |
| **Internal Revolt** | Workers demand action publicly | Company forced to respond, divisions exposed |
| **Documentary/Podcast** | Long-form exposé gathers victims | Industry-wide reckoning, permanent damage |
| **Social Media Explosion** | Screenshots, recordings go viral | Immediate, uncontrollable, permanent |

---

## Chain Event Example

**Year:** 2025  
**Promotion:** Medium-sized national fed  
**Worker:** Midcarder caught harassing trainees backstage  
**Shield Strength:** Moderate (Dirty Loyalty, Corporate Overlord management)  
**Chain Risk:** High (modern era, severity medium-high, worker backlash high)

**Result Chain:**
1. Midcarder fired quietly
2. Whistleblower leaks firing story to major podcast
3. Investigation reveals executive enabling, unpaid backstage staff, unsafe locker room culture
4. Sponsors withdraw
5. Promotion loses TV deal within 6 months

---

## Chain Severity Escalation

Each chain event adds damage multipliers:

| Chain Level | Damage Multiplier | Description |
|-------------|-------------------|-------------|
| Single Scandal | 1.0× | Baseline damage |
| First Chain | 1.5× | Cover-up exposed |
| Second Chain | 2.5× | Pattern established |
| Third Chain+ | 4.0× | Company credibility destroyed |

---

## Preventing Chain Events

| Action | Chain Risk Reduction |
|--------|----------------------|
| Immediate transparency | -30% chain risk |
| Clean Hands management response | -20% chain risk |
| Whistleblower Friendly culture | -15% chain risk (workers trust internal handling) |
| Genuine reform measures | -25% chain risk (rebuilds trust) |
| Quick termination of perpetrator | -15% chain risk (shows accountability) |

| Action | Chain Risk INCREASE |
|--------|----------------------|
| Dirty Cover-Up Artist response | +25% chain risk |
| Threatening victims/witnesses | +40% chain risk |
| Retaliating against whistleblowers | +50% chain risk |
| Public denial when evidence exists | +35% chain risk |
| Protecting high-value perpetrators | +20% chain risk |

---

## Historical Chain Examples

| Case | Initial Scandal | Chain Events | Final Outcome |
|------|-----------------|--------------|---------------|
| **WWF Ring Boy** | Terry Garvin accusations | → Patterson exposed → McMahon sued → Congressional interest | Partial containment, long-term damage |
| **Vince McMahon 2022-2024** | Affair hush money | → More victims come forward → SEC investigation → Trafficking lawsuit | Career destruction, company sale |
| **SpeakingOut 2020** | Single accusation | → Industry-wide chain → Dozens exposed → Promotions scramble | Permanent industry shift |
| **Benoit Tragedy** | Initial death reports | → Murder-suicide revealed → Steroid/brain damage links → Congressional hearings | Complete erasure, policy changes |

---

## System Rules

| Situation | Consequence |
|-----------|-------------|
| Shield breaks naturally | Massive sudden backlash explosion, worse than if owned early |
| Shield holds successfully | Scandal fades over time (roll chance to fully "burn off" after X months) |
| Multiple scandals stack | Shield weakens dramatically with each new scandal tied to promotion |
| Loyalty drops over time | Fan loyalty erosion weakens future shields |
| "Whistleblower" Random Events | Sometimes shield is forcefully broken by leaks, even if initially successful |

---

## Connected Systems

- [[Scandal Shielding System|Star Protection System]] - Initial shielding attempts
- [[Management Behaviour Tags]] - Tags modify chain risk
- [[Era-Based Response]] - Era affects chain probability
- [[Fan Loyalty Resistance]] - Chains accelerate loyalty collapse
- [[Toxic Worker Consequences]] - Chains from keeping bad actors

---

## Implementation Notes

```json
{
  "chain_event": {
    "original_scandal_id": "scan_001",
    "chain_trigger": true,
    "chain_type": "whistleblower_leak",
    "chain_level": 1,
    "damage_multiplier": 1.5,
    "new_scandals_exposed": [
      "scan_002_enabled_culture",
      "scan_003_previous_victim"
    ],
    "fallout": {
      "sponsor_loss": ["sponsor_001", "sponsor_002"],
      "tv_deal_risk": 0.65,
      "fan_loyalty_modifier": -0.35,
      "institutional_rot_added": 25
    }
  }
}
```

---

## Open Questions

- [ ] Exact chain risk roll thresholds
- [ ] Chain prevention action implementation
- [ ] Multiple simultaneous chain paths?
- [ ] Recovery from chain events (different from single scandal recovery?)

---

**Document Status:** Locked (Vol 2 Chunk 06)  
**Last Updated:** 2025-12-26  
**Next Review:** Integrate with Crisis Response System
