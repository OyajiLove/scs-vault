# Emergency Rebooking System

📛 **NAME:** Emergency Rebooking System  
🧭 **CATEGORY:** Booking System / Crisis Management  
🔑 **KEYWORDS:** no-show, walkout, emergency, rebooking, crisis, substitution, angle, scramble  
📝 **SUMMARY:** Handles real-time booking adjustments when workers no-show, walk out, get injured, or refuse to perform. Includes available rebooking tools, Crisis Management skill, and aftermath consequences.

⚙️ **LOGIC OVERVIEW:**
- Triggers when star no-shows, walks out, or becomes unavailable mid-show
- Promotion has multiple rebooking tools with varying risk/reward
- Crisis Management (promotion-level hidden stat) affects outcome quality
- Aftermath affects fan memory, worker morale, and promotion reputation
- Workers who step up can gain "Company Guy" status; absentees get "Unprofessional" tag

🔬 **LLM INTEGRATION:** Yes (generate improvised angle dialogue, shoot promo content, emergency storyline justifications)

📌 **ORIGIN:** Vol 5 lines 74-81 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Worker Resistance]] - Personality determines walkout likelihood
- [[Clique_Formation_System]] - Crisis response reveals political camps
- [[Crowd_Memory]] - Emergency handling becomes fan memory
- [[Morale System]] - How crisis is handled affects locker room

❓ **OPEN QUESTIONS:**
- Exact Crisis Management skill calculation
- Integration with live show pacing engine
- Fan tolerance thresholds for improvisation

✅ **STATUS:** Locked

---

## 1. EMERGENCY TRIGGERS

| Trigger | Example |
|---------|---------|
| **Star No-Shows** | Walks out mid-show, refuses to appear, disappears day-of |
| **Star Walks Out Before Match** | Refuses to lose, quits when finish revealed |
| **Sudden Injury** | Worker hurt during previous match or backstage |
| **Backstage Fight** | Political chaos or physical altercation changes roster |
| **External Crisis** | Visa issues, travel delays, media scandals just before showtime |

---

## 2. REBOOKING TOOLS

| Option | Description | Risks |
|--------|-------------|-------|
| **Substitution** | Throw in another worker (same division/archetype preferred) | Star power drop → crowd heat collapse |
| **Angle-ify the Absence** | Create storyline ("attacked backstage," "fired on air") | Brilliant if executed well; desperate if botched |
| **Rewrite Match Structure** | Improvise triple threat, gauntlet, battle royal | Chaotic feel, may save excitement or confuse fans |
| **Cancel Segment** | Cut match, pad with promos/angles/non-wrestling | Breaks pacing; heavy penalty unless covered well |
| **Shoot Promo (Rare)** | Bold worker cuts worked-shoot about missing star | Extremely volatile; can save show or trigger scandal |
| **Worker Switcheroo** | Lower star impersonates/parodies missing star | Heat death unless perfect; angers fans and locker room |

---

## 3. CRISIS MANAGEMENT SKILL

Each promotion has a hidden **Crisis Management** attribute based on:
- Booker personality
- Locker room morale
- Past experience with chaos

| Level | Effect |
|-------|--------|
| **High** | Clean improvisation, shows survive or become legendary (Foley winning title unexpectedly) |
| **Medium** | Shows get messy but loyal fans forgive |
| **Low** | Crowds turn hostile, press buries company, workers lose faith |

---

## 4. LOCKER ROOM RESPONSE

Who steps up during emergencies (see also: [[Clique_Formation_System]]):

| Worker Type | Behavior |
|-------------|----------|
| **Backstage Leaders** | Propose fixes, rally troops |
| **Old-School Veterans** | Insist on working double duty to "save the town" |
| **Opportunists** | Politic for surprise main event slot |
| **Chaos Agents** | Exploit chaos to turn locker room against management |

---

## 5. AFTERMATH EFFECTS

### Post-Show System Effects

| Effect | Behavior |
|--------|----------|
| **Fan Memory** | Emergency improv that works = beloved folklore; failures = humiliation for years |
| **Worker Morale** | If replacements seem political, locker room splits deepen |
| **World Perception** | Repeated bungled emergencies = "disorganized" reputation |
| **Worker Reputation Shift** | Workers who step up gain "Company Guy" tag |

### Absentee Worker Fallout

| Consequence | Description |
|-------------|-------------|
| **Contractual Breach** | Fines, suspension, potential termination |
| **Reputation Loss** | "Unprofessional" tag possible |
| **New Angles of Tension** | Storyline or real heat with home promotion |
| **Blacklisting Risk** | Other promotions may refuse to sign known no-showers |

---

## 6. PRE-MATCH RESISTANCE (WALKOUT PREVENTION)

Workers may refuse before the match happens:

| Situation | Description |
|-----------|-------------|
| **Worker Sniffs Out Plan** | Learns they'll be jobbing badly, resists before match |
| **Refusal to Show (Hogan Move)** | High Ego + Low Loyalty stars pull out last-second |
| **Negotiation Attempts** | Worker pre-negotiates ("I'll lose if you promise XYZ later") |
| **Injury Excuses** | Fake injuries to duck booking (Low Morality + High Ego) |

### Last-Second Save Options

| Option | Effect |
|--------|--------|
| **Cash Bonus** | Ego vs Bribe check; may save booking |
| **Future Promise** | Title shot, redemption arc guarantee |
| **Finish Modification** | Protect worker in defeat (DQ, distraction, protected loss) |

---

## 7. HISTORICAL EXAMPLES

| Event | Real-World Fallout |
|-------|-------------------|
| **Hansen vs Hogan (1990 AJPW/NJPW)** | Hogan backs out, leaves Hansen scrambling |
| **Warrior No-Show (WWF 1991)** | Immediate firing post-main event hostage threat |
| **Sid Vicious WCW Refusal** | Pre-show chaos, mass rewrites |
| **Jeff Jarrett WWE 1999** | Forced to pay him off day-of to drop title |
| **Scott Hall WCW Chaos** | No-shows blended with on-screen mockery, reputation death spiral |

---

## IMPLEMENTATION NOTES

```json
{
  "emergency_event": {
    "event_id": "walkout_main_event_2024",
    "trigger_type": "WALKOUT_BEFORE_MATCH",
    "missing_worker": "worker_123",
    "match_importance": "MAIN_EVENT",
    "crisis_management_level": 65,
    "rebooking_choice": "ANGLE_IFY_ABSENCE",
    "execution_quality": 78,
    "outcome": {
      "fan_reaction": "POSITIVE_SURPRISED",
      "memory_anchor": true,
      "stepping_up_workers": ["worker_456", "worker_789"],
      "company_guy_tags_awarded": ["worker_456"],
      "absentee_reputation_hit": -25
    }
  }
}
```

---

## RELATED SYSTEMS

- [[Worker Resistance]] - Walkout personality factors
- [[Clique_Formation_System]] - Crisis reveals political camps
- [[Crowd_Memory]] - Emergency handling becomes memory
- [[Worker Absentee Fallout]] - Consequences for no-showers
- [[Shoot_Promo_System]] - Emergency promo tool

---

**Document Status:** Locked  
**Source:** Vol 5 lines 74-81  
**Next Review:** Integration with live show simulation engine
