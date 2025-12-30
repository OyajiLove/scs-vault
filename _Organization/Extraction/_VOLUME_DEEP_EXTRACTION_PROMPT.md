# SCS Volume Deep Extraction Protocol

## 🎯 PURPOSE

This prompt guides a systematic, exhaustive pass through each SCS design volume to extract:
- **Missed locked mechanics** (formulas, thresholds, specific values)
- **Half-baked ideas** (concepts mentioned but never developed)
- **Unanswered questions** (things flagged for "later" that never got resolved)
- **Design decisions** (rationale for why things work the way they do)
- **Edge cases** (weird scenarios discussed but not formalized)
- **Terminology** (definitions, distinctions, naming conventions)
- **Examples** (concrete scenarios that illustrate mechanics)
- **Contradictions** (things that conflict with locked systems)
- **Dependencies** (systems that reference each other)
- **TODO markers** (anything flagged for future work)

---

## 📋 EXTRACTION CHECKLIST (Per Volume)

Use this checklist for each volume pass:

### 1. Search Patterns
Run these searches against the volume text:

**Lock Markers:**
- `locked`, `final`, `canonical`, `confirmed`
- `✅`, `✓`, `approved`, `shipped`
- `this is how`, `we're going with`, `settled on`

**Half-Baked Markers:**
- `maybe`, `possibly`, `could be`, `might work`
- `later`, `eventually`, `future`, `someday`
- `TODO`, `TBD`, `placeholder`, `stub`
- `not sure`, `unclear`, `need to figure out`
- `what if`, `consider`, `explore`

**Question Markers:**
- `?` (especially in tovarisch's messages)
- `should we`, `do we need`, `how does`
- `what about`, `where does`, `when do`
- `open question`, `unresolved`, `decision needed`

**Numeric Values:**
- Any numbers (thresholds, multipliers, ranges)
- Percentages, scales, formulas
- Time durations (days, weeks, months)
- Decay rates, growth rates

**Examples & Scenarios:**
- Worker names (real or fictional)
- Promotion names
- Match descriptions
- Booking scenarios
- "For example", "like when", "imagine if"

**Worker Agency & Resistance (CRITICAL):**
- `refuse`, `demand`, `negotiate`, `unwilling`
- `resist`, `pushback`, `complain`, `walk`, `quit`
- `creative control`, `protect`, `leverage`
- `package deal`, `bond`, `loyalty`

**Emotional/Philosophical Language (CRITICAL):**
- `feel`, `felt`, `struggle`, `heart`, `soul`, `beauty`
- `visceral`, `raw`, `real`, `authentic`
- `tears`, `silence`, `gasp`, `cry`, `scream`
- Philosophy statements: "the goal is", "what matters is", "this is why"

**Relationship & Chemistry:**
- `loyalty`, `trust`, `betray`, `grudge`, `respect`
- `tension`, `heat`, `chemistry`, `bond`
- `friend`, `enemy`, `rival`, `clique`
- `memory of slights`, `resentment`

**TEW/Competitor Critique (Hidden Gold):**
- `TEW`, `EWR`, `Fire Pro`, `OOTP`
- `dog shit`, `broken`, `stinks`, `flaw`
- `fix`, `better`, `should be`, `instead`
- Rants often contain the REAL design intent

**Aging & Career Arc:**
- `age`, `aging`, `decline`, `peak`, `prime`
- `veteran`, `rookie`, `debut`, `retire`
- `lifestyle`, `genetics`, `wear`, `scar`

**World Building & Settings:**
- `era`, `region`, `territory`, `culture`
- `kayfabe`, `modern`, `social media`
- `slider`, `setting`, `option`, `toggle`

### 2. Extraction Categories

For each item found, categorize as:

| Category | Description | Action |
|----------|-------------|--------|
| 🔒 LOCKED | Confirmed mechanic with specifics | Add to existing bible entry |
| 🟡 HALF-BAKED | Concept without full spec | Add to Parking Lot |
| ❓ UNANSWERED | Question never resolved | Add to system's Open Questions |
| 💡 DESIGN RATIONALE | Why something works this way | Add as Implementation Note |
| ⚠️ EDGE CASE | Weird scenario discussed | Add to system's Edge Cases |
| 📖 DEFINITION | Term or distinction clarified | Add to Glossary/relevant system |
| 📊 EXAMPLE | Concrete scenario | Add to system as example |
| ⚔️ CONTRADICTION | Conflicts with locked system | Flag for resolution |
| 🔗 DEPENDENCY | System references another | Verify wikilink exists |
| 📝 TODO | Flagged for future work | Add to Parking Lot |

### 3. System-by-System Sweep

For each known system, search for:
- The system name and variations
- Related keywords
- Connected mechanics

**Core Systems to Check:**
1. Worker Skills (skills, stats, ratings, 1-20)
2. Hidden Personality (ego, loyalty, morality, drive, archetypes)
3. Tags System (tags, anchors, boolean, categories)
4. Popularity (pop, over, regional, demographic)
5. Booking Engine (phase, booking, show, card)
6. Emotional Flow (pacing, crowd energy, stamina)
7. Crowd Memory (remember, forget, decay, anchor)
8. Feud Memory (feud, rivalry, history, heat)
9. Turn Engine (turn, heel, face, betrayal)
10. Predictability (predictable, surprise, stakes, cynicism)
11. Match Engine (match, bout, quality, spots)
12. Buzz System (buzz, heat, momentum, viral)
13. Gimmick System (gimmick, character, persona)
14. Contract System (contract, deal, money, negotiate)
15. Injury System (injury, hurt, recovery, pain)
16. Scandal System (scandal, controversy, heat)
17. Title System (title, belt, championship, lineage)
18. Faction System (faction, stable, alliance, clique)
19. Training System (train, develop, improve, dojo)
20. Aging System (age, decline, peak, veteran)

---

## 🔍 VOLUME-SPECIFIC PROMPT

Copy and adapt this prompt for each volume:

```
I'm doing a deep extraction pass on SCS Volume [X] to ensure nothing was missed during the initial bible creation. The goal is to find:

1. **Missed Locked Mechanics** - Any formulas, thresholds, or specific values not yet in the bible
2. **Half-Baked Ideas** - Concepts mentioned but never fully developed
3. **Unanswered Questions** - Things flagged for "later" that were never resolved
4. **Design Rationale** - Explanations for WHY systems work the way they do
5. **Edge Cases** - Weird scenarios discussed but not formalized
6. **Examples** - Concrete scenarios that illustrate mechanics
7. **TODO Markers** - Anything explicitly flagged for future work

**Current Bible Status:**
- 36 systems extracted across 159 files
- Tiers 1-3 complete
- All major mechanics documented

**What I Need:**
1. Search the volume for the patterns listed above
2. For each finding, categorize it (Locked/Half-Baked/Question/Rationale/Edge Case/Example/TODO)
3. Note which existing system it belongs to (or if it's a new concept)
4. Extract the specific content with context
5. Flag any contradictions with existing locked systems

**Output Format:**
For each finding:
```
### [CATEGORY EMOJI] Finding: [Brief Title]
**System:** [Which system this belongs to]
**Source:** Vol [X], approximately [context]
**Content:** [The actual extracted text/concept]
**Action:** [Add to X / Update Y / Flag for review / Add to Parking Lot]
```

**Volume [X] Focus Areas:**
[Add volume-specific focus based on known content]

Let's go line by line and miss nothing. Start with a structural overview of the volume, then systematic extraction.
```

---

## 📚 VOLUME-SPECIFIC NOTES

Use these notes to focus each volume pass:

### Volume 1 (~1MB, ~160 pages)
**Primary Content:** Foundation conversation, archetypes, initial booking logic, TEW+++ vision
**Nature:** Exploratory dialogue, not formal design doc. Ideas embedded in rants and tangents.
**Focus Areas:**
- Early vision statements (what was the original intent?)
- Initial worker personality concepts
- Match engine prototypes
- Booking logic first drafts
- Any deprecated concepts that got replaced
- TEW critiques (contain design intent)
- Emotional/philosophical statements about wrestling
- Worker resistance/agency concepts
- Package deal mechanics for teams/managers

**EXTRACTION COMPLETE:** 99 items across 6 sections (A-F)
- A: Worker Skills (6)
- B: Archetypes (23) 
- C: Additional Mechanics (11)
- D: Booking & Simulation (11)
- E: Half-Baked Ideas (37)
- F: Final Sweep Additions (11)

### Volume 2 (~150 pages)
**Primary Content:** Booking Engine Phases 1-3, Feud Memory
**Focus Areas:**
- Phase 1-3 specific formulas
- Feud memory decay rates
- Crowd memory thresholds
- Turn engine specifics
- Predictability calculations

### Volume 3 (~200 pages)
**Primary Content:** Emotional Flow, Fighting Spirit, Tags finalization
**Focus Areas:**
- Emotional tag definitions
- Pacing formulas
- Fighting Spirit archetype details
- Tag category distinctions
- Hidden Personality early specs

### Volume 4 (~215 pages)
**Primary Content:** Hidden Personality expansion, Sim-World Systems
**Focus Areas:**
- All 17 archetype stat ranges
- Contract system formulas
- Injury calculation specifics
- Title lineage mechanics
- Faction power struggle details
- Training system mechanics

### Volume 5 (~150 pages)
**Primary Content:** Booking Trails, Buzz System
**Focus Areas:**
- Trail milestone definitions
- Buzz calculation formulas
- Heat evolution into Buzz
- Long-term booking mechanics
- Calendar integration

### Volume 6 (~100 pages)
**Primary Content:** Hall of Fame, Gimmick, Crowd Signals
**Focus Areas:**
- HoF induction thresholds
- Gimmick lock mechanics
- Crowd signal triggers
- Chant emergence rules
- Era-specific behaviors

### Volume 7 (~80 pages)
**Primary Content:** Promo Response, Visual systems
**Focus Areas:**
- Promo scoring mechanics
- Crowd derailment rules
- Response type definitions
- Render/visual concepts
- Character appearance systems

### Volume 8 (~60 pages)
**Primary Content:** Character development, Bobby Shy, Don Sangre
**Focus Areas:**
- Specific character profiles
- Ringstate lore details
- Narrative examples
- Regional flavor
- Cultural authenticity notes

### Volume 8.5 (~40 pages)
**Primary Content:** Supplemental material
**Focus Areas:**
- Anything not covered in Vol 8
- Clarifications
- Additional examples
- Edge cases

### Volume 9 (~50 pages)
**Primary Content:** Systems refinement
**Focus Areas:**
- Updates to earlier systems
- Conflict resolutions
- Formula refinements
- New edge cases

### Volume 10 (~80 pages)
**Primary Content:** Tag Audit begins
**Focus Areas:**
- Tag/Anchor distinction development
- Batch audits (which tags survived?)
- Categorization decisions
- Deprecation reasons

### Volume 11 (~100 pages)
**Primary Content:** V5 Master List finalization
**Focus Areas:**
- Final 394 tags
- Present-tense conversion
- Anchor seed list
- Category finalization

### Volume 12 (~? pages)
**Primary Content:** System Audit part 1
**Focus Areas:**
- LLM integration decisions
- Memory handling architecture
- Platform scaling concepts
- Performance optimization

### Volume 13 (~? pages)
**Primary Content:** System Audit part 2
**Focus Areas:**
- AI booker specifications
- Simulation fidelity tiers
- Final system validations
- Future roadmap items

---

## 📤 OUTPUT STRUCTURE

After each volume pass, compile findings into:

### 1. Additions to Existing Systems
```markdown
## Additions from Vol [X]

### [System Name]
- **New mechanic:** [description]
- **Formula found:** [formula]
- **Edge case:** [scenario]
- **Example:** [concrete example]
```

### 2. Parking Lot Additions
```markdown
## New Parking Lot Items from Vol [X]

### [Concept Name]
**Source:** Vol [X]
**Description:** [what it is]
**Status:** [half-baked / question / deprecated?]
**Related Systems:** [what it might connect to]
```

### 3. Open Questions Found
```markdown
## Unanswered Questions from Vol [X]

### Q: [Question]
**Context:** [where it came up]
**Related System:** [which system this affects]
**Possible Answers:** [any partial answers found]
```

### 4. Contradictions Found
```markdown
## Contradictions from Vol [X]

### [Topic]
**Vol [X] says:** [content]
**Locked system says:** [content]
**Resolution:** [which is canonical / needs decision]
```

---

## ⚡ QUICK START

To begin extraction on any volume:

1. Load the volume text
2. Run structural scan (headers, sections, topic flow)
3. Search for lock markers first (capture confirmed mechanics)
4. Search for question markers (capture unresolved items)
5. Search for half-baked markers (capture ideas)
6. System-by-system keyword search
7. Compile findings by category
8. Update bible entries and parking lot
9. Log in migration tracker

---

## 🎯 SUCCESS CRITERIA

A volume is "sucked dry" when:
- [ ] All lock markers searched and findings extracted
- [ ] All question markers searched and findings extracted
- [ ] All half-baked markers searched and findings extracted
- [ ] All 20 core systems searched for mentions
- [ ] All numeric values captured
- [ ] All examples documented
- [ ] All contradictions flagged
- [ ] Findings compiled into structured output
- [ ] Bible entries updated
- [ ] Parking lot updated
- [ ] Migration log updated

---

*"Leave nothing on the mat."* 🤼

---

## 🚨 LESSONS LEARNED (Vol 1 Extraction)

### Why We Almost Missed 11 Critical Ideas

**1. Search Term Tunnel Vision**
Early passes focused on "locked", "final", "canonical". But gems like "Package Integrity: 95%" or "Austin refuses to job clean under 15 minutes" don't ping those terms.

**2. Conversational Format**
Volumes are dialogue, not docs. The Tag Team Package Deal stuff came up in a TEW rant. The Draw Power formula was embedded in calling Star Quality "dog shit." Match Report philosophy was in a tangent about Japanese wrestling making you *feel*.

**3. Philosophy vs. Formulas Bias**
We prioritized hard numbers (Menace 16+, Gimmick Fit 85%). Statements like "the struggle must be felt, not told" got skipped as vibes. But they're *core design philosophy* that guides implementation.

**4. Fresh Search Angles Matter**
The final sweep used terms we hadn't tried:
- "refuse/demand/negotiate" → worker resistance, creative control
- "protect/resistance" → package deals, push resistance  
- "lifestyle/aging" → lifestyle tracker concept
- "feel/struggle/heart" → emotional philosophy

### The Fix: Run Multiple Search Passes

**Pass 1: Mechanical** (formulas, thresholds, numbers)
**Pass 2: Conceptual** (maybe, could, what if, later)
**Pass 3: Emotional/Philosophical** (feel, struggle, soul, why)
**Pass 4: Critique-Based** (TEW, broken, should be, fix)
**Pass 5: Relationship/Agency** (refuse, demand, loyalty, betray)
**Pass 6: World Building** (era, region, culture, slider)

### Critical Insight
**The soul of SCS is in the rants as much as the tables.**

When tovarisch complains about TEW, they're describing what SCS *should* do. When they wax poetic about Japanese wrestling, they're defining match report philosophy. When they demand tag teams be respected, they're locking a core mechanic.

*Never skip the emotional language. That's where the vision lives.*

---

## 📋 VOLUME TRACKING

| Volume | Status | Findings | Last Pass |
|--------|--------|----------|-----------|
| Vol 1 | ✅ Complete | 99 items | 2024-12-23 |
| Vol 2 | ⬜ Pending | - | - |
| Vol 3 | ⬜ Pending | - | - |
| Vol 4 | ⬜ Pending | - | - |
| Vol 5 | ⬜ Pending | - | - |
| Vol 6 | ⬜ Pending | - | - |
| Vol 7 | ⬜ Pending | - | - |
| Vol 8 | ⬜ Pending | - | - |
| Vol 8.5 | ⬜ Pending | - | - |
| Vol 9 | ⬜ Pending | - | - |
| Vol 10 | ⬜ Pending | - | - |
| Vol 11 | ⬜ Pending | - | - |
| Vol 12 | ⬜ Pending | - | - |
| Vol 13 | ⬜ Pending | - | - |

---

*Created: 2025-12-22*
*Purpose: Ensure complete extraction before implementation phase*
