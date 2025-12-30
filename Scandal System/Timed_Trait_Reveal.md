# Timed Trait Reveal System

📛 **NAME:** Timed Trait Reveal System
🧭 **CATEGORY:** Scandal System / World Simulation
🔑 **KEYWORDS:** historical scandals, activation dates, exposure timeline, era-appropriate knowledge
📝 **SUMMARY:** Hidden traits have historical activation dates for Strict History mode. Game start date determines what's publicly known vs hidden. Players starting in 1987 see "clean" Hogan; players starting in 2017 see the stained legacy.

⚙️ **LOGIC OVERVIEW:**
- Each hidden tag carries an optional `historical_exposure_date`
- Game start date comparison determines initial visibility
- If start date > exposure date: tag starts as Public
- If start date < exposure date: tag starts as Hidden
- In Strict History mode, exposure events trigger at historical dates
- Promotions/fans react naturally over time, not retroactively

🔬 **LLM INTEGRATION:** No (pure data/date comparison)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Hidden Traits System]] (visibility states)
- [[Alt-History Mode]] (organic alternative)
- [[Scandal System]] (fallout mechanics)
- [[Global Event Stream]] (world context for exposures)

❓ **OPEN QUESTIONS:**
- How granular should dates be? (year vs month vs exact day)
- Should some exposures have "buildup" periods before full revelation?
- How to handle disputed/unclear historical dates?

✅ **STATUS:** Locked

---

## Core Mechanics

### Date Comparison Logic

```
IF game_start_date > historical_exposure_date:
    tag.visibility = "public"
    scandal_fallout = already_calculated
ELSE:
    tag.visibility = "hidden"
    await exposure_trigger
```

### Example: Hulk Hogan Timeline

| Year | Game Start Status | Notes |
|------|-------------------|-------|
| 1987 | Racist (Hidden) | "Normal" casual racism tolerated at time; not publicly scandalous |
| 2005 | Aging Star | Still beloved by casuals; progressive fans mildly skeptical |
| 2015 | Tape Leaks | Racist Tag + Deep Racism Tag revealed publicly |
| 2016 | Fallout Year | Sponsors sever, WWE cuts ties temporarily, fanbase fractures |
| 2017+ | Stained Legacy | Starting here means tag is already public knowledge |

### Example: Chris Benoit Timeline

| Year | Status | Notes |
|------|--------|-------|
| 1995 | Beloved Workhorse | No negative traits public; minor Self-Destructive tendency hidden |
| 2000 | High Level Career | Minor CTE signs hidden, no public red flags |
| 2006 | Deepening Instability (Hidden) | Quiet backstage concerns, unseen to players |
| 2007 | Murder-Suicide Event | Hidden tags explode into public view |
| Post-2007 | Blacklisted | Starting post-2007 = all tags public, legacy destroyed |

---

## Implementation

### Tag Data Structure (Extended)

```json
{
  "tag_id": "racist_deep",
  "worker_id": "hulk_hogan",
  "visibility": "hidden",
  "strength": 85,
  "historical_exposure_date": "2015-07-24",
  "exposure_event_type": "media_leak",
  "exposure_event_description": "Sex tape with racist rant leaked to media"
}
```

### Game Start Initialization

```
FOR each worker:
    FOR each hidden_tag:
        IF tag.historical_exposure_date <= game_start_date:
            tag.visibility = "public"
            calculate_legacy_fallout(tag)
        ELSE:
            tag.visibility = "hidden"
```

---

## Gameplay Effects

| Scenario | Effect |
|----------|--------|
| Starting in Past | Only public knowledge to that year visible |
| Starting Later | Scandal-revealed tags immediately visible, legacy already altered |
| Playing Through Time | Scandals break dynamically at historical dates (Strict Mode) |
| Alternate Histories | Players can potentially prevent/accelerate exposure (Alt-History Mode) |

---

## Historical Exposure Database (Sample Entries)

| Worker | Tag | Exposure Date | Event |
|--------|-----|---------------|-------|
| Hulk Hogan | Racist (Deep) | 2015-07-24 | Sex tape leak |
| Chris Benoit | Self-Destructive Collapse | 2007-06-25 | Murder-suicide |
| Vince McMahon | Predator, Cover-Up Artist | 2022-06-15 | WSJ investigation |
| Bill DeMott | Trainee Tyrant | 2015-03-06 | Multiple complaints |
| Fabulous Moolah | Predator, Pimp | 2018-03-12 | #MeToo era revelations |
| Jerry Lawler | Various | Multiple dates | Various accusations over decades |

---

## RELATED SYSTEMS

- **[[Hidden Traits System]]:** Core visibility mechanics
- **[[Alt-History Mode]]:** Alternative to timed reveals
- **[[Scandal System]]:** Fallout calculation
- **[[Global Event Stream]]:** World context

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Build comprehensive historical exposure database
