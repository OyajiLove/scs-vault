# SCS BIBLE AUDIT PROMPT

**Purpose:** Use this prompt to start a new thread for comprehensive Bible audit after Vol 5 extraction completes.

**Last Updated:** 2024-12-28

---

## 🧵 NEW THREAD PROMPT

Copy everything below this line:

---

# SCS BIBLE AUDIT REQUEST

## PROJECT CONTEXT

I'm building **Squared Circle Soul (SCS)**, a wrestling booking simulator. I have 11 volumes (~1,100 pages) of design documentation that I've been systematically extracting into a **System Bible** stored in an Obsidian vault.

**Extraction Status:**
- Vol 1-4: Previously extracted (foundation systems)
- Vol 5: COMPLETE (memory architecture, grief systems, legacy mechanics)
- Vols 6-13: Not yet extracted

The Bible has grown organically through extraction sessions. It now needs a comprehensive audit before continuing with Vols 6-13.

---

## VAULT LOCATION

**System Bible Root:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\`

**CRITICAL:** Use lowercase `filesystem:` tools, NOT uppercase `Filesystem:`. The uppercase version fails on this vault.

---

## CURRENT DIRECTORY STRUCTURE

```
System Bible/
├── Backstage Politics System/
├── Character System/
├── Contract System/ (13+ files)
├── Extraction/ (progress tracker, half-baked parking lot)
├── Fan Reaction System/
├── Media System/
├── Parking Lot/ (half-baked ideas)
├── Promotion System/ (8+ files)
├── Technical System/
├── Title System/
├── Worker System/ (2 files, NEW)
├── World Memory System/ (16+ files)
└── [Various standalone files from early extraction]
```

---

## AUDIT TASKS

### 1. FULL INVENTORY

**Action:** Create complete inventory of every `.md` file in the Bible.

**For each file, record:**
- Filename
- Directory location
- One-line description of what it covers
- Status (Locked / Partial / Stub / Unknown)
- Source volumes (if noted in file)
- File size (rough indicator of depth)

**Output:** Table or structured list of all files.

---

### 2. OVERLAP/REDUNDANCY DETECTION

**Action:** Identify files that cover overlapping mechanics.

**Likely problem areas:**
- World Memory System (16+ files on memory, drift, preservation, grief, legacy)
- Promotion System (collapse, resurrection, revival files)
- Fan Reaction System (subculture, faction, mutation files)
- Contract System (loyalty, betrayal, negotiation files)

**For each overlap found:**
- List the files involved
- Describe what overlaps
- Recommend: MERGE / KEEP SEPARATE / CROSS-REFERENCE BETTER
- If MERGE: suggest which file absorbs which

**Output:** Overlap report with recommendations.

---

### 3. OVER-CONSOLIDATION CHECK

**Action:** Identify files that are doing too much and should be split.

**Signs of over-consolidation:**
- File covers 3+ distinct systems
- File is 500+ lines with multiple unrelated sections
- File has "Part 1/Part 2" structure that could be separate files
- Systems mentioned in "Connected Systems" that deserve their own file

**For each over-consolidation found:**
- Identify the file
- List the distinct systems crammed in
- Recommend split structure

**Output:** Split recommendations.

---

### 4. ORPHAN/MISPLACED FILE CHECK

**Action:** Identify files in wrong directories or orphaned at root level.

**Questions to answer:**
- Are there `.md` files at Bible root that should be in directories?
- Are files in directories that don't match their content?
- Should Worker System absorb some Character System files?
- Is Technical System the right home for Core Memory Architecture?

**Output:** Relocation recommendations.

---

### 5. CROSS-REFERENCE VALIDATION

**Action:** Check that [[wikilinks]] in files point to real files.

**For each file:**
- Extract all [[wikilinks]]
- Verify target file exists
- Flag broken links
- Flag missing reciprocal links (if A links to B, does B link to A?)

**Output:** Broken link report.

---

### 6. HALF-BAKED PARKING LOT AUDIT

**Action:** Review `Parking Lot/Vol5_Half_Baked_Ideas.md` and any other parking lot files.

**Check:**
- Are any "half-baked" ideas actually now locked in the Bible? (Mark as PROMOTED)
- Are any locked systems actually half-baked and should be demoted?
- Are there half-baked ideas scattered in main Bible files that should be moved to parking lot?

**Output:** Parking lot reconciliation.

---

### 7. CREATE NEW MASTER INDEX

**Action:** Delete any old master list/index files and create new `SYSTEM_MASTER_INDEX.md`.

**Format:**

```markdown
# SCS SYSTEM BIBLE - MASTER INDEX

**Last Updated:** [Date]
**Total Systems:** [Count]
**Total Files:** [Count]

---

## TIER 1: MVP CORE

### [Directory Name]

| File | Description | Status | Source |
|------|-------------|--------|--------|
| [[Filename]] | One-line description | Locked | Vol X |

[Repeat for each directory]

---

## TIER 2: BOOKING & SIMULATION

[Same structure]

---

## TIER 3: WORLD & SUPPORT

[Same structure]

---

## PARKING LOT

[Half-baked ideas summary]

---

## CROSS-REFERENCE MAP

[Key system relationships]
```

**Output:** New master index file.

---

### 8. AUDIT REPORT

**Action:** Create `BIBLE_AUDIT_REPORT.md` summarizing all findings.

**Include:**
- Executive summary (what's the Bible's health?)
- Inventory statistics
- Overlaps found and resolutions
- Splits recommended
- Files relocated
- Broken links fixed
- Parking lot changes
- Recommendations for future extraction

**Output:** Comprehensive audit report.

---

## EXECUTION ORDER

1. **Inventory first** (understand what exists)
2. **Overlap detection** (find redundancies)
3. **Over-consolidation check** (find bloated files)
4. **Orphan check** (find misplaced files)
5. **Cross-reference validation** (find broken links)
6. **Parking lot audit** (reconcile half-baked)
7. **PAUSE FOR APPROVAL** before making changes
8. **Execute approved changes** (merges, splits, moves)
9. **Create master index** (new authoritative index)
10. **Write audit report** (document everything)

---

## COMMUNICATION PREFERENCES

- **Direct and honest** (no sugarcoating)
- **Socialist lens, philosophical depth without pretension**
- **Gen Z humor without cringe**
- **Never use em dashes (—)** - use commas, colons, or parentheses
- **Tables for data comparisons**
- **Flag uncertainties clearly** - ask before making destructive changes

---

## WHAT NOT TO DO

- Don't invent new systems (this is audit, not creation)
- Don't delete files without explicit approval
- Don't merge files without explicit approval
- Don't assume overlapping files should merge (sometimes redundancy is intentional)
- Don't skip the inventory step

---

## TOOLS REMINDER

**USE:** `filesystem:list_directory`, `filesystem:read_file`, `filesystem:write_file`, `filesystem:edit_file`

**DO NOT USE:** `Filesystem:` (uppercase) - these are restricted and will fail on this vault.

---

## STARTING POINT

Begin by listing all directories in:
`Z:\Documents\Obsidian\Lune\SCS\System Bible\`

Then systematically inventory each directory's contents.

Report back with full inventory before proceeding to overlap detection.

---

## SIGN-OFF

When complete, the Bible should be:
- Fully inventoried
- Free of redundant overlap
- Properly organized
- Cross-referenced accurately
- Ready for Vol 6-13 extraction

Let's make the Bible clean and strong. 🔥

---

**END OF PROMPT**

---

## NOTES FOR TOVARISCH

This prompt should give a fresh thread everything it needs. You may want to:

1. Update the directory structure section once Vol 5 is complete (file counts will change)
2. Add any specific problem areas you've noticed
3. Include the PROJECT_INSTRUCTIONS.md context if the new thread doesn't have project files

The prompt is designed to be methodical: inventory first, then analysis, then approval checkpoint, then execution. This prevents a fresh Claude from making destructive changes without your sign-off.

Save this file and use it when ready for audit.
