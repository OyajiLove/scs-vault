# VOLUME 1 INTEGRATION PLAN

**Created:** 2024-12-23
**Purpose:** Map extracted Vol 1 content to existing Bible systems, identify conflicts

---

## SUMMARY

| Category | Items | Destination | Status |
|----------|-------|-------------|--------|
| Worker Calibrations | 15+ | Worker_Skills.md | MERGE |
| Archetypes | 25+ finalized | NEW: Archetypes System | CREATE |
| New Tags | 10+ | Tags_System.md | MERGE |
| Overness Details | 1 system | Popularity_System.md | MERGE |
| Booking Systems | 8+ | Various existing | VERIFY |
| Lucha Politics | 1 system | NEW file | CREATE |
| Design Philosophy | 1 | README or new file | CREATE |

---

## 🔴 CONFLICTS IDENTIFIED

### 1. Archetype Location
**Issue:** Hidden_Personality.md has ~17 archetypes, extraction has 25+ detailed archetypes with skill ranges
**Resolution:** Create separate **Archetypes System** directory/file. Hidden_Personality should reference archetypes but not contain full definitions.

### 2. Overness vs Popularity
**Issue:** Extraction has detailed "Overness System 0-100" (#235), Popularity_System already covers this
**Resolution:** MERGE into Popularity_System.md. Add regional tracking examples, soft cap mechanics, Flair 1983 calibration example.

### 3. Basics Skill (#249)
**Issue:** New stat "Basics" (footwork, timing, ring movement) not in current Worker_Skills.md
**Resolution:** ADD to Worker_Skills.md Bell-to-Bell section. Calibrations: Arn 20, Windham 20, Hokuto 12-13.

---

## 📁 NEW FILES NEEDED

### 1. Archetypes System (Directory)
Location: `Z:\Documents\Obsidian\Lune\SCS\System Bible\Archetypes\`

Files needed:
- `_Archetypes_Index.md` - Master list, core skills rule
- `Technician.md` - #219 + subtypes
- `High_Flyer.md` - #220 + subtypes
- `Brawler.md` - #218 + subtypes
- `Shooter.md` - #221 + subtypes
- `Monster.md` - (from earlier extraction)
- `Giant.md` - #226 + subtypes
- `Hardcore.md` - #223 + subtypes
- `Charismatic_Entertainer.md` - #222 + subtypes
- `Heroic_Babyface.md` - #227 + subtypes
- `Tecnico.md` - #238 + subtypes (Lucha)
- `Rudo.md` - #239 + subtypes (Lucha)
- `Tweener.md` - #233 + subtypes
- `Heel_Ace.md` - #234 + subtypes
- `Wildcard.md` - #260 + subtypes
- `Cowardly_Heel.md` - #261 + subtypes
- `Junior_Puroresu.md` - #263 + 7 subtypes
- `Stoic_Ace.md` - #264 + subtypes
- `Defiant_Soul.md` - #265 + subtypes
- `Muga_Practitioner.md` - #268 + subtypes
- `Shady_Heel_Technician.md` - #267 + subtypes
- `Territory_Lifer.md` - #242 + subtypes
- `Jobber.md` - #252 + subtypes
- `Enforcer.md` - #255 (Technical Bruiser)
- `Old_School_Hero.md` - #258 + subtypes
- `Pure_Heel.md` - #259 + subtypes
- `Freak_Show_Attraction.md` - #240

### 2. Lucha Politics System
Location: `Z:\Documents\Obsidian\Lune\SCS\System Bible\Lucha_Politics.md`
Source: #241
Content: Family dynasties, No Yob Clause, mask protection, regional politics

### 3. Design Philosophy
Location: `Z:\Documents\Obsidian\Lune\SCS\System Bible\Design_Philosophy.md`
Source: #266 "Beauty in Struggle"
Content: Core design principles, litmus test, tagline

---

## 📝 MERGES INTO EXISTING FILES

### Worker_Skills.md
Add:
- [ ] Calibration reference table (#1-2): Rock, Vader, Sid, Luger, Steiner, Bret, Misawa, Jumbo, Inoki, Santo, Austin, Cena
- [ ] Design insights: "Charisma ≠ Flamboyance", "Menace Must Be Mythic", etc.
- [ ] Basics Skill (#249): New stat, add to Bell-to-Bell section
- [ ] Worker calibrations (#244, #246-248, #256-257, #269): Embry, Hokuto, Kawada, Hansen, FTR, Undertaker, Miz

### Tags_System.md
Add:
- [ ] Stiff Worker (#5): Regional reception table
- [ ] Fragile Warrior (#250): Definition, examples
- [ ] Selective Big Man Seller (#251): Definition, examples
- [ ] Weekend Warrior (#254): Definition, effects
- [ ] Scar Tissue (#224): Dynamic acquisition, effects
- [ ] Beauty In Struggle (#266): If used as tag vs philosophy

### Popularity_System.md
Add:
- [ ] Regional tracking example: Flair 1983 by territory (#235)
- [ ] Soft caps based on charisma/believability/cultural fit
- [ ] Overness Momentum (climbing/sliding)
- [ ] Hidden Reputation Modifiers
- [ ] Fan Type Reaction Modifiers

### Hidden_Personality.md
Update:
- [ ] Reference new Archetypes System directory
- [ ] Remove detailed archetype definitions (move to Archetypes/)
- [ ] Keep personality trait definitions

---

## ✅ VERIFICATIONS NEEDED

These items in extraction should confirm existing content:

| Item | Extraction # | Existing File | Action |
|------|--------------|---------------|--------|
| Master Skill Chart | #3 | Worker_Skills.md | VERIFY alignment |
| Worker Bio Fields | #4 | Worker_Skills.md | VERIFY present |
| Overness 0-100 | #6, #235 | Popularity_System.md | VERIFY scale matches |
| Psychology multiplier | Multiple | Worker_Skills.md | VERIFY documented |

---

## 🚧 HALF-BAKED (DO NOT INTEGRATE YET)

These go to SCS_PARKING_LOT.md:
- HB-42: Battle-Hardened Ace (Phase 2)
- HB-43: Strong Style Archetype (partial)
- HB-44: Tag Team Specialist Archetype (mentioned only)

---

## 📋 INTEGRATION ORDER

### Phase 1: Merges (Quick Wins)
1. Tags_System.md - Add new tags
2. Popularity_System.md - Add overness details
3. Worker_Skills.md - Add calibrations and Basics stat

### Phase 2: New Files
4. Create Archetypes directory
5. Create _Archetypes_Index.md
6. Create individual archetype files (can batch)

### Phase 3: Cleanup
7. Update Hidden_Personality.md to reference Archetypes/
8. Create Lucha_Politics.md
9. Create Design_Philosophy.md
10. Update _INDEX.md with new files

---

## QUESTIONS FOR USER

1. **Archetype granularity:** One file per archetype, or group by style (e.g., all Lucha archetypes in one file)?
2. **Calibrations placement:** Add to Worker_Skills.md main file, or create separate Worker_Calibrations.md?
3. **Lucha Politics:** Standalone file or subfolder under Territory System?

---

**Ready to begin Phase 1 merges on your go.**
