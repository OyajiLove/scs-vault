# Era-Based Scandal Response

📛 **MECHANIC:** Era-Dependent Scandal Handling
🔗 **PARENT SYSTEM:** [[_Scandal System Index|Scandal System]]
🧭 **CATEGORY:** Worker Simulation / Media
🔑 **KEYWORDS:** era, territory, modern, social media, kayfabe, scandal response, cultural context
📌 **ORIGIN:** Vol 4 (Era-dependent scandal mechanics throughout)
✅ **STATUS:** Locked

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 1.0 | Vol 4 | 🔒 LOCKED |

---

## Overview

How scandals are handled varies dramatically by era. Territory days protected kayfabe and minimized public exposure. Modern era creates instant, permanent records with sponsor pressure. Understanding era context is essential for realistic scandal simulation.

---

## Era Comparison Overview

| Era | Documentation | Spread Speed | Permanence | Tolerance |
|-----|---------------|--------------|------------|-----------|
| **Territory (1950s-1980s)** | Minimal | Slow (word of mouth) | Low | High |
| **National TV (1980s-1990s)** | Moderate | Medium (magazines, newsletters) | Medium | Medium |
| **Monday Night Wars (1996-2001)** | Growing | Fast (early internet) | Medium-High | Medium |
| **Post-Attitude (2002-2010s)** | High | Fast (internet standard) | High | Lower |
| **Modern (2010s-Present)** | Maximum | Instant (social media) | Permanent | Variable |

---

## Territory Era (1950s-1980s)

### Scandal Characteristics
| Factor | Description |
|--------|-------------|
| **Kayfabe Protection** | Promoters actively suppressed scandal info to protect business |
| **Local Scope** | Scandals often stayed regional; could escape by changing territory |
| **Tough Guy Culture** | Violence, drinking normalized; less "scandalous" |
| **No Permanent Record** | Photos, videos rare; word of mouth faded |
| **Promoter Power** | Boss decided what was scandal vs. "just the boys" |

### Common "Non-Scandals"
- Bar fights (expected)
- Substance use (normalized)
- Relationship drama (private)
- Violence between workers (settled internally)

### Actual Scandals (Territory Era)
- Breaking kayfabe publicly
- Shooting on opponents without approval
- Stealing money from promoter
- Getting arrested in ways that hit newspapers
- Crossing promoter's family/allies

---

## National TV Era (1980s-1990s)

### Scandal Characteristics
| Factor | Description |
|--------|-------------|
| **Magazine Coverage** | Wrestling magazines covered backstage drama |
| **Newsletter Culture** | Meltzer, Keller emerging; insider info spreading |
| **Corporate Image** | WWF/NWA becoming brands with image to protect |
| **Steroid Scandal** | Government involvement changed stakes |
| **TV Advertiser Pressure** | Beginning of sponsor concerns |

### Scandal Response Evolution
- More formal PR responses needed
- Suspensions becoming standard
- Cover-up attempts (often successful)
- Talent shuffle to minimize exposure

### Notable Scandals
- WWF Steroid Trial
- Various arrest incidents
- Early substance-related deaths gaining attention

---

## Monday Night Wars Era (1996-2001)

### Scandal Characteristics
| Factor | Description |
|--------|-------------|
| **Internet Emergence** | Newsboards, early websites spreading info |
| **Tape Trading Culture** | Footage of incidents could circulate |
| **Shoot Interview Boom** | Workers talking openly about industry |
| **Edgy Content Blur** | Hard to distinguish work from shoot sometimes |
| **Competition** | Workers could jump ship, taking heat with them |

### Scandal Response Evolution
- Internet rumors harder to suppress
- Shoot promos incorporated real drama
- "Reality" becoming part of product
- Still some corporate protection possible

---

## Post-Attitude Era (2002-2010s)

### Scandal Characteristics
| Factor | Description |
|--------|-------------|
| **WWE Monopoly** | One major employer = more power over workers |
| **Wellness Policy** | Formal drug testing after Benoit |
| **Internet Standard** | Everyone online, news spreads fast |
| **YouTube Era** | Video evidence easily distributed |
| **Social Media Beginning** | Twitter/Facebook creating direct worker-fan connection |

### Scandal Response Evolution
- Wellness violations publicized
- Suspensions announced officially
- PR departments fully developed
- Sponsor pressure increasing
- Benoit case = industry-changing scandal

---

## Modern Era (2010s-Present)

### Scandal Characteristics
| Factor | Description |
|--------|-------------|
| **Instant Documentation** | Every incident potentially recorded |
| **Permanent Record** | Screenshots, archives last forever |
| **Social Media Direct** | Workers speak directly to fans (and get in trouble) |
| **Sponsor Sensitivity** | Advertisers can force action |
| **Cancel Culture Dynamics** | Rapid mobilization for/against workers |
| **Multiple Platforms** | AEW, WWE, indie alternatives change dynamics |

### Modern Scandal Response
| Response Type | Description |
|---------------|-------------|
| **Immediate Suspension** | No waiting for facts; protect brand first |
| **PR Statement Within Hours** | Social media demands rapid response |
| **Sponsor Pressure** | Advertisers may force release decisions |
| **Social Media Pile-On** | Public opinion forms instantly |
| **Investigation Culture** | #SpeakingOut type movements |

### Modern Paradox
- Minor scandals blow up faster
- But redemption cycles also faster for some issues
- Substance abuse more sympathetic than before
- Sexual misconduct less tolerated than ever
- Political statements can be career-defining

---

## Era-Specific Tolerance Levels

| Issue | Territory | National TV | Modern |
|-------|-----------|-------------|--------|
| **Substance Abuse** | Normal | Concern | Sympathetic (if addressed) |
| **Bar Fights** | Expected | Bad PR | Firing offense |
| **Racism/Bigotry** | Normalized | Overlooked | Career-ending |
| **Sexism** | Normalized | Overlooked | Major scandal |
| **Relationship Drama** | Private | Gossip | Public spectacle |
| **Political Statements** | Kayfabe | Avoided | Polarizing/risky |

---

## Media Ecosystem by Era

| Era | Primary Media | Secondary Media |
|-----|---------------|-----------------|
| **Territory** | Local newspapers, word of mouth | None |
| **National TV** | Wrestling magazines | Newsletters |
| **MNW** | Wrestling websites, newsletters | Early social media |
| **Post-Attitude** | Wrestling websites, mainstream news | Social media emerging |
| **Modern** | Social media, mainstream news | Podcasts, YouTube, streaming |

---

## Access to History by Era

How fans can research workers' pasts:

| Era | Research Ability |
|-----|------------------|
| **Territory** | Very limited; rely on secondhand accounts, books |
| **National TV** | Magazines, newsletters, some video |
| **MNW** | Internet archives, tape trading networks |
| **Post-Attitude** | YouTube, Wikipedia, comprehensive databases |
| **Modern** | Everything searchable; Cagematch, ProFightDB, social archives |

**Implication:** Modern scandals are permanent; territory scandals can be genuinely forgotten.

---

## Connected Mechanics

- [[Scandal Types]] - Era affects severity of scandal types
- [[Public Image Impact]] - Era modifies coverage intensity
- [[Scandal Flex System]] - Era affects memory decay rate
- [[Redemption Arcs]] - Era affects forgiveness speed
- [[Media System]] - Era determines available media channels

---

## Open Questions

- [ ] Exact era modifier values for scandal calculations
- [ ] Transition period mechanics (e.g., 1995-1997 internet emergence)
- [ ] Regional variations within eras (Japan vs. US vs. Mexico)
- [ ] How workers can exploit era limitations
- [ ] Cross-era scandal discovery (old scandal surfaces in new era)

---

## Implementation Notes

```json
{
  "era_scandal_config": {
    "era": "modern",
    "documentation_level": "maximum",
    "spread_speed": "instant",
    "permanence": "permanent",
    "base_tolerance": {
      "substance_abuse": "sympathetic",
      "violence": "low_tolerance",
      "racism": "zero_tolerance",
      "sexism": "very_low_tolerance",
      "relationship": "moderate_interest"
    },
    "media_channels": ["social_media", "mainstream_news", "podcasts", "youtube"],
    "sponsor_pressure": true,
    "response_time_expected": "hours",
    "recovery_speed_modifier": 1.2,
    "decay_rate_modifier": 0.5
  }
}
```
