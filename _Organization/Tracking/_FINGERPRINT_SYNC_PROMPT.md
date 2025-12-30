# FINGERPRINT VERIFICATION & SYNC PROMPT

**Purpose:** Verify the fingerprint file contains everything from the extraction report, then establish workflow for future additions.

---

## 🎯 TASK

You need to:
1. Read the full VOL1_EXTRACTION_REPORT.md (all sections A-J)
2. Cross-reference against _EXTRACTION_FINGERPRINT.txt
3. Add any missing items to the fingerprint
4. Confirm the two files are in sync

---

## 📂 FILES TO WORK WITH

Use `filesystem:read_text_file` (lowercase!) to read:

1. **Extraction Report:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\VOL1_EXTRACTION_REPORT.md`
   - This is the MASTER source (196 items across 10 sections)
   - Read in chunks if needed (it's ~158KB, ~2000 lines)

2. **Fingerprint:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\_EXTRACTION_FINGERPRINT.txt`
   - This should MIRROR the extraction report for quick Ctrl+F lookup
   - Currently may be missing items from sections C-G

---

## 📋 VERIFICATION PROTOCOL

### Section-by-Section Check:

| Section | Items | Line Range (approx) | Status |
|---------|-------|---------------------|--------|
| A: Worker Skills | 1-6 | 1-100 | Verified ✅ |
| B: Archetypes | 7-29 | 100-400 | Verified ✅ |
| C: Additional Mechanics | 30-40 | 400-500 | NEEDS CHECK |
| D: Booking & Simulation | 41-51 | 500-600 | NEEDS CHECK |
| E: Half-Baked Ideas | 52-88 | 600-900 | NEEDS CHECK |
| F: Final Sweep | 89-99 | 900-1000 | NEEDS CHECK |
| G: Deep Sweep | 100-152 | 1000-1400 | NEEDS CHECK |
| H: Major Systems | 107-118 | 1400-1600 | Verified ✅ |
| I: Extended Systems | 119-137 | 1600-1800 | Verified ✅ |
| J: Final Sweep Systems | 138-150 | 1800-2000 | Verified ✅ |

### For Each Section:
1. Read the section from extraction report
2. List every numbered item (## XX. ITEM NAME or [SYSTEM #XXX])
3. Check fingerprint for each item
4. Note any MISSING items
5. Add missing items to fingerprint

---

## 📝 OUTPUT FORMAT

After verification, produce:

```markdown
## FINGERPRINT SYNC REPORT
**Date:** YYYY-MM-DD

### SECTION C VERIFICATION
| Item # | Name | In Fingerprint? |
|--------|------|-----------------|
| 30 | [name] | ✅ / ❌ |
| 31 | [name] | ✅ / ❌ |
...

### SECTION D VERIFICATION
[same format]

### ITEMS ADDED TO FINGERPRINT
| Item # | Name | Section |
|--------|------|---------|
| XX | [name] | C/D/E/F/G |

### SYNC STATUS
⬜ Incomplete - more sections need checking
✅ Complete - fingerprint matches extraction report
```

---

## 🔄 UPDATING THE FINGERPRINT

When adding items, maintain the structure:
- Group by section (## SECTION C: ADDITIONAL MECHANICS)
- Include item numbers (# 30. Tag Team Booking Logic)
- Add brief description or key terms for Ctrl+F matching

---

## ⚠️ CRITICAL RULES

1. **Extraction Report is MASTER** - fingerprint should match it, not vice versa
2. **Use lowercase `filesystem:`** - uppercase will fail on vault
3. **Read in chunks if needed** - file is large, may need multiple reads
4. **Don't invent** - only add what's explicitly in extraction report
5. **Preserve structure** - fingerprint has section markers, keep them

---

## 🛠️ TOOL USAGE

```
# Read extraction report (may need to chunk)
filesystem:read_text_file path="Z:\Documents\Obsidian\Lune\SCS\System Bible\VOL1_EXTRACTION_REPORT.md" head=500

# Read specific line range
filesystem:read_text_file path="..." view_range=[400, 600]

# Read fingerprint
filesystem:read_text_file path="Z:\Documents\Obsidian\Lune\SCS\System Bible\_EXTRACTION_FINGERPRINT.txt"

# Update fingerprint
filesystem:write_file path="Z:\Documents\Obsidian\Lune\SCS\System Bible\_EXTRACTION_FINGERPRINT.txt" content="..."
```

---

## 📌 AFTER SYNC IS COMPLETE

Update the extraction prompt to clarify the workflow:

**When chunk sweeps find NEW items:**
1. Add to VOL1_EXTRACTION_REPORT.md (with proper section/number)
2. Add to _EXTRACTION_FINGERPRINT.txt (to keep in sync)
3. Note in chunk report that files were updated

This keeps the extraction report as the canonical master list.

---

## 🚀 START HERE

1. Read extraction report sections C-G (lines ~400-1400)
2. For each numbered item, check if it's in fingerprint
3. Add any missing items
4. Report what was added
5. Confirm sync is complete

**Go.**
