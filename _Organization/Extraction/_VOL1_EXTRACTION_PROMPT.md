# SCS VOL 1 EXTRACTION PROMPT
## Line-by-Line Verification Sweep

**Copy this into a new chat when starting work on Volume 1 extraction.**

---

## 🎯 TASK

You are performing a **line-by-line extraction sweep** of SCS Volume 1, Chunk **XX** (lines **XXX-XXX**).

This is NOT pattern-matching or keyword searching. You are reading every line, checking against the fingerprint, and documenting anything not already captured.

**Workflow:**
1. READ the fingerprint (what's already captured)
2. READ the chunk (raw source material)
3. FIND items in chunk not in fingerprint
4. WRITE new items to Extraction Report first, then Fingerprint

---

## 📂 FILES TO READ

Use `filesystem:read_text_file` (lowercase!) to load:

1. **Fingerprint:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\_EXTRACTION_FINGERPRINT.txt`
   - This contains all concepts already extracted from Vol 1
   - Use Ctrl+F against this when evaluating if something is NEW

2. **Chunk Tracker:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\_VOL1_CHUNKS\README.md`
   - Shows which chunks have been reviewed
   - Update status when done

3. **Source Chunk:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\_VOL1_CHUNKS\VOL1_CHUNK_XX_lines_XXX-XXX.txt`
   - This is the RAW SOURCE MATERIAL you are scanning
   - Read the ENTIRE chunk line by line
   - Do not skim, do not pattern-match, do not skip "boring" parts

## 📂 FILES TO WRITE (if new items found)

4. **Extraction Report:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\VOL1_EXTRACTION_REPORT.md`
   - MASTER file for all extracted items
   - Add new items here FIRST with proper numbering

5. **Fingerprint:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\_EXTRACTION_FINGERPRINT.txt`
   - Mirror of extraction report for quick searching
   - Update AFTER adding to extraction report

---

## 📋 EXTRACTION PROTOCOL

For EACH line in the chunk:

1. **Read it fully** (even if it looks like meta-discussion)
2. **Check fingerprint** for any concept, mechanic, or calibration mentioned
3. **If NOT in fingerprint:** Document it with:
   - Name/concept
   - Type: MECHANIC / CONCEPT / FORMULA / CALIBRATION / HALFBAKED / QUOTE
   - Brief description
   - Line number or approximate location

### What counts as NEW:
- Any specific numeric value not in fingerprint
- Any wrestler calibration example not listed
- Any formula or threshold not documented
- Any system interaction not captured
- Any half-baked idea not in the HB list
- Any locked design decision stated definitively

### What does NOT count as NEW:
- General discussion about AI capabilities
- Timeline predictions
- Meta-discussion about the project itself
- Repetition of concepts already in fingerprint

---

## 📝 OUTPUT FORMAT

After reading the chunk, produce:

```markdown
## CHUNK XX EXTRACTION REPORT
**Lines:** XXX-XXX
**Date:** YYYY-MM-DD

### NEW ITEMS FOUND
| # | Name | Type | Description | Line/Location |
|---|------|------|-------------|---------------|
| 1 | [name] | [type] | [description] | ~line XXX |

### ITEMS CONFIRMED (already in fingerprint)
[List major systems/concepts that appeared and were already captured]

### NOTES
[Any ambiguities, things that need cross-referencing, etc.]

### FILES UPDATED
- [ ] VOL1_EXTRACTION_REPORT.md (added items #XXX-XXX)
- [ ] _EXTRACTION_FINGERPRINT.txt (synced)
- [ ] _VOL1_CHUNKS\README.md (marked complete)

### STATUS
⬜ More items may exist (incomplete read)
✅ Chunk fully reviewed, all items captured
```

---

## ⚠️ CRITICAL RULES

1. **NO SKIMMING** - Every line must be read
2. **NO ASSUMPTIONS** - Check fingerprint before calling something "already captured"
3. **NO INVENTION** - Only extract what's stated, don't infer or expand
4. **FLAG UNCERTAINTY** - If unsure whether something is new, list it anyway with a ? marker
5. **UPDATE BOTH FILES** - Extraction Report is master, Fingerprint mirrors it

---

## 🔄 AFTER COMPLETING CHUNK

1. **If NEW items found:**
   - Add to `VOL1_EXTRACTION_REPORT.md` FIRST (master file)
     - Use next available item number in appropriate section
     - Follow existing format (## XX. ITEM NAME, DESTINATION, TYPE, ACTION)
   - Then add to `_EXTRACTION_FINGERPRINT.txt` (keep in sync)
     - Add under appropriate section header
     - Include key terms for Ctrl+F matching

2. **Update tracker:** Mark chunk complete in `_VOL1_CHUNKS\README.md`

3. **Note for later:** If items need proper mechanic files, flag them

**The Extraction Report is the canonical master list. The Fingerprint mirrors it for quick searching.**

---

## 📊 CHUNK INDEX

| Chunk | Lines | Size | Content Focus |
|-------|-------|------|---------------|
| 01 | 001-127 | 119KB | AI timeline discussion, vision |
| 02 | 128-254 | 93KB | [TBD] |
| 03 | 255-381 | 94KB | [TBD] |
| 04 | 382-508 | 122KB | [TBD] |
| 05 | 509-635 | 110KB | [TBD] |
| 06 | 636-762 | 127KB | [TBD] |
| 07 | 763-889 | 96KB | [TBD] |
| 08 | 890-1016 | 121KB | [TBD] |
| 09 | 1017-1143 | 100KB | [TBD] |
| 10 | 1144-1265 | 64KB | [TBD] |

---

## 🛠️ TOOL USAGE REMINDER

**ALWAYS use lowercase `filesystem:` tools, NEVER uppercase `Filesystem:`.**

The uppercase version will fail on the Obsidian vault.

---

## 🚀 QUICK START

Copy this into a new chat (replace XX with chunk number):

```
I'm doing a line-by-line extraction sweep of SCS Volume 1, Chunk XX (lines XXX-XXX).

Read the full instructions at:
Z:\Documents\Obsidian\Lune\SCS\System Bible\_VOL1_EXTRACTION_PROMPT.md

Then:
1. Load the fingerprint (what's already captured)
2. Read the chunk file (raw source to scan)
3. Find anything new, add to Extraction Report + Fingerprint

Source chunk:
Z:\Documents\Obsidian\Lune\SCS\System Bible\_VOL1_CHUNKS\VOL1_CHUNK_XX_lines_XXX-XXX.txt

Use lowercase filesystem: tools only.
```
