# Media System

📛 **SYSTEM ID:** MEDIA-001
🧭 **CATEGORY:** World Interaction / External Coverage
🔑 **KEYWORDS:** media, press, dirtsheet, newspaper, coverage, interview, rumor, leak, journalist, social media
📝 **SUMMARY:** 

The Media System governs how wrestling is covered by external media, from mainstream newspapers to insider dirtsheets to (in modern eras) social media. Media coverage affects popularity, buzz, scandal impact, and public perception. Different eras have different media landscapes, from kayfabe-protected newspaper coverage in the territories to instant virality in the social media age.

⚙️ **LOGIC OVERVIEW:**
- Media outlets have different reach, credibility, and access
- Coverage probability based on newsworthiness and outlet type
- Dirtsheets break kayfabe, mainstream protects it (in territory era)
- Scandals require media coverage to become public
- Interviews and press conferences create promo opportunities
- Era determines media landscape (1985 vs. 2005 vs. 2020)

🔬 **LLM INTEGRATION:** High (generating articles, interview content, social media posts)

📌 **ORIGIN:** Vol 1-4 (mentions throughout), Booking Engine (buzz/dirtsheet references), Scandal System (coverage concepts)

📎 **CONNECTED SYSTEMS:** 
- [[Popularity_System|Popularity]] - Media affects pop growth
- [[Buzz System/_Buzz System Index|Buzz System]] - Media creates buzz
- [[Scandal System/_Scandal System Index|Scandal System]] - Media coverage determines scandal impact
- [[Booking_Engine_P1-3|Booking Engine]] - Segments include media interactions
- [[Gimmick System/_Gimmick System Index|Gimmick System]] - Kayfabe protection

❓ **OPEN QUESTIONS:**
- Media outlet types and reach formulas
- Coverage probability calculations
- Rumor/leak mechanics
- Interview system mechanics
- Press conference booking
- Social media posting (modern eras)
- Era-specific media landscapes

✅ **STATUS:** Conceptual (referenced in other systems, never built as standalone)

---

## VERSION HISTORY

**Version 0.5 (Vol 1-4) [CONCEPTUAL]**
- Media concepts referenced throughout other systems
- Dirtsheet mentions in Buzz System
- Scandal coverage concepts in Scandal System
- Kayfabe protection discussed in Gimmick System
- No standalone mechanics defined yet

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Media Outlets]] | Types of media and their characteristics | 📝 Conceptual |
| [[Coverage Mechanics]] | How events become news | 📝 Conceptual |
| [[Era Media Landscape]] | How media changes by era | 📝 Conceptual |

---

## Design Philosophy

Media isn't just flavor; it's how wrestling reaches the public. The relationship between wrestling and media has evolved dramatically:

**Territory Era (1985):** Kayfabe protected by mainstream press. Dirtsheets are underground, limited reach. Local newspapers cover wrestling as sport.

**Monday Night Wars (1995-2001):** Media attention increases. Internet dirtsheets emerge. Kayfabe erodes as behind-the-scenes becomes news.

**Modern Era (2010+):** Social media makes everyone a reporter. Instant virality. Kayfabe impossible to maintain. Workers have direct fan access.

---

## Integration with Existing Systems

**With Popularity:**
- Positive coverage boosts pop
- Negative coverage (scandal) damages pop
- No coverage = slower growth

**With Buzz:**
- Media attention creates buzz
- Dirtsheet coverage signals "insider heat"
- Viral moments spike buzz

**With Scandal:**
- Scandals don't exist publicly until covered
- Media outlet type determines scandal spread
- Cover-up success depends on media management

---

## Implementation Priority

**Phase 1:** Basic coverage effects on popularity/buzz
**Phase 2:** Era-specific media landscapes
**Phase 3:** Full interview/press conference system

---

**Document Status:** Index Complete, System Conceptual
**Last Updated:** 2025-12-21
**Next Review:** Design media outlet typology
