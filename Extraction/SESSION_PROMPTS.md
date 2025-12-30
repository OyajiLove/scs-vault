# SCS EXTRACTION SESSION PROMPT

---

## 🟢 ULTRA-MINIMAL PROMPT (Just Say This)

```
SCS extraction session. Check the tracker and go.
```

**What Claude does:**
1. Reads `EXTRACTION_PROGRESS_TRACKER.md` (this folder)
2. Finds next unfinished volume/line position
3. Starts extracting using line-range method
4. Updates tracker when done

That's it. You don't need to know the volume or line number.

---

Copy/paste this at the start of any extraction session. Fill in the blanks.

---

## 🚀 QUICK START PROMPT

```
SCS EXTRACTION SESSION

Volume: [X]
Start Line: [XXXX]
Source: C:\Users\Oyaji\Desktop\SCS\_Main Volume PDFs\txt_conversions\SCS Vol. [X].txt

TASK: Line-range extraction using view tool with view_range. 
Read 100-200 lines at a time. Append findings to running extraction file.

OUTPUT FILES:
- Extraction: Z:\Documents\Obsidian\Lune\SCS\System Bible\Extraction\Vol[X]_Running_Extraction.md
- Tracker: Z:\Documents\Obsidian\Lune\SCS\System Bible\Extraction\EXTRACTION_PROGRESS_TRACKER.md
- Parking Lot: Z:\Documents\Obsidian\Lune\SCS\System Bible\Parking Lot\

EXTRACT THESE CATEGORIES:
1. LOCKED SYSTEMS (formal, specified mechanics)
2. SYSTEM MODIFICATIONS (additions to existing Bible systems)
3. HALF-BAKED IDEAS (seeds, tangents, undeveloped concepts) ← PRIORITY, DON'T SKIP
4. TERMINOLOGY LOCKS (definitions)
5. TAGS MENTIONED (name, category, effect)
6. CASE STUDIES / EXAMPLES (worker examples, booking examples)
7. FORMULAS / VALUES (any specific numbers or calculations)

RULES:
- Use lowercase filesystem: tools (NOT uppercase Filesystem:)
- Append to extraction file, don't overwrite
- Update tracker with new line position after each batch
- Half-baked ideas are SACRED, capture every weird tangent
- If context getting full, stop at natural break and note line position

GO.
```

---

## 📋 EXTRACTION FILE FORMAT

When creating a new volume's extraction file, start with this header:

```markdown
# VOL [X] - RUNNING EXTRACTION

📅 **Started:** [Date]
📍 **Source:** SCS Vol. [X].txt
🔄 **Status:** In Progress

---

## LINES [START]-[END] (extracted [date])

### 🔒 Locked Systems
- 

### 🔧 System Modifications
- 

### 🍳 Half-Baked Ideas
- 

### 📖 Terminology
- 

### 🏷️ Tags
- 

### 📚 Case Studies / Examples
- 

### 🔢 Formulas / Values
- 

---
```

---

## 🔄 END OF SESSION PROMPT

When ending a session, make sure to:

```
END SESSION CHECKLIST:
1. Update EXTRACTION_PROGRESS_TRACKER.md with:
   - Current line position
   - Date
   - Brief note on what was covered
2. Note any half-baked ideas that need Parking Lot development
3. Flag any systems that need immediate Bible integration
```

---

## 📂 FILE LOCATIONS REFERENCE

| What | Where |
|------|-------|
| Source Volumes | `C:\Users\Oyaji\Desktop\SCS\_Main Volume PDFs\txt_conversions\` |
| Progress Tracker | `Z:\Documents\Obsidian\Lune\SCS\System Bible\Extraction\EXTRACTION_PROGRESS_TRACKER.md` |
| Running Extractions | `Z:\Documents\Obsidian\Lune\SCS\System Bible\Extraction\Vol[X]_Running_Extraction.md` |
| Parking Lot | `Z:\Documents\Obsidian\Lune\SCS\System Bible\Parking Lot\` |
| System Bible | `Z:\Documents\Obsidian\Lune\SCS\System Bible\[Category]\` |

---

## 🛠️ TOOL REMINDERS

**CRITICAL:** Always use lowercase `filesystem:` tools, NEVER uppercase `Filesystem:`

| Tool | Use For |
|------|---------|
| `filesystem:read_text_file` with `head` or `tail` | Quick file peeks |
| `view` with `view_range` | Reading specific line ranges from volumes |
| `filesystem:write_file` | Creating/overwriting files |
| `filesystem:read_text_file` | Reading full file content |
| `filesystem:list_directory` | Checking folder contents |

---

## 🎯 INTEGRATION SESSION PROMPT (Separate from Extraction)

```
SCS INTEGRATION SESSION

Volume(s) to integrate: [X]
Extraction file: Z:\Documents\Obsidian\Lune\SCS\System Bible\Extraction\Vol[X]_Running_Extraction.md

TASK: Read extraction file, cross-reference existing Bible, write integrations.

OUTPUTS:
- New Bible entries → System Bible/[Category]/
- Expansions to existing → System Bible/[Category]/[System]_Vol[X]_Expansion.md
- Half-baked development → Parking Lot/

RULES:
- Check existing files before creating new ones (fingerprinting)
- Don't duplicate content already in Bible
- Develop half-baked ideas with potential system connections
- Update tracker when integration complete

GO.
```

---

## 💡 HALF-BAKED IDEA DEVELOPMENT PROMPT

```
SCS HALF-BAKED DEVELOPMENT SESSION

Focus: [Specific idea or general sweep]
Source: Parking Lot files + extraction files

TASK: Take half-baked seeds and develop them into potential systems.

FOR EACH IDEA:
1. What problem does it solve?
2. What existing systems does it connect to?
3. What would MVP implementation look like?
4. What's the full vision?
5. Priority tier (MVP adjacent / Alpha / Beta / Post-release)

OUTPUT: Enhanced Parking Lot entries with development notes

GO.
```
