# Hidden Traits System

📛 **NAME:** Hidden Traits System
🧭 **CATEGORY:** Worker Foundation / Scandal System
🔑 **KEYWORDS:** hidden tags, scandal exposure, trait visibility, trust, betrayal, revelation events
📝 **SUMMARY:** Certain worker tags (especially scandalous personality traits) remain hidden from the game world until triggered by specific events. Models trust, betrayal, and the shock of revelation when "beloved stars" are exposed as monsters.

⚙️ **LOGIC OVERVIEW:**
- Tags have a Visibility Flag: Public or Hidden
- Hidden tags exist but don't affect public perception until exposed
- Exposure occurs through specific trigger events (scandals, leaks, court cases, etc.)
- Once exposed, normal scandal fallout mechanics apply
- Some workers may have multiple hidden traits that expose at different times
- Workers can die or retire with hidden traits never surfacing

🔬 **LLM INTEGRATION:** Minimal (data flag system, not generation)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Scandal System]] (exposure triggers fallout)
- [[Tags System]] (tag visibility attribute)
- [[Fan Loyalty Resistance]] (post-exposure reactions)
- [[Timed Trait Reveal]] (historical activation dates)
- [[Alt-History Mode]] (organic vs scripted exposure)

❓ **OPEN QUESTIONS:**
- Should hidden traits affect backstage/locker room even when publicly hidden?
- Can workers with hidden traits be "suspected" by other workers before exposure?
- How do promotions "know" about hidden traits vs public knowledge?

✅ **STATUS:** Locked

---

## Tag Visibility System

### Visibility States

| State | Description |
|-------|-------------|
| Public | Known to game world, fans, media, sponsors |
| Hidden | Exists but unknown until exposure event |
| Suspected | (Optional) Rumors exist but no confirmation |

### Tags That Should Default to Hidden

| Category | Example Tags |
|----------|--------------|
| Scandalous Personality | Racist, Sexist, Homophobic, Transphobic, Predator, Blackmailer |
| Abusive Behavior | Abusive Trainer, Rookie Abuser, If He Dies He Dies |
| Criminal/Seedy | Seedy Operator, Abuser of Animals |
| Political/Corporate | Dirty Loyalty, Cover-Up Artist, Corruption Sympathizer |
| Mental Instability | Dangerously Intoxicated, Self-Destructive (severe), Bunker Mentality |
| Locker Room Dangers | Snake in the Grass, Self-Preserver, Powder Keg Temper |
| Decline Risks | Substance Abuse Downslide (if not publicly known) |

### Tags That Should Be Public

| Category | Examples |
|----------|----------|
| In-Ring Skills | All performance skills |
| Work Ethic | Consummate Professional, Reliable, etc. |
| Known Personality | Yapper, Storyteller, etc. (unless secret) |
| Physical Attributes | Size, style, appearance |
| Career Status | Veteran, Rising Star, etc. |

---

## Exposure Trigger Events

| Trigger | Description |
|---------|-------------|
| Scandal Event | Direct scandal breaks (assault charges, leaked content, etc.) |
| Shoot Interview | Ex-colleague airs grievances publicly |
| Locker Room Leaks | Whispers reach media, partial exposure |
| Social Media Blow-Up | Worker posts something revealing their true nature |
| Investigative Journalism | Reporter uncovers hidden behavior patterns |
| Court Cases | Legal records become public |
| Death/Retirement | Sometimes secrets emerge posthumously |
| Whistleblower | Specific worker or staff member breaks silence |

### Exposure Flow

```
[Hidden Tag Exists]
       ↓
[Exposure Trigger Event Occurs]
       ↓
[Tag Visibility → Public]
       ↓
[Scandal Fallout Mechanics Activate]
       ↓
[Fan/Sponsor/Media Reactions Calculate]
```

---

## Historical Examples

| Worker | Hidden Tag | Exposure Event | Year |
|--------|-----------|----------------|------|
| Hulk Hogan | Racist (Deep) | Sex tape leak with racist rant | 2015 |
| Chris Benoit | Self-Destructive Collapse, Severe CTE | Murder-suicide tragedy | 2007 |
| Vince McMahon | Multiple abuse/cover-up tags | WSJ investigation, legal filings | 2022 |
| Bill DeMott | Trainee Tyrant | Multiple trainee complaints go public | 2015 |

---

## Implementation Notes

### Data Structure

```json
{
  "tag_id": "racist_deep",
  "tag_name": "Racist (Deep)",
  "category": "Scandalous Personality",
  "visibility": "hidden",
  "exposure_date": null,
  "exposure_trigger": null,
  "historical_exposure_date": "2015-07-24",
  "strength": 85
}
```

### Key Fields
- `visibility`: "public" | "hidden" | "suspected"
- `exposure_date`: When tag became public (null if still hidden)
- `exposure_trigger`: What event caused exposure
- `historical_exposure_date`: For Strict History mode, when it actually happened

---

## RELATED SYSTEMS

- **[[Scandal System]]:** Handles fallout once tags are exposed
- **[[Timed Trait Reveal]]:** Historical activation dates for Strict History mode
- **[[Alt-History Mode]]:** Organic exposure rolls in sandbox play
- **[[Fan Loyalty Resistance]]:** How fans react to revelations
- **[[Tags System]]:** Core tag architecture

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Connect to Scandal Fallout mechanics, verify tag list completeness
