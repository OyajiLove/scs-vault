# Financial System

📛 **SYSTEM:** Economics and Financial Management
🧭 **CATEGORY:** Business / Promotion Management
🔑 **KEYWORDS:** finances, revenue, expenses, gate, merch, TV deals, budget, economics, sponsorship, attendance, draw
📝 **SUMMARY:** Governs promotion financial health, revenue streams, and expense management. Includes merchandise calculations, sponsorship dynamics, and attendance/draw power systems.

⚙️ **LOGIC OVERVIEW:**
- Revenue: gate receipts, TV deals, merchandise, sponsorships, PPV
- Expenses: worker contracts, venue costs, production, travel, staff, marketing
- Financial health affects: hiring ability, show quality, worker retention
- Promotion can go bankrupt if expenses exceed revenue
- Worker marketability directly affects merchandise revenue

🔬 **LLM INTEGRATION:** Minimal

📌 **ORIGIN:** Vol 1 Extraction #130, #135, #144, Referenced throughout Vol 1-4

📎 **CONNECTED SYSTEMS:**
- [[Contract System/_Contract System Index|Contract System]] (Payroll, guaranteed money)
- [[SCS_BIBLE_12_TV_BROADCAST_SYSTEM|TV Broadcast System]] (TV revenue)
- [[Title System/_Title System Index|Title System]] (Title prestige affects merch)
- [[Injury System/_Injury System Index|Injury System]] (Healthcare costs)
- [[Arena System/_Arena System Index|Arena System]] (Venue costs, production budget)
- [[_Popularity System Index|Popularity System]] (Draw power)

❓ **OPEN QUESTIONS:**
- Exact revenue calculation formulas
- Bankruptcy mechanics and recovery
- Loan/investment options
- Era-specific financial norms

✅ **STATUS:** Locked (Concept)

---

## Version History

| Version | Source | Status |
|---------|--------|--------|
| 0.5 | Vol 1-4 | 📐 CONCEPTUAL |
| 1.0 | Vol 1 Extraction #130, #135, #144 | 🔒 LOCKED (concept) |

---

## Revenue Streams (#135)

| Source | Factors |
|--------|---------|
| **Gate** | Attendance × ticket price |
| **TV Deal** | Company prestige, ratings, market size |
| **Merchandise** | Worker overness, marketability tags |
| **Sponsorship** | Brand image, era, scandal exposure |
| **PPV/Streaming** | Event prestige, card quality, buy rate |
| **Licensing** | Video games, toys, media deals |

### Gate Revenue

```
Gate Revenue = Attendance × Average Ticket Price × Venue Cut
```

| Factor | Effect |
|--------|--------|
| Main event draw | Primary attendance driver |
| Card depth | Supporting factor |
| Venue location | Regional pricing variance |
| Time of year | Seasonal attendance patterns |

### TV Deal Revenue

| Deal Tier | Annual Value | Requirements |
|-----------|--------------|--------------|
| **Local/Regional** | Low | Minimal production standards |
| **Cable/National** | Medium | Professional production, ratings minimums |
| **Network/Premium** | High | Top-tier production, exclusive content |
| **Streaming** | Variable | Content volume, subscriber metrics |

### Sponsorship Revenue

| Era | Sponsorship Availability |
|-----|--------------------------|
| **Pre-1990s** | Limited, wrestling had few sponsors |
| **1990s** | Growing, tied to ratings boom |
| **Post-2000s** | Significant, brand-sensitive |

**Sponsor Sensitivity:** Sponsors pull money immediately if scandals taint brand in post-90s eras.

---

## Expenses (#135)

| Cost | Factors |
|------|---------|
| **Talent** | Contracts, per-appearance fees, bonuses |
| **Production** | Venue, staging, pyro (see [[Production & Entrance Mechanics]]) |
| **Travel** | Roster size, distances, schedule density |
| **Staff** | Road agents, trainers, refs, creative |
| **Marketing** | Promotion, advertising, PR |
| **Medical** | Healthcare, injury costs |

### Profit/Loss Calculation

```
Net Income = Total Revenue - Total Expenses
```

| Financial Health | Effect |
|------------------|--------|
| **Profitable** | Can expand, sign talent, improve production |
| **Break-Even** | Stable but limited growth |
| **Loss (Manageable)** | Cost-cutting required, reduced investment |
| **Loss (Critical)** | Desperation mode, fire sales, potential bankruptcy |

---

## Merchandise System (#130)

### Marketability Tags

| Tag | Effect |
|-----|--------|
| **Marketing Nightmare** | Heavily penalized merch sales |
| **Unmarketable** | Penalized merch sales |
| **Easily Marketable** | Boosted merch sales |
| **Marketing Dream** | Massively boosted merch sales |
| **Merch Machine** | Massive merchandise multiplier |
| **Visual Icon** | Recognizable look boosts posters/marketing |

### Temporary Merch Boosts

| Boost | Effect | Duration |
|-------|--------|----------|
| **Hot New Catchphrase** | Bonus to angles where they talk + merch boost | 3 months to 2 years |
| **Flavour of the Month** | Bonus to match/angle ratings + merch boost | 1-3 months |
| **Groundswell of Support** | Large merch boost, organic fan movement | 6 months to 2 years |

### Sex Appeal Factor

Sex appeal is important for:
- Crossover potential (mainstream media)
- Merchandise sales (posters, calendars)
- Social media stardom
- Sponsor attractiveness

### Merch Revenue Formula (Conceptual)

```
Worker Merch Revenue = Base Sales × Popularity Modifier × Marketability Modifier × Boost Modifier
```

---

## Attendance/Draw Power System (#144)

### Draw Calculation

| Factor | Weight |
|--------|--------|
| Main Event Quality | 30% |
| Title Matches | 20% |
| Feud Heat | 25% |
| Company Prestige | 15% |
| Regional Factors | 10% |

### Attendance Effects

| Attendance Level | Effect |
|------------------|--------|
| **Sellout** | Hot crowd, better match ratings, morale boost |
| **Strong (80%+)** | Good energy, normal operations |
| **Moderate (50-80%)** | Crowd energy suffers slightly |
| **Poor (under 50%)** | Cold crowd, performance suffers, morale hit |
| **Disaster** | Empty seats visible, media attention, major morale hit |

### Trend Tracking

| Trend | Effect |
|-------|--------|
| **Consistent sellouts** | Prestige rises, TV deal negotiations strengthen |
| **Declining attendance** | Warning signs, media questions, talent concerns |
| **Regional variations** | Market-specific booking required |

---

## Financial Health States

| State | Characteristics |
|-------|-----------------|
| **Thriving** | Surplus funds, expansion possible, top talent attracted |
| **Stable** | Meeting expenses, modest growth, normal operations |
| **Struggling** | Tight margins, cost-cutting, talent retention issues |
| **Critical** | Desperation decisions, fire sales, closure risk |
| **Bankrupt** | Game over or buyout scenario |

### Desperation Mode Effects

When in critical financial state:
- Forced to release high-paid talent
- Production quality drops
- Talent refuses to sign
- TV deal renegotiation (worse terms)
- Potential buyout offers

---

## Implementation Notes

```json
{
  "promotion_id": "promo_001",
  "financial_state": "stable",
  "finances": {
    "revenue": {
      "gate": 250000,
      "tv_deal": 500000,
      "merch": 150000,
      "sponsorship": 100000,
      "ppv": 200000
    },
    "expenses": {
      "talent": 400000,
      "production": 150000,
      "travel": 100000,
      "staff": 75000,
      "marketing": 50000
    },
    "net_income": 425000
  },
  "attendance_trend": "stable",
  "average_attendance_percentage": 0.78
}
```

---

## Connected Mechanics

- [[Contract System/_Contract System Index|Contract System]] - Payroll management
- [[Arena System/_Arena System Index|Arena System]] - Venue costs, production budget
- [[_Popularity System Index|Popularity]] - Draw power calculation
- [[Territory System/_Territory System Index|Territory System]] - Regional market size
- [[_Media System Index|Media System]] - TV deal negotiations

---

## Open Questions

- [ ] Exact formulas for all revenue streams
- [ ] Bankruptcy mechanics (restructuring, buyout, closure)
- [ ] Loan/investor mechanics
- [ ] Era-specific financial norms (1985 vs 2020)
- [ ] Multi-promotion economic competition

---

**Document Status:** Locked (Concept)
**Last Updated:** 2025-12-25
**Next Review:** Design exact revenue/expense formulas
