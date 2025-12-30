# CRIMINAL LEVERAGE & CATASTROPHIC EVENTS SYSTEM

📛 **NAME:** Criminal Leverage & Catastrophic Events  
🧭 **CATEGORY:** Backstage Politics, Worker Safety, Industry Events, Dark Content  
🔑 **KEYWORDS:** criminal leverage, blackmail, murder, death, overdose, suicide, CTE, abuse, scandal, catastrophic events, industry learning, content toggle, whistleblowing  
📝 **SUMMARY:**

This system handles events and leverage that go beyond normal backstage politics into criminal territory and industry-shaking catastrophes. It includes: criminal-grade blackmail (where exposure destroys both parties), worker deaths (all causes), career-ending injuries, abuse scandals, CTE accumulation, and the industry learning curve that follows major tragedies. This is the "dark content" layer that can be toggled based on player preference.

⚙️ **LOGIC OVERVIEW:**

- Criminal leverage operates differently from normal leverage (never expires, mutual assured destruction, extreme escape options only)
- Catastrophic events trigger permanent state changes, not reputation damage/recovery cycles
- Deaths can be caused by: substance abuse, CTE, suicide, murder, in-ring accidents, health crises
- CTE accumulation is style-specific and era-dependent
- Industry awareness evolves through tragedy (Benoit-style awakening)
- Abuse/assault scandals follow whistleblowing mechanics with power differential modifiers
- All dark content can be toggled via Content Severity setting

🔬 **LLM INTEGRATION:** Yes, HIGH (with sensitivity). LLM can generate:
- Criminal leverage confrontations
- Victim's breaking point internal monologue
- Industry response to catastrophic events
- Memorial segments and tribute shows
- Whistleblower courage/fear moments
- Post-tragedy policy announcements

📌 **ORIGIN:** Developed in Claude conversation (Dec 2024), building on Scheme Discovery system. Calibrated through historical examples (Benoit, Owen Hart, Bruiser Brody/Invader, Ring Boy Scandal, Vince allegations, Fabulous Moolah exposé). Designed with content toggle to respect player preferences while not sanitizing industry reality.

📎 **CONNECTED SYSTEMS:**
- **DISC-001: Scheme Discovery** - Criminal schemes escalate from this system
- **HIDE-001: Hidden Personality** - Drives victim breaking points and perpetrator behavior
- **HEALTH-001: Injury System** - Feeds into CTE, career-ending injuries
- **SUBSTANCE-001: Substance Abuse** - Feeds into overdose risk
- **MORALE-001: Morale System** - Suicide risk factors
- **STYLE-001: Wrestling Styles** - CTE accumulation rates
- **ERA-001: Era System** - Industry awareness levels, policy contexts

❓ **OPEN QUESTIONS:**
- Legal system depth (trials, sentencing, appeals?)
- Insurance/liability mechanics for promotions
- Worker estate/family mechanics post-death
- Memorial show booking effects

✅ **STATUS:** CODE-READY (Core mechanics specified, edge cases flagged)

---

## CONTENT SEVERITY TOGGLE

### Settings

| Mode | Deaths | Causes | Assault/Abuse | Language |
|------|--------|--------|---------------|----------|
| **Full Realism** | Yes | Specific (overdose, suicide, murder, CTE) | Fully modeled | Direct |
| **Softened** | Yes | Vague ("passed away", "health complications") | Referenced, not detailed | Indirect |
| **Kenny Mode** | Yes | Absurd ("eaten by alligator", "spontaneous combustion") | "Altercations" with suspensions | Comic |
| **Sanitized** | No | N/A (workers "retire" or "leave") | Not present | Clean |

### Implementation

```
Setting stored in: Game_Options.content_severity

All dark content checks:
IF content_severity = "sanitized" → Skip/substitute
IF content_severity = "kenny" → Use absurd alternatives
IF content_severity = "softened" → Use vague language
IF content_severity = "full_realism" → Full detail
```

### Default Recommendation

- First-time players: Softened
- Returning players: Remember last setting
- Never auto-select Full Realism (require explicit opt-in)

---

## CRIMINAL LEVERAGE

### How It Differs From Normal Leverage

| Aspect | Normal Leverage | Criminal Leverage |
|--------|-----------------|-------------------|
| Expiration | Weeks to years | Never (or statute of limitations) |
| Going public | Nullifies leverage | Destroys BOTH parties (MAD) |
| Refusal consequence | Snitch/leak, career damage | Prison, life destruction |
| Escape options | Confession, buyout, wait | Extreme measures only |
| Holder risk | Minimal | Complicity exposure |

### Criminal Leverage Sources

| Source | Example | Holder's Complicity |
|--------|---------|---------------------|
| Witnessed crime, stayed silent | Saw assault, didn't report | Accessory after the fact |
| Helped cover up crime | Bribed police, hid evidence | Active conspiracy |
| Participated in crime | Drove getaway, held victim | Co-perpetrator |
| Blackmail itself | "Pay me or I talk" | Extortion (separate crime) |

### The Ash Morrow Model

**Setup:**
```
Worker: Ash Morrow
Crime: Manslaughter (barfight, accidental death)
Witness: Used car salesman (shifty, opportunistic)
Cover-up: Salesman bribed police
Leverage holder: Salesman (now promotion owner)
Duration: Years of servitude
```

**Why Normal Escape Fails:**

| Escape Route | Why It Fails |
|--------------|--------------|
| Confess publicly | Prison for Morrow |
| Wait it out | Salesman has no reason to stop |
| Buy out | What's the price for "prison whenever I want"? |
| Kill leverage holder | More murder charges |

### Victim Options (Criminal Leverage)

| Option | Risk Level | Outcome If Successful | Outcome If Failed |
|--------|------------|----------------------|-------------------|
| **Continue compliance** | Low (immediate) | Survival but soul death | N/A |
| **Find counter-leverage** | Medium | MAD standoff, possible freedom | Holder retaliates |
| **Preemptive confession** | High | Prison, but FREE | Prison anyway |
| **Eliminate the threat** | Extreme | Freedom if clean | Murder charges |
| **Disappear** | High | Escape, lose everything | Found, worse position |
| **Legal play** | Variable | Freedom if successful | Holder warned, retaliates |
| **Build power base** | Long-term | Too valuable to burn | Holder may act before you're protected |

### Counter-Leverage Mechanics

For MAD standoff to work, victim needs dirt on holder:

| Holder Vulnerability | Example |
|---------------------|---------|
| Their own crimes | Tax fraud, assault, etc. |
| Cover-up complicity | They bribed cops too |
| Ongoing illegal activity | Drug dealing, money laundering |
| Reputation-destroying secret | Affair, hidden identity, etc. |

```
IF Victim_Counter_Leverage >= Holder_Leverage
  → MAD standoff
  → Neither can act without destroying both
  → Uneasy peace until balance shifts
```

### Compliance Meter

Criminal leverage victims accumulate compliance damage:

```
Compliance_Meter: 0-100

Increases:
  + Each demand fulfilled (+5 to +15 depending on humiliation)
  + Public humiliation (+10 to +20)
  + Forced to harm others (+15 to +25)
  + Years of servitude (+2 per year baseline)

Decreases:
  - Successful small rebellions (-5 to -10)
  - Finding allies who know (-10 to -15)
  - Holder shows weakness (-5 to -10)
```

### Breaking Point

```
Breaking_Point_Threshold = 100 - (Patience × 2) - (Hope × 2) + (Desperation × 2)

Low patience, low hope, high desperation = breaks early
High patience, high hope, low desperation = endures longer

When Compliance_Meter >= Breaking_Point_Threshold:
  → Snap Event triggers
  → AI evaluates options based on personality
  → Executes chosen path
```

### Snap Event Resolution

| Personality Factors | Likely Snap Type |
|--------------------|------------------|
| High Morality, Low Violence | Public confession route |
| Low Morality, High Violence | Elimination attempt |
| High Self-Preservation | Disappearance |
| High Connections | Legal/power play |
| Desperate + Impulsive | Chaotic (random from pool) |

### Holder Greed Spiral

Leverage holders can push too hard:

```
Holder_Greed: 0-100

Increases:
  + Each successful demand (+5 to +10)
  + Victim shows weakness (+5)
  + Holder's own desperation (+10 to +20)

Risk:
  IF Holder_Greed > 70 → Demands escalate
  IF Holder_Greed > 90 → May push victim past breaking point
```

Smart holders keep demands sustainable. Greedy/desperate holders create snap events.

---

## CATASTROPHIC EVENTS

Events that break normal mechanics and trigger permanent state changes.

### Event Types

| Event | Trigger | Immediate Effect |
|-------|---------|------------------|
| **Worker Death (Natural)** | Health crisis, age | Worker removed, memorial |
| **Worker Death (Overdose)** | Substance abuse + risk factors | Worker removed, investigation possible |
| **Worker Death (Suicide)** | Mental health crisis + risk factors | Worker removed, industry reflection |
| **Worker Death (Murder)** | Criminal action | Worker removed, perpetrator to legal system |
| **Worker Death (In-Ring)** | Match accident + risk factors | Worker removed, promotion investigation, policy changes |
| **Career-Ending Injury** | Match accident or assault | Worker forced retirement |
| **Abuse Scandal (Exposed)** | Whistleblowing success | Perpetrator consequences, promotion fallout |
| **CTE Crisis** | Accumulation threshold | Worker decline, possible death/suicide link |
| **Mass Tragedy** | Plane crash, venue disaster | Multiple deaths, industry shock |

### Death Risk Factors

#### Overdose Risk

```
Overdose_Risk = Base × Combined_Modifier

Base: 0.001 per month (very rare baseline)

Combined_Modifier = min(30, Substance_Severity × Support_Inverse × Pressure_Modifier)
  (Capped at 30x to prevent runaway probabilities)

Substance_Severity:
  - Recreational use: ×1.0
  - Regular use: ×3.0
  - Dependency: ×8.0
  - Severe addiction: ×20.0

Support_Inverse:
  - Strong support system: ×0.5
  - Average: ×1.0
  - Isolated: ×2.0
  - Enabled by environment: ×3.0

Pressure_Modifier:
  - Low pressure: ×0.8
  - Normal: ×1.0
  - High pressure (main event, contract year): ×1.5
  - Crisis (divorce, scandal, career collapse): ×3.0

Maximum monthly risk: 3% (30x cap)
```

#### Suicide Risk

```
Suicide_Risk = Base × Combined_Modifier

Base: 0.0005 per month (extremely rare baseline)

Combined_Modifier = min(50, Mental_Health × Support_Inverse × Crisis × CTE)
  (Capped at 50x to prevent runaway probabilities)

Mental_Health_Modifier:
  - No known issues: ×1.0
  - Mild depression/anxiety: ×2.0
  - Moderate mental health issues: ×5.0
  - Severe untreated: ×15.0

Support_Inverse:
  - Strong support: ×0.3
  - Average: ×1.0
  - Isolated: ×3.0

Crisis_Modifier:
  - No crisis: ×1.0
  - Career setback: ×2.0
  - Major life crisis (divorce, death in family): ×4.0
  - Multiple compounding crises: ×8.0

CTE_Modifier:
  - No CTE: ×1.0
  - Early CTE: ×2.0
  - Moderate CTE: ×4.0
  - Severe CTE: ×8.0

Maximum monthly risk: 2.5% (50x cap)
```

#### In-Ring Death Risk

```
InRing_Death_Risk = Base × Move_Danger × Worker_Condition × Safety_Culture

Base: 0.00001 per match (extremely rare)

Move_Danger:
  - Standard wrestling: ×1.0
  - High spots: ×3.0
  - Piledrivers/head drops: ×5.0
  - Unprotected chair shots: ×4.0
  - Deathmatch spots: ×10.0

Worker_Condition:
  - Healthy, well-rested: ×1.0
  - Fatigued: ×2.0
  - Working injured: ×5.0
  - Impaired (substances): ×8.0

Safety_Culture:
  - Promotion prioritizes safety: ×0.5
  - Average: ×1.0
  - "Don't be soft" culture: ×2.0
  - Negligent: ×4.0
```

### Death Event Resolution

```
1. DEATH EVENT TRIGGERS
   └── Cause determined (overdose, suicide, murder, accident, natural)

2. IMMEDIATE EFFECTS
   ├── Worker status → Deceased
   ├── Active storylines → Interrupted
   ├── Scheduled matches → Canceled/replaced
   └── Contracts → Terminated

3. INVESTIGATION (if applicable)
   ├── Overdose → Possible dealer prosecution
   ├── Murder → Criminal system activates
   ├── In-ring → Promotion liability check
   └── Suicide → No investigation, but industry reflection

4. INDUSTRY RESPONSE
   ├── Memorial shows/tributes
   ├── Moment of silence
   ├── Retirement of signature moves (sometimes)
   └── Policy discussions (if pattern emerging)

5. LONG-TERM EFFECTS
   ├── Worker legacy established
   ├── Related workers: grief modifier
   ├── Promotion reputation: hit if negligence involved
   └── Industry learning: possible policy trigger
```

---

## CTE ACCUMULATION SYSTEM

### Core Formula

```
CTE_Per_Match = 0.01 × Style_Modifier

CTE_Monthly_Accumulation = (Matches_This_Month × 0.01 × Style_Modifier) + Incident_Points - Recovery_Modifier

CTE_Score: 0-100 accumulator over career
```

**Design Note:** CTE damage comes primarily from direct head trauma (chair shots, headbutts), NOT from "hard" wrestling generally. Strong style damages necks and backs. Chair shot era damages brains.

### Style Modifiers

| Style | Modifier | Rationale |
|-------|----------|-----------|
| Unprotected Chair Shot Era (Attitude, ECW) | ×3.0 | Direct repeated head trauma, the real killer |
| Hardcore/Deathmatch | ×2.5 | Weapons to head, but not every match |
| Flying Headbutt Users | ×2.5 | Self-inflicted repeated trauma (Benoit, Dynamite Kid) |
| King's Road Head Drops (90s AJPW) | ×1.8 | Specific dangerous spots, not constant |
| Strong Style | ×1.0 | Neck damage, not brain damage |
| American Main Event (80s) | ×0.8 | Pre-chair shot era, mostly safe |
| High Flyer/Lucha | ×0.6 | Bad landing risk exists but rare |
| Technical/Mat Wrestling | ×0.5 | Controlled bumps, minimal head contact |
| Modern WWE Style (2010s+) | ×0.4 | Post-awareness protocols, banned moves |
| Comedy | ×0.3 | Minimal real impact |

**Key Insight:** The CTE epidemic wasn't "wrestling" generically. It was specifically:
- Chair shots to the head (normalized in late 90s/2000s)
- Flying headbutt as signature move
- Concussions worked through instead of rested
- "Don't be soft" culture specifically around head trauma

Strong style guys get broken necks and bad backs. Chair shot guys get CTE.

### Career Projections (Sanity Check)

| Career Path | Matches/Year | Style Mod | Per Year | 20 Year Total | Status |
|-------------|--------------|-----------|----------|---------------|--------|
| Technical, safe | 150 | ×0.5 | 0.75 | 15 | Healthy ✅ |
| High flyer/lucha | 180 | ×0.6 | 1.1 | 22 | Healthy ✅ |
| American 80s | 180 | ×0.8 | 1.4 | 28 | Healthy ✅ |
| Strong style (Misawa type) | 200 | ×1.0 | 2.0 | 40 | Early symptoms |
| Hardcore regular | 100 | ×2.5 | 2.5 | 50 | Moderate |
| Chair shot era main eventer | 200 | ×3.0 | 6.0 | 120 | Critical ✅ |
| Benoit (headbutt + chair shots) | 200 | ×2.75 | 5.5 + incidents | 110+ | Critical ✅ |

### Match Type Modifiers

| Match Type | Modifier |
|------------|----------|
| Standard singles/tag | ×1.0 |
| Cage match | ×1.3 |
| Ladder match | ×1.5 |
| Table match | ×1.3 |
| Hardcore stipulation | ×1.8 |
| Last Man Standing | ×1.5 |
| I Quit | ×1.2 |
| Deathmatch | ×2.5 |

### Specific Incidents

These are BIG moments, not routine occurrences. Most years = 0-2 incident points. Bad years = 5-10.

| Incident | CTE Points |
|----------|------------|
| Unprotected chair shot to head | +3 to +5 |
| Piledriver/head drop | +2 to +4 |
| Bad landing on head/neck | +5 to +10 |
| Knockout (legit) | +8 to +12 |
| Concussion (diagnosed, rested) | +10 to +15 |
| Concussion (worked through) | +15 to +20 |

### Recovery Modifier

```
Time_Off_Months × 0.3 = Recovery points

Maximum recovery per year: 4 points
Cannot reduce below previous floor (damage is permanent, just slows accumulation)
```

Recovery represents brain healing during rest periods, not reversing damage.

### CTE Thresholds

| Score | Status | Effects |
|-------|--------|---------|
| 0-30 | Healthy | None |
| 31-50 | Early Symptoms | Memory issues, headaches (hidden from player, worker may not know) |
| 51-70 | Moderate | Personality changes, mood swings, depression link (+modifier to suicide risk) |
| 71-85 | Severe | Significant cognitive impairment, career should end |
| 86-100 | Critical | Life-threatening, high mortality risk |

### Era Context (Pre-Awareness vs Post-Awareness)

| Era State | Effect |
|-----------|--------|
| **Pre-Awareness** | No CTE diagnosis exists in-game. Workers accumulate silently. Symptoms attributed to "being crazy" or "pills." No concussion protocols. |
| **Post-Awareness** | CTE recognized. Major promotions implement protocols. Chair shots to head banned (mostly). Workers can be diagnosed. Public pressure on safety. |

### Industry Awareness Trigger

```
IF Catastrophic_Event (murder-suicide, high-profile death)
  AND Autopsy/Investigation reveals CTE link
  AND Public attention threshold met
  → Industry_Awareness_Flag = True
  → Policy cascade begins
```

**Not era-locked.** Must be triggered by in-game events. A 1985 start has no awareness until tragedy creates it.

### Post-Awareness Policy Cascade

```
After Industry_Awareness triggers:

Major Promotions (within 1-3 months):
  - Ban unprotected chair shots to head
  - Implement concussion protocols
  - PR statements about worker safety

Mid-Size Promotions (within 6-12 months):
  - Follow major promotion lead (most)
  - Some resist ("we're not corporate")

Indies/Deathmatches:
  - May ignore entirely
  - Public pressure if high-profile

Effect on CTE Accumulation:
  - Post-awareness major promotions: -30% accumulation
  - Post-awareness compliant promotions: -20% accumulation
  - Non-compliant promotions: No change
```

---

## ABUSE/ASSAULT SCANDAL SYSTEM

### Scandal Types

| Type | Severity | Evidence Difficulty | Power Differential |
|------|----------|--------------------|--------------------|
| Harassment (verbal, non-physical) | Moderate | Medium | Moderate |
| Sexual harassment | Severe | Medium-High | High |
| Physical assault | Severe | Medium | Moderate |
| Sexual assault | Extreme | High | Extreme |
| Child abuse | Extreme | High | Extreme |
| Pattern of abuse (multiple victims) | Extreme | Medium (corroboration helps) | Extreme |

### Scandal Lifecycle

```
1. ABUSE OCCURS
   └── Victim(s) created, perpetrator flagged

2. KNOWLEDGE SPREADS (or doesn't)
   ├── Victim tells someone → Witness pool
   ├── Others notice signs → Suspicion pool
   └── Perpetrator brags/slips → Discovery pool

3. WHISTLEBLOWING DECISION
   ├── Each knowledgeable party evaluates (see Scheme Discovery whistleblowing)
   └── Power differential heavily suppresses action

4. IF REPORT MADE
   ├── Anonymous → Low evidence weight
   ├── Named → High evidence weight, high career risk
   └── Multiple accusers → Corroboration bonus

5. ACCUSATION WEIGHT CALCULATION
   └── Evidence × Corroboration × Era_Modifier × (1 / Power_Level)

6. OUTCOME DETERMINATION
   ├── Weight < Threshold → Accusation fails, accuser suffers
   ├── Weight >= Threshold → Investigation/consequences
   └── Weight >> Threshold → Career destruction for perpetrator
```

### Power Differential Effect

| Accused Power Level | Accusation Threshold | Notes |
|---------------------|---------------------|-------|
| Jobber/low card | 20 | Easy to remove |
| Midcard | 35 | Some scrutiny |
| Main eventer | 50 | "He said/she said" default |
| Locker room leader | 65 | Boys close ranks |
| Management | 80 | Active suppression |
| Owner | 95 | Near impossible without overwhelming evidence |

### Corroboration Mechanics

```
Accusation_Weight = Base_Evidence × (1 + (Additional_Accusers × 0.4)) × Era_Modifier

One accuser vs owner: 30 × 1.0 × 1.0 = 30 (fails against 95 threshold)
Five accusers vs owner: 30 × 2.6 × 1.0 = 78 (still fails, but closer)
Five accusers + documentation: 50 × 2.6 × 1.0 = 130 (succeeds)
```

### Era Modifier

| Era | Modifier | Context |
|-----|----------|---------|
| Pre-internet | ×0.6 | No platform, industry controls narrative |
| Early internet (90s-00s) | ×0.8 | Dirtsheets exist, limited reach |
| Social media era | ×1.0 | Wider reach, but also harassment |
| Post-#SpeakingOut/MeToo | ×1.3 | Public more willing to believe, corroboration culture |

### Failed Accusation Consequences

| Outcome | Effect on Accuser |
|---------|-------------------|
| Disbelieved | Reputation damage (-20 to -40), "troublemaker" label |
| Accused retaliates | Career sabotage, possible firing, blacklist |
| Legal action (defamation) | Financial ruin, career destruction |
| Partial belief | Stalemate, both damaged |

### Successful Accusation Consequences

| Perpetrator Level | Consequence |
|-------------------|-------------|
| Low-level worker | Fired immediately, possible blacklist |
| Midcard | Fired, blacklisted, public statement |
| Main eventer | "Suspended pending investigation," probably fired |
| Management | Resignation, legal exposure, promotion reputation hit |
| Owner | Legal system, promotion sale/closure possible |

### Promotion Complicity

| Promotion Response | Effect |
|--------------------|--------|
| **Didn't know** | Minor reputation hit for "not seeing signs" |
| **Should have known** | Moderate hit, negligence narrative |
| **Knew, did nothing** | Severe hit, potential legal liability |
| **Actively covered up** | Catastrophic hit, leadership must go |
| **Enabled/participated** | Promotion may not survive |

### Institutional Memory

```
IF Scandal_Exposed
  AND Promotion_Complicity >= "Knew, did nothing"
  → Permanent_Reputation_Modifier applied
  → Future accusations against this promotion get evidence bonus
  → "Pattern of abuse" narrative established
```

---

## MURDER MECHANICS

### Murder Types

| Type | Perpetrator | Victim | Trigger |
|------|-------------|--------|---------|
| Heat of passion | Worker | Worker/civilian | Rage + opportunity |
| Premeditated (leverage escape) | Leverage victim | Leverage holder | Breaking point + elimination path |
| Premeditated (rivalry) | Worker | Worker | Extreme hatred + instability |
| Murder-suicide | Worker | Family/self | CTE/mental health crisis |
| Manslaughter | Worker | Civilian | Accident during altercation |

### Murder Risk Factors

```
Murder_Risk = Base × Violence_Modifier × Stability_Modifier × Trigger_Modifier

Base: 0.0001 per month (extremely rare)

Violence_Modifier:
  - Low violence trait: ×0.3
  - Average: ×1.0
  - High violence trait: ×3.0
  - History of violence: ×5.0

Stability_Modifier:
  - Stable: ×0.5
  - Average: ×1.0
  - Unstable: ×3.0
  - In crisis: ×8.0

Trigger_Modifier:
  - No trigger: ×1.0
  - Recent severe humiliation: ×3.0
  - Criminal leverage at breaking point: ×10.0
  - CTE + mental health crisis: ×5.0
```

### Murder Event Resolution

```
1. MURDER OCCURS
   ├── Victim status → Deceased
   └── Perpetrator status → Suspect

2. INVESTIGATION
   ├── Evidence quality determined
   ├── Witnesses identified
   └── Arrest probability calculated

3. IF ARRESTED
   ├── Trial system activates
   ├── Conviction probability based on evidence
   └── Sentencing if convicted

4. IF NOT ARRESTED (escaped/unsolved)
   ├── Perpetrator continues (with paranoia modifier)
   ├── Cold case may reopen
   └── Industry suspicion

5. INDUSTRY RESPONSE
   ├── If perpetrator was known: massive scandal
   ├── If unsolved: rumors, suspicion
   └── Victim memorial
```

### Legal System (Simplified)

```
Arrest_Probability = Evidence_Quality × Investigation_Quality × Witness_Availability

Trial:
  Conviction_Probability = Evidence × Witness_Testimony × Legal_Quality_Differential

Sentencing:
  - Manslaughter: 5-15 years
  - Murder 2: 15-30 years
  - Murder 1: 25-life
  - Modifiers for circumstances
```

### Brody/Invader Case Model

```
Incident: Bruiser Brody stabbed by Invader in locker room
Evidence: High (witnesses, weapon)
Local factors: Puerto Rico, closed system, intimidation
Arrest: Yes
Trial: Yes
Conviction: Acquitted (witnesses intimidated, local politics)
Outcome: Invader continues career (in Puerto Rico), industry pariah elsewhere

System must account for:
  - Regional legal variation
  - Witness intimidation
  - Industry closing ranks (or not)
```

---

## MASS TRAGEDY EVENTS

### Types

| Event | Example | Scale |
|-------|---------|-------|
| Plane crash | 1975 plane carrying wrestling talent | Multiple deaths |
| Venue disaster | Fire, collapse, stampede | Multiple deaths, civilians too |
| Bus/car accident | Van crash on tour | 1-6 deaths typical |
| Violence at event | Shooting, bombing | Multiple deaths, civilians |

### Trigger Probability

```
Plane_Crash_Risk = Flights_Per_Year × Era_Safety_Modifier × Airline_Quality

1970s: Higher baseline risk
2020s: Lower baseline risk

Bus_Crash_Risk = Road_Miles × Driver_Fatigue × Vehicle_Quality

Tour schedules affect fatigue
Indie van life = higher risk
```

### Mass Tragedy Resolution

```
1. EVENT OCCURS
   └── Casualty list generated (weighted by who was traveling)

2. IMMEDIATE EFFECTS
   ├── All affected workers → status updated
   ├── Scheduled events → canceled
   └── Industry shock modifier

3. INDUSTRY RESPONSE
   ├── Memorial shows across promotions
   ├── Moment of silence for weeks/months
   ├── Possible policy changes (travel safety)
   └── Promotion reputation (if their negligence)

4. LONG-TERM EFFECTS
   ├── "Generation lost" narrative if young talent
   ├── Promotion may not recover (small promotions)
   └── Industry safety discussions
```

---

## DATA STRUCTURES

### Criminal Leverage Object

```json
{
  "leverage_id": "CRIM-001",
  "holder_id": "WKR-088",
  "victim_id": "WKR-045",
  "crime_type": "manslaughter",
  "crime_date": "1979-06-15",
  "holder_complicity": "cover_up",
  "secrecy_status": "secret",
  "victim_compliance_meter": 67,
  "victim_breaking_point": 75,
  "holder_greed_level": 45,
  "demands_history": [
    {"date": "1980-01-01", "demand": "job_to_holder", "complied": true},
    {"date": "1982-03-15", "demand": "public_endorsement", "complied": true}
  ],
  "counter_leverage": null,
  "escape_attempts": []
}
```

### CTE Tracker Object

```json
{
  "worker_id": "WKR-045",
  "cte_score": 58,
  "cte_status": "moderate",
  "primary_style_modifier": 3.0,
  "accumulation_history": [
    {"year": 1998, "matches": 200, "style_modifier": 3.0, "incidents": 8, "accumulated": 14},
    {"year": 1999, "matches": 220, "style_modifier": 3.0, "incidents": 12, "accumulated": 18.6}
  ],
  "diagnosed": false,
  "symptoms_visible": true,
  "last_concussion": "1999-08-22",
  "career_incidents": [
    {"date": "1998-04-15", "type": "chair_shot", "points": 4},
    {"date": "1999-01-24", "type": "concussion_worked", "points": 18}
  ]
}
```

### Catastrophic Event Object

```json
{
  "event_id": "CAT-001",
  "event_type": "worker_death",
  "subtype": "overdose",
  "date": "1988-03-15",
  "victim_ids": ["WKR-045"],
  "perpetrator_id": null,
  "location": "hotel_room",
  "investigation_status": "closed",
  "public_knowledge": true,
  "industry_response": {
    "memorials_held": true,
    "policy_changes": false,
    "awareness_triggered": false
  }
}
```

### Abuse Scandal Object

```json
{
  "scandal_id": "SCAN-001",
  "perpetrator_id": "WKR-088",
  "victim_ids": ["WKR-012", "WKR-034"],
  "abuse_type": "sexual_harassment",
  "duration": "1985-1989",
  "accusers": ["WKR-012"],
  "corroboration_level": 1.4,
  "evidence_quality": 40,
  "era_modifier": 0.8,
  "power_differential": 80,
  "accusation_weight": 44.8,
  "outcome": "failed",
  "accuser_consequences": ["reputation_damage", "blacklisted"],
  "perpetrator_consequences": []
}
```

### Industry Awareness Object

```json
{
  "awareness_type": "cte",
  "triggered": true,
  "trigger_event": "CAT-015",
  "trigger_date": "2007-06-25",
  "policy_adoption": {
    "major_promotions": "2007-08-01",
    "mid_size": "2008-01-01",
    "indies": "partial"
  },
  "accumulation_modifier": 0.7
}
```

---

## HISTORICAL VALIDATION

### Chris Benoit (2007)

- **Event:** Murder-suicide (family)
- **Contributing factors:** Severe CTE, mental health crisis, substance history
- **Industry response:** Drug policy overhaul, CTE awareness begins
- **System validation:** CTE accumulation (years of headbutts) + mental health + crisis = high risk. Murder-suicide as possible outcome. Industry awareness triggered. ✅

### Owen Hart (1999)

- **Event:** In-ring death (equipment failure)
- **Contributing factors:** Dangerous stunt, equipment negligence
- **Investigation:** Lawsuit against promotion, settled
- **Industry response:** Reduced dangerous stunts (temporarily)
- **System validation:** In-ring death from non-wrestling factor, promotion liability. ✅

### Bruiser Brody (1988)

- **Event:** Murder (stabbing)
- **Perpetrator:** Invader I
- **Evidence:** High (witnesses)
- **Outcome:** Acquittal (witness intimidation, local factors)
- **System validation:** Regional legal variation, intimidation mechanics, industry pariah status for perpetrator. ✅

### Ring Boy Scandal (1992)

- **Event:** Child abuse by ring crew
- **Power differential:** Protected by management initially
- **Corroboration:** Multiple victims eventually
- **Outcome:** Scandal exposed, perpetrators prosecuted, management survived (barely)
- **System validation:** High power threshold, corroboration required, promotion complicity damaged but didn't destroy. ✅

### Vince McMahon Allegations (2022-2024)

- **Event:** Sexual misconduct allegations
- **Power differential:** Maximum (owner)
- **Corroboration:** Multiple accusers, documentation
- **Era modifier:** Post-#MeToo (×1.3)
- **Outcome:** Resignation, ongoing legal
- **System validation:** Even owner-level can fall with enough corroboration in modern era. ✅

---

## PROCESSING NOTES

### When To Calculate

| Check | Frequency | Performance Impact |
|-------|-----------|-------------------|
| CTE accumulation | Per match | Low |
| Death risk factors | Monthly | Low |
| Criminal leverage status | Weekly | Low |
| Abuse scandal checks | Event-triggered | Low |
| Mass tragedy risk | Per travel event | Very low |

### Hardware Tier Implications

| Tier | Dark Content Processing |
|------|------------------------|
| Potato | Player company only, simplified death checks |
| Standard | Player + rivals, standard checks |
| Beefy | All major promotions, full detail |
| War Machine | Everyone, every detail |

---

## RELATED SYSTEMS

- **DISC-001:** Scheme Discovery (criminal schemes escalate from here)
- **HIDE-001:** Hidden Personality (breaking points, violence traits)
- **HEALTH-001:** Injury System (CTE, career-enders)
- **SUBSTANCE-001:** Substance Abuse (overdose risk)
- **MORALE-001:** Morale System (suicide risk, isolation)
- **STYLE-001:** Wrestling Styles (CTE accumulation rates)
- **ERA-001:** Era System (awareness levels, legal contexts)
- **REP-001:** Reputation System (scandal fallout)

---

**Document Status:** CODE-READY  
**Content Warning:** This system deals with death, abuse, and trauma. Designed with content toggle to respect player preferences while not sanitizing industry reality.  
**Next Steps:** Implement with content toggle, playtest carefully, gather feedback on tone/handling

---

*"The wrestling business has killed people. It still does. Pretending that away dishonors the dead and removes consequences that should make players think twice. This isn't exploitation. It's honesty."*