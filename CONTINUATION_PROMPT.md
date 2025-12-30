# SCS SYSTEM BIBLE DOCUMENTATION - CONTINUATION PROMPT

**Created:** 2025-12-29
**Last Updated:** 2025-12-29
**Purpose:** Resume System Bible master index documentation in a new thread

---

## CONTEXT

I'm building **Squared Circle Soul (SCS)**, a wrestling booking simulator. I have a System Bible with ~480 files across ~40 systems. We've been documenting these systems in a master index file.

**What we're doing:** Reading each system's files and adding summary entries to `SYSTEM_MASTER_INDEX.md`

**What we're NOT doing:** Creating new files, editing system files, or extracting from PDFs. Just reading existing `.md` files and summarizing them in the index.

---

## CURRENT PROGRESS

**Files Documented:** 324 of ~480 (~68%)
**Systems Indexed:** 31 of ~40+

### COMPLETED SYSTEMS (DO NOT RE-DO):

| # | System | Files |
|---|--------|-------|
| 1 | Worker Foundation | 5 |
| 2 | Worker Skills | 8 |
| 3 | Worker Lifecycle | 9 |
| 4 | Tags | 5 |
| 5 | Booking | 8 |
| 6 | Character | 10 |
| 7 | Trails | 18 |
| 8 | Buzz | 14 |
| 9 | Match Engine | 17 |
| 10 | Fan Memory | 21 |
| 11 | Backstage Politics | 12 |
| 12 | Faction | 18 |
| 13 | Contract | 7 |
| 14 | Aging | 5 |
| 15 | Scandal | 8 |
| 16 | Injury | 8 |
| 17 | Popularity | 6 |
| 18 | Gimmick | 14 |
| 19 | Hall of Fame | 9 |
| 20 | Crowd Signals | 14 |
| 21 | Fan Reaction | 6 |
| 22 | Financial | 2 |
| 23 | Manager | 4 |
| 24 | Media | 12 |
| 25 | Promotion | 13 |
| 26 | Retirement | 6 |
| 27 | Segment Promo | 12 |
| 28 | Tag Team | 2 |
| 29 | Territory | 16 |
| 30 | Title | 11 |
| 31 | Training | 10 |

---

## NEXT SYSTEMS TO DOCUMENT

**Remaining systems (check these folders exist, then read and index):**
- World Events
- World Memory System
- Era System
- Arena System
- Match Types
- Game Modes
- Game Settings
- UI System
- World Builder
- Archetypes
- Health System
- Legacy Tracker
- Technical System
- Ringstate (may be large)

---

## FILE LOCATIONS

**CRITICAL - Use lowercase `filesystem:` tools, NEVER uppercase `Filesystem:`**

| Location | Purpose |
|----------|---------|
| `Z:\Documents\Obsidian\Lune\SCS\System Bible\` | Main Bible folder |
| `Z:\Documents\Obsidian\Lune\SCS\System Bible\SYSTEM_MASTER_INDEX.md` | The index we're building |

---

## METHODOLOGY (FOLLOW EXACTLY)

### Step 1: List one system folder
```
filesystem:list_directory on Z:\Documents\Obsidian\Lune\SCS\System Bible\[System Name]
```

### Step 2: Read files (MAX 3 at a time to avoid context overflow)
```
filesystem:read_multiple_files with max 3 paths
```

### Step 3: Add to master index (ONE edit per system)
Add a section like:
```markdown
## [NUMBER]. [SYSTEM NAME]

[One-line description]

| Mechanic | Description |
|----------|-------------|
| [[File Name]] | Brief summary of what it covers |
```

Then update the SUMMARY table count and total.

### Step 4: Confirm completion, move to next system

---

## PITFALLS TO AVOID

1. **NO GREEDY EDITS** - One system per edit operation. Don't try to add multiple systems in one edit.

2. **MAX 3 FILES PER READ** - Reading too many files at once causes context overflow.

3. **CHECK AFTER COMPACTION** - If context compacts, read the transcript file to see where you left off.

4. **DON'T RE-DO COMPLETED SYSTEMS** - Check the list above before starting any system.

5. **USE LOWERCASE `filesystem:`** - The uppercase `Filesystem:` tools have restricted access and will fail on the Obsidian vault.

6. **CHUNK WORK** - If a system has many files (10+), consider stopping after that system to save progress.

---

## INDEX ENTRY FORMAT

Each system section should look like:

```markdown
## [NUMBER]. [SYSTEM NAME IN CAPS]

[One sentence describing what the system does]

| Mechanic | Description |
|----------|-------------|
| [[_System Index]] | Master: [key concepts] |
| [[File Name]] | [What it covers: key mechanics, formulas, etc.] |
| [[Another File]] | [Brief description] |

---
```

Keep descriptions concise but specific. Include key mechanics, not vague summaries.

---

## MY PREFERENCES

- Direct and honest, no sugarcoating
- Socialist lens, philosophical depth without pretension
- Gen Z humor without cringe
- Never use em dashes (use commas, colons, parentheses instead)
- Flag uncertainties rather than guessing

---

## VALIDATION

After each system is added, confirm:
- [ ] Section number is correct (sequential from 32 onward)
- [ ] All files from that system folder are listed
- [ ] SUMMARY table count updated
- [ ] TOTAL count updated

---

**Ready to continue. Start with World Events System, then proceed through remaining systems one at a time. Stop and save progress when context gets heavy.**
