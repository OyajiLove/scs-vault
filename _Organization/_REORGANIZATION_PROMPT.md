# SCS SYSTEM BIBLE REORGANIZATION PROMPT

## PROJECT CONTEXT

Squared Circle Soul (SCS) System Bible reorganization. Vol 1 extraction complete (311 items across 7 batches). Now organizing loose files into proper folder structure.

## CURRENT STATE

**Bible Root:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\`

### EXISTING FOLDERS (26)
```
Aging System/          Faction System/        Match Engine/
Archetypes/            Fan Memory Engine/     Match Types/
Arena System/          Gimmick System/        Media System/
Backstage Politics/    Hall of Fame/          Popularity System/
Booking System/        Health System/         Promo System/
Booking Trails/        Injury System/         Retirement System/
Buzz System/           Integration/           Scandal System/
Contract System/       Legacy Tracker/        Segment Promo System/
Crowd Signals/         Manager System/        Tag Team System/
                       Territory System/      Title System/
                       Training System/       Worker Skill Baseline/
                       _VOL1_CHUNKS/
```

### LOOSE FILES TO SORT (36 system files + 18 meta files)

**Meta/Organization Files (18):**
```
_CHUNK_09_10_EXTRACTION.md       _PROGRESS.md
_EXTRACTION_FINGERPRINT.txt      _REVIEW_CHECKLIST.md
_FINGERPRINT_SYNC_PROMPT.md      _VOL1_CHUNK_TRACKER.md
_HANDOFF_PROMPT.md               _VOL1_EXTRACTION_PROMPT.md
_ID_NAMING_CONVENTION.md         _VOL1_INTEGRATION_PLAN.md
_INDEX.md                        _VOLUME_DEEP_EXTRACTION_PROMPT.md
_JSON_SCHEMA_VALIDATION.md       _VOLUME_EXTRACTION_TEMPLATE.md
_MASTER_MECHANICS_INDEX.md       _WIKILINK_AUDIT.md
_MECHANIC_SPOT_CHECK.md          VOL1_EXTRACTION_REPORT.md
SESSION_3_PROGRESS.md            SCS_PARKING_LOT.md
```

**System Files (36):**
```
AI_Tiered_Integration.md         News & Events System.md
Booking_Engine_P1-3.md           Popularity_System.md
Ceremony Tools.md                Portrait System.md
Commentary System.md             Predictability_Stakes.md
Crowd_Memory.md                  Relationship System.md
Design_Philosophy.md             Ringstate_Factions.md
Draft System.md                  Scouting System.md
Emotional_Show_Flow.md           SCS_BIBLE_12_LIVE_DASHBOARD.md
Era System.md                    SCS_BIBLE_12_TV_BROADCAST_SYSTEM.md
Era_UI_System.md                 SCS_BIBLE_13_CROSS_PROMOTION_SYSTEM.md
Feud_Memory.md                   SCS_BIBLE_14_TERRITORY_SYSTEM.md
Financial System.md              SCS_BIBLE_15_MEDIA_SYSTEM.md
Hidden_Personality.md            SCS_BIBLE_16_ARENA_SYSTEM.md
Lucha_Politics.md                Tags_System.md
Morale System.md                 Turn_Engine.md
                                 Worker_Skills.md
                                 World Builder System.md
```

---

## PROPOSED ORGANIZATION

### PHASE 1: Create _Organization Folder

Move all meta/process files:
```
_Organization/
├── Extraction/
│   ├── _VOL1_CHUNKS/
│   ├── Integration/
│   ├── VOL1_EXTRACTION_REPORT.md
│   ├── _VOL1_CHUNK_TRACKER.md
│   ├── _VOL1_EXTRACTION_PROMPT.md
│   ├── _VOL1_INTEGRATION_PLAN.md
│   ├── _CHUNK_09_10_EXTRACTION.md
│   ├── _VOLUME_DEEP_EXTRACTION_PROMPT.md
│   └── _VOLUME_EXTRACTION_TEMPLATE.md
├── Tracking/
│   ├── _INDEX.md
│   ├── _PROGRESS.md
│   ├── _MASTER_MECHANICS_INDEX.md
│   ├── _EXTRACTION_FINGERPRINT.txt
│   ├── _FINGERPRINT_SYNC_PROMPT.md
│   └── SESSION_3_PROGRESS.md
├── Standards/
│   ├── _ID_NAMING_CONVENTION.md
│   ├── _JSON_SCHEMA_VALIDATION.md
│   └── _REVIEW_CHECKLIST.md
├── Audits/
│   ├── _WIKILINK_AUDIT.md
│   └── _MECHANIC_SPOT_CHECK.md
└── _HANDOFF_PROMPT.md
```

### PHASE 2: Sort System Files by Cluster

**Booking System/** (merge loose files into existing folder)
- Booking_Engine_P1-3.md
- Emotional_Show_Flow.md
- Predictability_Stakes.md
- Turn_Engine.md
- Draft System.md

**Worker Foundation/** (NEW folder)
- Worker_Skills.md
- Hidden_Personality.md
- Tags_System.md
- Morale System.md
- Relationship System.md

**Memory Systems/** (NEW folder, or merge into Fan Memory Engine)
- Crowd_Memory.md
- Feud_Memory.md

**Media System/** (merge into existing folder)
- Commentary System.md
- News & Events System.md
- Portrait System.md
- SCS_BIBLE_12_LIVE_DASHBOARD.md
- SCS_BIBLE_12_TV_BROADCAST_SYSTEM.md
- SCS_BIBLE_15_MEDIA_SYSTEM.md

**Territory System/** (merge into existing folder)
- Lucha_Politics.md
- SCS_BIBLE_13_CROSS_PROMOTION_SYSTEM.md
- SCS_BIBLE_14_TERRITORY_SYSTEM.md
- Scouting System.md

**Era System/** (NEW folder)
- Era System.md
- Era_UI_System.md

**Arena System/** (merge into existing folder)
- SCS_BIBLE_16_ARENA_SYSTEM.md

**Financial System/** (NEW folder)
- Financial System.md

**World Builder/** (NEW folder)
- World Builder System.md
- Design_Philosophy.md

**Ringstate/** (NEW folder)
- Ringstate_Factions.md
- (Future: Atlas files if not elsewhere)

**Technical/** (NEW folder)
- AI_Tiered_Integration.md

**Catch-All/** (NEW folder for orphans)
- Ceremony Tools.md
- Any files that don't fit

**Root Level (keep):**
- SCS_PARKING_LOT.md (reference doc)
- Popularity_System.md (check if duplicate of folder)

---

## PHASE 3: Audit & Cross-Reference

After reorganization:
1. Update all wikilinks to new paths
2. Verify no broken links
3. Update _INDEX.md with new structure
4. Check for duplicate content between files

---

## CHUNKED WORKFLOW

### CHUNK 1: Create _Organization structure
1. Create `_Organization/` and subfolders
2. Move meta files (18 files)
3. Move `_VOL1_CHUNKS/` and `Integration/` folders
4. Verify moves completed

### CHUNK 2: Booking System consolidation
1. Move 5 files into `Booking System/`
2. Check for duplicates with existing folder content
3. Update any wikilinks

### CHUNK 3: Worker Foundation setup
1. Create `Worker Foundation/` folder
2. Move 5 files
3. Check relationship to `Worker Skill Baseline/` folder

### CHUNK 4: Memory Systems consolidation
1. Decide: New folder or merge into `Fan Memory Engine/`?
2. Move Crowd_Memory.md and Feud_Memory.md
3. Update links

### CHUNK 5: Media System consolidation
1. Move 6 files into existing `Media System/`
2. Rename SCS_BIBLE files to cleaner names
3. Update links

### CHUNK 6: Territory System consolidation
1. Move 4 files into existing `Territory System/`
2. Check for duplicates (Lucha_Politics might overlap)
3. Update links

### CHUNK 7: New system folders
1. Create Era System/, Financial System/, World Builder/, Ringstate/, Technical/
2. Move respective files
3. Update links

### CHUNK 8: Final cleanup
1. Handle Catch-All items
2. Check Popularity_System.md vs Popularity System/ folder
3. Verify SCS_PARKING_LOT.md location
4. Final duplicate check

### CHUNK 9: Wikilink audit
1. Run comprehensive link check
2. Fix broken references
3. Update _INDEX.md

---

## FILE LOCATIONS

**Bible Root:** `Z:\Documents\Obsidian\Lune\SCS\System Bible\`
**Project Files:** `/mnt/project/` (read-only reference)

## CRITICAL TOOL NOTES

**ALWAYS use lowercase `filesystem:` tools** (full Z:\ access)
**NEVER use uppercase `Filesystem:`** (restricted, will fail)

## PREFERENCES

- No em dashes (use commas, colons, parentheses)
- Direct communication
- Flag uncertainties
- Chunk actions to avoid context limits

---

## STARTING COMMAND

Begin with CHUNK 1:

```
filesystem:create_directory
path: Z:\Documents\Obsidian\Lune\SCS\System Bible\_Organization
```

Then create subfolders and begin moving files.

---

## DECISION POINTS (Ask if unsure)

1. **Memory Systems:** New folder or merge into Fan Memory Engine?
2. **Worker Foundation vs Worker Skill Baseline:** Merge or separate purposes?
3. **Popularity_System.md:** Duplicate of folder content?
4. **SCS_BIBLE_XX files:** Rename to cleaner names or preserve numbering?
5. **Ceremony Tools.md:** What system does this belong to?

---

**Ready to organize. Start with Chunk 1.**
