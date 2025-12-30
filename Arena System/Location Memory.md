# Location Memory

📛 **MECHANIC:** Venue-Specific Event History
🔗 **PARENT SYSTEM:** [[_Arena System Index|Arena System]]
🧭 **CATEGORY:** Memory / History
🔑 **KEYWORDS:** location memory, venue history, callback, where it happened, arena anchor
📌 **ORIGIN:** Vol 1-4 (conceptual), Crowd Memory System (memory anchors)
✅ **STATUS:** Conceptual (needs mechanics)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1-4 | 📐 CONCEPTUAL |

---

## Overview

Location Memory tracks significant events that occurred at specific venues. When a show returns to a venue, past events become available for callbacks, affecting crowd reactions and booking opportunities. "This is where it happened" moments create powerful emotional resonance.

---

## Location Memory Types

### Match History

| What's Tracked | Duration | Callback Effect |
|----------------|----------|-----------------|
| **Title Changes** | Permanent | Major callback opportunity |
| **Classic Matches** | Years-Permanent | Prestige boost, expectations |
| **Controversial Finishes** | Years | Mixed reactions, heat |
| **Debuts/Returns** | Years | Pop on reference |
| **Retirements** | Permanent | Emotional weight |

### Storyline Events

| What's Tracked | Duration | Callback Effect |
|----------------|----------|-----------------|
| **Betrayals** | Years | Heat on callback |
| **Reunions** | Months-Years | Pop on reference |
| **Injuries** | Years | Sympathy, concern |
| **Promos** | Months-Years | Quote potential |
| **Brawls** | Months | Action association |

### Crowd Moments

| What's Tracked | Duration | Callback Effect |
|----------------|----------|-----------------|
| **Chants** | Months-Years | Can be triggered again |
| **Crowd Turns** | Years | Memory of shift |
| **Riots/Incidents** | Permanent | Caution, heat |
| **Sellouts** | Years | Prestige boost |

---

## Location Memory Mechanics

### Memory Recording

When significant event occurs:
```
Location Memory Entry = {
  venue_id,
  event_date,
  event_type,
  participants,
  emotional_intensity,
  outcome,
  memory_decay_rate
}
```

### Memory Retrieval

When show returns to venue:
```
Available Callbacks = All entries where:
  - memory_intensity > threshold (not forgotten)
  - time_since < max_memory_duration
  - relevant_workers present OR
  - anniversary/significant date
```

### Memory Decay

| Emotional Intensity | Annual Decay | Permanent Floor |
|---------------------|--------------|-----------------|
| **Legendary** | 0% | 90% |
| **High** | 5% | 50% |
| **Medium** | 10% | 20% |
| **Low** | 20% | 0% |

---

## Callback Opportunities

### Anniversary Returns

| Anniversary | Effect |
|-------------|--------|
| **1 Year** | Strong callback, fresh memory |
| **5 Years** | "Remember when" nostalgia |
| **10 Years** | Legacy callback, veteran crowd |
| **25 Years** | Historic significance |

### Participant Returns

| Scenario | Effect |
|----------|--------|
| **Same workers, same venue** | Maximum callback potential |
| **One worker returns** | Personal history callback |
| **Successor to lineage** | Legacy callback |
| **No original participants** | Commentary reference only |

### Callback Quality

| Quality | Effect |
|---------|--------|
| **Organic** | +10 to +20 pop/heat |
| **Forced** | +5, risk of feeling cheap |
| **Overdone** | -5, crowd fatigue |
| **Perfect Timing** | +15 to +30, legendary moment |

---

## Hometown Show Dynamics

When a worker performs in their hometown:

### Positive Effects

| Effect | Modifier |
|--------|----------|
| **Crowd Support** | +20% pop for faces |
| **Nuclear Heat** | +30% heat for heels |
| **Family Stories** | Promo material |
| **Local Media** | Coverage boost |

### Negative Effects

| Effect | Risk |
|--------|------|
| **Pressure** | May underperform |
| **Overexposure** | Diminishing returns |
| **Personal Distractions** | Family, friends backstage |

### Hometown Memory

| Event | Memory Duration |
|-------|-----------------|
| **Hometown title win** | Permanent |
| **Hometown loss** | Years (disappointment) |
| **Hometown betrayal** | Permanent (legendary heat) |
| **Hometown debut** | Years |

---

## Historical Examples

| Venue | Memory | Callback Potential |
|-------|--------|-------------------|
| **MSG** | Hogan/Andre | Any Hogan return |
| **Montreal** | Screwjob | Any Bret/HBK reference |
| **ECW Arena** | Every ECW moment | ECW reunion shows |
| **Korakuen** | Countless classics | Wrestling tradition |
| **Georgia Dome** | Goldberg streak | Streak references |

---

## Venue-Specific Traditions

Some venues develop ongoing traditions:

| Venue | Tradition | Effect |
|-------|-----------|--------|
| **MSG** | Main event expectations | Must deliver |
| **Korakuen** | Respectful silence | Crowd culture |
| **Philadelphia** | Hostile smart crowd | "ECW!" chants |
| **Memphis** | Lawler territory | Lawler always over |
| **Chicago** | CM Punk association | Punk chants |

---

## Connected Mechanics

- [[Arena Prestige]] - Venue significance
- [[_Crowd Memory System Index|Crowd Memory]] - Integration with main memory system
- [[_Booking Engine Index|Booking Engine]] - Callback booking
- [[_Popularity System Index|Popularity]] - Hometown bonuses

---

## Open Questions

- [ ] How many memories per venue before pruning?
- [ ] Cross-venue memory (worker-specific, not venue)?
- [ ] Venue destruction/replacement effects
- [ ] Memory inheritance (old arena → new arena)?
- [ ] Fed-specific venue memory vs. universal

---

**Document Status:** Conceptual
**Last Updated:** 2025-12-21
**Next Review:** Design memory recording mechanics
