# Newgen Portrait System

📛 **NAME:** Newgen Portrait System
🧭 **CATEGORY:** UI System, Asset Pipeline, Character Generation
🔑 **KEYWORDS:** newgen, portraits, auto-assign, renders, generation, TEW, free pic
📝 **SUMMARY:** Automated portrait assignment system for generated workers (newgens) that avoids TEW's "free pic" manual assignment hell. Uses style-consistent pre-rendered art banks with smart tagging for automatic assignment based on era, region, gender, and archetype.

⚙️ **LOGIC OVERVIEW:**
- Pre-rendered art bank (500-2000 portraits) in consistent Ringstate style
- Auto-assignment based on worker attributes (era, region, gender, archetype)
- No manual folder hunting or tag assignment required
- Duplicate detection and reassignment
- Optional player expansion via modding folder

🔬 **LLM INTEGRATION:** Minimal (tagging logic could use LLM for edge cases)

📌 **ORIGIN:** Vol 7 Line 75

📎 **CONNECTED SYSTEMS:** [[Portrait_Generation_System]], [[Worker Generator]], Character Database

❓ **OPEN QUESTIONS:**
- Initial pool size needed for launch (150-300 for MVP, expandable)
- Filter/aging system for reusing renders across career stages
- Exact LoRA models to ship with game

✅ **STATUS:** Locked (Vol 7 Lines 75-100)

---

## The Problem: TEW's "Free Pic" Hell

TEW used a broken system where players had to:
- Manually assign image tags through the game
- Hunt through folders for appropriate images
- Break immersion constantly with mismatched renders
- Accept that newgens looked "pasted in" from outside

**SCS Goal:** Every newgen feels like they belong to the same living, breathing world as the rest — visually, narratively, and structurally.

---

## 🔒 CRITICAL RULE: No Render-Based Cheating

| ❌ Not Allowed | Why |
|----------------|-----|
| Renders only generating when title is won | Cheat code for spotting top prospects |
| Delayed generation based on success | Immersion break (sudden appearance shift) |
| "Star gets face" logic | Telegraphs sim logic, not reality |

**All workers treated equally — no image = no cheat.**

---

## 🔒 REVERSE FLOW GENERATION (Critical Innovation)

Instead of: "Create worker → randomly assign pic"

We do: **"Assign render first → generate bio based on render's traits"**

**The image drives the bio, not the other way around.**

This prevents:
- Prettyboy render → "scarred outlaw brawler" mismatch
- Masked horror heel → "charming young flier" mismatch

You get:
- Handsome face + aristocratic pose → "Noble junior who speaks like a statesman"
- Heavyset scarred man → "Veteran barroom brawler, respected in the Gulf"

**No stat mismatch. No vibe break. Full immersion.**

---

## Solution Architecture

### Option A: Pre-Rendered Art Bank (Primary)

| Element | Specification |
|---------|---------------|
| **Pool Size** | 500-2000 portraits |
| **Style** | Ringstate painterly-realism (transparent PNGs) |
| **Assignment** | Automatic based on worker attributes |

**Assignment Criteria:**
- Era (1970s, 1980s, 1990s, etc.)
- Region (USA South, Japan, Mexico, etc.)
- Gender presentation
- Archetype flags (e.g. "hardcore throwback," "charismatic babyface," "masked monster")

**Benefits:**
- Eliminates broken immersion
- Keeps style uniform
- Feels native — like each render was born for the engine
- Pool expandable over time
- Many reusable with filters (aging, hair color) for legacy characters

### Option B: Auto-Crop Hero Renders (Secondary)

For top newgens pushed mid-game (someone pushed to the moon):
- Game assigns "hero render" slot
- Engine crops or styles a portrait on demand
- Uses base image from bank with filters/style tags
- Feels "new" without requiring whole new render

### Option C: Player-Added Expansions (Optional)

For modders who want custom portraits:

```
/renders/newgens/
    portrait_001.png
    portrait_001.json  (or .yml)
    portrait_002.png
    portrait_002.json
    ...
```

- Players drop transparent PNGs into folder
- Game reads associated tag files
- Adds to auto-assign pool
- Never required, but system welcomes it

---

## Auto-Assignment Logic

### Smart Matching (Not Filename)

| Attribute | Weight | Notes |
|-----------|--------|-------|
| Era | High | 1980s render won't auto-assign to 2020s worker |
| Region | High | Japanese render won't auto-assign to Texas worker |
| Gender | Required | Must match presentation |
| Archetype | Medium | Masked monster won't get clean-cut babyface render |
| Build | Low | Heavyweight vs cruiserweight consideration |

### Duplicate Prevention

- Engine tracks which renders are assigned
- If two workers accidentally share a render, game notices
- Reassigns behind the scenes unless player has locked assignment
- Prevents "wait, that's the same guy" moments

---

## 🔒 RENDER TAG SCHEMA (Locked)

Each render in the bank has associated metadata:

| Tag Type | Examples | Purpose |
|----------|----------|--------|
| **Face Type** | Rugged, Handsome, Scarred, Unusual, Prettyboy, Blank | Drives charisma, menace, believability, sex appeal |
| **Body Type** | Lanky, Bulky, Athletic, Soft | Ties to strength, durability, match style |
| **Gimmick Aura** | Shooter, Clown, Monster, Technician, Noble, Dirtbag | Informs alignment, fan reception |
| **Era Fit** | 70s, 80s, 90s | Keeps aesthetic cohesion |
| **Mask Status** | Unmasked, Masked (full), Partial, Painted | Affects style, mystery, promo fluency |
| **Gender Presentation** | Masc, Femme, Andro, Ambiguous | Sexual appeal, commentary tone |
| **Ethnicity Marker** | Optional, subtle | Regional realism (not stereotypes) |
| **Age Band** | Young (20s), Prime (30s), Veteran (40+) | Syncs with debut age and wear |

### JSON Example

```json
{
  "filename": "masked_brawler_013.png",
  "face": "Rugged",
  "body": "Bulky",
  "gimmick": "Monster",
  "mask": "Full",
  "gender": "Masc",
  "age": "Prime",
  "region_hint": "South",
  "era": "80s"
}
```

### Matching Algorithm

1. Filter by required attributes (gender, era)
2. Score by affinity matches (region, archetype)
3. Select highest-scoring unassigned render
4. Mark as assigned to worker ID
5. Generate bio based on render tags

### Fail-Safes

- If render bank runs dry on a match (e.g. "Femme-presenting Japanese shooter in 1975"):
  - Pull closest viable match (same tags, minor visual deviation)
  - Or cue AI-generation if enabled
- Rare visual-text mismatches treated as gimmick anomalies
  - e.g. "too pretty to be this violent" becomes a commentary thread

---

## 🔒 MVP LIBRARY REQUIREMENTS

| Requirement | Specification |
|-------------|---------------|
| **Starting Size** | 150-300 renders |
| **Archetypes** | 10-15 key types (Shooter, Monster, Gimmick Babyface, Femme Fatale, Masked Luchador, etc.) |
| **Coverage** | Balanced across gender, race/ethnicity, era |
| **Tags Per Image** | 10-15 properties |
| **Goal** | Enough range for first 5-10 in-game years without duplications |

**You don't need thousands to start — you need coverage, not volume.**

---

## 🔒 NO MICROTRANSACTIONS (Critical Lock)

> "I don't want microtransactions. Gotta be a local SD pipeline with various LoRA models."

**All AI render generation is handled locally using Stable Diffusion pipelines.**

### Core Principles

- ✅ No online dependency — game ships with built-in generation tools
- ✅ No paid layers — no per-image costs, no API calls, no premium gating
- ✅ Flexible visual styles — players can use multiple LoRAs
- ✅ Accessible for modders — drag-and-drop LoRA folders and prompt templates

### LoRA Style Options

| Style | Description |
|-------|-------------|
| **Ringstate** | Default painterly-realism (primary) |
| **Comic** | Bold lines, graphic novel aesthetic |
| **Anime** | Japanese animation style |
| **Semi-Realistic** | Balanced realism |
| **Photorealistic** | Maximum realism |
| **Legacy** | TEW-style AI images for TEW IX fanbase compatibility |

---

## 🔒 FINAL SYSTEM ARCHITECTURE (Locked)

### Step 1: Default = Render Bank Assignment

- Game assigns transparent PNG from curated library
- Tag-based logic ensures facial/body/gimmick alignment
- Bio and stats generated to fit the image
- **Instant, no delay**

### Step 2: Optional Regenerate (User-Initiated)

**"Don't like their look? Rebuild it."**

- Player clicks "Regenerate Render"
- Game runs local AI generation using:
  - Original image's tags
  - Worker's gimmick
  - Player changes (e.g. "mask them," "make her look rougher," "add facial scars")
- **Delay:** 5-30 seconds depending on system
- **Output:** Clean transparent PNG, cropped and styled automatically
- Bio may update slightly to reflect new visual traits

### Step 3: Render Tuning UI (Power Users)

Only shown if user opens "Customize Worker Look" panel:

| Control | Options |
|---------|--------|
| Face Vibe | Handsome, Scarred, Plain, Prettyboy, etc. |
| Body | Bulky, Lanky, Athletic, Soft |
| Aura | Noble, Sleazy, Gimmick-heavy, Monster |
| Gender Presentation | Masc, Femme, Andro, Ambiguous |
| Mask/Paint/Accessories | Various options |

Game builds AI prompt behind the scenes and generates on demand.

### Anti-Cheat Measures

- ❌ No render tied to success level
- ❌ No render changes at title wins
- ❌ No visual "power creep"
- ✅ All renders match in-era fashion, silhouette, and tone

---

## Generation Time Expectations

| Method | Time | Notes |
|--------|------|-------|
| Pre-Banked Assets | Instant | Perfect consistency, no delay |
| Local AI (Gaming PC) | 5-15s | RTX 3060 or better |
| Local AI (Mid-Range) | 30-90s | 16GB RAM, integrated GPU |

---

## Render Generation Settings Panel (Locked)

| Setting | Options | Description |
|---------|---------|-------------|
| **Render Source** | Use Prebuilt Bank (default) / Local AI Generation | Primary source for worker portraits |
| **Render Style** | Ringstate / Comic / Anime / Semi-Realistic / Photorealistic / Legacy | Which LoRA and prompt set is used |
| **Resolution** | 1024×1536 (locked) | All renders output to Ringstate standard |
| **Face Crop Mode** | Auto-crop for popups (Y/N) | Toggle for generating face-only variants |
| **Generate on Worker Creation** | On/Off | All newgens born with unique AI render |
| **Queue Renders While Simulating** | On/Off | Background generation during idle time |
| **Render Save Location** | User-defined folder | For players who want to reuse or mod images |
| **Quality** | Fast / Standard / High | Speed vs quality tradeoff |

---

## 🔒 LoRA FOLDER SYSTEM (Mod-Friendly)

The game scans a folder structure for available styles:

```
/SCS/AI_Renders/LoRA/
   ├── Ringstate/
   │   ├── model.safetensors
   │   ├── prompts.json
   ├── Comic/
   ├── Anime/
   ├── Photoreal/
   ├── Legacy/
```

**Each folder contains:**
- LoRA model file (.safetensors or .ckpt)
- Prompt templates (tagged by archetype/gender/era)
- Optional negative prompts for style purity

**Users can add LoRAs or tweak prompts freely.**

---

## 🔒 HIGH-END USER BYPASS

**Setting: "Use Prebuilt Renders" = OFF**

When disabled:
- All workers (newgens, imports, legacy reskins) generated from scratch
- Uses selected LoRA model + tag-driven prompt scaffolding
- Background SD pipeline handles generation
- Never see a recycled face or mismatched aesthetic
- Sim slows slightly during render but stays 100% immersive

> "Feels like a living world with infinite variation, built in your machine's own aesthetic fire."

### Smart Cache

Generated renders stored in local cache (`/renders/generated/`):
- Reusable across saves or universes if desired
- Cache can be disabled for fresh runs
- Prevents regenerating the same worker twice

---

## Developer Mode (Optional Debug)

Enable visual debug mode showing:
- Image tag match success/fail
- Render seed, style, prompt details
- Re-assign or force-regenerate buttons
- Only visible if debugging enabled in settings

---

## Feature Summary

| Feature | Status |
|---------|--------|
| Style-consistent, auto-assigned renders | ✅ Planned |
| No "free pic" folder hell | ✅ Avoided |
| Expandable bank for player-created renders | ✅ Optional |
| Matching based on region/gimmick/archetype | ✅ Built in |
| Visual uniqueness preserved via smart tagging | ✅ Engine-managed |
| Duplicate detection | ✅ Automatic |

---

## Implementation Notes

### Phase 1: MVP
- Start with 50-100 renders covering major archetypes
- Basic era/region/gender matching
- No player expansion yet

### Phase 2: Expansion
- Grow pool to 500+ renders
- Add archetype-specific matching
- Enable modding folder

### Phase 3: Polish
- Filter/aging system for career progression
- "Hero render" slot for breakout stars
- Full JSON schema for modders

---

## Related Systems

- [[Portrait_Generation_System]] - How renders are created
- [[Worker Generator]] - Creates the workers needing portraits
- [[Era System]] - Determines era-appropriate assignment

---

**Document Status:** Conceptual (design locked)
**Next Review:** Define exact tagging schema, determine MVP pool size
