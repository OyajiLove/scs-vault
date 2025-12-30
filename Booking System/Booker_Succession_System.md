# BOOKER SUCCESSION SYSTEM

📛 **NAME:** Booker Succession System  
🧭 **CATEGORY:** Career / Federation Management  
🔑 **KEYWORDS:** succession, ouster, career mode, power transition, regime change  
📝 **SUMMARY:**

What happens when you're not the booker anymore? Whether forced resignation, scandal fallout, death, or kayfabe exit angle, this system allows the federation to continue (changed but alive) and gives the player multiple paths forward including starting fresh elsewhere.

⚙️ **LOGIC OVERVIEW:**

- Multiple triggers can end a booking reign
- Several succession paths with different power dynamics
- New regime creates new era marker and DNA recalibration
- Player can observe, apply elsewhere, start own fed, or try to reclaim
- Your first run is remembered, affecting future interactions

🔬 **LLM INTEGRATION:** High (interview dialogue, era naming, legacy callbacks)

📌 **ORIGIN:** Vol 3 lines 398-412

📎 **CONNECTED SYSTEMS:**
- [[Company_DNA_Evolution]] - Succession triggers DNA recalibration
- [[Era_Markers_Legacy_Milestones]] - New regime = new era marker
- [[Job Interview System]] - Applying for new positions
- [[Global World Mode]] - Observer mode after stepping down

❓ **OPEN QUESTIONS:**
- How long before player can attempt reclamation?
- Can AI bookers also be ousted?
- Multiple player-controlled feds simultaneously?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 398-412 | 🔒 LOCKED |

---

## SUCCESSION TRIGGERS

| Trigger | Description |
|---------|-------------|
| **Creative Collapse** | Lost the locker room, fans, sponsors, agents. Forced out. |
| **Walkout or Power Coup** | Talent factions install someone else ("The Elite Era," "The Agency Years") |
| **Retirement** | Choose to step down and hand the reins over |
| **Illness, arrest, scandal, death** | Optional or rare scripted events (based on personality profile or chosen challenge mode) |
| **Player-Driven** | Choose to "retire" and watch how others run it, or try to regain control |

---

## SUCCESSION PATHS

| Path | Result |
|------|--------|
| **Agent Elevation** | A road agent becomes booker (Patterson, Gedo, etc.). Brings their own tone. |
| **Talent Committee** | Wrestlers form collective leadership group. Democratic but slow. |
| **Network Appointee** | TV/sponsor picks someone from outside. Possibly disconnected from the business. |
| **Veteran Top Star** | Cena, Omega, Misawa types take over with legacy booking agendas. |
| **Player-Controlled Replacement** | You create or select your successor. |
| **Chaos Mode** | Nobody takes full control. Creative power struggle persists. |

---

## WHAT CHANGES WITH A NEW BOOKER?

| Area | Shift |
|------|-------|
| **DNA Drift** | New tone, pacing, match structure norms |
| **Worker Morale** | Resets partially. Some excited, others betrayed. |
| **Faction Alignment** | New cliques form, old loyalists may lose favour |
| **TV & Sponsors** | May get cold feet or reengage depending on rep |
| **Era Marker** | Automatically logs a new era |

**Example Era Names:**
- "The Redemption Run (2027-)"
- "After the Storm Era"
- "The [New Booker] Years"

---

## SYSTEM STRUCTURE

| Phase | Gameplay |
|-------|----------|
| 1. Trigger fires | Collapse threshold crossed, death angle, etc. |
| 2. Successor pool generated | Based on agent rep, talent support, external pressure |
| 3. Locker room & sponsor vote (optional) | Weighted based on loyalty, morale, power |
| 4. New regime begins | You may take over as them or step back as passive observer |
| 5. DNA recalibration begins | Players choose new tone, or it emerges organically from successor style |
| 6. Trust rebuild phase | Fan trust, agent buy-in, union activity react to the change |

---

## LEGACY SYSTEM EFFECTS

- Your first run is remembered
- If you return later (as a "surprise" or "heel return"), agents/workers react
- Fans may chant for your name long after you're gone ("BRING BACK TOMA")
- You can even run reboots where you book as yourself against your former successor

---

## PLAYER OPTIONS AFTER OUSTER

Once you lose the booking position, a crossroads screen appears:

| Option | System Response |
|--------|-----------------|
| **Apply for another booking role** | → [[Job Interview System]] |
| **Try to regain power** | Rebuild relationships, make a play |
| **Start your own promotion** | → [[Startup Promotion System]] |
| **Stay as passive observer** | → [[Global World Mode]] |
| **Retire** | Retire with legacy log |

---

## RECLAIM OLD PROMOTION

"I made this fed. They forgot that."

**How it works:**
- Create a worked shoot, backstage coup, or fan-driven pressure
- Use:
  - Agent loyalists
  - Union leverage
  - TV dissatisfaction with current product
  - Worker walkouts
- Reclaim control and reset the fed's course

**This becomes a new Era Marker:**
- "The Second Coming"
- "The Exile Returns"
- "Redemption or Ruin"

**Note:** Returning doesn't mean everything resets. Old wounds linger.

---

## IMPLEMENTATION NOTES

### Succession Event Structure

```json
{
  "succession_id": "succession_001",
  "trigger": "creative_collapse",
  "trigger_date": "2027-09-01",
  "outgoing_booker": "player_001",
  "succession_path": "agent_elevation",
  "new_booker": "agent_brennigan",
  "era_name": "The Brennigan Restoration",
  "morale_reset": {
    "excited": ["worker_rookie_01", "worker_tag_team_a"],
    "betrayed": ["worker_ace", "worker_veteran_heel"]
  },
  "dna_shift_direction": "toward_traditional"
}
```

---

## RELATED SYSTEMS

- **[[Job Interview System]]:** Applying for positions elsewhere
- **[[Global World Mode]]:** Watching the world evolve after stepping down
- **[[Startup Promotion System]]:** Building your own fed from scratch
- **[[Company_DNA_Evolution]]:** Succession triggers DNA recalibration

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Integration with AI booker collapse mechanics
