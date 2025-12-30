# VISUAL ART DIRECTION

📛 **NAME:** Visual Art Direction (Box Art, Splash Screen, Key Art)  
🧭 **CATEGORY:** UI System, Visual Identity  
🔑 **KEYWORDS:** mordançage, art style, splash screen, box art, key art, darkroom, analog, aesthetic, branding  
📝 **SUMMARY:** SCS employs mordançage photography as its signature visual style for box art, splash screens, and promotional materials. This analog darkroom technique, where emulsion lifts from the paper creating spectral dissolving effects, perfectly embodies wrestling's central tension: bodies simultaneously real and performed, characters bleeding into (or out of) their performers.

⚙️ **LOGIC OVERVIEW:**
- Mordançage creates figures caught between solid and ghost, dissolution and form
- Technique involves bleaching developed prints, causing blacks to lift and curl like smoke
- Visual style maps directly to wrestling's "soul" concept: the liminal space between performer and character
- Analog process honors Ringstate's 1985 era authenticity
- Distinct from pixel nostalgia, CGI shine, or corporate sim minimalism

🔬 **LLM INTEGRATION:** No (purely visual/asset creation)

📌 **ORIGIN:** Design discussion (Dec 2024), building on Vol 4's AI art direction notes

📎 **CONNECTED SYSTEMS:** [[Era_Based_Office_UI]], [[Era_System]], Asset Pipeline

❓ **OPEN QUESTIONS:**
- ComfyUI workflow feasibility vs actual analog darkroom process?
- How many key art pieces needed for launch? (Splash, box, 3-5 promotional?)
- Should in-game portraits echo this style or remain distinct?
- Color vs pure B&W? (Traditional mordançage is B&W, but sepia/duo-tone possible)

✅ **STATUS:** CONCEPT LOCKED (Style chosen, implementation path TBD)

---

## WHY MORDANÇAGE

### Thematic Resonance

The dissolution effect mirrors the central tension of professional wrestling:

| Wrestling Reality | Mordançage Visual |
|-------------------|-------------------|
| Bodies simultaneously real and performed | Figures caught between solid and ghost |
| Pain that's genuine but contextualized | Form dissolving at the edges |
| Characters that consume their performers | Gimmick bleeding out of/into physical form |
| Memory and legacy fading/persisting | Blacks lifting like smoke or memory |

A mordançage wrestler looks like someone **mid-transformation**, their gimmick literally emerging from (or consuming) their physical form. The "soul" in Squared Circle Soul, visualized.

### Era Authenticity

For Ringstate's 1985 setting, an analog darkroom technique feels *right* in ways digital effects cannot match:
- Authentically of that moment (tail end of darkroom experimentation before digital)
- Material, tactile, handmade quality
- Honors the era without being nostalgic pastiche
- Feels *discovered* in an archive, like wrestling's secret history made visible

### Market Differentiation

This immediately separates SCS from every other wrestling game:

| Competitor Style | SCS Mordançage |
|------------------|----------------|
| Pixel art nostalgia (RetroMania) | Analog photography, fine art |
| CGI realism (WWE 2K) | Handcrafted, textural |
| Corporate sim minimalism (TEW) | Expressive, emotionally resonant |
| Cartoon stylization (various) | Haunting, serious, artistic |

The visual says: "This is not like other wrestling games. This takes the artform seriously."

---

## TECHNIQUE REFERENCE

### Traditional Mordançage Process

1. **Develop** a high-contrast black and white print
2. **Bleach** the print (potassium ferricyanide or similar)
3. **Watch** as the black silver areas lift from the paper
4. **Manipulate** the lifted emulsion while wet (curl, stretch, remove)
5. **Re-fix** to stabilize the image
6. **Dry** with the distorted emulsion in place

The result: areas that were solid black become translucent, curling tendrils. Figures appear to dissolve, emerge from void, or exist in multiple states simultaneously.

### Key Visual Characteristics

- **Lifted blacks:** Dark areas curl away from the paper surface
- **Spectral edges:** Figures fade into abstraction at boundaries
- **Textural depth:** Physical paper grain visible, not digitally smooth
- **High contrast base:** Strong blacks and whites before dissolution
- **Unpredictability:** Each print unique due to chemical/manipulation variables

---

## SPLASH SCREEN CONCEPT

### Primary Vision

A single wrestler figure, mid-pose in the ring:
- Ring ropes dissolving into abstract lines
- Crowd becoming suggestion rather than detail
- Blacks lifting and curling like smoke or memory
- The figure caught between emergence and dissolution
- Sense of summoning something from the void

### Mood Keywords
- Haunting
- Liminal
- Transformative
- Archival
- Serious
- Artistic

### Text Treatment

Game title should feel:
- Hand-set or letterpress aesthetic
- Slightly degraded/imperfect
- Integrated with the image, not floating above it
- "Squared Circle Soul" as if stamped or burned into the print

---

## BOX ART CONCEPT

### Front Cover

- Central mordançage figure (iconic pose, not specific wrestler)
- Ring environment suggested through abstract lines
- Title treatment integrated with image
- Minimal text (title, platform, rating)
- Lots of visual breathing room

### Back Cover

- Smaller mordançage vignettes (3-4 figures in different states of dissolution)
- Brief feature descriptions
- Screenshots in contained frames (contrast with art style)
- System requirements, legal text

### Spine

- Title only, high contrast
- Small logo element

---

## IMPLEMENTATION PATHS

### Path A: ComfyUI Digital Recreation

**Pros:**
- Iterative, controllable
- No darkroom access needed
- Consistent reproducibility for multiple pieces

**Cons:**
- May lack authentic texture/grain
- Requires significant workflow development
- Risk of looking "filtered" rather than genuine

**Potential Workflow:**
1. Generate or source high-contrast base image
2. Edge detection pass (isolate figure boundaries)
3. Displacement mapping (simulate emulsion lift)
4. Noise/grain layer (paper texture)
5. Careful compositing with manual touchup
6. Multiple passes for different dissolution levels

### Path B: Actual Analog Process

**Pros:**
- Authentic texture and unpredictability
- Unique originals (could be sold/displayed)
- True to technique's spirit

**Cons:**
- Requires darkroom access
- Chemical sourcing (potassium ferricyanide, etc.)
- Experimentation time for paper/bleach formula
- Single originals, would need high-res scanning

**Process:**
1. Source or shoot high-contrast wrestler reference photos
2. Print in darkroom (fiber paper recommended)
3. Mordançage process with manipulation
4. Scan at very high resolution (4000+ DPI)
5. Digital cleanup of dust/scratches only

### Path C: Hybrid Approach

- Create 1-2 genuine analog pieces for key art (splash, box front)
- Develop ComfyUI workflow based on studying the originals
- Use digital recreation for secondary materials
- Best of both worlds: authenticity where it matters, efficiency elsewhere

---

## ASSET LIST (ESTIMATED)

| Asset | Priority | Size | Notes |
|-------|----------|------|-------|
| Splash Screen | Critical | 1920x1080 minimum, 4K preferred | First impression |
| Box Art Front | Critical | Print resolution (300 DPI at final size) | Steam, storefronts |
| Box Art Back | High | Print resolution | Physical/press kit |
| Promotional Key Art (3-5) | High | Various | Marketing, social |
| Loading Screen Variants | Medium | 1920x1080 | Could use details/crops from key art |
| Steam Capsule Images | High | Various Steam specs | May need adapted compositions |

---

## REFERENCE ARTISTS

### Mordançage Practitioners
- **Man Ray** (surrealist pioneer, solarization adjacent)
- **Pierre Cordier** (chemigram innovator)
- **Floris Neusüss** (photogram/experimental)

### Mood/Tone References
- Film noir promotional stills
- Boxing photography (1950s-70s)
- German Expressionist cinema posters
- Vintage wrestling promotional photos (territory era)

---

## PROMPT FRAMEWORKS (ComfyUI Exploration)

```
"High contrast black and white photograph of a wrestler mid-suplex, 
dramatic lighting, studio portrait style, strong shadows, 
grain texture, 1980s aesthetic"
```

Post-processing direction:
```
"Mordançage effect, emulsion lifting from paper, blacks dissolving 
into spectral tendrils, figure caught between solid and ghost, 
analog darkroom texture, curling edges"
```

Note: These are starting points. Actual mordançage simulation will require significant ControlNet/IPAdapter work and possibly custom nodes.

---

## INTEGRATION WITH GAME UI

### In-Game Portrait Question

Should character portraits within the game echo mordançage style?

| Approach | Pros | Cons |
|----------|------|------|
| **Yes, full mordançage** | Unified visual identity | May reduce readability, production heavy |
| **Subtle echo** | Cohesive but functional | Requires careful calibration |
| **Distinct style** | Cleaner UI, easier production | Less distinctive overall |

**Recommendation:** Subtle echo. Portraits use high-contrast B&W with slight grain and edge softening, but not full dissolution effect. Reserve full mordançage for key art and special moments (Hall of Fame inductions, career retrospectives, death notifications).

### Loading Screens

- Use crops/details from key art pieces
- Full mordançage treatment appropriate here
- Rotating selection from promotional art pool
- Could include subtle animation (grain flicker, slight drift)

---

## RELATED SYSTEMS

- [[Era_Based_Office_UI]] - Office visual style (distinct but complementary)
- [[Era_System]] - Time period detection
- [[Hall_of_Fame_System]] - Ceremony visuals could use mordançage treatment
- [[Legacy_Tracker]] - Retrospective moments

---

**Document Status:** CONCEPT LOCKED (Style direction confirmed, implementation path TBD)  
**Next Review:** Attempt ComfyUI workflow, evaluate results vs analog feasibility
