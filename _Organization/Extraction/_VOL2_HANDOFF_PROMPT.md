# SCS SESSION HANDOFF: VOL 2 DEEP EXTRACTION

**Created:** 2025-12-25
**For:** Next Claude session
**Project:** Squared Circle Soul (SCS) Wrestling Booking Simulator

---

## 🎯 MISSION

Deep extract Volume 2 using the same line-by-line methodology that successfully captured 311 items from Volume 1.

---

## 📍 CURRENT STATE

### Vol 1: ✅ COMPLETE
- 311 items extracted (line-by-line, 10 chunks)
- 7 integration batches (A-G) merged into Bible
- 6 new system files created
- 44 half-baked concepts added to Parking Lot
- All tracking files updated

### System Bible Status
- **36 folders** | **~165 files** | **43 systems** | **~320 mechanics**
- Duplicates resolved, wikilinks validated, INDEX v2.0 complete

---

## 📂 KEY FILE LOCATIONS

### Source Material
```
C:\Users\Oyaji\Desktop\SCS\_Main Volume PDFs\txt_conversions\SCS Vol. 2 - [filename].txt
```

### Bible Root
```
Z:\Documents\Obsidian\Lune\SCS\System Bible\
```

### Tracking Files
```
Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization\Tracking\_PROGRESS.md
Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization\Tracking\_MASTER_MECHANICS_INDEX.md
Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization\Tracking\_INDEX.md
```

### Extraction Files
```
Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization\Extraction\
```

---

## 🔧 METHODOLOGY (Proven with Vol 1)

### Step 1: Chunk the Volume

Vol 2 is ~150 pages. Create manageable chunks:

```bash
# Check file size and line count first
wc -l "C:\Users\Oyaji\Desktop\SCS\_Main Volume PDFs\txt_conversions\SCS Vol. 2*.txt"

# Read in chunks of ~100-150 lines
head -n 150 [file]           # Chunk 1
sed -n '151,300p' [file]     # Chunk 2
# etc.
```

Create a chunk tracker file:
```
Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization\Extraction\_VOL2_CHUNK_TRACKER.md
```

### Step 2: Line-by-Line Extraction

For each chunk, scan for:
- **Numbers/formulas** (+10, ×1.5, 1-20 scale, thresholds)
- **System keywords** (tag, trait, modifier, bonus, penalty, threshold)
- **Design decisions** ("should," "could," "locked," "final")
- **Real wrestling examples** used as design basis
- **Mechanics buried in prose** (Vol 1 had many)

### Step 3: Document Findings

For each item found:
```markdown
### #XXX - [CONCEPT NAME]
**Source:** Vol 2, Chunk X, ~Line Y
**Category:** MECHANIC / CONCEPT / HALFBAKED / REFERENCE
**Description:** [What it does]
**Destination:** [Which Bible file to update, or NEW]
```

Number items sequentially starting from #312 (Vol 1 ended at #311).

### Step 4: Batch Organization

Group items by domain for integration:
- **Batch A:** Worker Foundation (skills, personality, tags)
- **Batch B:** Booking Core (engine, trails, momentum)
- **Batch C:** Match Performance (engine, types, chemistry)
- **Batch D:** Worker Lifecycle (contracts, injuries, aging, retirement)
- **Batch E:** World/Business (territory, media, financial)
- **Batch F:** Governance/Meta (AI, LLM, simulation)
- **Batch G:** Catchall/Half-Baked (parking lot)

### Step 5: Integration

For each batch:
1. Check existing Bible files for related content
2. Add new mechanics to appropriate sections
3. Create new files only if system doesn't exist
4. Update Master Mechanics Index
5. Verify wikilinks

---

## ⚠️ CRITICAL REMINDERS

### Tool Usage
**ALWAYS use lowercase `filesystem:` tools** for file operations.
- ✅ `filesystem:read_text_file`
- ✅ `filesystem:write_file`
- ❌ `Filesystem:read_text_file` (will fail on Z:\ drive)

### Extraction Principles
1. **Extract, don't invent** - Capture what exists, don't add new ideas
2. **Check before adding** - Search existing files to avoid duplication
3. **Track provenance** - Always note Vol/Chunk/Line for new items
4. **Flag uncertainties** - Use ❓ for open questions, 📝 for concepts needing work
5. **Preserve half-baked** - Don't discard exploratory ideas, park them

### Vol 2 Expected Content (from Synthesis Report)
- Worker archetypes (12 core + expansions)
- Booking engine refinements
- Push strategies and false popularity
- Momentum vs Popularity distinction
- Early feud memory concepts
- Turn engine foundations

---

## 📋 FIRST SESSION TASKS

1. **Locate Vol 2 txt file** in source folder
2. **Check file size** and determine chunk count
3. **Create `_VOL2_CHUNK_TRACKER.md`** with chunk table
4. **Process Chunk 01** (first ~100-150 lines)
5. **Document findings** with item numbers starting #312
6. **Update tracker** with progress

---

## 🗣️ COMMUNICATION STYLE

- Direct and honest, no sugarcoating
- Socialist lens, philosophical depth without pretension
- Gen Z humor without cringe
- Never use em dashes (use commas, colons, parentheses)
- Cross-reference past work to avoid drift

---

## 📞 IF STUCK

- Check `_PROGRESS.md` for project status
- Check `_MASTER_MECHANICS_INDEX.md` for existing mechanics
- Check `_INDEX.md` for folder structure
- Search existing Bible files before creating new ones
- Ask user for clarification on ambiguous content

---

## 🎯 SUCCESS CRITERIA

Vol 2 is "sucked dry" when:
- [ ] All chunks processed line-by-line
- [ ] All items numbered and documented
- [ ] All batches integrated into Bible
- [ ] Master Mechanics Index updated
- [ ] Chunk tracker shows all ✅
- [ ] No unique content left unextracted

---

**Let's extract Volume 2. Same methodology, same rigor, same results. 🔥**
