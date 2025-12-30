# ERA-DEPENDENT UI SYSTEM

📛 **NAME:** Era-Dependent UI System  
🧭 **CATEGORY:** User Interface, Immersion, Visual Design  
🔑 **KEYWORDS:** UI, interface, era, decade, aesthetic, theme, immersion, customization, office, computer, mobile  
📝 **SUMMARY:**

The UI transforms based on the in-game year, immersing players in the era they're booking. 1970s gameplay feels like running a territory from a smoke-filled office with rotary phones and desk calendars. 1990s feels like early Windows. 2020s feels like booking from a phone. The system treats UI as part of the fiction: you're not playing a game SET in 1978, you're booking FROM 1978. Promotion size and resources can further modify the aesthetic within each era.

⚙️ **LOGIC OVERVIEW:**

- UI theme automatically shifts based on in-game year
- Each era has distinct visual language, interaction patterns, and metaphors
- Promotion status (size, money, style) modifies UI within era constraints
- Players can toggle era-appropriate UI on/off (accessibility option)
- Players can customize offices/workspaces within era bounds
- All eras provide identical functionality, just different presentation

🔬 **LLM INTEGRATION:** No (pure visual/UX system)

📌 **ORIGIN:** Conversation thread (December 2024), Vol 1 Extraction #149

📎 **CONNECTED SYSTEMS:** Promotion Identity System, Financial System, all UI elements

❓ **OPEN QUESTIONS:**

- Exact year breakpoints for era transitions
- Transition animations between eras?
- How much office customization is feasible for v1?
- Asset creation pipeline for multiple era themes
- Accessibility considerations for each era aesthetic

✅ **STATUS:** Exploratory (December 2024 conversation, UI planning)

---

## VERSION HISTORY

**Version 0.1 (December 2024 Conversation)**

- Transcript: https://claude.ai/share/4bb953d9-44fb-4759-9950-862697c769f1
- Established era progression concept
- Defined major era breakpoints
- Linked promotion status to UI variation within eras
- Confirmed toggle option for players who prefer modern UI

---

## DESIGN PRINCIPLES

1. **Immersion Through Medium:** The interface IS the time period
2. **Function Over Form:** All eras provide same functionality, different feel
3. **Player Choice:** Era UI can be disabled for clean modern interface
4. **Promotion Identity:** Your office reflects your promotion's status
5. **Accessibility First:** Era aesthetics never compromise usability

---

## ERA PROGRESSION

### Era 1: Smoke-Filled Office (1970s - Mid 1980s)

**Year Range:** 1970-1985

**Visual Language:**
- Wood-paneled office walls
- Haze/smoke atmospheric effect (toggleable)
- Warm incandescent lighting
- Physical desk with items as UI elements

**UI Metaphors:**

| Function | Metaphor |
|----------|----------|
| Roster | Rolodex or filing cabinet |
| Schedule | Desk calendar you flip through |
| Contracts | Paper documents with pen |
| Phone calls | Rotary phone on desk |
| Finances | Ledger book |
| News | Newspaper clippings, mail |
| Show booking | Index cards on corkboard |

**Audio:**
- Rotary dial clicks
- Paper shuffling
- Typewriter for text entry
- Phone ring (old bell style)

**Promotion Scaling:**
- Small outlaw: Dingy back room, folding table
- Regional: Modest office, functional furniture
- National: Mahogany desk, leather chair, trophy case

---

### Era 2: Early Computing (Late 1980s - Early 1990s)

**Year Range:** 1986-1994

**Visual Language:**
- CRT monitor on desk (green or amber phosphor)
- DOS/command-line aesthetic
- Office still visible around the computer
- Harsh fluorescent lighting mixed with desk lamp

**UI Metaphors:**

| Function | Metaphor |
|----------|----------|
| Roster | Database listing (ASCII tables) |
| Schedule | Text calendar |
| Contracts | Digital forms |
| Communications | Early email/BBS style |
| Finances | Spreadsheet (Lotus 1-2-3 style) |
| News | Text feed |
| Show booking | List interface |

**Audio:**
- Keyboard clacking
- CRT hum
- Dot matrix printer
- Modem sounds for "loading"

**Promotion Scaling:**
- Small: Single monitor, cramped space
- Regional: Proper office setup, maybe two monitors
- National: Early network, multiple workstations implied

---

### Era 3: Windows 95/98 (Mid 1990s - Early 2000s)

**Year Range:** 1995-2003

**Visual Language:**
- Classic Windows grey boxes
- That teal/cyan desktop color
- Beveled buttons, 3D effects
- Start menu energy

**UI Metaphors:**

| Function | Metaphor |
|----------|----------|
| Navigation | Windows Explorer / File Manager |
| Roster | Database application |
| Schedule | Calendar application |
| Contracts | Word processor documents |
| Communications | Email client (Outlook Express style) |
| Finances | Excel-style spreadsheet |
| News | Web browser (early IE aesthetic) |
| Show booking | Custom application window |

**Audio:**
- Windows startup sound (era-appropriate homage)
- Click sounds
- Error dings
- "You've got mail" style notifications

**Promotion Scaling:**
- Small: Basic Windows, few applications
- Regional: More professional software suite
- National: Corporate IT aesthetic

---

### Era 4: Windows XP (Early-Mid 2000s)

**Year Range:** 2004-2011

**Visual Language:**
- Luna theme (blue title bars, green start button)
- Bliss wallpaper homage
- Rounded corners, gradients
- Cleaner, more colorful than 95/98

**UI Metaphors:**
- Similar to Era 3 but visually updated
- More polished application windows
- Better graphics, icons
- Taskbar-centric navigation

**Promotion Scaling:**
- Reflects corporate growth of wrestling in this era
- Indies: Basic setup
- Major: Full corporate IT infrastructure feel

---

### Era 5: Modern Desktop (2010s)

**Year Range:** 2012-2019

**Visual Language:**
- Windows 10 flat design
- Tiles, clean lines
- Metro/Modern UI influence
- Minimalist aesthetic

**UI Metaphors:**
- Dashboard-style interfaces
- Cards and tiles for information
- Clean data visualization
- Social media integration aesthetic

**Promotion Scaling:**
- Reflects streaming era, digital-first presentation
- Indies: Simpler, web-based feel
- Major: Full data analytics dashboard

---

### Era 6: Mobile/Contemporary (2020s+)

**Year Range:** 2020+

**Visual Language:**
- Mobile phone interface
- App-style navigation
- Notifications, push alerts
- Dark mode option

**UI Metaphors:**

| Function | Metaphor |
|----------|----------|
| Navigation | Bottom tab bar, hamburger menu |
| Roster | Contact-style list with photos |
| Schedule | Mobile calendar |
| Contracts | E-signature style |
| Communications | Messaging app |
| Finances | Banking app aesthetic |
| News | Social media feed |
| Show booking | Task management app |

**Promotion Scaling:**
- Reflects mobile-first modern wrestling
- All promotions: Similar base aesthetic
- Size differences in notification volume, features unlocked

---

## IMPLEMENTATION ARCHITECTURE

### Theme System:

```
themes/
├── era_1970s/
│   ├── assets/
│   ├── layouts/
│   ├── sounds/
│   └── theme.json
├── era_1980s_late/
├── era_1990s_mid/
├── era_2000s/
├── era_2010s/
├── era_2020s/
└── modern_clean/  (toggle option)
```

### Theme Switching:

```python
func update_ui_era(game_year: int):
    var era = get_era_for_year(game_year)
    if era != current_era:
        transition_to_era(era)
        current_era = era

func get_era_for_year(year: int) -> String:
    if year <= 1985:
        return "era_1970s"
    elif year <= 1994:
        return "era_1980s_late"
    elif year <= 2003:
        return "era_1990s_mid"
    elif year <= 2011:
        return "era_2000s"
    elif year <= 2019:
        return "era_2010s"
    else:
        return "era_2020s"
```

### Promotion Modifiers:

Within each era, promotion status modifies:
- Office quality/size
- Furniture/equipment
- Ambient details
- Available "features" (more monitors, fancier phone, etc.)

---

## PLAYER OPTIONS

### Era UI Toggle:
- **ON (Default):** UI changes with game year
- **OFF:** Always use modern clean interface

### Era Lock:
- Player can lock to a specific era aesthetic regardless of game year
- "I want Windows 95 forever"

### Transition Effects:
- **Instant:** Era changes immediately on year transition
- **Fade:** Smooth transition between eras
- **OFF:** No special transition effect

### Accessibility Options:
- Disable smoke effects
- High contrast mode per era
- Font size independent of era aesthetic
- Screen reader compatibility

---

## ASSET REQUIREMENTS

### Per Era:
- Background/environment art
- UI element sprites (buttons, panels, frames)
- Icons for all functions
- Sound effects library
- Font selections

### Promotion Variants (Per Era):
- 3 tiers minimum: Small, Regional, National
- Variations in office environment
- Different equipment/furniture

### Estimated Asset Count:
- 6 eras × ~50 UI elements = 300 base UI assets
- 6 eras × 3 promotion tiers × ~10 office variants = 180 environment assets
- 6 eras × ~20 sound effects = 120 audio assets

---

## v0.1 SCOPE

For initial release, minimal viable implementation:

**Include:**
- Modern clean UI only
- Architecture supports future era themes
- Theme switching hooks in place

**Defer:**
- Full era theme artwork
- Promotion-scaled variants
- Sound design per era
- Office customization

**Rationale:**
Era UI is polish, not core. Get the game working with clean modern UI. Layer era immersion after core loop is proven.

---

## FUTURE ENHANCEMENTS

### Office Customization:
- Players choose items for their desk
- Unlock decorations through achievements
- Trophies, belts, photos accumulate over career

### Dynamic Office Changes:
- After big PPV success: champagne on desk
- After scandal: newspaper headlines visible
- After financial trouble: items disappear

### Streaming Integration:
- Overlay mode for streamers
- Clean capture-friendly variants

---

## ERA-SPECIFIC NEWS PRESENTATION (#149)

📌 **Source:** Vol 1 Extraction #149

### News Format by Era

| Era | Visual Style | News Format |
|-----|--------------|-------------|
| **70s-80s** | Typewriter fonts, paper textures, smoke-filled office | Physical newsletters, magazines, phone hotlines |
| **90s** | Early web aesthetic, newsletters | Wrestling Observer style sheets, AOL posts |
| **2000s** | Professional websites, Flash-era design | Website news, early forums |
| **2010s+** | Modern responsive, social media integration | Twitter feeds, podcast mentions, viral clips |

### News Content Types

| Type | Description |
|------|-------------|
| **Wrestling Observer Style** | In-depth analysis, star ratings, insider perspective |
| **Kayfabe News** | In-universe coverage, storyline as real |
| **Dirtsheet Rumors** | Backstage gossip, may be true or false |
| **Social Media Feeds** | Quick updates, fan reactions, viral moments |

### Integration with [[News & Events System]]

News content is generated by the News & Events System; Era UI controls how that content is visually presented to the player.

---

## RELATED SYSTEMS

- Promotion Identity System: Determines promotion tier for UI scaling
- Financial System: Wealth affects office quality
- [[News & Events System]]: Content generation for era-styled presentation
- [[Era System]]: Core era definitions
- All UI elements: Must support era theming architecture

---

**Document Status:** Exploratory, UI planning for post-v0.1  
**Next Review:** After v0.1 completion, prioritize era asset creation
