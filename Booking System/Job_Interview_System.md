# JOB INTERVIEW SYSTEM

📛 **NAME:** Job Interview System  
🧭 **CATEGORY:** Career Mode / Dialogue  
🔑 **KEYWORDS:** interview, hiring, career, vision, strategy pitch  
📝 **SUMMARY:**

Not every fed wants you. You must prove you understand the business. When applying for a booking position at another promotion, you go through a realistic interview process where owners/network execs evaluate your vision, philosophy, and fit with their goals.

⚙️ **LOGIC OVERVIEW:**

- Interviews triggered when applying for open booking positions
- Questions cover vision, philosophy, immediate strategy, crisis management
- Success depends on reputation, answer alignment, and realism
- Failed interviews have cooldown before retry
- Same system used for investor pitches when starting own promotion

🔬 **LLM INTEGRATION:** Very High (dialogue generation, response evaluation, personality matching)

📌 **ORIGIN:** Vol 3 lines 410-412

📎 **CONNECTED SYSTEMS:**
- [[Booker_Succession_System]] - Interviews happen after ouster
- [[Startup Promotion System]] - Similar pitch system for investors
- [[Booker_Memory_Engine]] - Your history affects interview outcomes
- [[Company_DNA_Evolution]] - Your DNA history is evaluated

❓ **OPEN QUESTIONS:**
- Interview length and question count?
- Can you research the fed before interview?
- Multiple interview rounds for bigger positions?

✅ **STATUS:** 🔒 LOCKED

---

## VERSION HISTORY

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 3 lines 410-412 | 🔒 LOCKED |

---

## INTERVIEW FLOW

When you apply for a job:

1. Board of owners or network execs invite you to "interview"
2. You're asked questions across several categories
3. Your answers are evaluated against their goals and your history
4. Success or rejection determined

---

## INTERVIEW QUESTIONS

| Question Type | Example |
|---------------|---------|
| **Vision** | "Where do you see this promotion in five years?" |
| **Creative Tone** | "What's your booking philosophy?" |
| **Fix or Preserve** | "What would you change? What would you protect?" |
| **Immediate Strategy** | "Walk us through your first 6 months." |
| **Crisis Management** | "What would you have done during the Tsukasa Strike?" |
| **Cultural Fit** | "How do you feel about unions? About spectacle over sport?" |
| **Talent Trust** | "Why do you think the locker room would follow you?" |

---

## INTERVIEW SUCCESS FACTORS

Success depends on:

- **Your reputation + history** (DNA record, scandal fallout, past eras)
- **How aligned your answers are with:**
  - Their current goals
  - TV expectations
  - Internal locker room mood
- **Whether you're realistic or full of BS**

---

## INTERVIEW OUTCOMES

**Success:**
- You get the position
- Start booking with their existing roster and situation
- Inherit their DNA, problems, and opportunities

**Failure:**
- "Thank you for your time. We're going in a different direction."
- Cooldown period before you can reapply
- May affect your reputation (too many rejections = perceived as washed)

---

## INVESTOR PITCH (STARTUP VARIANT)

When starting your own promotion, you pitch to potential investors using the same system:

| Question Type | Example |
|---------------|---------|
| **Market Vision** | "Why does wrestling need another promotion?" |
| **Differentiation** | "How will you stand out from existing feds?" |
| **Financial Plan** | "How do you plan to be sustainable in year one?" |
| **Talent Strategy** | "Who are you building around?" |
| **Risk Assessment** | "What's your biggest vulnerability?" |

**Investor Pitch Success Factors:**
- Your track record
- Market conditions
- How much capital you're asking for
- How realistic your plan sounds

---

## IMPLEMENTATION NOTES

### Interview Structure

```json
{
  "interview_id": "interview_001",
  "position": "head_booker",
  "promotion": "federation_xyz",
  "interviewer_type": "board_committee",
  "questions_asked": [
    {
      "type": "vision",
      "question": "Where do you see this promotion in five years?",
      "player_response": "...",
      "alignment_score": 72
    },
    {
      "type": "crisis_management",
      "question": "What would you have done during the Tsukasa Strike?",
      "player_response": "...",
      "alignment_score": 85
    }
  ],
  "reputation_modifier": +15,
  "total_score": 78,
  "threshold": 70,
  "outcome": "hired"
}
```

---

## RELATED SYSTEMS

- **[[Booker_Succession_System]]:** Interviews happen after ouster
- **[[Global World Mode]]:** Apply for jobs while observing
- **[[Startup Promotion System]]:** Investor pitches use similar mechanics
- **[[Company_DNA_Evolution]]:** Your DNA history is part of evaluation

---

**Document Status:** 🔒 LOCKED  
**Last Updated:** 2025-12-26  
**Next Review:** Question pool expansion
