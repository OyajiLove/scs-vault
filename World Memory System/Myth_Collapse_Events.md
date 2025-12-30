# Myth Collapse Events

📛 **NAME:** Myth Collapse Events  
🧭 **CATEGORY:** World Memory System / Legacy Dynamics  
🔑 **KEYWORDS:** myth, collapse, scandal, betrayal, hero, legend, reputation, revisionism  
📝 **SUMMARY:** Models how myths die: when legends are exposed as selfish/abusive/hollow, when Golden Eras are reevaluated as toxic, when beloved promotions are revealed as exploitative. Public betrayals, scandals, cultural drift, and retrospective disillusionment can shatter the myths fans built around heroes, eras, and institutions.

⚙️ **LOGIC OVERVIEW:**
- 4 collapse triggers (betrayals, scandals, cultural drift, retrospective disillusionment)
- 3 collapse types (Golden Hero, Golden Era, Promotion Legacy)
- Historical Memory Re-Rolls when myths collapse
- Fanbase fractures between old loyalists and new critics
- Even living legends suffer reduced trust, HOF prestige, merchandising power

🔬 **LLM INTEGRATION:** Moderate (LLM could generate scandal exposés, revisionist takes, fan debate discourse, worker apology scripts)

📌 **ORIGIN:** Vol 5 lines 479-482 (locked)

📎 **CONNECTED SYSTEMS:**
- [[World_Memory_Drift]] - Myth collapse is a form of memory drift
- [[Rediscovery_Cultural_Rehabilitation]] - Opposite of myth collapse
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Individual betrayal tracking
- [[Golden_Era_Collapse_Memory]] - Era-level collapse
- [[Hall of Fame System]] - HOF affected by myth collapse

❓ **OPEN QUESTIONS:**
- Myth collapse reversibility (can myths be rebuilt?)
- Threshold for full myth destruction vs partial damage
- Cross-generational myth collapse propagation
- Regional variation in myth collapse impact

✅ **STATUS:** Locked

---

## 1. COLLAPSE TRIGGERS (4 CAUSES)

| Trigger | Description |
|---------|-------------|
| **Public Betrayals** | Legends caught sabotaging others, politically backstabbing, or exposed as morally rotten |
| **Scandals** | Racism, abuse, criminal activity, or public disgrace |
| **Cultural Drift Exposing Hollow Values** | Generational shifts cause younger fans to re-examine old myths critically |
| **Retrospective Disillusionment** | Long-term booking exposure (bad late-career runs, political manipulation) damages pristine memories |

---

## 2. COLLAPSE TYPES (3 LEVELS)

| Type | Collapse Target | Example |
|------|-----------------|---------|
| **Golden Hero Collapse** | Individual legend revealed to have been selfish, political, abusive, or hollow | Hulk Hogan post-scandal |
| **Golden Era Collapse** | An entire supposed "golden" period reevaluated as toxic, cynical, or overrated | Attitude Era revisionism |
| **Promotion Legacy Collapse** | Beloved company exposed as abusive, exploitative, or corporate sellouts long after heyday | ECW financial/exploitation exposure |

### Collapse Severity Scale

| Severity | Description | Recovery Possibility |
|----------|-------------|---------------------|
| **Minor Tarnish** | Small scandal, quickly forgotten by most | Full recovery possible |
| **Significant Damage** | Major scandal, fanbase fractures, some permanent | Partial recovery over decades |
| **Severe Collapse** | Career/era-defining scandal, mainstream coverage | Limited recovery, permanent scar |
| **Total Destruction** | Unforgivable revelation, universal condemnation | No recovery possible |

---

## 3. SIMULATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Historical Memory Re-Rolls** | Workers, promotions, eras undergo emotional re-valuation based on scandal, betrayal, rediscovery, or cultural drift events |
| **Fanbase Fractures** | Older loyalists cling to old myths; younger fans reject or reinterpret legacies |
| **Worker Trust Damage** | Even living legends suffer reduced trust bonuses, Hall of Fame prestige, merchandising power after myth collapse |
| **Promotion Loyalty Decay** | Brands once associated with golden eras lose emotional anchor strength across generations |

### Trust Damage by Collapse Type

| Collapse Type | Trust Modifier | Duration |
|---------------|----------------|----------|
| **Minor Tarnish** | -5 to -15 | 1-3 years |
| **Significant Damage** | -15 to -35 | 5-15 years |
| **Severe Collapse** | -35 to -60 | Permanent (slow recovery possible) |
| **Total Destruction** | -75 to -100 | Permanent (no recovery) |

### Fanbase Fracture Patterns

| Fan Group | Response to Myth Collapse |
|-----------|---------------------------|
| **Older Loyalists** | Denial, defensiveness, "separate art from artist" |
| **Moderate Fans** | Disappointment, reduced engagement, "complicated legacy" |
| **Younger Fans** | Rejection, mockery, "told you so" |
| **Hardcore Critics** | Vindication, amplification, "we always knew" |

---

## 4. HISTORICAL MODELS

| Event | Myth Collapse Type | Outcome |
|-------|-------------------|---------|
| **Hulk Hogan Post-Scandal** | Golden Hero Collapse | Massive brand damage, fanbase fracture, nostalgia erosion. WWE distanced, then slowly rehabilitated. |
| **Attitude Era Revisionism** | Golden Era Revaluation | Modern fans recognize sexism, homophobia, racism beneath chaotic spectacle. Era still celebrated but with caveats. |
| **ECW Myth** | Promotion Legacy Collapse (partial) | Romanticized by some, but others highlight financial corruption, end-stage rot, Paul Heyman's exploitation of worker loyalty |
| **Chris Benoit** | Golden Hero Collapse (Total) | Complete erasure from WWE history. No rehabilitation possible. |
| **Vince McMahon** | Golden Hero Collapse (Severe) | Ongoing reevaluation of entire WWE history through lens of allegations. Legacy permanently complicated. |

### Hulk Hogan Case Study

**Initial Myth:** All-American hero, face of wrestling's mainstream explosion, beloved across generations.

**Collapse Trigger:** Racism scandal (2015 tape leak).

**Collapse Type:** Golden Hero Collapse (Severe).

**Immediate Effects:**
- WWE terminated contract
- HOF page removed
- Merchandise pulled
- Sponsors fled

**Fanbase Fracture:**
- Older loyalists: "It was a different time" / denial
- Moderate fans: Reduced nostalgia, "complicated"
- Younger fans: Mockery, rejection
- Critics: Vindication

**Recovery Attempt:** Gradual WWE rehabilitation (HOF restoration, appearances).

**Current Status:** Permanently tarnished but partially rehabilitated. Myth survives in diminished form for some fans, destroyed for others.

---

## 5. MYTH COLLAPSE PROPAGATION

Myth collapse can spread beyond the initial target:

| Propagation Type | Description |
|------------------|-------------|
| **Association Damage** | Workers/promotions associated with collapsed figure lose reputation |
| **Era Contamination** | Collapse of one hero taints entire era |
| **Institutional Damage** | Promotion that protected/enabled collapsed figure loses trust |
| **Movement Damage** | Philosophy associated with collapsed figure loses credibility |

---

## 6. IMPLEMENTATION NOTES

```json
{
  "myth_collapse": {
    "subject_type": "WORKER",
    "subject_id": "hulk_hogan",
    "collapse_type": "GOLDEN_HERO",
    "trigger": "SCANDAL",
    "scandal_type": "RACISM",
    "year": 2015,
    "severity": "SEVERE",
    "trust_damage": -55,
    "fanbase_fracture": {
      "loyalists_remaining": 0.35,
      "moderate_disengaged": 0.30,
      "younger_rejection": 0.25,
      "critics_vindicated": 0.10
    },
    "institutional_response": "TERMINATION_THEN_REHABILITATION",
    "recovery_status": "PARTIAL",
    "years_to_partial_recovery": 4,
    "permanent_scar": true,
    "propagation": {
      "era_contamination": "80S_WWF_PARTIALLY_TAINTED",
      "institutional_damage": "WWE_MINOR"
    }
  }
}
```

---

## 7. PHILOSOPHY

> "Every myth is a promise. The promise that heroes are real, that golden eras were pure, that the things we loved were worth loving. When myths collapse, we don't just lose respect for a person or a time. We lose a piece of ourselves that believed. That's why myth collapse hurts so much, and why some fans will defend the indefensible rather than face that loss."

Myth collapse is not purely negative. It's also a form of truth-telling. Wrestling history, like all history, is full of things that should be remembered honestly, not just mythologized. SCS models both the pain of collapse and the integrity of facing hard truths.

---

## 8. LOCKED PHILOSOPHY

> "Rebellions keep history alive. Myths die under the weight of truth. Wrestling's soul is always a battlefield."

---

## 9. RELATED SYSTEMS

- [[World_Memory_Drift]] - Myth collapse is a form of memory drift
- [[Rediscovery_Cultural_Rehabilitation]] - Opposite of myth collapse
- [[Hidden_Worker_Betrayal_Redemption_Memories]] - Individual betrayal tracking
- [[Golden_Era_Collapse_Memory]] - Era-level collapse
- [[Hall of Fame System]] - HOF affected by myth collapse
- [[Scandal System]] - Scandal mechanics

---

**Document Status:** Locked  
**Source:** Vol 5 lines 479-482  
**Next Review:** Integration with Scandal System severity mechanics
