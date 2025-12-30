# External Accidents

📛 **MECHANIC:** External Accident Events
🔗 **PARENT SYSTEM:** [[_Injury System Index|Injury System]]
🧭 **CATEGORY:** Worker Simulation
🔑 **KEYWORDS:** car crash, plane crash, freak accident, non-wrestling injury, life events
📌 **ORIGIN:** Vol 4 (locked as part of Worker Health and Injury System)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

Wrestling isn't a bubble. External life events can destroy careers: car crashes, plane crashes, bar fights, freak accidents. These random life risks spice emotional narrative, occurring rarely but with real consequences when they happen.

---

## External Accident Types

| Accident Type | Notes | Era Prevalence |
|---------------|-------|----------------|
| **Car Accidents** | Common in territory days: bad roads, overwork, drunk driving | High (Territory), Moderate (Modern) |
| **Plane Crashes** | Ric Flair (1975), other territory crash legends: kills careers or alters them permanently | High (Territory), Rare (Modern) |
| **Bar Fights** | Workers injured off-hours due to lifestyle or celebrity status | Moderate (All Eras) |
| **Gym Accidents** | Blown muscles, dropped weights, career-ruining tears | Moderate (All Eras) |
| **Domestic/Personal Incidents** | Assaults, freak accidents, self-inflicted injuries | Variable |
| **Travel Illnesses/Infections** | Food poisoning, blood infections, immune crashes during heavy tours | Moderate (Territory/Tours) |

---

## Era-Specific Risk Factors

### Territory Era (1950s-1980s)
| Risk Factor | Description |
|-------------|-------------|
| **Endless Driving** | Hundreds of miles between towns, exhausted driving |
| **Personal Planes** | Promoters and workers using small private aircraft |
| **Heavy Drinking Culture** | Drunk driving after shows normalized |
| **Limited Medical Care** | Injuries treated poorly on the road |
| **No GPS/Communication** | Getting lost, stranded, delayed |

### Modern Era (2000s-Present)
| Risk Factor | Description |
|-------------|-------------|
| **Commercial Air Travel** | Safer but delays, lost luggage stress |
| **Social Media Incidents** | Confrontations from being recognized |
| **Extreme Sports Hobbies** | Motocross, skydiving, other injury sources |
| **Training Facility Accidents** | More gyms, more gym injuries |

---

## Accident Probability

External accidents are rare but possible:

| Factor | Effect on Probability |
|--------|----------------------|
| **Era** | Territory era = higher vehicle risk |
| **Lifestyle Tags** | Hardcore Partier, Substance Abuse = higher risk |
| **Schedule Intensity** | Heavy touring = increased travel risk |
| **Personal Choices** | Dangerous hobbies, risky behavior |
| **Random** | Some accidents just happen |

### Base Monthly Probability
```
External Accident Risk = Base (0.1%) + Lifestyle Modifier + Era Modifier + Schedule Modifier

Territory Era: +0.2%
Hardcore Partier: +0.1%
Substance Issues: +0.15%
Heavy Tour Schedule: +0.1%
```

---

## Accident Outcomes

| Outcome | Description | Career Impact |
|---------|-------------|---------------|
| **Minor** | Missed time but full recovery | 2-8 weeks off |
| **Moderate** | Significant recovery needed | 2-6 months off |
| **Major** | Career-altering damage | 6+ months, permanent limitations |
| **Catastrophic** | Career-ending | Forced retirement |
| **Fatal** | Death | Legacy impact, industry ripple |

---

## Historical Examples

| Worker | Accident | Outcome |
|--------|----------|---------|
| **Ric Flair (1975)** | Plane crash | Broken back, career continued but altered |
| **Magnum T.A. (1986)** | Car accident | Career ended at peak |
| **Droz (1999)** | In-ring (but similar category) | Paralysis |
| **Perro Aguayo Jr. (2015)** | In-ring accident | Fatal |
| **Various Territory Workers** | Car crashes | Numerous minor to fatal incidents |

---

## Training Accident Subset

Rare but devastating: trainees or workers can die or be seriously injured during training:

| Risk | Description |
|------|-------------|
| **Trainee Death** | Rare, catastrophic, causes investigations |
| **Serious Training Injury** | Ends career before it starts |
| **Trainer Negligence** | Can result in trainer departure, promotion guilt |
| **Cover-Up Attempts** | Promotion may try to keep incidents quiet |

### Ripple Effects
- Loss of public trust
- Lawsuits against promotion
- Trainer departures (e.g., Hase leaving NJPW after Kensuke incident)
- Company guilt memory
- Media scrutiny

---

## Drunk Driving Mechanics

Territory and party culture create drunk driving risk:

| Factor | Effect |
|--------|--------|
| **Substance Abuse Tag** | +20% accident probability |
| **Hardcore Partier Tag** | +15% accident probability |
| **Territory Era** | Normalized, less stigma but more frequent |
| **Modern Era** | Scandal if caught, severe reputation damage |

### Consequences
- Injury (if accident occurs)
- Arrest (legal consequences, scandal)
- Promotion response (suspension, firing)
- Fan backlash (modern era especially)

---

## Connected Mechanics

- [[Injury Types]] - External accidents cause same injury types
- [[Surgery and Recovery]] - Treatment same as wrestling injuries
- [[Scandal System]] - DUI, fights can become scandals
- [[Hidden Personality]] - Lifestyle traits affect risk
- [[Contract System]] - Morality clauses may be violated

---

## Open Questions

- [ ] Exact probability tables for each accident type
- [ ] How player is notified of off-screen accidents
- [ ] Insurance/coverage for non-work injuries
- [ ] Investigation mechanics for training accidents
- [ ] Promotion liability when workers are injured traveling

---

## Implementation Notes

```json
{
  "external_accident": {
    "accident_id": "acc_001",
    "worker_id": "worker_001",
    "type": "car_accident",
    "date": "1985-03-22",
    "location": "on_road",
    "cause": "fatigue_driving",
    "severity": "moderate",
    "injuries": [
      { "type": "back_strain", "severity": "minor" },
      { "type": "whiplash", "severity": "moderate" }
    ],
    "time_off_weeks": 8,
    "permanent_impact": false,
    "scandal_generated": false,
    "legal_consequences": false,
    "promotion_response": "supportive"
  }
}
```
