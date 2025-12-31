# Push Gap

📛 **NAME:** Push Gap
🧭 **CATEGORY:** Push System / Detection Mechanic
🔑 **KEYWORDS:** push gap, overpush, organic popularity, manufactured star, threshold
📝 **SUMMARY:** The Push Gap measures the difference between how hard a promotion is pushing a worker (Push Level) and how much the crowd has organically accepted them (Organic Popularity). When this gap exceeds certain thresholds, it triggers negative states.

---

## Core Formula

**Push Gap = Push Level - Organic Popularity**

Both values are 0-100 scales.

---

## Gap Thresholds

| Gap Range | State | Crowd Response |
|-----------|-------|----------------|
| -20 to +10 | **Healthy** | Push matches popularity, crowd accepts |
| +11 to +19 | **Warning Zone** | Some resistance, "why is this person pushed?" murmurs |
| +20 to +29 | **False Popularity** | Active rejection, hostile crowds, backlash |
| +30+ | **Severe Overpush** | Nuclear heat (wrong kind), intervention required immediately |

---

## Negative Gap (Underpush)

When Organic Pop exceeds Push Level by significant margin:

| Gap | State | Effect |
|-----|-------|--------|
| -10 to -20 | **Underutilized** | Crowd frustrated, chants for worker |
| -21 to -30 | **Criminally Underbooked** | Crowd hijacks shows, "Daniel Bryan problem" |
| -31+ | **Buried Star** | Crowd may turn on company, demand change |

Underpush creates different problems covered in [[Crowd Memory]] and [[Predictability_Stakes]].

---

## Detection Timing

False Popularity doesn't trigger instantly. System requires:

- Push Gap ≥ 20 sustained for **4+ consecutive weeks**
- Brief spikes (hot angle, temporary main event) don't trigger
- Sustained overpush does

This prevents false positives from one-off spotlights.

---

## Push Level Calculation

Push Level derived from booking decisions:

| Factor | Weight | Example |
|--------|--------|---------|
| Card Position | 25% | Main event = 90-100, opener = 10-30 |
| Win Percentage | 20% | 80%+ wins = high push |
| Title Proximity | 20% | Champion = 100, challenger = 80, nowhere = 20 |
| TV/Promo Time | 15% | Long segments = high push |
| Booking Protection | 20% | Never loses clean = maximum protection |

**Simplified Formula:**
```
Push Level = (Card Position × 0.25) + (Win% × 0.20) + 
             (Title Proximity × 0.20) + (TV Time × 0.15) + 
             (Protection Score × 0.20)
```

---

## Organic Popularity

Organic Popularity = The popularity earned through:
- Crowd connection (genuine pops, not piped)
- Match quality reactions
- Character work resonance
- Merch sales (actual, not pushed)
- Social media engagement (genuine, not manufactured)

**Key Distinction:** A worker can have high Popularity from sustained booking but low *Organic* Popularity if the crowd never actually bought in.

---

## System Flags

When Push Gap reaches concerning levels, system generates warnings:

| Gap | Flag |
|-----|------|
| +15 | "Warning: [Worker] approaching overpush territory" |
| +20 | "Alert: [Worker] triggering False Popularity state" |
| +25 | "Critical: [Worker] severely overpushed, crowd hostile" |
| +30+ | "Emergency: [Worker] push is damaging promotion reputation" |

---

## Regional Variation

Different regions have different tolerance for manufactured stars:

| Region | Tolerance Modifier | Notes |
|--------|-------------------|-------|
| Japan | +5 | Company loyalty tradition, more patience |
| Mexico | +3 | Family lineage matters, some extra patience |
| US (Smart Fan Era) | 0 | Baseline, lowest tolerance |
| UK/Europe | -2 | Working class authenticity valued, less tolerance |

**Effect:** Japan triggers False Popularity at gap of 25, US at 20.

---

## Connected Mechanics

- [[False_Popularity]] - What happens when gap triggers
- [[Push_System]] - Overall push tracking
- [[Popularity System/Popularity_System|Popularity System]] - Organic Pop baseline

---

**Document Status:** Locked
**Last Updated:** 2025-12-30
