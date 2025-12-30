# Contract System

📛 **SYSTEM:** Contract System
🧭 **CATEGORY:** Business & Labour
🔑 **KEYWORDS:** contracts, negotiations, firing, guaranteed money, merch cuts, union, CBA, labour relations
📝 **SUMMARY:** Comprehensive contract and labour relations system covering worker agreements, termination mechanics, merchandise compensation, and union dynamics. Transforms wrestling booking into labour management simulation with real consequences.

⚙️ **LOGIC OVERVIEW:**
- Contracts come in multiple forms with realistic clauses and fail states
- Firing has massive consequences, especially under unionization
- Merch cuts are contract clauses with real gameplay impact
- Every labour decision is remembered and sometimes leaked
- Contract morality score affects morale, trust, and media perception

🔬 **LLM INTEGRATION:** Minimal
- Contract negotiation dialogue generation (optional)
- Agent advice on worker demands (optional)
- Public statement templates for firings/scandals

📌 **ORIGIN:** Vol 4 (locked at lines 70402, 70519)

---

## VERSION HISTORY

**Version 1.0 (Vol 4) [CURRENT - LOCKED]**
- Contract System fully formalized
- 6 contract types defined (Handshake to Unionized)
- Negotiation clauses system created
- Merch cut mechanics established
- Guaranteed money and buyout rules
- Contract Morality Score introduced
- Firing System with consequence tracking
- Worker Resistance mechanics
- Loyalty System with multiple axes
- Historical context (Favoured Nations, WCW disasters, union attempts)

---

📎 **CONNECTED SYSTEMS:**
- [[Hidden_Personality|Hidden Personality]] (Ego, Loyalty, Morality affect negotiations)
- [[Tags_System|Tags System]] (Career Goals: Enjoy Life, Money First, Chase Greatness, etc.)
- [[Morale System]] (Contract satisfaction affects performance)
- [[Turn_Engine|Turn Engine]] (Contract disputes can trigger betrayals)
- [[Faction System/_Faction System Index|Faction System]] (Collective bargaining, faction loyalty)
- [[Worker Resistance]] (Pushback mechanics)
- [[Scandal System/_Scandal System Index|Scandal System]] (PR fallout from firings)

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Contract Types]] | 6 base contract types and their use cases | Locked |
| [[Negotiation Clauses]] | Contract features and special clauses | Locked |
| [[Merch Cut System]] | Merchandise compensation mechanics | Locked |
| [[Guaranteed Money & Payouts]] | Payout liability and buyout rules | Locked |
| [[Contract Morality Score]] | Hidden scoring affecting morale/trust | Locked |
| [[Firing System]] | Termination mechanics by contract type | Locked |
| [[Worker Resistance]] | Pushback, refusals, and leverage | Locked |
| [[Loyalty System]] | Multiple loyalty axes affecting decisions | Locked |

---

## Design Philosophy

This system transforms you from "fantasy GM" to "labour boss in a volatile ecosystem." Wrestling has always been about exploitation of workers under the guise of "independent contractor" status. The Contract System makes this tension playable:

- **Handshake deals** represent the territory era's brutal informality
- **Guaranteed contracts** create the 90s WCW disaster potential
- **Union contracts** represent the dream that never was (and could be)
- **Merch cuts** are where workers actually make their money

Every decision is remembered. Word gets out. Your reputation as a boss follows you.

---

## Historical Context

Real-world contract dynamics inform this system:
- **Favoured Nations Clause**: Hall/Nash WCW deals (auto-raise to match highest paid)
- **Handshake Culture**: CMLL, territory era, Vaquer/WWE predation
- **Guaranteed Money**: WCW's downfall, current AEW model
- **Union Attempts**: Jesse Ventura organizing, Hogan snitching to protect his position

---

## Open Questions

- [ ] Exact formulas for contract negotiation success rates
- [ ] Agent influence on worker demands (percentages)
- [ ] Media leak probability calculations
- [ ] Settlement negotiation mechanics for guaranteed contracts
- [ ] Cross-promotion poaching rules and penalties

---

## Implementation Notes

```json
{
  "contract": {
    "id": "contract_001",
    "worker_id": "worker_001",
    "promotion_id": "promo_001",
    "type": "written_time_locked",
    "term_days": 365,
    "base_pay": 250000,
    "guaranteed": false,
    "clauses": {
      "push_promise": { "tv_matches_per_month": 2 },
      "title_opportunity": false,
      "creative_control": false,
      "favoured_nations": false,
      "merch_cut": { "type": "standard", "worker_percent": 30 },
      "exclusive_branding": false,
      "limited_dates": false
    },
    "morality_score": 72,
    "signed_date": "1985-01-15",
    "expires_date": "1986-01-15"
  }
}
```

---

**Document Status:** Locked (Vol 4)
**Last Updated:** 2025-12-20
**Next Review:** Add exact negotiation formulas when specified
