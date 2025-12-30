# Alt-History Mode

📛 **NAME:** Alt-History Mode
🧭 **CATEGORY:** World Simulation / Game Settings
🔑 **KEYWORDS:** alternate history, organic scandals, random injuries, sandbox, emergent storytelling
📝 **SUMMARY:** Optional game mode where scandals, injuries, and major events aren't locked to historical dates. Hidden traits may never surface, or may explode at unexpected moments based on organic factors like locker room morale, media aggressiveness, and worker behavior.

⚙️ **LOGIC OVERVIEW:**
- When enabled, historical exposure dates are disarmed
- Hidden traits roll for exposure based on in-world factors
- Injuries/health events also become probabilistic rather than scripted
- Players experience unique timelines every playthrough
- Same workers, different fates

🔬 **LLM INTEGRATION:** Minimal (roll calculations, not generation)

📌 **ORIGIN:** Vol 2 Chunk 08

📎 **CONNECTED SYSTEMS:**
- [[Hidden Traits System]] (what can be exposed)
- [[Timed Trait Reveal]] (historical alternative)
- [[Injury Risk System]] (organic health events)
- [[Global Event Stream]] (world events mode)
- [[Scandal System]] (fallout mechanics)

❓ **OPEN QUESTIONS:**
- Should major historical deaths (Owen Hart, etc.) be possible to prevent?
- How to balance "interesting chaos" vs "completely random nonsense"?
- Should some events be marked "cannot be prevented" even in alt-history?

✅ **STATUS:** Locked

---

## Mode Options

| Mode | Description |
|------|-------------|
| Strict History | Scandals/injuries happen at real dates. No deviation. |
| Alt-History: Wrestling Only | Real-world history stays accurate; wrestling world diverges freely |
| Alt-History: Full Chaos | Even world events randomized (recessions, wars, pandemics shift) |
| Mixed/Custom | Player chooses which aspects are strict vs random |

### Custom Mode Toggles

| Setting | Options |
|---------|---------|
| World Events | Strict / Random |
| Wrestling Scandals | Strict / Organic |
| Worker Injuries | Strict / Organic |
| Worker Deaths | Strict / Organic / Protected |
| Career Trajectories | Strict / Organic |

---

## Organic Scandal Exposure System

### When Alt-History Mode Enabled:

1. Hidden Tags still exist
2. Real-world exposure date is disarmed (no guarantee it happens)
3. Organic Exposure System activates
4. Monthly/quarterly exposure rolls based on in-world factors
5. If exposure hits: tag becomes public, fallout begins
6. If exposure never happens: worker may retire with secrets intact

### Exposure Roll Modifiers

| Factor | Effect on Exposure Chance |
|--------|---------------------------|
| Locker Room Morale Low | +Higher chance (leaks, resentment) |
| Media Aggressiveness High | +Higher chance (investigative reporting) |
| Dirty Loyalty Management | +Higher chance (cover-ups rot, leaks grow) |
| Whistleblower-Friendly Culture | -Lower chance (internal handling) |
| Worker High Popularity | -Lower chance (media/fans protect stars) |
| Worker Political Outbursts | +Much higher chance (talk themselves into exposure) |
| Scandal Severity | Severe tags roll more aggressively over time |

### Exposure Roll Flow

```
[Quarter Begins]
       ↓
[For Each Worker with Hidden Scandalous Tags]
       ↓
[Calculate Base Exposure Risk]
       + Locker Room Morale Modifier
       + Media Climate Modifier
       + Promotion Culture Modifier
       + Worker Behavior Modifier
       + Tag Severity Modifier
       ↓
[Roll Against Threshold]
       ↓
[Success = Exposure Event Triggered]
[Failure = Tag Remains Hidden, Slight Risk Accumulation]
```

---

## Organic Injury/Health System

### Same Philosophy for Injuries:

- Historical injuries (Pillman crash, Jumbo hepatitis) not guaranteed
- Health events roll based on:
  - Durability stat
  - Bad Luck tag
  - Wrestling style risk
  - Promotion intensity
  - Substance abuse
  - Fatigue/schedule

### Example: Brian Pillman in Alt-History

**Strict Mode:** Crash happens before October 1997 Badd Blood
**Alt-History:**
- WWF schedules lighter
- Fewer risky indie dates booked
- "High Risk Travel" roll fails (no crash)
- Pillman keeps ascending
- Maybe reaches IC title level, heel turn vs Austin later
- **Completely different life unfolds**

---

## Example Scenario: Hogan in Alt-History

### 1987 Game Start (Alt-History Mode)
- Hogan has Racist (Deep) Tag: Hidden
- No scandal guaranteed

### 2010s Simulation:
- Locker room morale stays moderate
- Hogan keeps political shit-talking quiet
- Media culture is aggressive (social media era)

### Exposure Rolls:
- 2012: Roll fails (hidden)
- 2015: Roll fails (no leak)
- 2017: Worker gives sloppy racist backstage speech at HOF after-party → new random event triggers exposure!
- Racist (Deep) Tag finally becomes public in 2017 (not 2015!)

**Result:** Different fallout, different fanbase damage, different historical path

---

## Implementation Notes

### Settings Structure

```json
{
  "game_mode": "alt_history",
  "settings": {
    "world_events": "strict",
    "wrestling_scandals": "organic",
    "worker_injuries": "organic",
    "worker_deaths": "protected",
    "career_trajectories": "organic"
  }
}
```

### Exposure Roll Calculation

```
base_risk = tag.severity_rating * 0.5
morale_mod = (100 - locker_room_morale) * 0.2
media_mod = media_aggressiveness * 0.3
behavior_mod = worker.recent_outbursts * 10
culture_mod = promotion.transparency_rating * -0.1

total_risk = base_risk + morale_mod + media_mod + behavior_mod + culture_mod
roll = random(1, 100)

IF roll <= total_risk:
    trigger_exposure_event()
```

---

## RELATED SYSTEMS

- **[[Hidden Traits System]]:** What tags can be exposed
- **[[Timed Trait Reveal]]:** Historical alternative
- **[[Injury Risk System]]:** Organic health events
- **[[Global Event Stream]]:** World events handling
- **[[Scandal System]]:** Fallout mechanics

---

**Document Status:** Locked
**Source:** Vol 2 Chunk 08
**Next Review:** Balance exposure roll numbers through playtesting
