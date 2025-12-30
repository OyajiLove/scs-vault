# Shoot Promo System

📛 **NAME:** Shoot Promo System  
🧭 **CATEGORY:** Segment/Promo System / Reality Blur  
🔑 **KEYWORDS:** shoot, promo, pipebomb, worked-shoot, reality, blurred lines, controversy  
📝 **SUMMARY:** Models reality-warping promos that blur kayfabe and real events. Shoots can resurrect careers, destroy reputations, reshape fan perception, and alter promotion culture. Includes worker tolerance stats and promotion policy settings.

⚙️ **LOGIC OVERVIEW:**
- Shoots become possible after betrayals, exiles, contract expiry, or management-sanctioned situations
- Worker "Shoot Tolerance" hidden stat determines controlled vs disastrous execution
- Promotion "Shoot Policy" setting (Encourage/Allow Rarely/Ban) affects availability
- Successful shoots reshape narratives; failed shoots burn bridges permanently
- Fan reception splits based on timing, charisma, and truth resonance

🔬 **LLM INTEGRATION:** Yes, Primary (generate shoot promo content, blurred reality dialogue, reference real events appropriately)

📌 **ORIGIN:** Vol 5 lines 132-136 (locked)

📎 **CONNECTED SYSTEMS:**
- [[Clique_Coup_System]] - Exiled cliques use shoots for warfare
- [[Crowd_Memory]] - Shoots reframe public perception
- [[Hidden_Personality_System]] - Ego, Morality affect shoot behavior
- [[Promo Evaluation]] - Shoot quality evaluation

❓ **OPEN QUESTIONS:**
- Exact Shoot Tolerance calculation
- How management-sanctioned vs unsanctioned shoots differ mechanically
- Integration with real-time show simulation

✅ **STATUS:** Locked

---

## 1. SHOOT TRIGGERS

| Trigger | Example |
|---------|---------|
| **Post-Betrayal Fallout** | Worker shoots on screwjob, backstage injustices |
| **Clique Exile or Coup Failure** | Fired/jumping workers cut blurred reality promos |
| **Emergency Booking** | Last-second real heat turned into on-screen angle |
| **Locker Room Chaos** | Opportunists/chaos agents use discontent for attention |
| **Contract Expiry** | Departing workers "say what they want" on way out |
| **Management Sanctioned** | Promotions intentionally script blurred promos (ECW, Russo WCW) |

---

## 2. SHOOT EFFECTS

| Layer | Simulation Outcome |
|-------|-------------------|
| **Fan Memory Mutation** | Shoots reframe perception: betrayals, alliances, heroism can flip |
| **Locker Room Polarization** | Shoots either embolden support or worsen divides |
| **Worker Career Trajectory** | Great shoots rebuild reputations; bad shoots burn bridges |
| **Promotion Cultural Tilt** | Frequent shoots = chaotic/unpredictable; lose prestige or gain cult loyalty |
| **Future Contract Negotiations** | Shoot-prone workers = high-risk/high-reward signings |

---

## 3. SHOOT MECHANICS

### Worker "Shoot Tolerance" (Hidden)

Some workers naturally better at controlled blurring; others spiral into disaster.

| Tolerance Level | Behavior |
|-----------------|----------|
| **High** | Can blur reality while staying "in bounds," create magic moments |
| **Medium** | Risky but potentially impactful; needs good booking support |
| **Low** | Likely to go off-script, burn bridges, create real heat |

### Personality Factors

| Hidden Stat | Effect on Shoots |
|-------------|------------------|
| **High Ego** | More likely to shoot; harder to control |
| **Low Morality** | May weaponize shoots for personal gain |
| **High Drive** | Uses shoots strategically for career advancement |
| **High Paranoia** | Shoots may spiral into conspiracy accusations |

---

## 4. PROMOTION SHOOT POLICY

| Policy | Description | Example |
|--------|-------------|---------|
| **Encourage** | Shoots are a feature, not a bug | ECW style |
| **Allow Rarely** | Occasional strategic blurring | Attitude Era WWF |
| **Ban and Punish** | Shoots result in fines, suspension, firing | Early WCW, corporate WWE |

---

## 5. AUDIENCE RECEPTION

Depending on timing, charisma, and truth resonance:

| Reception | Fan Behavior |
|-----------|--------------|
| **Rally Behind** | "Tell 'em!" Anti-authority support surges |
| **Turn Against** | "Crybaby! Ungrateful!" Worker seen as selfish |
| **Mixed/Confused** | Some fans buy it, others reject; polarization |

### Reception Factors

| Factor | Effect |
|--------|--------|
| **Truth Resonance** | Shoots that reflect real grievances land harder |
| **Worker Charisma** | High charisma = better delivery = better reception |
| **Timing** | Post-betrayal = sympathy; random = selfish |
| **Promotion Reputation** | Fans already skeptical of management = easier rally |

---

## 6. LONG-TERM RIPPLE

| Effect | Behavior |
|--------|----------|
| **Storyline Reshaping** | Shoots that land reshape power structures, storylines |
| **World History Arcs** | Major shoots become era-defining moments |
| **Worker Legend Status** | Pipebomb-tier shoots create lasting legacy |
| **Promotion Trust Erosion** | Too many shoots = fans can't tell real from work |

---

## 7. MOCKERY AND HUMILIATION BOOKING

Post-betrayal, management may use mockery angles to control narrative:

| Action | Effect |
|--------|--------|
| **Parody Angles** | Impersonators, fake tribute matches, belt defacements |
| **Fan Split Risk** | Tasteless mockery alienates traditional fans |
| **Short-Term Pop vs Long-Term Damage** | Immediate heel heat vs eroding moral credibility |
| **Worker Trust Collapse** | Locker room sees how legends are treated |

### Mockery Outcomes

| If Mockery "Works" | If Mockery "Fails" |
|--------------------|-------------------|
| New heel regime established | Homegrown credibility collapses |
| Betrayed figure fades to footnote | Fans revolt (Austin-style anti-authority boom) |
| | Locker room morale collapses |

---

## 8. HISTORICAL EXAMPLES

| Event | Simulation Model |
|-------|-----------------|
| **CM Punk Pipebomb (2011)** | Career resurrection, anti-hero rises after near-exile |
| **Hall/Nash Outsider Promos (1996)** | Blurred reality creates nWo |
| **MJF "Fire Me" Promo (2022)** | Blurred contract dispute into reality-shifting war |
| **Russo-Era WCW** | Shoot chaos backfires, long-term trust erosion |
| **DX Little Person "Bret" Mockery** | Humiliation booking, symbolic public execution |

---

## IMPLEMENTATION NOTES

```json
{
  "shoot_promo": {
    "promo_id": "punk_pipebomb_2011",
    "worker_id": "cm_punk",
    "trigger": "CONTRACT_EXPIRY",
    "sanctioned": true,
    "shoot_tolerance": 85,
    "content_type": "GRIEVANCE_MANIFESTO",
    "truth_resonance": 90,
    "execution_quality": 95,
    "fan_reception": "RALLY_BEHIND",
    "effects": {
      "career_trajectory_shift": +40,
      "promotion_culture_tilt": "MORE_EDGY",
      "locker_room_polarization": 30,
      "legacy_anchor": true
    }
  }
}
```

---

## RELATED SYSTEMS

- [[Promo Evaluation]] - Base promo quality mechanics
- [[Clique_Coup_System]] - Exiles use shoots for warfare
- [[Crowd_Memory]] - Shoots become memory anchors
- [[Hidden_Personality_System]] - Stats affect shoot behavior
- [[Emergency_Rebooking_System]] - Shoots as crisis tool

---

**Document Status:** Locked  
**Source:** Vol 5 lines 132-136  
**Next Review:** LLM prompt engineering for shoot content generation
