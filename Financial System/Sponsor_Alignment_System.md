# CUSTOM SPONSOR BUILDER & ALIGNMENT SYSTEM

📛 **NAME:** Custom Sponsor Builder & Alignment System  
🧭 **CATEGORY:** Financial / External Relations  
🔑 **KEYWORDS:** sponsor, brand alignment, advertising, money, DNA fit, red flags  
📝 **SUMMARY:**

Now that your fed has eras, scandals, and shifting DNA, it's time to let the outside money have opinions about all of it. Sponsors aren't just logos on the ring skirt: they're living forces with culture, red lines, and expectations. You're not just booking for fans anymore. You're booking with money in the room.

⚙️ **LOGIC OVERVIEW:**

- Sponsors have personality: tone preference, red/green flags, spending tier
- Alignment matrix determines sponsor happiness with your DNA
- Misalignment triggers warnings, pressure, or walkouts
- Some sponsors adapt, some don't. Some demand you adapt.
- Custom sponsor builder for advanced players and modders

🔬 **LLM INTEGRATION:** Medium (sponsor personality generation, crisis dialogue)

📌 **ORIGIN:** Vol 3 lines 308-310

📎 **CONNECTED SYSTEMS:**
- [[Company_DNA_Evolution]] - Sponsors evaluate DNA fit
- [[Era_Markers_Legacy_Milestones]] - Sponsors reference your era history
- [[Scandal System]] - Scandals trigger sponsor reactions
- [[Media System]] - Buzz and media coverage affect sponsor interest

❓ **OPEN QUESTIONS:**
- Sponsor negotiation mechanics?
- Exclusive sponsor deals?
- Sponsor-driven storyline requirements?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 308-310 | 🔒 LOCKED |

---

## BUILD-A-SPONSOR: BASE FIELDS

When creating (or generating) a sponsor, SCS uses the following core traits:

| Field | Description |
|-------|-------------|
| **Brand Type** | Energy Drink, Tech Company, Toy Line, Streaming Service, Political Org, Cult Indie Label |
| **Target Demo** | Age range, gender lean, income level, political/cultural lean |
| **Tone Preference** | Wholesome, Edgy, Rebellious, Socially Conscious, Sleek/Corporate |
| **Red Flags** | No blood, no swearing, no LGBTQ themes, no ex-cons, no political references, etc. |
| **Green Flags** | Push women's division, anti-racist themes, visibility campaigns, fan engagement |
| **Spending Tier** | Small pot, regional exposure, major TV partner, legacy partner |
| **Longevity Bias** | Do they like one-time spots, seasonal arcs, or multi-year relationships? |

---

## ALIGNMENT MATRIX (BRAND-DNA FIT)

Every sponsor has an alignment profile that interacts with your fed's:

- DNA (tone, style, morality)
- Federation Identity (scandal history, talent treatment)
- Current Era Marker (is this your Grit Era, or your Chaos Era?)

| Alignment | Impact |
|-----------|--------|
| **Strong Alignment** | Higher money, co-promotions, brand crossover gear, sponsored tournaments |
| **Partial Alignment** | They stay for visibility, but pressure you with soft notes |
| **Misalignment** | They may threaten to pull, issue warnings, or demand firings |
| **Anti-Alignment** | They may actively leak to media, fund competitors, or sponsor walkouts |

---

## SPONSOR DYNAMIC TRAITS

| Trait | Meaning |
|-------|---------|
| **Buzz Sensitivity** | Reacts to social media, trending angles, memes. Either loves it or fears it. |
| **Worker History Watch** | Won't sponsor feds who hire "certain" workers (abusers, political figures, sex offenders) |
| **Media Discipline** | Expects you to use PR templates properly. May fire you for "loose cannon" responses. |
| **Trend Adaptability** | Can evolve their red/green flags based on real-world cultural trends |

**Some will adapt. Some won't. And some may demand you adapt instead.**

---

## CUSTOM SPONSOR CREATION UI

For modders, advanced users, or late-game players:

| Editable Fields | Optional Features |
|-----------------|-------------------|
| Sponsor name + logo | Add campaign goals (e.g. "Women's Division Push" or "Latinx Showcase") |
| Brand blurb + slogan | Set PR contact tone (chummy, formal, sinister) |
| Red/green flag list | Define crisis threshold: how many scandals before they walk? |
| Tone preference slider | Set tolerance for chaos, realism, goofiness |
| Contract type (tour, show, year) | Link sponsorship to belt, team, or storyline arc |

---

## IMPLEMENTATION NOTES

### Sponsor Structure

```json
{
  "sponsor_id": "sponsor_001",
  "name": "Voltage Energy",
  "brand_type": "energy_drink",
  "target_demo": {
    "age_range": "18-34",
    "gender_lean": "male",
    "cultural_lean": "edgy_mainstream"
  },
  "tone_preference": "edgy",
  "red_flags": ["excessive_blood", "political_content", "child_endangerment"],
  "green_flags": ["high_spots", "extreme_stunts", "youth_push"],
  "spending_tier": "major_partner",
  "longevity_bias": "multi_year",
  "buzz_sensitivity": 0.8,
  "trend_adaptability": 0.6
}
```

### Sponsor-DNA Alignment Check

```json
{
  "sponsor_id": "sponsor_001",
  "fed_id": "promotion_001",
  "alignment_score": 72,
  "alignment_level": "partial",
  "concerns": [
    "DNA trending toward nihilistic (sponsor prefers edgy, not nihilistic)",
    "Recent scandal involving worker conduct"
  ],
  "action_required": "soft_warning_issued",
  "contract_status": "active_with_reservations"
}
```

---

## RELATED SYSTEMS

- **[[Company_DNA_Evolution]]:** Sponsors evaluate DNA fit constantly
- **[[Era_Markers_Legacy_Milestones]]:** Sponsors may reference era history
- **[[Scandal System]]:** Scandals trigger sponsor reactions
- **[[Financial System]]:** Sponsor money flows into fed budget

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Integration with scandal triggers
