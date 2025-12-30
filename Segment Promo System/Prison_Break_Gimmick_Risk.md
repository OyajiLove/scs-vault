# Prison Break Gimmick Risk System

📛 **NAME:** Prison Break Gimmick Risk System  
🧭 **CATEGORY:** Segment/Promo System / Debut Dynamics  
🔑 **KEYWORDS:** prison break, new signing, debut, shoot, ex-wwe, anti-promotion, parasitism  
📝 **SUMMARY:** Models the dynamic where newly signed workers trash their old employer through "I was held down" or "I escaped" narratives. Short-term pop vs long-term parasitism risk. Tied to worker Ego, Drive, and Grievance Memory.

⚙️ **LOGIC OVERVIEW:**
- Workers leaving restrictive promotions often cut shoots on old boss/system
- Promotion may actively encourage anti-old-promotion angles (early TNA, AEW debuts)
- High Ego + High Drive + Grievance Memory = more likely to push shooty narratives
- Short-term pop but long-term risk of "WWE Second-Hand Store" identity
- Overuse pigeonholes worker as "the guy who only talks about old company"

🔬 **LLM INTEGRATION:** Yes (generate shoot promo content referencing old promotion dynamics)

📌 **ORIGIN:** Vol 5 lines 143-146 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Shoot_Promo_System]] - Parent system for reality-blur promos
- [[Hidden_Personality_System]] - Ego, Drive, Grievance affect likelihood
- [[Crowd_Memory]] - Fans remember shoot narratives
- [[Fanbase_Trust_and_Betrayal]] - Repeated parasitism erodes unique identity

❓ **OPEN QUESTIONS:**
- Exact threshold for "overuse" triggering parasitism penalty
- How regional/demographic fanbases respond differently
- Integration with cross-promotion rivalry systems

✅ **STATUS:** Locked

---

## 1. WHEN PRISON BREAK HAPPENS

| Trigger | Effect |
|---------|--------|
| **Worker Leaves Restrictive Promotion** | Upon debuting in new promotion, can cut shoots on old boss/system |
| **Promotion Encourages Anti-Old Angles** | AEW, early TNA actively pushed "free at last" storylines |
| **Worker Ego + Drive + Grievance Memory** | Workers with high Drive and wounded Ego more likely to push shooty narratives |

### Worker Personality Factors

| Hidden Stat | Effect |
|-------------|--------|
| **High Ego** | More likely to feel wronged, more aggressive shoots |
| **High Drive** | Strategic use of shoot for career momentum |
| **Grievance Memory** | Past slights fuel authentic shoot content |
| **High Paranoia** | May go off-script, spiral into conspiracy accusations |

---

## 2. RISKS AND REWARDS

| Outcome | Effect |
|---------|--------|
| **Short-Term Pop** | Fans cheer the rebellion initially, gets buzz and new momentum |
| **Long-Term Parasitism** | If overused, promotion starts feeling like "WWE Second-Hand Store" or "Revenge Fed," killing independent brand identity |
| **Fanbase Perception Split** | Some fans love shooty rebellion; others see it as bitterness or desperate marketing |
| **Worker Pigeonholing Risk** | Worker becomes "the guy who only talks about his old company," limiting future angles |

### Parasitism Threshold

When multiple workers use prison break gimmicks without developing unique identities:

| Condition | Penalty |
|-----------|---------|
| **2-3 Prison Break Debuts in 6 Months** | Minor identity warning |
| **4+ Prison Break Debuts in 6 Months** | "Revenge Fed" reputation starts forming |
| **Primary Angle Identity = Anti-Other-Promotion** | Severe independent brand damage |
| **No Unique Storylines After 3 Months** | Worker stuck in "bitter ex" role |

---

## 3. HISTORICAL EXAMPLES

| Worker/Event | Old Promotion | New Promotion | Outcome |
|--------------|---------------|---------------|---------|
| **Kurt Angle Early TNA** | WWF | TNA | Shot on WWF in first weeks, got attention but set tone |
| **Cody Rhodes AEW Launch** | WWE | AEW | Strategic anti-WWE positioning, helped launch but risked parasitism |
| **Jeff Hardy TNA 2004** | WWE | TNA | "Free at last" but limited long-term identity development |
| **Lex Luger WCW 1995** | WWF | WCW | Appeared on Nitro premiere, shock value over substance |
| **Multiple Ex-WWE in AEW 2019-2022** | WWE | AEW | Mix of successful identity development (Moxley) and parasitism risk (others) |

### Success vs Failure Factors

| Success Factor | Failure Factor |
|----------------|----------------|
| Quick pivot to unique identity | Ongoing WWE references past debut |
| Strategic single reference | Repeated shoot promos on same topics |
| Authentic grievance resonance | Bitter/whiny perception |
| Promotion builds new stories | Promotion relies on anti-competitor heat |

---

## 4. PROMOTION BOOKING DECISIONS

### Encouraging Prison Break Angles

| Policy | Effect |
|--------|--------|
| **Lean Into It** | High short-term buzz, parasitism risk |
| **One-Time Reference** | Controlled pop, then move on |
| **Ignore Old Promotion Entirely** | Clean slate, may waste built-in heat |
| **Sustained Anti-Competitor Campaign** | Maximum buzz, maximum identity risk |

### Identity Recovery

If promotion falls into "Revenge Fed" trap:

| Recovery Action | Time to Recover |
|-----------------|-----------------|
| **Develop Unique Storylines** | 6-12 months |
| **Stop Hiring Ex-Major-Promotion Workers Temporarily** | 3-6 months of roster stability |
| **Create Homegrown Stars** | 12-24 months |
| **Win Critical Acclaim for Original Content** | Variable |

---

## IMPLEMENTATION NOTES

```json
{
  "prison_break_event": {
    "worker_id": "kurt_angle",
    "old_promotion": "wwf",
    "new_promotion": "tna",
    "debut_type": "PRISON_BREAK_SHOOT",
    "personality_factors": {
      "ego": 85,
      "drive": 90,
      "grievance_memory": ["contract_dispute", "booking_frustration"]
    },
    "short_term_pop": 40,
    "parasitism_contribution": 15,
    "pigeonhole_risk": 0.3,
    "follow_up_identity": "OLYMPIC_HERO_REINVENTION"
  },
  "promotion_parasitism_meter": {
    "promotion_id": "tna",
    "current_parasitism": 45,
    "threshold_warning": 50,
    "threshold_severe": 75,
    "recent_prison_breaks": 3
  }
}
```

---

## RELATED SYSTEMS

- [[Shoot_Promo_System]] - Parent system for reality-blur mechanics
- [[Hidden_Personality_System]] - Ego, Drive, Grievance factors
- [[Crowd_Memory]] - Shoots become memory anchors
- [[Fanbase_Trust_and_Betrayal]] - Overuse erodes promotion identity
- [[Contract System]] - Departure circumstances affect shoot authenticity

---

**Document Status:** Locked  
**Source:** Vol 5 lines 143-146  
**Next Review:** Integration with cross-promotion rivalry tracking
