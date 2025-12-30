# LIVE DASHBOARD / SECONDARY DISPLAY SYSTEM

📛 **NAME:** Live Dashboard System  
🧭 **CATEGORY:** UI/UX / Information Display  
🔑 **KEYWORDS:** dashboard, secondary display, pop-out, tournament standings, show card, real-time, glance not click, multi-device, localhost, QR code, information architecture  
📝 **SUMMARY:** A detachable, real-time information display system that shows booking-relevant data (tournament brackets, show cards, championship status, storyline heat, roster notes) on a secondary window, browser tab, or mobile device. Designed around the "glance don't click" principle: critical information should be visible without interrupting gameplay flow.

⚙️ **LOGIC OVERVIEW:**
- Dashboard exists as a separate rendering target from main game window
- Pulls live data from game state (roster, shows, storylines, tournaments, championships)
- Updates automatically when relevant game state changes
- User configures which panels appear and their arrangement
- Supports multiple display modes: native Godot window, localhost browser, network-accessible endpoint
- Mobile access via local network with QR code connection
- Themes match or contrast with main UI based on user preference

🔬 **LLM INTEGRATION:** No  
Dashboard is pure data display with no generative content. All information comes from deterministic game state.

📌 **ORIGIN:** New system designed December 2024. Not extracted from volumes. Created to address information density challenges identified during UI planning.

📎 **CONNECTED SYSTEMS:**
- **BOOK-001:** Booking Engine (show cards, match outcomes, booking history)
- **POP-001:** Popularity System (worker over/under status by region)
- **FEUD-001:** Feud Memory Tracker (active feuds, heat levels, timeline)
- **CROWD-001:** Crowd Memory System (what fans remember, pattern warnings)
- **Tournament System:** (bracket status, advancement, match history)
- **Title System:** (championship lineage, current holders, upcoming defenses)
- **Roster System:** (worker status, availability, injuries, contracts)

❓ **OPEN QUESTIONS:**
1. Should dashboard support multiple simultaneous viewers (e.g., local co-op booking)?
2. How much historical data should be accessible (last 3 shows? full season?)?
3. Should dashboard have any input capability (quick notes, reminders) or pure output?
4. Performance budget for update frequency on lower-tier hardware?
5. Should theming be automatic (match game era) or fully manual?
6. Network security considerations for localhost access (LAN-only vs. any device)?

✅ **STATUS:** Exploratory / New Design (not extracted from volumes)

---

## DESIGN PHILOSOPHY

### The Problem This Solves

Wrestling booking is information-dense. During a single session, a player juggles:

- Current show card and match order
- Tournament bracket positions
- Championship status across multiple titles
- Active feud heat levels
- Worker availability (injuries, contracts, morale)
- Storyline timelines and upcoming payoffs
- Historical booking patterns (predictability warnings)
- Regional popularity variations

Without a secondary display, players must constantly navigate menus, breaking gameplay flow. The mental load isn't the booking decisions themselves; it's the *context retrieval* required to make those decisions well.

### The "Glance Don't Click" Principle

**Core Idea:** Information relevant to booking decisions should be visible at a glance, without requiring clicks, menu navigation, or screen switching.

**Analogy:** A pit crew doesn't flip through manuals during a race. Critical data lives on dashboards, visible peripherally, updated in real-time.

**Implementation:** The Live Dashboard acts as an always-visible reference panel. The player's eyes can flick to the side (or to a phone) and immediately see:
- "Oh right, Kenny's feuding with Omega, heat is at 78"
- "Tournament semi-finals are next week, bracket's tight"
- "Goldberg's on a 3-match win streak, predictability warning"

### What This Isn't

- **Not a control panel:** Dashboard displays information; it doesn't accept booking inputs
- **Not a replacement for main UI:** Complex interactions (match construction, contract negotiation) stay in main game
- **Not a distraction:** Information density is carefully managed; less important data is collapsible or hidden
- **Not mandatory:** Players who prefer single-screen play lose nothing

---

## DISPLAY MODES

### Mode 1: Native Godot Window (Default)

**Implementation:** Secondary window spawned via Godot's multi-window support.

**Pros:**
- Lowest latency (direct memory access to game state)
- Native look and feel
- No network stack overhead
- Works offline by definition

**Cons:**
- Requires second monitor for ideal experience
- Window management varies by OS
- Can't easily move to different device

**Best For:** Desktop players with dual monitors, streamers showing dashboard on stream.

```gdscript
# Conceptual structure
var dashboard_window: Window

func spawn_dashboard():
    dashboard_window = Window.new()
    dashboard_window.title = "SCS Dashboard"
    dashboard_window.size = Vector2i(800, 600)
    dashboard_window.add_child(dashboard_scene.instantiate())
    get_tree().root.add_child(dashboard_window)
```

### Mode 2: Localhost Browser

**Implementation:** Embedded HTTP server serves lightweight HTML/JS dashboard. Browser connects to `localhost:PORT`.

**Pros:**
- Cross-platform browser support
- Easy to put on tablet or second laptop
- Familiar web interface patterns
- Can be styled extensively with CSS

**Cons:**
- Slightly higher latency (HTTP polling or WebSocket)
- Requires browser open
- Port conflicts possible

**Best For:** Players using tablet as secondary display, those who prefer browser interfaces.

**Tech Stack:**
- Lightweight embedded server (Godot HTTPServer or similar)
- WebSocket for real-time updates (preferred) or polling (fallback)
- Vanilla HTML/CSS/JS (no framework bloat)
- JSON API for data transmission

```json
// Example API response
{
  "show": {
    "name": "Summer Slam '85",
    "date": "1985-08-15",
    "venue": "Madison Square Garden",
    "matches": [
      {
        "order": 1,
        "type": "singles",
        "participants": ["Hogan", "Savage"],
        "stakes": "WWF Championship",
        "status": "scheduled"
      }
    ]
  },
  "tournaments": [...],
  "championships": [...],
  "active_feuds": [...]
}
```

### Mode 3: LAN Network Access

**Implementation:** Same as localhost, but binds to LAN IP instead of 127.0.0.1. Other devices on same network can connect.

**Pros:**
- Phone as dashboard (very common use case)
- Multiple viewers supported
- No cables, no window management

**Cons:**
- Security considerations (LAN exposure)
- Network configuration varies (firewalls, router settings)
- Latency depends on network quality

**Best For:** Phone/tablet as secondary display, local multiplayer viewing, streaming setups.

**QR Code Connection:**
- Game generates QR code containing `http://[LAN_IP]:[PORT]`
- Player scans with phone
- Dashboard loads automatically
- No manual URL typing required

```gdscript
# QR generation concept
func generate_dashboard_qr() -> Image:
    var ip = get_lan_ip()
    var url = "http://%s:%d" % [ip, DASHBOARD_PORT]
    return QRCode.generate(url)
```

### Mode Selection UI

Settings menu includes:

| Setting | Options | Default |
|---------|---------|---------|
| **Dashboard Mode** | Off / Native Window / Browser / Network | Off |
| **Network Port** | 8080-9999 | 8585 |
| **Allow LAN Access** | Yes / No | No |
| **Auto-Launch** | On Game Start / Manual | Manual |
| **Theme** | Match Game / Light / Dark / High Contrast | Match Game |

---

## INFORMATION ARCHITECTURE

### Panel Types

Dashboard is composed of modular panels. Players choose which panels to display and arrange them in a grid or freeform layout.

#### Panel: Active Show Card

**Purpose:** Current show's match lineup with status indicators.

**Contents:**
- Show name, date, venue
- Match order (1-N)
- Participants per match
- Match type
- Stakes (title, stipulation, tournament)
- Status: Scheduled / In Progress / Complete
- Quick outcome preview (winner, rating) for completed matches

**Update Triggers:** Match added, match completed, match order changed.

**Density Control:**
- **Compact:** Match number, names only, status icon
- **Standard:** Full match info, stakes visible
- **Expanded:** Adds booking intent notes, chemistry preview

#### Panel: Tournament Bracket

**Purpose:** Visual bracket for active tournaments.

**Contents:**
- Tournament name and type (single elim, round robin, etc.)
- Current round
- All bracket positions with worker names
- Match results (completed rounds)
- Upcoming matchups highlighted
- Advancement paths visible

**Update Triggers:** Tournament match completed, bracket redrawn.

**Density Control:**
- **Compact:** Current round only
- **Standard:** Full bracket, scrollable
- **Expanded:** Includes match ratings and dates

#### Panel: Championship Status

**Purpose:** All titles with current holders and defense history.

**Contents:**
- Title name
- Current holder (with portrait if enabled)
- Days/defenses held
- Last defense (opponent, date, rating)
- Next scheduled defense (if booked)
- Title heat indicator (prestigious vs. devalued)

**Update Triggers:** Title change, defense scheduled, title created/retired.

**Density Control:**
- **Compact:** Title + holder only
- **Standard:** Adds reign length and last defense
- **Expanded:** Full history, multiple previous holders

#### Panel: Active Feuds

**Purpose:** Ongoing storylines with heat levels and timeline.

**Contents:**
- Feud participants
- Current heat level (0-100, visual thermometer)
- Weeks active
- Key moments (last 3 story beats)
- Projected blowoff window (if system predicts)
- Staleness warning (if feud is cooling)

**Update Triggers:** Feud heat change, story beat added, feud ended.

**Density Control:**
- **Compact:** Names + heat bar only
- **Standard:** Adds timeline and last beat
- **Expanded:** Full feud history, predicted outcomes

#### Panel: Roster Quick View

**Purpose:** At-a-glance worker status.

**Contents:**
- Worker name
- Current status: Available / Injured / Suspended / On Leave / Contract Expiring
- Popularity (main region)
- Active storyline indicator
- Morale indicator (if visible to player)
- Days until status change (injury recovery, contract expiry)

**Update Triggers:** Status change, popularity shift, contract event.

**Density Control:**
- **Compact:** Name + status icon only
- **Standard:** Adds popularity and storyline flag
- **Expanded:** Full status details, upcoming events

#### Panel: Booking Warnings

**Purpose:** System-generated alerts about booking concerns.

**Contents:**
- Predictability warnings ("Hogan has won 5 straight, crowds may turn cynical")
- Feud fatigue alerts ("Savage vs. Jake at 12 weeks, consider blowoff")
- Crowd energy warnings ("Three long matches scheduled back-to-back")
- Contract alerts ("DiBiase's contract expires in 2 shows")
- Pattern detection ("You always book clean finishes in main events")

**Update Triggers:** Warning conditions met or cleared.

**Density Control:**
- **Compact:** Warning count badge only (click to expand)
- **Standard:** Top 3 warnings visible
- **Expanded:** All active warnings with context

#### Panel: Calendar/Schedule

**Purpose:** Upcoming shows and story beats.

**Contents:**
- Next N shows (user configurable, default 4)
- Show type (TV, PPV, house show)
- Scheduled title defenses
- Tournament rounds
- Contract expirations in window
- Scheduled storyline payoffs

**Update Triggers:** Show created, event scheduled, time advanced.

**Density Control:**
- **Compact:** Next show only
- **Standard:** Next 4 shows with key events
- **Expanded:** Full calendar view with all scheduled items

#### Panel: Notes (Optional Input Panel)

**Purpose:** Player's personal booking notes.

**Contents:**
- Free-text notes field
- Can be organized by: Show / Worker / Storyline
- Persists between sessions

**Implementation Note:** This is the one panel that accepts input. Keep it simple (textarea, not rich text). Optional to include; some players prefer external notes.

---

## UPDATE BEHAVIOR

### Sync Philosophy

**Principle:** Dashboard should feel "live" without consuming excessive resources.

**Approach:** Event-driven updates with rate limiting.

### Update Triggers (Event-Driven)

| Event | Dashboard Update |
|-------|------------------|
| Match booked | Show Card panel |
| Match completed | Show Card + Tournament + Stats |
| Feud heat change | Active Feuds panel |
| Title change | Championship Status panel |
| Worker status change | Roster Quick View panel |
| Time advanced (day/week) | All panels (batch) |
| Show started | Show Card panel (highlight current) |
| Show ended | All panels (batch) |
| Warning condition triggered | Booking Warnings panel |

### Update Frequency Limits

**Native Window:** Updates fire immediately on event (minimal overhead).

**Browser/Network:** Updates batched and sent every 500ms minimum.
- Prevents flooding with rapid changes
- WebSocket preferred for push updates
- Polling fallback at 2-second intervals

**Low-Performance Mode:** Updates batched to 2-second intervals, reduced panel animations.

### State Consistency

**Critical:** Dashboard must never show stale data that could mislead booking decisions.

**Approach:**
1. Dashboard subscribes to game state events
2. Events include monotonic sequence number
3. Dashboard tracks last received sequence
4. On reconnect (browser refresh), dashboard requests full state sync
5. Sequence gaps trigger automatic resync

```gdscript
# Event structure
class DashboardEvent:
    var sequence: int
    var event_type: String
    var panel_affected: String
    var data: Dictionary
    var timestamp: float
```

---

## CUSTOMIZATION

### Panel Selection

Player enables/disables panels individually:

| Panel | Default State |
|-------|---------------|
| Active Show Card | Enabled |
| Tournament Bracket | Enabled (if tournament active) |
| Championship Status | Enabled |
| Active Feuds | Enabled |
| Roster Quick View | Disabled (can be overwhelming) |
| Booking Warnings | Enabled |
| Calendar/Schedule | Enabled |
| Notes | Disabled |

### Layout Options

**Grid Mode:** Panels snap to grid cells. 2x3 or 3x4 layouts available.

**Freeform Mode:** Panels can be dragged and resized freely. Position persists.

**Preset Layouts:**
- **Booker Focus:** Show Card + Feuds + Warnings
- **Tournament Mode:** Bracket + Show Card + Schedule
- **Overview:** All panels at compact density
- **Minimal:** Show Card only

### Theme Matching

**Match Game Era (Default):**
- Dashboard adopts main game's current era theme
- 1970s smoky office → Dashboard has wood textures, green tones
- 2000s corporate → Dashboard has sleek grays, digital feel
- Maintains immersion even on secondary display

**Fixed Themes:**
- Light: Clean white background, high readability
- Dark: Low-light friendly, reduced eye strain
- High Contrast: Accessibility-focused, sharp color distinctions

**Custom Colors:** Advanced option to set primary/secondary/accent colors manually.

### Information Density

**Global Setting:** Compact / Standard / Expanded

**Per-Panel Override:** Each panel can have its own density setting.

**Responsive Behavior:** If dashboard window is small, automatically shift toward compact mode.

---

## MULTI-DEVICE SUPPORT

### Phone as Dashboard

**Target Use Case:** Player at desktop, phone propped up showing dashboard.

**Requirements:**
- Responsive design (portrait and landscape)
- Touch-friendly panel expansion
- Readable text at phone scale
- Low bandwidth (cellular fallback)

**Mobile-Specific Features:**
- Swipe between panels (instead of all visible)
- Double-tap to expand panel
- Pull-to-refresh (manual sync)
- Haptic feedback on warnings (optional)

### QR Code Connection Flow

1. Player opens Settings > Dashboard
2. Enables "Network Access"
3. Game displays QR code with LAN URL
4. Player scans QR with phone camera
5. Dashboard loads in phone browser
6. Phone and game stay synced while on same network

**Fallback:** Manual URL entry for devices without camera.

### Multiple Simultaneous Viewers

**Supported:** Multiple devices can connect to same dashboard endpoint.

**Use Cases:**
- Second player viewing during co-op booking
- Streamer showing dashboard to audience
- Commentary/analysis while someone else plays

**Limitations:**
- Read-only for all viewers
- Same data shown to all (no per-viewer customization over network)
- Performance scales with viewer count (recommend max 4)

---

## INTEGRATION POINTS

### Data Flow Architecture

```
┌─────────────────────────────────────────────────────────┐
│                     GAME STATE                          │
│  (Roster, Shows, Tournaments, Feuds, Titles, etc.)      │
└────────────────────────┬────────────────────────────────┘
                         │
                         ▼
         ┌───────────────────────────────┐
         │     DASHBOARD STATE MANAGER    │
         │  (Subscribes to game events)   │
         │  (Maintains dashboard-ready    │
         │   data structures)             │
         └───────────────┬───────────────┘
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
    ┌──────────┐   ┌──────────┐   ┌──────────┐
    │  Native  │   │  Browser │   │  Network │
    │  Window  │   │  (local) │   │  (LAN)   │
    └──────────┘   └──────────┘   └──────────┘
```

### System-Specific Data Pulls

| Source System | Data Provided to Dashboard |
|---------------|---------------------------|
| **BOOK-001 Booking Engine** | Current show structure, match list, outcomes, booking intent |
| **POP-001 Popularity** | Worker popularity by region, trend indicators |
| **FEUD-001 Feud Memory** | Active feuds, heat levels, timeline, recommended blowoff |
| **CROWD-001 Crowd Memory** | Pattern warnings, what fans remember, cynicism alerts |
| **PRED-001 Predictability** | Stakes warnings, staleness alerts, streak tracking |
| **Tournament System** | Bracket state, advancement, round progress |
| **Title System** | Current holders, reign length, title prestige |
| **Contract System** | Expiration warnings, negotiation windows |
| **Injury System** | Worker availability, recovery timelines |

### Event Subscription Example

```gdscript
# Dashboard subscribes to relevant events
func _ready():
    GameState.booking_engine.match_added.connect(_on_match_added)
    GameState.booking_engine.match_completed.connect(_on_match_completed)
    GameState.feud_tracker.heat_changed.connect(_on_feud_heat_changed)
    GameState.title_system.title_changed.connect(_on_title_changed)
    GameState.roster.worker_status_changed.connect(_on_worker_status_changed)
    # etc.
```

---

## EDGE CASES

### Mid-Show Dashboard Behavior

**Scenario:** Player has dashboard open, starts running a show.

**Behavior:**
- Show Card panel highlights "current match" (if match simulation visible)
- Completed matches show outcomes in real-time
- Crowd energy indicator updates (if Phase 4 data available)
- No dashboard input accepted during show execution

### During Draft/Roster Changes

**Scenario:** Major roster shake-up (mass signings, releases, draft).

**Behavior:**
- Roster Quick View updates live but may flicker during rapid changes
- "Batch update in progress" indicator during mass operations
- Once batch completes, full refresh
- Feud/storyline panels handle removed workers gracefully (strike-through or "departed")

### Data Conflicts

**Scenario:** Dashboard shows Hogan as champion, but player just booked a title change that hasn't processed yet.

**Behavior:**
- Dashboard shows data as of last processed event
- Pending changes not reflected until committed
- If player cancels booking change, dashboard never showed wrong data
- Consistency over immediacy

### Network Disconnection (Browser/LAN Mode)

**Scenario:** Phone loses WiFi connection.

**Behavior:**
- Dashboard shows "Connection Lost" overlay
- Auto-reconnect attempts every 5 seconds
- On reconnect, full state sync
- No stale data displayed (overlay prevents reading outdated info)

### Performance Degradation

**Scenario:** Player on low-spec hardware, dashboard causing frame drops.

**Behavior:**
- Auto-detect performance issues (frame timing)
- Suggest reducing dashboard update frequency
- Offer to disable animated elements
- Worst case: prompt to close dashboard

### Multi-Save Switching

**Scenario:** Player loads different save while dashboard is open.

**Behavior:**
- Dashboard detects save switch
- Full state reset
- All panels repopulate from new save data
- Layout preferences persist (per-user, not per-save)

---

## IMPLEMENTATION DATA STRUCTURES

### Dashboard Configuration

```json
{
  "dashboard_config": {
    "mode": "native_window",
    "network": {
      "enabled": false,
      "port": 8585,
      "allow_lan": false
    },
    "auto_launch": false,
    "theme": "match_game",
    "global_density": "standard",
    "layout": {
      "type": "grid",
      "preset": "booker_focus",
      "panels": [
        {
          "id": "show_card",
          "enabled": true,
          "density": "standard",
          "position": {"row": 0, "col": 0}
        },
        {
          "id": "active_feuds",
          "enabled": true,
          "density": "standard",
          "position": {"row": 0, "col": 1}
        },
        {
          "id": "booking_warnings",
          "enabled": true,
          "density": "expanded",
          "position": {"row": 1, "col": 0, "colspan": 2}
        }
      ]
    },
    "mobile_prefs": {
      "swipe_navigation": true,
      "haptic_warnings": true
    }
  }
}
```

### Dashboard State Snapshot

```json
{
  "snapshot": {
    "sequence": 12847,
    "timestamp": "2024-12-24T10:30:00Z",
    "show_card": {
      "show_id": "show_001",
      "name": "WrestleMania III",
      "date": "1987-03-29",
      "venue": "Pontiac Silverdome",
      "matches": [
        {
          "order": 1,
          "match_id": "match_001",
          "type": "singles",
          "participants": ["Hogan", "Andre"],
          "stakes": "WWF Championship",
          "status": "scheduled",
          "booking_intent": "coronation"
        }
      ]
    },
    "tournaments": [...],
    "championships": [...],
    "active_feuds": [...],
    "roster_status": [...],
    "warnings": [...]
  }
}
```

---

## PERFORMANCE CONSIDERATIONS

### Resource Budget

| Mode | Target Frame Impact | Memory Budget |
|------|---------------------|---------------|
| Native Window | <1ms per frame | 50MB |
| Browser (local) | 0ms (separate process) | 20MB (browser) |
| Network (LAN) | 0ms (separate process) | 20MB (browser) + network overhead |

### Optimization Strategies

1. **Delta Updates:** Only send changed data, not full state
2. **Lazy Panel Loading:** Collapsed panels don't compute/render
3. **Throttled Updates:** Batch rapid-fire events
4. **Image Caching:** Worker portraits cached, not re-transmitted
5. **Text Compression:** JSON payloads gzipped for network mode

### Minimum Hardware Tiers

| Tier | Dashboard Support |
|------|-------------------|
| **Low (Potato)** | Browser mode only, reduced update frequency |
| **Medium** | All modes, standard performance |
| **High** | All modes, maximum update frequency, animations |

---

## ACCESSIBILITY

### Visual Accessibility

- High contrast theme available
- Scalable text (font size setting)
- Color-blind friendly status indicators (shapes + colors, not color alone)
- Screen reader compatible panel headers (for browser mode)

### Motor Accessibility

- Keyboard navigation in native window
- No time-sensitive interactions
- Panel expansion via single click/tap (no drag required)

### Cognitive Accessibility

- Compact mode reduces information overwhelm
- Preset layouts provide sensible defaults
- Warnings use clear, plain language
- No flashing or rapid animations

---

## FUTURE EXPANSION

### Potential Enhancements (Post-MVP)

1. **Commentary Integration:** Live match commentary appears in dedicated panel
2. **Social/Streaming:** Direct OBS integration for streamers
3. **Historical Mode:** Browse past shows, not just current
4. **Comparison View:** Side-by-side worker/feud comparisons
5. **Voice Alerts:** Optional audio cues for critical warnings
6. **Widget Mode:** System tray/desktop widget (Windows/Mac)
7. **Cloud Sync:** Dashboard accessible from any device via cloud (premium feature)

### Modding Support

- Dashboard panel types could be moddable
- Custom themes via CSS (browser mode)
- Plugin architecture for additional data sources

---

## RELATED SYSTEMS

- **BOOK-001:** Booking Engine (primary data source for show cards)
- **POP-001:** Popularity System (worker status data)
- **FEUD-001:** Feud Memory Tracker (active feud data)
- **CROWD-001:** Crowd Memory System (pattern warnings)
- **PRED-001:** Predictability Logic (staleness alerts)
- **EMOFLOW-001:** Emotional Show Flow (crowd energy during shows)
- **UI System:** (pending documentation, coordinates with main game interface)

---

## DOCUMENT HISTORY

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024-12-24 | Initial design. New system, not extracted from volumes. |

---

**Document Status:** Exploratory / New Design (not extracted from volumes)  
**Implementation Priority:** Medium (quality of life, not MVP-critical)  
**Next Steps:** 
- Technical prototype of native window mode
- WebSocket server spike for browser mode
- Mobile responsive design mockups
- Integration point audit with existing systems

---

*The best booking decisions come from clear information. The dashboard doesn't make you a better booker; it removes the friction between you and the data you need to book well.*
