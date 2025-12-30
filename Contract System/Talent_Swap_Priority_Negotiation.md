# Talent Swap and Priority Negotiation Systems

📛 **NAME:** Talent Swap and Priority Negotiation Systems  
🧭 **CATEGORY:** Contract System / Inter-Promotion Relations  
🔑 **KEYWORDS:** talent, swap, loan, negotiation, priority, agreement, pact, respectful, transition  
📝 **SUMMARY:** Models how promotions negotiate respectful worker priority shifts without triggering betrayal memory. Talent sharing pacts, temporary priority swaps, mutual loyalty clauses, and respectful farewell arcs all allow workers to move between promotions while preserving emotional integrity. Worker consent matters: high loyalty workers may resist even agreed shifts.

⚙️ **LOGIC OVERVIEW:**
- 4 negotiation scenarios (sharing pacts, temporary swaps, loyalty clauses, farewell arcs)
- Negotiation rolls based on relationship strength and worker loyalty
- Talent loan agreements prevent loyalty decay
- Compensation packages can secure priority shifts
- Worker consent checks for high loyalty/traditionalism workers

🔬 **LLM INTEGRATION:** Minimal (deterministic negotiation calculations; LLM could generate negotiation dialogue, contract language, farewell promo scripts)

📌 **ORIGIN:** Vol 5 lines 518-520 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Worker_Prioritization_Multi_Promotion]] - What's being negotiated
- [[Worker_Formative_Loyalty]] - Loyalty being protected
- [[Betrayal_Memory_Formative_Desertions]] - What happens without negotiation
- [[Contract Types]] - Contract framework
- [[Promotion Relationships]] - Inter-promotion relations

❓ **OPEN QUESTIONS:**
- Exact negotiation roll mechanics
- Maximum loan duration before loyalty effects
- Compensation package scaling
- Failed negotiation consequences

✅ **STATUS:** Locked

---

## 1. NEGOTIATION SCENARIOS (4 TYPES)

| Scenario | Description | Loyalty Protection |
|----------|-------------|-------------------|
| **Talent Sharing Pacts** | Promotions agree in advance on talent availability schedules (e.g., "Worker X prioritizes Home Promotion Events unless Y Tournament") | FULL |
| **Temporary Priority Swaps** | For big one-off events (Dome shows, anniversary PPVs), promotions negotiate temporary priority shifts | FULL |
| **Mutual Loyalty Clauses** | Contracts include respect for formative loyalty (no forced no-shows without mutual agreement unless extreme circumstances) | FULL |
| **Respectful Farewell Arcs** | If workers transition promotions, mutual booking arcs negotiated (retirement matches, farewell tours) to protect loyalty memories | HIGH |

---

## 2. NEGOTIATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Negotiation Rolls** | Based on promotions' relationship strength, booking flexibility, worker loyalty, and world perception (media friendliness) |
| **Talent Loan Agreements** | Formal deals where workers are "loaned" temporarily, priority shifts agreed cleanly, no emotional loyalty decay |
| **Compensation Packages** | Promotions sometimes offer higher appearance fees, title shots, or respectful booking to secure priority shifts |
| **Worker Consent Checks** | Workers with high loyalty/traditionalism hidden stats may resist forced shifts even if promotions agree, requiring personal buy-in |

### Negotiation Roll Factors

| Factor | Weight |
|--------|--------|
| **Promotion Relationship** | 30% |
| **Worker Loyalty to Both** | 25% |
| **Financial Offer** | 20% |
| **Event Importance** | 15% |
| **Historical Precedent** | 10% |

### Negotiation Outcomes

| Roll Result | Outcome |
|-------------|---------|
| **Critical Success (90+)** | Full agreement, bonus goodwill, future negotiations easier |
| **Success (70-89)** | Agreement reached, standard terms |
| **Partial Success (50-69)** | Agreement with compromises, some conditions |
| **Failure (30-49)** | No agreement, relationship strain |
| **Critical Failure (<30)** | No agreement, relationship damaged, public tension possible |

---

## 3. AGREEMENT TYPES

### Talent Sharing Pact Structure

```
TALENT SHARING PACT
Between: [Promotion A] and [Promotion B]
Duration: [Time Period]
Workers Covered: [List]
Priority Rules:
- Home promotion major events: Always priority
- Partner promotion major events: Negotiable per case
- Tournaments: [Specific rules]
- Conflicts: [Resolution process]
Compensation: [Terms]
Exit Clause: [Conditions]
```

### Temporary Priority Swap Terms

| Term | Standard | Premium |
|------|----------|---------|
| **Duration** | Single event | Event series |
| **Compensation** | Appearance fee only | Fee + booking guarantee |
| **Exclusivity** | Non-exclusive | Exclusive for period |
| **Marketing Rights** | Shared | Full to borrowing fed |
| **Return Commitment** | Immediate | Negotiated timeline |

### Farewell Arc Elements

| Element | Purpose |
|---------|---------|
| **Announcement Match** | Public acknowledgment of transition |
| **Tribute Segment** | Honor worker's contributions |
| **Final Match** | Proper sendoff, often against significant opponent |
| **Locker Room Moment** | Emotional closure with colleagues |
| **Fan Acknowledgment** | Allow fans to say goodbye |

---

## 4. WORKER CONSENT MECHANICS

High loyalty workers may resist priority shifts even when promotions agree:

| Loyalty Level | Resistance Threshold |
|---------------|---------------------|
| **Very High (80+)** | Will resist unless personally convinced |
| **High (60-79)** | May resist, needs good reason |
| **Medium (40-59)** | Generally accepts if promotions agree |
| **Low (<40)** | Accepts almost any agreement |

### Convincing Resistant Workers

| Approach | Success Modifier |
|----------|------------------|
| **Personal Meeting** | +20% |
| **Increased Pay** | +10-30% based on amount |
| **Booking Guarantees** | +15% |
| **Loyalty Acknowledgment** | +25% |
| **Formative Fed Blessing** | +35% |

---

## 5. HISTORICAL MODELS

| Event | Priority Negotiation |
|-------|---------------------|
| **AEW/NJPW Forbidden Door Deals** | Workers like Moxley, Omega, and Tanahashi shift priority fluidly between promotions through respectful negotiations, maintaining emotional loyalty layers |
| **NOAH/All Japan Wrestler Transitions** | Many early 2000s jumps handled poorly. Workers seen as betrayers or cowards based on whether farewell handling was respectful. |
| **Crockett/NJPW Crossovers (80s)** | Priority deals around tournaments like IWGP built through mutual respect arcs, preventing loyalty damage |
| **CMLL/NJPW Long-Term Pact** | Decades of talent sharing with clear priority rules, minimal betrayal perception |

### Forbidden Door Case Study

**Parties:** AEW, NJPW

**Agreement Type:** Ongoing Talent Sharing Pact

**Key Terms:**
- Major AEW events: AEW talent prioritizes AEW
- Major NJPW events: NJPW talent prioritizes NJPW
- Forbidden Door: Joint priority, negotiated per talent
- Tournaments: Case-by-case negotiation

**Worker Consent:** High-profile workers consulted personally

**Outcome:** Successful priority management, minimal betrayal perception, enhanced legitimacy for both promotions

---

## 6. IMPLEMENTATION NOTES

```json
{
  "talent_agreement": {
    "type": "TALENT_SHARING_PACT",
    "promotions": ["aew", "njpw"],
    "start_year": 2021,
    "duration": "ONGOING",
    "workers_covered": ["moxley", "omega", "danielson"],
    "priority_rules": {
      "home_major_events": "ALWAYS_HOME",
      "partner_major_events": "NEGOTIABLE",
      "tournaments": "CASE_BY_CASE",
      "forbidden_door": "JOINT_PRIORITY"
    },
    "relationship_strength": 75,
    "historical_precedent": true,
    "public_perception": "POSITIVE",
    "betrayal_incidents": 0
  }
}
```

---

## 7. PHILOSOPHY

> "Real loyalty cannot be bought — but it can be honored, protected, or betrayed forever. The difference between a respected transition and a burning bridge is whether everyone involved treated the worker's emotional ties as something worth protecting, not just a contract clause to be exploited."

Talent negotiation isn't just business: it's emotional diplomacy. Promotions that handle it well build lasting relationships. Those that don't create grudges that echo for decades.

---

## 8. RELATED SYSTEMS

- [[Worker_Prioritization_Multi_Promotion]] - What's being negotiated
- [[Worker_Formative_Loyalty]] - Loyalty being protected
- [[Betrayal_Memory_Formative_Desertions]] - What happens without negotiation
- [[Contract Types]] - Contract framework
- [[Promotion Relationships]] - Inter-promotion relations
- [[Historical_Betrayal_Fracture_Points]] - When negotiations fail publicly

---

**Document Status:** Locked  
**Source:** Vol 5 lines 518-520  
**Next Review:** Integration with AI booking negotiations
