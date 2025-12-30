# Public Image Impact

📛 **MECHANIC:** Scandal Public Image Effects
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]
🧭 **CATEGORY:** Worker Simulation / Media
🔑 **KEYWORDS:** reputation, public image, booking trust, fan perception, media coverage
📌 **ORIGIN:** Vol 4 (Scandal and Public Image Layer)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Scandals don't just affect backstage politics: they reshape how the entire world sees a worker. Public image impact determines media coverage intensity, fan reaction shifts, booking trust erosion, and long-term career trajectory changes.

---

## Immediate Scandal Effects

| Effect | Description |
|--------|-------------|
| **Reputation Score Drop** | Immediate numerical decrease based on severity |
| **Media Coverage Spike** | Era-dependent intensity of press/social attention |
| **Booking Trust Erosion** | Promotion's willingness to push/protect worker decreases |
| **Fan Perception Shift** | Crowd reactions change (sympathy, rejection, or morbid curiosity) |
| **Sponsor/Advertiser Risk** | Modern era: sponsors may pressure promotion to act |

---

## Reputation Score Impact

Base reputation hit by scandal severity:

| Severity | Immediate Impact | Long-Term Impact |
|----------|------------------|------------------|
| **Minor** | -5 to -10 | Recovers within months |
| **Moderate** | -15 to -25 | Recovers within 1-2 years |
| **Major** | -30 to -50 | May never fully recover |
| **Catastrophic** | -75 to -100 | Career likely destroyed |

### Modifiers
| Factor | Effect |
|--------|--------|
| **High Popularity** | Larger raw drop (more to lose) |
| **First Offense** | Slightly reduced impact |
| **Pattern of Behavior** | Multiplied impact (1.5x per prior scandal) |
| **Era** | Modern era = 1.5x multiplier due to permanence |
| **Fan Loyalty** | Devoted fans may protect reputation partially |

---

## Media Coverage Intensity

| Level | Description | Duration |
|-------|-------------|----------|
| **Minimal** | Trade press only, brief mention | 1-2 weeks |
| **Moderate** | Wrestling media, some mainstream | 2-4 weeks |
| **High** | Major mainstream coverage | 1-3 months |
| **Intense** | National/international news | 3-6 months |
| **Permanent** | Defining career moment, never forgotten | Indefinite |

### Era-Based Coverage
| Era | Coverage Pattern |
|-----|------------------|
| **Territory** | Local papers, word of mouth, kayfabe protected some |
| **National TV** | Wrestling magazines, newsletters, some TV |
| **Monday Night Wars** | Emerging internet, newsletters, tabloid TV |
| **Modern** | Instant social media, permanent record, viral spread |

---

## Booking Trust Effects

How scandals affect promotion's willingness to invest:

| Trust Level | Description | Booking Behavior |
|-------------|-------------|------------------|
| **Trusted** | No scandal concerns | Normal push consideration |
| **Cautious** | Minor scandal history | Hesitant on major investments |
| **Wary** | Moderate scandal risk | Limited to midcard, tested carefully |
| **Damaged** | Major scandal history | Jobber duty, possible release |
| **Toxic** | Catastrophic scandal | Immediate release, industry blacklist |

### Trust Recovery Timeline
| Scandal Severity | Time to Trust Recovery |
|------------------|------------------------|
| **Minor** | 3-6 months of clean behavior |
| **Moderate** | 1-2 years + redemption effort |
| **Major** | 3-5 years + significant redemption |
| **Catastrophic** | May never fully recover |

---

## Fan Perception Categories

How fans respond to scandal:

| Response Type | Description | Crowd Behavior |
|---------------|-------------|----------------|
| **Sympathetic** | Fans support worker through trouble | Cheers, forgiveness chants |
| **Disappointed** | Fans sad but not hostile | Muted reactions, wait-and-see |
| **Hostile** | Fans reject worker | Boos, "you sold out" type chants |
| **Morbid Curiosity** | Fans fascinated by trainwreck | Mixed reactions, increased attention |
| **Erased** | Fans pretend worker doesn't exist | Dead silence, no reactions |

### Fan Response Factors
| Factor | Effect |
|--------|--------|
| **Pre-scandal Fan Bond** | Strong bond = more forgiveness potential |
| **Scandal Type** | Substance abuse = sympathy; assault = hostility |
| **Worker Response** | Genuine apology = better reception |
| **Era** | Modern fans more judgmental on some issues, forgiving on others |
| **Cultural Context** | Regional/political context affects response |

---

## Promotion Response Options

How promotions react to scandal:

| Response | When Used | Effect |
|----------|-----------|--------|
| **Ignore/Protect** | Minor scandal, valuable worker | Minimal career impact |
| **Public Statement** | Moderate scandal, PR necessary | Damage control attempt |
| **Suspension** | Moderate-Major scandal | Time off, rehab/investigation |
| **Storyline Integration** | Scandal can be worked | Turn controversy into angle |
| **Quiet Release** | Major scandal, liability concern | Career disruption |
| **Public Firing** | Catastrophic scandal | PR distancing, maximum damage |
| **Erasure** | Unforgivable scandal | Removed from all media, history |

---

## Cross-Promotion Effects

Scandals follow workers:

| Scenario | Effect |
|----------|--------|
| **Leave Before Scandal Breaks** | May escape initial heat, but follows if public |
| **Hired Post-Scandal** | New promotion takes risk, may face backlash |
| **Industry-Wide Blacklist** | No major promotion will hire |
| **International Escape** | Different region may have different standards |

---

## Sponsor/Advertiser Impact

Modern era adds sponsor pressure:

| Scandal Severity | Sponsor Response |
|------------------|------------------|
| **Minor** | Monitoring, no action |
| **Moderate** | Private pressure on promotion |
| **Major** | Public distancing, ad pulls |
| **Catastrophic** | Full withdrawal, promotion forced to act |

---

## Connected Mechanics

- [[Scandal Types]] - What kind of scandal determines response
- [[Scandal Flex System]] - Long-term legacy effects
- [[Redemption Arcs]] - How to rebuild image
- [[Era-Based Response]] - Era modifies all responses
- [[Crowd Memory]] - Fan perception persistence

---

## Open Questions

- [ ] Exact reputation score formulas with all modifiers
- [ ] Media coverage duration calculations
- [ ] Sponsor relationship mechanics for modern era
- [ ] How promotion reputation affects scandal handling
- [ ] Cross-promotion information sharing mechanics

---

## Implementation Notes

```json
{
  "public_image_state": {
    "worker_id": "worker_001",
    "base_reputation": 75,
    "scandal_modifier": -20,
    "current_reputation": 55,
    "media_coverage": {
      "level": "moderate",
      "duration_remaining_weeks": 3,
      "primary_outlets": ["wrestling_press", "tabloids"]
    },
    "booking_trust": "wary",
    "fan_perception": "disappointed",
    "promotion_response": "suspension",
    "sponsor_risk": "low",
    "recovery_timeline": {
      "trust_recovery_date": "1987-01-15",
      "reputation_recovery_rate": 2
    }
  }
}
```
