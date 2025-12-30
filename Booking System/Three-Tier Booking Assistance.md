# Three-Tier Booking Assistance

📛 **MECHANIC:** Three-Tier Booking Assistance
🔗 **PARENT SYSTEM:** [[Booking_Engine_P1-3|Booking Engine]]
🧭 **CATEGORY:** Player Assistance / AI Integration
🔑 **KEYWORDS:** booking assistance, freeform, semi-assisted, full auto, AI booker
📌 **ORIGIN:** Vol 1 Extraction #210
✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 1 | 🔒 LOCKED (concept) |

---

## Overview

Players have three modes for booking assistance, allowing them to choose their level of involvement. This accommodates different playstyles from hardcore simulationists to casual players who want to focus on specific aspects.

---

## The Three Tiers

### Tier 1: Freeform Mode

**Full Manual Control**

| Feature | Description |
|---------|-------------|
| Player Role | You are the booker |
| Match Selection | Manual selection of all participants |
| Outcomes | You decide winners/losers |
| Promos | Write or approve all segments |
| AI Support | Suggestions only, no auto-decisions |
| Difficulty | Highest learning curve |

**Best For:**
- Experienced players
- Simulation purists
- Those who want total control
- Story-focused players

**AI Provides:**
- Chemistry suggestions
- Crowd reaction predictions
- Historical context/callbacks
- Warning flags (overexposure, fatigue)

---

### Tier 2: Semi-Assisted Mode

**Collaborative Booking**

| Feature | Description |
|---------|-------------|
| Player Role | Creative director |
| Match Selection | AI suggests cards, you approve/modify |
| Outcomes | AI recommends, you decide |
| Promos | AI drafts, you edit |
| AI Support | Active assistance with final decisions yours |
| Difficulty | Medium learning curve |

**Best For:**
- Players learning the system
- Those who want guidance without autopilot
- Busy players who want efficiency
- First-time booking sim players

**AI Provides:**
- Pre-built card suggestions
- "What would happen if..." scenarios
- Promo drafts matching character DNA
- Storyline continuation recommendations
- Automatic handling of undercard

---

### Tier 3: Full Auto Mode

**AI Booker Takes Over**

| Feature | Description |
|---------|-------------|
| Player Role | Owner/Observer |
| Match Selection | AI handles completely |
| Outcomes | AI determines |
| Promos | AI generates |
| AI Support | Full autonomous operation |
| Difficulty | Lowest (spectator mode) |

**Best For:**
- Casual players
- Testing "what if" scenarios
- Running background promotions
- Learning by watching AI decisions
- Vacation mode

**Player Retains:**
- Hiring/firing decisions
- Major storyline vetoes
- Budget allocation
- Promotion philosophy settings

---

## AI Booker Personalities (#210 Expansion)

When using Semi-Assisted or Full Auto, the AI booker can have different "personalities":

| Personality | Style | Example |
|-------------|-------|---------|
| **Conservative** | Protect top stars, slow builds | Old NWA territorial style |
| **Crash TV** | Swerves, fast-paced, shock value | Vince Russo |
| **Long-Term** | Patient storytelling, callbacks | Gedo |
| **Star Factory** | Focus on building new talent | Paul Heyman |
| **Spectacle First** | Big moments over logic | Modern WWE |
| **Purist** | Workrate focus, less entertainment | Mid-2000s ROH |
| **Regional** | Territory-appropriate booking | Era-specific |

**Player Can Set:**
- AI personality at promotion level
- Different AI for different shows
- Hybrid approaches (Gedo logic with Crash TV pacing)

---

## Mode Switching

Players can switch modes at any time:

| Transition | Effect |
|------------|--------|
| Freeform → Semi | AI catches you up on storyline threads |
| Semi → Auto | AI continues your direction |
| Auto → Semi | Review AI decisions, course correct |
| Auto → Freeform | Full handoff with context briefing |

---

## Implementation Considerations

### Context Windows

| Mode | AI Context Needed |
|------|-------------------|
| Freeform | Minimal (suggestions only) |
| Semi-Assisted | Moderate (card building, promo drafts) |
| Full Auto | Maximum (all decisions, storyline tracking) |

### Performance Impact

| Mode | Processing Load |
|------|-----------------|
| Freeform | Low |
| Semi-Assisted | Medium |
| Full Auto | High |

---

## Connected Mechanics

- [[Booking_Engine_P1-3]] - Core booking systems
- [[Promo System/Promo DNA Profile|Promo DNA Profile]] - Promo generation
- [[Crowd_Memory]] - AI remembers crowd reactions
- [[Hidden_Personality]] - AI considers worker personalities

---

## Open Questions

- How does AI handle complex multi-promotion scenarios?
- Can AI personalities evolve based on success/failure?
- How detailed are the AI booker personality presets?

---

**Document Status:** Concept Locked
**Last Updated:** 2024-12-23
