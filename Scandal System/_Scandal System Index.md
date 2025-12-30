# Scandal System

📛 **SYSTEM:** Scandal and Public Image System
🧭 **CATEGORY:** Worker Simulation / Media
🔑 **KEYWORDS:** scandal, public image, controversy, redemption, legacy, morality, PR, media
📝 **SUMMARY:** Comprehensive system governing how scandals affect workers' careers, public perception, and long-term legacy. Scandals range from substance abuse to criminal activity, with era-dependent responses and redemption pathways. The world reacts to workers not just based on booking, but on perceived morality.

⚙️ **LOGIC OVERVIEW:**
- Hidden Morality rating (1-20) shapes scandal threshold and behavior
- Scandal types have different severity levels and recovery difficulty
- Era determines public and promotion response intensity
- Redemption is possible for most scandals, but must be earned
- Some scandals (child abuse, sexual assault) cannot be fully erased
- Fan memory and legacy interact with scandal through Scandal Flex system

🔬 **LLM INTEGRATION:** Minimal
- Scandal news article generation (optional)
- Public apology template generation (optional)
- Media reaction flavour text (optional)

📌 **ORIGIN:** Vol 4 (Worker Morality and Loyalty Systems section, Scandal and Public Image Layer)

---

## VERSION HISTORY

**Version 1.1 (Vol 2 Chunk 06) [CURRENT - LOCKED]**
- Added Scandal Chain Events (cascading scandal mechanics)
- Added Crisis Response System (player/AI scandal management)
- Added Toxic Worker Consequences (retention fallout)
- Connected to Management Behaviour Tags system
- Connected to Fanbase DNA System for demographic-specific reactions

**Version 1.0 (Vol 4) [LOCKED]**
- Scandal System fully formalized
- Hidden Morality rating (1-20) established
- Scandal type categories and severity levels defined
- Era-based response mechanics
- Redemption arc pathways created
- Scandal Flex system for legacy interaction
- Scandal-related tags defined
- Historical examples integrated

---

📎 **CONNECTED SYSTEMS:**
- [[Hidden_Personality|Hidden Personality]] (Morality rating determines scandal threshold)
- [[Contract System/_Contract System Index|Contract System]] (Morality clauses, firing risk)
- [[Crowd_Memory|Crowd Memory]] (Fan perception shifts with scandals)
- [[Injury System/Addiction Risk System|Addiction Risk System]] (Substance scandals originate here)
- [[Contract System/Firing System|Firing System]] (Scandals trigger termination)
- [[Hall of Fame/_Hall of Fame Index|Hall of Fame]] (Scandals affect eligibility)
- [[Media System/_Media System Index|Media System]] (Scandal coverage and narrative)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Scandal Types]] | Categories, severity levels, examples | Locked |
| [[Public Image Impact]] | How scandals affect reputation and career | Locked |
| [[Scandal Flex System]] | Long-term legacy interaction with scandals | Locked |
| [[Redemption Arcs]] | Recovery pathways and requirements | Locked (v1.2) |
| [[Era-Based Response]] | How different eras handle scandals | Locked |
| [[Star Protection System]] | How star power shields from consequences | Locked |
| [[Scandal Chain Events]] | Cascading scandal escalation mechanics | Locked (Vol 2) |
| [[Crisis Response System]] | Player/AI scandal management decisions | Locked (Vol 2) |
| [[Toxic Worker Consequences]] | Fallout from retaining scandal-tainted workers | Locked (Vol 2) |
| [[Japanese_Humiliation_Ritual_Reset]] | Japanese career reset rituals (head shaving, young lion reversion) | Locked (Vol 5) |

📎 **See Also:** [[Fan Reaction System/_Fan Reaction Index|Fan Reaction System]] for fanbase tolerance, loyalty resistance, and backlash mechanics

---

## Design Philosophy

Workers are not machines. They betray friends, protect enemies, destroy themselves, save themselves, sell out, atone: just like real life. Wrestling history is both a graveyard and cathedral of loyalty and betrayal.

**Core truths this system captures:**
- The world reacts to workers based on perceived morality, not just booking
- Redemption is possible, but it must be earned
- Some scandals cannot be erased, only marginalized over decades
- Era context dramatically changes scandal impact
- Fan memory challenges official narratives through documentary and discourse

---

## Hidden Morality Rating

The foundation of scandal behavior:

| Range | Behavior Tendencies |
|-------|---------------------|
| 1-4 (Amoral Opportunist) | Cheats, betrays, burns bridges without remorse. Prioritizes self over everything. |
| 5-8 (Situational Moralist) | Follows some personal codes but easily compromises for gain or survival. |
| 9-12 (Conflicted) | Desires to do good, but vulnerable to temptation, peer pressure, or booking politics. |
| 13-16 (Principled) | Holds strong personal ethics: hard to corrupt, resists dirty bookings and betrayals. |
| 17-20 (Moral Idealist) | Loyalty, honor, self-sacrifice define career choices: sometimes to own detriment. |

Every worker has a hidden morality code shaping actions outside and inside the ring. Players and AI must learn workers' true natures over time.

---

## Scandal Categories Overview

| Category | Examples | Recovery Difficulty |
|----------|----------|---------------------|
| **Substance Abuse** | Drug arrests, public intoxication, failed tests | Moderate |
| **Legal Trouble** | Arrests, lawsuits, violence outside ring | Variable |
| **Backstage Betrayal** | Conspiring against friends, leaked schemes | Moderate |
| **Sexual/Assault** | Sexual misconduct, assault allegations | Near-impossible |
| **Criminal Activity** | Serious crimes, fraud, theft | Very difficult |
| **Public Meltdowns** | Social media explosions, interview disasters | Moderate-Low |
| **Relationship Scandals** | Affairs, divorces, cheating exposed | Era-dependent |

---

## Historical Examples

| Worker | Scandal Type | Outcome |
|--------|--------------|---------|
| **Chris Benoit** | Criminal (murder-suicide) | Full erasure, "Cancelled Immortal" |
| **Jeff Hardy** | Substance abuse (multiple) | Redemption arcs, continued career |
| **Edge/Lita/Matt Hardy** | Relationship scandal | Short-term heat, long-term recovery |
| **Hulk Hogan** | Racial slurs (leaked) | Major perception drop, partial recovery |
| **Ric Flair** | Sexual misconduct allegations | Legacy tainted, not erased |
| **CM Punk** | Public meltdown (podcast) | Mixed reception, career pivot |

---

## Scandal-Related Tags

| Tag | Description |
|-----|-------------|
| **Scandal Magnet** | Consistently finds themselves in controversies |
| **Drama Magnet** | Regular source of personal/professional drama |
| **Redemption Arc** | Career storyline built around second chances |
| **Cancelled Immortal** | Will never be canonized but never forgotten |
| **Controversial Truth-Teller** | Remembered for exposing industry truths |

---

## Open Questions

- [ ] Exact probability formulas for scandal occurrence by morality level
- [ ] Severity thresholds for different scandal types
- [ ] Media coverage intensity calculations
- [ ] Cross-promotion scandal impact (does it follow them?)
- [ ] Sponsor/advertiser response mechanics

---

## Implementation Notes

```json
{
  "scandal_event": {
    "scandal_id": "scan_001",
    "worker_id": "worker_001",
    "type": "substance_abuse",
    "severity": "moderate",
    "date_occurred": "1985-07-22",
    "public_knowledge": true,
    "media_coverage_level": "high",
    "promotion_response": "suspension",
    "fan_reaction": "sympathetic",
    "legacy_impact": {
      "immediate": -25,
      "long_term": -10,
      "redemption_eligible": true
    },
    "redemption_status": {
      "active": false,
      "path": null,
      "progress": 0
    }
  }
}
```

---

**Document Status:** Locked (Vol 4)
**Last Updated:** 2025-12-21
**Next Review:** Integrate with Media System for coverage mechanics
