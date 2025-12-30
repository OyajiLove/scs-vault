# Coverage Mechanics

📛 **MECHANIC:** How Events Become News
🔗 **PARENT SYSTEM:** [[_Media System Index|Media System]]
🧭 **CATEGORY:** Event Processing
🔑 **KEYWORDS:** coverage, newsworthiness, story, article, report, leak, rumor, interview
📌 **ORIGIN:** Vol 1-4 (conceptual), Booking Engine (buzz references)
✅ **STATUS:** Conceptual (needs formulas)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 0.5 | Vol 1-4 | 📐 CONCEPTUAL |

---

## Overview

Not every event becomes news. Coverage Mechanics determine which events get picked up by which outlets, how stories spread, and what effects coverage has on workers and promotions.

---

## Newsworthiness Calculation

```
Newsworthiness = Event Magnitude × Outlet Interest × Access Factor × Timing Modifier
```

### Event Magnitude

| Event Type | Base Magnitude |
|------------|----------------|
| **Death** | 100 |
| **Major Scandal** | 80-95 |
| **Title Change (major)** | 60-80 |
| **Major Signing/Departure** | 50-70 |
| **Injury (serious)** | 40-60 |
| **Title Change (minor)** | 30-50 |
| **Backstage Incident** | 30-50 |
| **Regular Show** | 10-20 |
| **Routine Match** | 5-10 |

### Outlet Interest Modifier

| Outlet Type | Interest Focus | Modifier Range |
|-------------|----------------|----------------|
| **Mainstream** | Scandals, deaths, crossover | 0.5x to 2.0x |
| **Trade** | Titles, matches, profiles | 0.8x to 1.5x |
| **Dirtsheet** | Backstage, business, rumors | 1.0x to 2.0x |
| **Social Media** | Everything, reaction-worthy | 0.5x to 3.0x |

### Access Factor

| Access Level | Modifier |
|--------------|----------|
| **Exclusive** | 2.0x |
| **Early Access** | 1.5x |
| **Standard** | 1.0x |
| **Delayed** | 0.7x |
| **No Access** | 0.3x |

### Timing Modifier

| Timing | Modifier |
|--------|----------|
| **Breaking (same day)** | 1.5x |
| **Fresh (within week)** | 1.0x |
| **Old News (week+)** | 0.5x |
| **Ancient (month+)** | 0.2x |

---

## Coverage Types

### Positive Coverage

| Type | Effect |
|------|--------|
| **Match Review (positive)** | +2 to +5 pop |
| **Profile Piece** | +5 to +10 pop |
| **Title Coverage** | +3 to +8 pop |
| **Mainstream Crossover** | +10 to +20 pop |
| **Viral Moment** | +15 to +30 buzz |

### Negative Coverage

| Type | Effect |
|------|--------|
| **Scandal Exposure** | -10 to -50 pop |
| **Burial by Critics** | -5 to -15 pop |
| **Backstage Dirt** | -5 to -10 pop, +5 buzz |
| **Public Controversy** | Variable (heat or rejection) |

### Neutral Coverage

| Type | Effect |
|------|--------|
| **Industry News** | Awareness, no pop change |
| **Results Reporting** | Minimal, documentation |
| **Rumor/Speculation** | Buzz, uncertainty |

---

## Story Lifecycle

### Phase 1: Breaking

| Element | Description |
|---------|-------------|
| **Duration** | 1-3 days |
| **Buzz** | Maximum |
| **Spread** | Rapid across outlets |
| **Effect** | Immediate pop/buzz impact |

### Phase 2: Developing

| Element | Description |
|---------|-------------|
| **Duration** | 3-14 days |
| **Buzz** | High but declining |
| **Spread** | Follow-up stories |
| **Effect** | Sustained attention |

### Phase 3: Fading

| Element | Description |
|---------|-------------|
| **Duration** | 14-30 days |
| **Buzz** | Low |
| **Spread** | Minimal new coverage |
| **Effect** | Memory formation |

### Phase 4: Dormant

| Element | Description |
|---------|-------------|
| **Duration** | Indefinite |
| **Buzz** | None |
| **Spread** | None |
| **Effect** | Part of history, can resurface |

---

## Rumor & Leak Mechanics

### Rumor Sources

| Source | Credibility | Speed |
|--------|-------------|-------|
| **Worker leak** | High | Fast |
| **Office leak** | Very High | Medium |
| **Fan speculation** | Low | Instant |
| **Competitor** | Medium (biased) | Variable |

### Rumor Accuracy

```
Rumor Accuracy = Source Credibility × Information Quality × Telephone Effect
```

**Telephone Effect:** Each retelling degrades accuracy by 10-20%

### Leak Consequences

| Consequence | Trigger |
|-------------|---------|
| **Fed investigation** | Major leak traced |
| **Worker punishment** | Identified as source |
| **Story change** | Leaked plans abandoned |
| **Trust damage** | Ongoing leak culture |

---

## Interview & Press Conference

### Interview Types

| Type | Control Level | Risk |
|------|---------------|------|
| **Fed-controlled** | High | Low |
| **Trade publication** | Medium | Low |
| **Mainstream** | Low | Medium |
| **Shoot interview** | None | High |

### Press Conference Events

| Event | Purpose | Risk Level |
|-------|---------|------------|
| **Announcement** | Controlled message | Low |
| **Contract Signing** | Kayfabe event | Low |
| **Response to Scandal** | Damage control | High |
| **Shoot Situation** | Worker goes off-script | Very High |

---

## Connected Mechanics

- [[Media Outlets]] - Who covers what
- [[Era Media Landscape]] - Era-specific patterns
- [[_Scandal System Index|Scandal]] - Scandal coverage specifics
- [[_Popularity System Index|Popularity]] - Coverage effects on pop

---

## Open Questions

- [ ] Exact newsworthiness formulas
- [ ] Rumor spread simulation
- [ ] Interview skill mechanics
- [ ] Damage control success rates
- [ ] Cross-outlet story spread

---

**Document Status:** Conceptual
**Last Updated:** 2025-12-21
**Next Review:** Design newsworthiness formulas
