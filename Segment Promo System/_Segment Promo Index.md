# Segment & Promo System

📛 **SYSTEM:** Segment & Promo Engine
🧭 **CATEGORY:** Booking & Simulation / Non-Match Content
🔑 **KEYWORDS:** segment, promo, interview, ambush, contract signing, derailing, mic skills, crowd hijack, DNA, voice, character
📝 **SUMMARY:** Manages non-wrestling content that builds feuds and characters. Includes segment types, promo evaluation, crowd response mechanics, derailing/recovery systems, and character DNA for content generation. Promos are era-locked and region-sensitive, with crowd hijacking as a real risk.

⚙️ **LOGIC OVERVIEW:**
- Segments use same evaluation framework as matches (Intent, Tone, Placement, Execution)
- Promo quality depends on worker mic skills, character work, and crowd response
- Promo DNA encodes character voice for generation across hardware tiers
- Angle DNA encodes physical storytelling patterns for attack segments
- Crowd can hijack segments ("What?" chants, competing chants, boredom)
- Derailing mechanics track when crowd takes over and recovery options
- Era-locked behaviors (certain chants only exist in certain periods)
- Segment outcomes affect Buzz, Feud Memory, and worker morale

🔬 **LLM INTEGRATION:** Yes. LLM generates promo scripts from DNA profiles, evaluates crowd response flavor, suggests recovery options for derailed segments, and creates era-appropriate dialogue. Scales from templates (potato) to full generation (high-end).

📌 **ORIGIN:** Vol 2-3 (segment engine in Booking Engine Phase 3), Vol 7 (Promo Response System with derailing mechanics), December 2024 conversation (DNA systems)

📎 **CONNECTED SYSTEMS:**
- [[Booking_Engine_P1-3|Booking Engine]] - segments are booking inputs
- [[Crowd Signals/_Crowd Signals Index|Crowd Signals]] - chants and reactions during promos
- [[Buzz System/_Buzz System Index|Buzz System]] - promo outcomes affect Buzz
- [[Feud_Memory|Feud Memory]] - promos create memory anchors
- [[Emotional_Show_Flow|Emotional Show Flow]] - segments have emotional tags
- [[Worker_Skills|Worker Skills]] - Mic Skills, Character Work affect quality
- [[Hidden_Personality|Hidden Personality]] - constrains DNA mutation and options
- [[AI_Tiered_Integration|AI Tiered Integration]] - determines generation approach

❓ **OPEN QUESTIONS:**
- Exact derailing threshold formula
- Scripted vs shoot promo mechanics
- Manager/mouthpiece delegation rules
- DNA mutation rates and triggers

✅ **STATUS:** Locked (core mechanics), Exploratory (DNA systems)

---

## VERSION HISTORY

**Version 1.0 (Vol 2-3)**
- Segment Engine introduced as Booking Engine Phase 3
- Basic segment types defined
- Promo evaluation framework established

**Version 2.0 (Vol 7)**
- Promo Response System fully formalized
- Derailing mechanics added (crowd hijack)
- Era-locked chant behaviors introduced
- Recovery options for failed segments
- "What?" chants and crowd takeover rules

**Version 2.1 (December 2024) [CURRENT]**
- Promo DNA system added for character voice generation
- Angle DNA system added for physical segment generation
- Integration with AI Tiered system for hardware scaling
- DNA mutation through anchors and career events

---

## Mechanics in This System

### Core Mechanics (Locked)
- [[Segment Types]] - Categories of non-match content
- [[Promo Evaluation]] - What makes a promo work or fail
- [[Promo Response]] - How crowds react, including derailing
- [[Segment Outcomes]] - Effects on Buzz, Memory, Morale
- [[Derailing Recovery]] - Options when crowd hijacks segment

### DNA Systems (Exploratory)
- [[Promo_DNA]] - Character voice encoding for content generation
- [[Angle_DNA]] - Physical storytelling patterns for attack segments
