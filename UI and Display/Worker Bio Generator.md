# Worker Bio Generator

📛 **NAME:** Worker Bio Generator
🧭 **CATEGORY:** UI / Display System
🔑 **KEYWORDS:** bio, profile, worker, modder, narrative, tags
📝 **SUMMARY:** System for generating and editing worker bios that feel human, reactive, and edit-friendly. Uses tags and booking memory to create living narratives without exposing raw stats.

⚙️ **LOGIC OVERVIEW:**
- Bios pull from modular components (public profile, career arc, commentary tone, flaws, edit hooks)
- Tags translate invisible ratings into lived feeling
- Dynamically assembled only when viewed or referenced
- Lightweight text files (static until triggered to refresh)
- Use tag hooks, not full stat sweeps, to build voice

🔬 **LLM INTEGRATION:** Yes — for narrative generation and tone calibration

📌 **ORIGIN:** Vol 6 (lines 494-499)

📎 **CONNECTED SYSTEMS:** Tags System, Booking Memory, Gimmick System, Commentary System

❓ **OPEN QUESTIONS:**
- Exact tag-to-narrative translation rules
- How often bios refresh
- Modder editing interface design

✅ **STATUS:** Conceptual (needs implementation spec)

---

## Design Goal

**Modular, believable, easy to edit.**

- Hints at rating-based behavior without saying "Drive: 20, Paranoia: 17"
- Reflects Booking Memory, Gimmick Drift, and Tag Influence
- Looks like a Wikipedia blurb, but smarter

---

## Bio Sections

### Section 1: Public Profile

**What fans see in menus, cards, fan pages.**

> "Once a bitter underdog with a loaded lariat, now a multi-time champion known for unpredictable aggression and big-match charisma. Famously walked out of the GWA in '83, only to return three months later with a sledgehammer and no apology. Most recently working slower, heavier matches while anchoring the next generation."

**Inputs (under the hood):**
- Booking memory: belt wins, face/heel shifts, match types
- Core skills: Charisma, Psychology, Brawling
- Tags: `Hardcore Comfort`, `Booking Walkout`, `Main Event Resilience`

---

### Section 2: Career Arc Snapshot

**Auto-generated one-liner based on trajectory.**

Examples:
- "From war dog to reluctant leader."
- "Bounced between brilliance and burnout — and made both draw money."
- "Built from scars, still wrestling like no one paid him yet."

**Inputs:**
- Match history momentum (hot streaks, title droughts, crowd pops)
- Tags like `Burnout Risk`, `Locker Room Loner`, `Franchise Workhorse`
- Gimmick Drift score pushes tone from "sharp" to "theatrical" when needed

---

### Section 3: Commentary Tone (External Voice)

**How commentators describe them.**

Examples:
- "You never know what version's walking down that ramp — but it'll be loud, and it'll hurt."
- "Still swings like he's proving something. Maybe he is."
- "One of the last guys the crowd really believes in — even when he's clearly bleeding for someone else's story."

**Inputs:**
- Believability score + Tag blend
- Gimmick subtype (e.g. `Defiant Soul`, `Antihero Bastard`, `Brawling Everyman`)
- Can be customized per alliance:
  - GWA might say: "He's money every time."
  - PWU might say: "He's a ghost with endorsements."

---

### Section 4: Flaws & Faultlines (Soft Warnings)

**Hinted via tone, not stated outright.**

Examples:
- "Highly respected. Occasionally volatile. Quietly known for walking if the room turns on him."
- "A traditionalist at heart, for better or worse."
- "Few challenge him. Fewer last long when they do."

**Inputs:**
- Personality ratings (Paranoia, Traditionalism, Ego)
- Tags like `Politicking Risk`, `Authority Conflict`, `Quiet Divider`
- Automatically softens if Popularity + Loyalty + Morality is high
- Escalates if multiple workers "refuse to work with" in memory logs

---

### Section 5: Edit Hooks (Modder Fields)

**For modders or players to write in specific character touches or story flavor.**

| Field | Example |
|-------|---------|
| **Nickname history** | The Blacksmith, The Hollow Hand, "Midnight Gospel" |
| **Infamous quote** | "I don't rehearse violence. I just try not to stutter." |
| **Known finishers** | "Broken Mercy" (avalanche piledriver), "Bleed on Me" (standing headbutt flurry into flash KO) |

---

## Handling Problematic Figures

**Realism without dropping anvils.**

Esther, Clint, and similar figures should not be presented as "Villain: Press A to Hate."

Instead, let subtext, worker gossip, and booking behavior tell the story.

**Tools for Subtle Framing:**
- Commentary Shifts — Workers may call them out in promo, fans may react oddly to their presence
- Worker Bios Say Things Like:
  - "Clint has been called 'traditional' and 'divisive' in equal measure."
  - "Esther's era of control is seen as both legendary… and increasingly controversial."
- Gimmick Resistance Tags — e.g. Black workers pushed despite DTW resistance, Queer wrestlers redlined in certain towns

**Let history and contradiction shape them, not exposition dumps.**

---

## Processing Efficiency

All bios are:
- Lightweight text files (static until triggered to refresh)
- Dynamically assembled only when viewed or referenced in promos/summaries
- Use tag hooks, not full stat sweeps, to build voice

---

## Related Systems

- [[SCS_BIBLE_02_TAGS_SYSTEM|Tags System]] - Core data layer
- [[Booking Memory]] - Career history
- [[Gimmick System]] - Character evolution
- [[Commentary System]] - External voice generation
