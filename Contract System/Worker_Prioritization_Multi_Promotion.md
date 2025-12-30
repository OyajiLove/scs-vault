# Worker Prioritization System (Multi-Promotion Booking)

📛 **NAME:** Worker Prioritization System for Multiple Promotions  
🧭 **CATEGORY:** Contract System / Booking Dynamics  
🔑 **KEYWORDS:** priority, booking, freelancer, loyalty, prestige, multi-promotion, conflict, schedule  
📝 **SUMMARY:** Models how workers decide which promotion to prioritize when booking conflicts arise. Fixes TEW's shallow "prestige wins" approach. Loyalty, role/stake, personality traits, and event importance all compete with prestige and money. Owner-workers nearly always prioritize their own fed. Workers feel emotionally real, not like prestige robots.

⚙️ **LOGIC OVERVIEW:**
- 6 core priority factors (loyalty, role/stake, contract type, money, prestige, personality)
- Dynamic priority scoring per booking conflict
- Soft commitments (emotional ties treated like contracts)
- Event special weighing (anniversary, tournament, storyline payoff = loyalty spike)
- No-show triggers loyalty decay, scandal, faction trust loss

🔬 **LLM INTEGRATION:** Minimal (deterministic priority calculations; LLM could generate worker internal monologue, negotiation dialogue)

📌 **ORIGIN:** Vol 5 lines 493-504 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Loyalty System]] - Base loyalty mechanics
- [[Worker_Loyalty_Drift]] - Loyalty changes over time
- [[Hidden Personality Traits]] - Ego, Drive, Traditionalism affect decisions
- [[Worker_Formative_Loyalty]] - Where worker was built matters
- [[Contract Types]] - Contract exclusivity levels

❓ **OPEN QUESTIONS:**
- Exact priority scoring weights
- How far in advance conflicts are resolved
- Player override mechanics
- Penalty severity for no-shows

✅ **STATUS:** Locked

---

## 1. CORE PRIORITY FACTORS (6 WEIGHTS)

| Factor | Description | Weight Range |
|--------|-------------|--------------|
| **Promotion Loyalty** | How emotionally attached the worker is to each promotion (not just who pays more) | 25-35% |
| **Promotion Role/Stake** | Are they founder, champion, booker, top face/heel, symbolic figure? | 15-25% |
| **Contract Type** | Full-time exclusive? Per-appearance? Freelancer but emotionally tied? | 10-20% |
| **Money Offered** | Can override emotional loyalty only if loyalty is low or worker is desperate | 10-20% |
| **Prestige Differential** | Size/prestige gap between promotions matters, but competes with loyalty | 10-15% |
| **Worker Personality Traits** | Hidden stats: Loyalty, Ego, Drive, Traditionalism | 10-15% |

### Personality Trait Effects

| Trait | High Score Effect | Low Score Effect |
|-------|-------------------|------------------|
| **Loyalty** | Strongly favors emotional ties | Chases best offer |
| **Ego** | May push toward bigger stages | Content with current position |
| **Drive** | Ambition could override comfort | Prioritizes stability |
| **Traditionalism** | Favors loyalty to "home base" | Open to new opportunities |

---

## 2. PRIORITY RESOLUTION EXAMPLES

| Scenario | Worker Decision |
|----------|-----------------|
| **Super Delfin: Osaka Pro vs NJPW** | High loyalty to Osaka Pro + ownership stake + symbolic leadership role = prioritizes Osaka Pro, even if NJPW offers more prestige and money for a one-off |
| **Freelancer with No Deep Ties** | Freelancer working low on card at small indie vs NJPW BOSJ slot = may prioritize NJPW, especially if Drive and Ego are high |
| **Worn-Down Star Near End of Career** | If loyalty weakens over time and Drive decreases, may chase bigger checks more readily. Drift toward prestige/finance if emotional ties decay. |
| **Champion at Home Fed** | Even freelancers will prioritize title defense at home fed over prestige appearance elsewhere |
| **Anniversary Show Conflict** | Home promotion anniversary spikes loyalty bonus, nearly impossible for outside offers to poach |

---

## 3. SIMULATION MECHANICS

| Mechanic | Behavior |
|----------|----------|
| **Priority Scoring** | Every show booking day, worker weighs offers based on dynamic loyalty-role-money-prestige-weighting score |
| **Soft Commitments** | Workers emotionally committed to promotions (without exclusive contracts) still treat them almost like contracts because of loyalty |
| **Event Special Weighing** | If home promotion show is Anniversary, Tournament Final, or Big Emotional Storyline Payoff, loyalty bonuses spike dramatically |
| **Tension Events** | If a worker no-shows a home promotion without good reason, triggers loyalty decay, potential scandal, faction trust loss, and fanbase resentment |

### Event Type Loyalty Modifiers

| Event Type | Loyalty Bonus |
|------------|---------------|
| **Regular Show** | +0 |
| **Major Show** | +10 |
| **Anniversary/Milestone** | +25 |
| **Tournament Final** | +20 |
| **Title Defense** | +30 |
| **Storyline Blowoff** | +25 |
| **Homecoming (after absence)** | +35 |

### No-Show Consequences

| Consequence | Severity |
|-------------|----------|
| **Loyalty Decay** | -15 to -30 with affected promotion |
| **Scandal Risk** | 40% chance of public incident |
| **Faction Trust Loss** | -10 to -20 with allied workers |
| **Fan Resentment** | Regional fanbase trust -10 to -25 |
| **Booking Grudge** | Booker may depush or blacklist |

---

## 4. SPECIAL CASES

### Owner-Worker / Booker-Worker

Near-absolute loyalty to their own fed. Nearly impossible to pry away unless:
- Promotion collapses
- Personal betrayal occurs
- Massive money or world-shaking cultural shift

| Owner Type | Priority Override Threshold |
|------------|----------------------------|
| **Founder/Owner** | 95% loyalty to own fed |
| **Head Booker** | 85% loyalty to own fed |
| **Minority Owner** | 70% loyalty to own fed |
| **Creative Consultant** | 60% loyalty to own fed |

### Dual-Role Legends

Some legends (e.g., Tenryu in WAR) may work others strategically but still prioritize their own creation first unless retirement phase kicks in.

| Career Phase | Priority Behavior |
|--------------|-------------------|
| **Active Prime** | Own fed first, always |
| **Winding Down** | May take prestige bookings more freely |
| **Retirement Tour** | Nostalgic returns to formative feds possible |
| **Post-Retirement** | One-offs anywhere emotionally resonant |

---

## 5. HISTORICAL MODELS

| Worker | Decision Pattern |
|--------|------------------|
| **Super Delfin (Osaka Pro)** | Prioritizes Osaka Pro home events over bigger prestige NJPW dates unless career stakes or loyalty decay force re-evaluation |
| **Jushin Liger** | Prioritizes NJPW strongly even during worldwide tours unless special circumstance (tournament invites, cross-promotional wars) |
| **Bobby Eaton (1990s)** | Loyal to WCW. Doesn't jump to WWF even during opportunities unless conditions (contract cut, loyalty decay) shift hard |
| **Onita (FMW)** | Absolute loyalty to own creation until financial collapse forced changes |

---

## 6. IMPLEMENTATION NOTES

```json
{
  "booking_conflict": {
    "worker_id": "super_delfin",
    "date": "1998-05-05",
    "offers": [
      {
        "promotion_id": "osaka_pro",
        "event_type": "ANNIVERSARY",
        "role": "MAIN_EVENT",
        "pay": 5000,
        "prestige": 25
      },
      {
        "promotion_id": "njpw",
        "event_type": "REGULAR",
        "role": "UNDERCARD",
        "pay": 15000,
        "prestige": 85
      }
    ],
    "worker_factors": {
      "osaka_pro_loyalty": 95,
      "njpw_loyalty": 40,
      "role_stake_osaka": "OWNER",
      "personality": {"loyalty": 85, "ego": 45, "drive": 60, "traditionalism": 80}
    },
    "priority_scores": {
      "osaka_pro": 92,
      "njpw": 48
    },
    "decision": "OSAKA_PRO",
    "reasoning": "Ownership stake + anniversary event + high loyalty/traditionalism override prestige/money differential"
  }
}
```

---

## 7. PHILOSOPHY

> "Prestige isn't everything. Money isn't everything. The question is: where does this worker's soul live? A founder won't abandon their creation for a bigger check. A loyal soldier won't skip their home promotion's biggest show for a dark match somewhere prestigious. Workers are people with emotional ties, not prestige-chasing algorithms."

This system ensures booking feels human, not mechanical. Workers make decisions that reflect their personalities, histories, and emotional investments.

---

## 8. RELATED SYSTEMS

- [[Loyalty System]] - Base loyalty mechanics
- [[Worker_Loyalty_Drift]] - Loyalty changes over time
- [[Hidden Personality Traits]] - Ego, Drive, Traditionalism affect decisions
- [[Worker_Formative_Loyalty]] - Where worker was built matters
- [[Contract Types]] - Contract exclusivity levels
- [[Talent_Sharing_Agreements]] - Mutual priority arrangements

---

**Document Status:** Locked  
**Source:** Vol 5 lines 493-504  
**Next Review:** Integration with AI booking logic
