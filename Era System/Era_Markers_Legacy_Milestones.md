# ERA MARKERS & LEGACY MILESTONES

📛 **NAME:** Era Markers & Legacy Milestones System  
🧭 **CATEGORY:** Federation Memory / Legacy  
🔑 **KEYWORDS:** era naming, legacy, memory, milestones, fed history, narrative anchors  
📝 **SUMMARY:**

The core memory system of your federation. Era markers are in-world terms (often fan or media-created) that name creative periods of your promotion. Legacy milestones are high-water marks that fans never forget. Together they create a living history that affects every interaction in the game.

⚙️ **LOGIC OVERVIEW:**

- Era markers emerge organically from booking choices, scandals, and tonal shifts
- You don't set era names. They happen to you.
- Legacy milestones become permanent narrative anchors
- History affects new talent signings, fan reactions, sponsor alignment, title prestige
- Announcers, workers, and fans reference eras naturally

🔬 **LLM INTEGRATION:** High (era naming, milestone commentary, historical callbacks)

📌 **ORIGIN:** Vol 3 lines 301-310

📎 **CONNECTED SYSTEMS:**
- [[Company_DNA_Evolution]] - DNA shifts trigger era transitions
- [[Major Event Inflection System]] - Major events create era boundaries
- [[Title System]] - Title prestige tied to era history
- [[Crowd Memory]] - Fans remember eras and milestones

❓ **OPEN QUESTIONS:**
- How many milestones can exist per era?
- Can eras be retroactively renamed?
- How do competing narratives (fan vs. company) resolve?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 301-310 | 🔒 LOCKED |

---

## WHAT IS AN ERA MARKER?

An Era Marker is an in-world term that names a creative period of your promotion. These aren't just year ranges. They're **emotional containers** for:

- Tone
- Identity
- Major feuds
- Booking philosophy
- Public perception

**You don't set these. They emerge organically (or are claimed after major events).**

---

## REAL WORLD EXAMPLES

| Federation | Era Marker | Trigger |
|------------|------------|---------|
| WWF | Attitude Era | Post-screwjob, Vince's heel turn, Stone Cold boom |
| AJPW | King's Road | Baba's stylistic standardization, Misawa ascendance |
| AEW | Pandemic Era | No fans, introspective storytelling, tournament-heavy |
| WCW | Russo Era | Creative chaos, swerve booking, collapse begins |
| NJPW | Tanahashi Era → Okada Era → Chaos Era | Top guy shifts, tone changes, Bullet Club era |

---

## IN-GAME EXAMPLES

- "SCS's Black Rope Period (2019-2021): Heavy betrayal arcs, minimal color, brutal endings."
- "The Grit Years: Worker-led creative, long builds, realist matches."
- "The Collapse Arc: Scandal after scandal. The fed nearly died. Some say it never recovered."
- "Network Era (TNT Run): Big money. Less freedom. Lots of pyro. Lots of firings."

---

## HOW ERA MARKERS ARE CREATED

They emerge automatically based on:

| Trigger | Effect |
|---------|--------|
| Creative overhaul (new booker, agent faction takes power) | Fans/media name the new era |
| Major scandal fallout | "Post-XYZ Era" begins |
| Union formation or collapse | DNA and morale spike/downshift |
| Tone reversal | Wholesome → Cynical, or Realist → Surreal |
| Top talent turnover | "The Worker Exodus" or "The Lost Generation" |
| Sustained identity drift | 6+ months of stable push patterns = soft era shift |

---

## ERA SNAPSHOT

At each marker transition, the system logs:

- Key talent associated
- Booking philosophy
- Notable promos/matches
- Crowd memory state
- Morale baseline
- External perception

**These influence:**
- How future talent references the past
- Whether workers feel "this is still that fed"
- How announcers frame current runs ("He's the first real star since The Fire Pit era...")

---

## LEGACY MILESTONES

These are high-water marks. Things fans never forget, no matter what comes after.

| Type | Effect |
|------|--------|
| **Match of the Era** | Referenced in storylines, promo callouts |
| **Greatest Walkout / Betrayal** | Remembered forever, can become recurring angle motif |
| **Unbreakable Title Run** | New champions always compared |
| **Notorious Firing or Exit** | Defines how fans view loyalty and power |
| **Fan Revolt / Hashtag Campaign** | Changed booking direction, now part of fed lore |
| **Line-Crossing Promo** | Revered or reviled, but never forgotten |
| **Era-Ending Moment** | "Everything changed that night." |

**Legacy Milestones are narrative anchors. They don't fade unless you overwrite them with something greater, and even then? Fans may resist.**

---

## ERA-DRIVEN DYNAMIC EFFECTS

| Area | Effect |
|------|--------|
| **New Talent Signing** | "You're not the fed from The Long Fall era anymore. Prove it." |
| **Fan Reaction** | "This match feels like the old days." Or: "We're still stuck in the Bad Push Era." |
| **Sponsor Alignment** | "We loved your Grit Era. Your current tone doesn't match our brand anymore." |
| **Title Prestige** | "This belt was buried in The Scandal Run. Do something with it." |

---

## IMPLEMENTATION NOTES

### Era Marker Structure

```json
{
  "era_id": "black_rope_period",
  "name": "The Black Rope Period",
  "year_range": {
    "start": "2019-03",
    "end": "2021-08"
  },
  "trigger": "sustained_tone_drift",
  "key_talent": ["worker_tsukasa", "worker_crane", "worker_viper"],
  "booking_philosophy": "realist",
  "emotional_tone": "nihilistic",
  "memorable_moments": [
    "The Glass Ceiling Match",
    "Tsukasa's Silent Walkout",
    "The Final Night Massacre"
  ],
  "crowd_memory_snapshot": {
    "trust": 45,
    "investment": 78,
    "fatigue": 62
  },
  "external_perception": "cult_classic"
}
```

### Legacy Milestone Structure

```json
{
  "milestone_id": "milestone_001",
  "type": "match_of_era",
  "name": "Tsukasa vs. Crane - Barbed Wire Death Match",
  "date": "2020-11-15",
  "era": "black_rope_period",
  "significance": 95,
  "referenced_count": 12,
  "associated_workers": ["worker_tsukasa", "worker_crane"],
  "narrative_hooks": [
    "Used as comparison for all subsequent deathmatches",
    "Crane references in every promo since"
  ]
}
```

---

## RELATED SYSTEMS

- **[[Company_DNA_Evolution]]:** DNA drift creates era boundaries
- **[[Major Event Inflection System]]:** Sudden events accelerate era changes
- **[[Crowd Memory]]:** Fans remember and reference eras
- **[[Title System]]:** Title prestige tied to era history

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Integration with Crowd Memory callbacks
