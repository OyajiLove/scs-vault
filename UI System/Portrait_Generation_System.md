# PORTRAIT GENERATION SYSTEM

📛 **NAME:** Portrait Generation System  
🧭 **CATEGORY:** UI System, Asset Pipeline, Technical  
🔑 **KEYWORDS:** portraits, ComfyUI, generation, workflow, prompts, consistency, renders, transparent, pipeline  
📝 **SUMMARY:** Technical pipeline for generating consistent character portraits across the Ringstate roster. Uses ComfyUI workflows to produce transparent PNG renders in the painterly-realism style, which are then dressed with modular overlays and backgrounds. System prioritizes consistency, efficiency, and flexibility across 150+ named workers.

⚙️ **LOGIC OVERVIEW:**
- Generate base renders as transparent PNGs using ComfyUI
- Apply overlays/backgrounds dynamically based on context
- Maintain style consistency through locked prompt templates and model settings
- Batch processing for roster generation
- Quality control pipeline to catch AI artifacts

🔬 **LLM INTEGRATION:** No (asset generation pipeline)

📌 **ORIGIN:** Design discussion (Dec 2024), portrait style experiments

📎 **CONNECTED SYSTEMS:** [[Ringstate_Art_Style]], [[Visual_Art_Direction]], Character Database, Asset Management

❓ **OPEN QUESTIONS:**
- Exact checkpoint model for best results (testing needed)
- LoRA requirements for wrestling-specific features
- Optimal resolution for game use vs marketing use
- Batch processing workflow automation
- Version control for portrait iterations

✅ **STATUS:** EXPLORATORY (Pipeline design, testing needed)

---

## PIPELINE OVERVIEW

```
┌─────────────────────────────────────────────────────────────────┐
│                    CHARACTER DATA                                │
│  (Name, description, archetype, era, region, gear details)       │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    PROMPT GENERATION                             │
│  (Template + character specifics → full prompt)                  │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    COMFYUI WORKFLOW                              │
│  (Model + prompt + settings → raw image)                         │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    BACKGROUND REMOVAL                            │
│  (Raw image → transparent PNG)                                   │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    QUALITY CONTROL                               │
│  (Artifact check, consistency check, approval/regen)             │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    ASSET DATABASE                                │
│  (Transparent render stored, linked to character ID)             │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    RUNTIME COMPOSITION                           │
│  (Render + overlay + background → final display)                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## PROMPT TEMPLATE SYSTEM

### Base Template Structure

```
[STYLE ANCHOR], [SUBJECT TYPE], [PHYSICAL DESCRIPTION], [CLOTHING/GEAR], [POSE], [EXPRESSION], [LIGHTING], [BACKGROUND], [QUALITY TAGS]
```

### Style Anchor (LOCKED)

This prefix ensures consistent painterly-realism across all portraits:

```
portrait photograph with subtle painterly texture, realistic but not hyperreal, 
high-end wrestling magazine style, studio portrait lighting, professional sports photography,
slight oil paint texture visible on close inspection
```

### Subject Type Templates

**Male Wrestler (In-Ring Gear):**
```
professional male wrestler, athletic muscular build, [HEIGHT/WEIGHT DESCRIPTOR],
[ETHNICITY/FEATURES], [HAIR DESCRIPTION], [FACIAL HAIR IF ANY]
```

**Female Wrestler (In-Ring Gear):**
```
professional female wrestler, athletic build, [HEIGHT/WEIGHT DESCRIPTOR],
[ETHNICITY/FEATURES], [HAIR DESCRIPTION]
```

**Manager/Valet (Formal):**
```
professional wrestling manager, [GENDER], [BUILD DESCRIPTOR],
[ETHNICITY/FEATURES], [HAIR DESCRIPTION], confident composed demeanor
```

**Masked Wrestler:**
```
professional masked wrestler, [MASK DESCRIPTION WITH COLORS AND DESIGN],
athletic build, [HEIGHT/WEIGHT DESCRIPTOR], [VISIBLE FEATURES IF ANY]
```

### Clothing/Gear Templates

**Classic Trunks (Male):**
```
wearing [COLOR] wrestling trunks with [TRIM COLOR] trim, [BOOT DESCRIPTION],
[OPTIONAL: knee pads, wrist tape, accessories]
```

**Singlet:**
```
wearing [COLOR] wrestling singlet with [DESIGN DETAILS], [BOOT DESCRIPTION]
```

**Manager Attire:**
```
wearing [FORMAL ATTIRE DESCRIPTION: suit, dress, etc.], [ACCESSORIES]
```

**1985 Era Specific:**
```
1985 wrestling aesthetic, era-appropriate gear, no modern materials or designs
```

### Pose Templates

| Pose Type | Prompt Fragment |
|-----------|-----------------|
| **Neutral Standing** | standing straight, arms at sides, facing camera |
| **Power Pose** | standing with hands on hips, confident stance |
| **Arms Crossed** | arms crossed over chest, assertive |
| **Fists Ready** | fists clenched at sides, ready to fight |
| **Championship** | one arm raised, championship pose |
| **Manager Composed** | hands clasped in front, composed professional |
| **Intimidating** | leaning slightly forward, intense |

### Expression Templates

| Expression | Prompt Fragment |
|------------|-----------------|
| **Neutral Intensity** | focused expression, eyes meeting camera |
| **Confident** | slight confident smile, assured |
| **Menacing** | scowling, intimidating expression |
| **Cocky Heel** | arrogant smirk, looking down nose |
| **Fired Up** | intense determined expression |
| **Mysterious** | enigmatic expression, unreadable |
| **Friendly Face** | warm approachable expression |

### Lighting (LOCKED)

```
professional studio portrait lighting, dramatic but balanced,
slight rim lighting for definition, warm key light
```

### Background (LOCKED for Generation)

```
solid [NEUTRAL COLOR] background, clean, no distractions
```

Note: Background is removed post-generation anyway, but a clean solid helps the removal process.

### Quality Tags (LOCKED)

```
high quality, detailed, sharp focus, professional photography,
8k uhd, high resolution
```

### Negative Prompt (LOCKED)

```
cartoon, anime, illustration, painting, drawing, sketch, 
3d render, cgi, video game, plastic skin, waxy skin,
extra fingers, mutated hands, deformed, blurry, 
bad anatomy, bad proportions, disfigured, ugly,
watermark, signature, text, logo,
hyperrealistic, uncanny valley, too smooth,
modern clothing, anachronistic elements
```

---

## EXAMPLE FULL PROMPTS

### Example 1: "Not Mike Awesome" Style Male Wrestler

```
portrait photograph with subtle painterly texture, realistic but not hyperreal, 
high-end wrestling magazine style, studio portrait lighting, professional sports photography,
slight oil paint texture visible on close inspection,

professional male wrestler, large muscular heavyweight build, 6'4" 290 lbs look,
Caucasian, brown mullet hairstyle with volume, clean shaven,

wearing blue wrestling trunks with white stripe down side, blue knee pads,
white wrestling boots, iridescent sport sunglasses,

standing straight facing camera, arms slightly away from body showing size,
intense focused expression behind sunglasses,

professional studio portrait lighting, dramatic but balanced,
slight rim lighting for definition, warm key light,

solid burgundy background, clean,

high quality, detailed, sharp focus, professional photography, 8k uhd
```

### Example 2: Leila Khoury Style Manager

```
portrait photograph with subtle painterly texture, realistic but not hyperreal, 
high-end wrestling magazine style, studio portrait lighting, professional sports photography,
slight oil paint texture visible on close inspection,

professional wrestling manager, female, elegant build,
Middle Eastern features, olive skin, dark wavy hair with volume styled in 1980s glamour,
dark defined eyebrows, deep red lipstick,

wearing black off-shoulder velvet dress, gold chandelier earrings,
sophisticated formal attire, 1985 aesthetic,

hands clasped in front at waist, composed confident pose,
knowing slight smile, eyes meeting camera with intelligence,

professional studio portrait lighting, dramatic but balanced,
slight rim lighting for definition, warm golden key light,

solid deep purple background, clean,

high quality, detailed, sharp focus, professional photography, 8k uhd
```

### Example 3: Masked Luchador

```
portrait photograph with subtle painterly texture, realistic but not hyperreal, 
high-end wrestling magazine style, studio portrait lighting, professional sports photography,
slight oil paint texture visible on close inspection,

professional masked wrestler, lucha libre style,
wearing ornate jaguar-themed mask in gold and green with black accents,
mask covers full face with eye holes showing intense dark eyes,
athletic muscular build, 5'10" 200 lbs look, bronze skin visible on arms and torso,

wearing green and gold wrestling tights with jaguar print design,
matching green boots with gold trim,

arms crossed over chest, powerful stance,
intense eyes visible through mask,

professional studio portrait lighting, dramatic but balanced,
slight rim lighting for definition,

solid dark green background, clean,

high quality, detailed, sharp focus, professional photography, 8k uhd
```

---

## COMFYUI WORKFLOW SPECIFICATIONS

### Recommended Models (Testing Required)

| Model Type | Candidates | Notes |
|------------|------------|-------|
| **Base Checkpoint** | SDXL, Juggernaut XL, RealVisXL | Test for best painterly-realism balance |
| **Refiner** | SDXL Refiner | Optional, may over-smooth |
| **LoRA (Optional)** | Wrestling-specific if available | May need custom training |

### Generation Settings

| Parameter | Value | Notes |
|-----------|-------|-------|
| **Resolution** | 1024x1536 (portrait) | 2:3 ratio for chest-up framing |
| **Steps** | 30-40 | Balance quality vs speed |
| **CFG Scale** | 7-8 | Not too strict, allows variation |
| **Sampler** | DPM++ 2M Karras | Good for realistic images |
| **Seed** | Lock per character | Consistency for regeneration |

### Background Removal

| Tool | Notes |
|------|-------|
| **RemBG node** | Built into many ComfyUI workflows |
| **Segment Anything** | More precise edges |
| **Manual cleanup** | For complex cases (hair, translucent elements) |

### Batch Processing Workflow

1. Load character database export (CSV/JSON)
2. Generate prompts from template + character data
3. Queue batch generation
4. Auto background removal
5. Export to QC folder
6. Manual review pass
7. Approved → Asset database
8. Rejected → Regen queue with notes

---

## CHARACTER DATA → PROMPT MAPPING

### From Character Profile to Prompt

| Character Field | Prompt Section |
|-----------------|----------------|
| `height_weight` | Build descriptor |
| `ethnicity` | Features description |
| `hair` | Hair description |
| `facial_hair` | Facial hair if any |
| `gear_description` | Clothing/gear section |
| `signature_accessories` | Accessories |
| `archetype` | Influences pose/expression |
| `alignment` | Influences expression |
| `era` | Era-specific elements |

### Example Mapping: Calhoun Trask

**Character Data:**
```json
{
  "name": "Calhoun Trask",
  "height": "6'1\"",
  "weight": "228 lbs",
  "ethnicity": "Caucasian",
  "hair": "dark, slicked-back, perfect part",
  "facial_hair": "clean-shaven",
  "gear_description": "Dark green trunks with gold trim, white boots",
  "signature_accessories": "family crest on gear",
  "archetype": "Technical Heel",
  "alignment": "Heel",
  "era": "1985"
}
```

**Generated Prompt Sections:**
```
Build: athletic muscular build, 6'1" 228 lbs lean technical wrestler physique
Features: Caucasian, sharp jawline, intense measuring gaze
Hair: dark hair slicked back with perfect part, not a strand out of place
Facial Hair: clean-shaven
Gear: wearing dark green wrestling trunks with gold trim, white wrestling boots, family crest emblem on trunks
Pose: arms crossed, looking down nose at camera (heel)
Expression: arrogant composed expression, slight contempt (heel)
```

---

## QUALITY CONTROL CHECKLIST

### Automatic Checks

| Check | Criteria |
|-------|----------|
| **Resolution** | Meets minimum 1024x1536 |
| **Alpha channel** | Present and clean |
| **File size** | Reasonable for asset management |
| **Color profile** | sRGB |

### Manual Review Checks

| Check | Pass Criteria |
|-------|---------------|
| **Hand/Finger count** | Correct number, natural position |
| **Ear integrity** | Not melted or deformed |
| **Eye alignment** | Both eyes focused, not wonky |
| **Teeth (if visible)** | Not too many, not fused |
| **Gear accuracy** | Matches description |
| **Era appropriateness** | No anachronistic elements |
| **Style consistency** | Matches established painterly-realism look |
| **Character recognition** | Would be recognizable as this character |
| **Mask accuracy** | For masked wrestlers, design correct |
| **Expression match** | Fits character alignment/archetype |

### Common Rejection Reasons

| Issue | Action |
|-------|--------|
| Extra/missing fingers | Regen with different seed |
| Melted ears | Regen, possibly adjust pose |
| Wrong gear colors | Fix prompt, regen |
| Too photorealistic | Adjust model settings |
| Too illustrated | Adjust model settings |
| Wrong era elements | Fix prompt (modern elements crept in) |
| Expression mismatch | Adjust expression prompt |

---

## FILE NAMING CONVENTION

### Transparent Renders

```
[CHARACTER_ID]_[VERSION]_render.png

Examples:
TRASK_CALHOUN_v1_render.png
KHOURY_LEILA_v1_render.png
AWESOME_MIKE_v2_render.png (after revision)
```

### Composed Finals (with overlay/background)

```
[CHARACTER_ID]_[CONTEXT]_[VERSION].png

Examples:
TRASK_CALHOUN_roster_v1.png
TRASK_CALHOUN_matchcard_v1.png
TRASK_CALHOUN_scandal_v1.png
```

### Folder Structure

```
/assets/portraits/
    /renders/           # Transparent base renders
    /composed/          # Context-applied finals
        /roster/        # Default roster view
        /matchcard/     # Match card variants
        /special/       # HoF, scandal, memorial, etc.
    /overlays/          # Overlay templates
    /backgrounds/       # Background templates
    /qc_pending/        # Awaiting review
    /rejected/          # Failed QC, notes attached
```

---

## OVERLAY TEMPLATES

### Default Overlay (Leila Style)

| Element | Specification |
|---------|---------------|
| **Texture** | Crackled/aged paper texture |
| **Opacity** | 15-25% |
| **Blend Mode** | Overlay or Soft Light |
| **Edge Treatment** | Subtle vignette, darker corners |

### Era-Specific Overlays

| Era | Overlay Character |
|-----|-------------------|
| **1970s** | Heavy film grain, warm color cast, faded edges |
| **1980s** | Medium grain, saturated, slight glow |
| **1990s** | Gritty grain, desaturated edges, high contrast |
| **2000s** | Minimal grain, clean, broadcast-ready |
| **2020s** | Optional film emulation, cinematic color |

### Special Context Overlays

| Context | Overlay |
|---------|---------|
| **Hall of Fame** | Gold tint layer, ornate frame overlay |
| **Scandal** | Red tint, heavy grain, desaturation |
| **Injury** | Slight blur, desaturation |
| **Memorial** | Black & white conversion, film grain |
| **Championship** | Gold accent highlights |

---

## BACKGROUND TEMPLATES

### Solid Colors (by Promotion)

| Promotion | Primary BG Color | Hex Code |
|-----------|------------------|----------|
| CCA | Deep Blue | #1a365d |
| GWA | Silver Gray | #718096 |
| PWU | Revolutionary Red | #9b2c2c |
| CFPW | Earth Green | #276749 |
| LGBTQW+ | Deep Purple | #553c9a |
| Blade | Blood Red | #742a2a |
| Independent | Varies | Per-promotion |
| Default | Rich Purple | #6b21a8 |

### Textured Backgrounds

Apply texture overlay to solid color:
- Paper crackle (Leila style)
- Canvas texture
- Leather grain
- Concrete/urban

### Gradient Backgrounds

For match cards and dramatic contexts:
- Dark center fade to black edges
- Top-lit gradient (darker bottom)
- Split backgrounds for vs. match cards

---

## CONSISTENCY STRATEGIES

### Character Locking

Once a portrait is approved:
1. Lock the seed value
2. Lock the exact prompt
3. Store in character database
4. Use locked values for any regeneration

### Style Reference Images

Maintain a folder of "approved style examples":
- Reference during QC
- Use as img2img reference if needed
- Helps maintain consistency across batch sessions

### Batch Processing by Type

Generate similar characters together:
- All male heavyweight wrestlers in one batch
- All managers in one batch
- All masked wrestlers in one batch

This helps maintain consistency within character types.

---

## SPECIAL CASES

### Masked Wrestlers

| Challenge | Solution |
|-----------|----------|
| Mask design accuracy | Detailed mask description in prompt |
| Eye visibility | Specify "eyes visible through mask holes" |
| Cultural accuracy | Research specific mask traditions (lucha, Tiger Mask style, etc.) |
| Unmasking events | Generate separate unmasked portrait |

### Aging Characters

| Scenario | Approach |
|----------|----------|
| Career progression | Generate multiple portraits at different ages |
| Active legend | Current age portrait |
| Historical flashback | Prime-era portrait |
| Memorial | Prime-era or iconic moment |

### Gender Non-Conforming Characters

| Consideration | Approach |
|---------------|----------|
| Presentation accuracy | Follow character description exactly |
| Avoid stereotypes | Authentic representation, not caricature |
| Era sensitivity | 1985 presentation may differ from 2024 |

### Teams and Factions

| Scenario | Approach |
|----------|----------|
| Matching gear | Generate with consistent color schemes |
| Group shots | Compose from individual renders |
| Visual identity | Shared elements (colors, symbols) in gear |

---

## FUTURE ENHANCEMENTS

### Potential Additions

| Feature | Description | Priority |
|---------|-------------|----------|
| **Pose variety** | Multiple poses per character | Medium |
| **Expression packs** | Happy/angry/shocked variants | Low |
| **Action shots** | Mid-move dynamic poses | Low |
| **Ring context** | Portraits with ring ropes blur | Low |
| **Custom LoRA** | Wrestling-specific fine-tuning | Medium |
| **Automated pipeline** | Full batch automation | High |

### Integration Points

- Character database auto-generates prompts
- Game engine requests appropriate context variant
- Asset management tracks versions and approvals
- Modding support for custom portraits

---

## RELATED SYSTEMS

- [[Ringstate_Art_Style]] - Overall visual direction
- [[Visual_Art_Direction]] - Key art (mordançage) style
- [[Era_Based_Office_UI]] - UI era theming
- Character Database - Source for character data
- Asset Management - Storage and retrieval

---

**Document Status:** EXPLORATORY (Pipeline designed, testing needed)  
**Next Review:** Test ComfyUI workflow with various checkpoints, establish exact model settings, generate test batch of 10-15 portraits for style calibration
