# Aging & Career Arcs System

📛 **SYSTEM ID:** AGE-001
🧭 **CATEGORY:** Worker Lifecycle / Long-Term Simulation
🔑 **KEYWORDS:** aging, career arc, peak years, decline, veteran, trajectory, lifecycle, role evolution
📝 **SUMMARY:** 

The Aging & Career Arcs System governs how workers progress through their careers from debut to retirement. It tracks the physical and mental changes that occur with age, defines peak performance windows by style, and provides arc templates that shape how workers' careers unfold over time. This system connects skill development, injury accumulation, and eventual transition to non-wrestling roles.

⚙️ **LOGIC OVERVIEW:**
- Workers have distinct career phases: Young, Peak, Veteran, Twilight
- Physical stats decline after peak years; mental stats may continue improving
- Different wrestling styles have different peak windows (high flyers peak earlier)
- Career arcs provide narrative templates (meteoric rise, journeyman grind, etc.)
- Accumulated wear from injuries and style accelerates decline
- Workers can transition to non-wrestling roles (manager, trainer, booker)
- Retirement triggers when physical decline crosses performance threshold

🔬 **LLM INTEGRATION:** Minimal (curve calculations), but LLM can generate career summaries, milestone narratives, and retirement ceremonies

📌 **ORIGIN:** Vol 4 (career arc templates, peak years concept), Worker Skills (growth/decline rates)

📎 **CONNECTED SYSTEMS:** 
- [[Training System/_Training System Index|Training System]] - Early career development
- [[Retirement System/_Retirement System Index|Retirement System]] - End of career handling
- [[Injury System/_Injury System Index|Injury System]] - Wear accumulation
- [[Worker_Skills|Worker Skills]] - Stat changes over time
- [[Hidden_Personality|Hidden Personality]] - Trait evolution
- [[Popularity_System|Popularity]] - Legacy building

❓ **OPEN QUESTIONS:**
- Exact formulas for stat decline curves
- How injury history modifies decline rate
- When does "twilight" phase begin (fixed age vs. performance-based)?
- Role evolution probability formulas
- How do career arcs interact with booking decisions?

✅ **STATUS:** Partially Locked (phases, templates from Vol 4), Open (formulas)

---

## VERSION HISTORY

**Version 1.0 (Vol 4) [PHASES & TEMPLATES LOCKED]**
- Career phases defined (Young, Peak, Veteran, Twilight)
- Career arc templates established
- Peak years by style concept locked
- Physical vs mental stat trajectories

**Version 1.5 (Vol 1-4) [CONCEPTUAL]**
- Physical decline curve formulas proposed
- Role evolution mechanics (manager, trainer, booker)
- Injury accumulation impact on decline
- Legacy building integration

---

## System Components

| File | Description | Status |
|------|-------------|--------|
| [[Career Phases]] | Lifecycle stages from debut to retirement | ✅ Locked |
| [[Career Arc Templates]] | Narrative trajectory patterns | ✅ Locked |
| [[Peak Years by Style]] | Style-specific performance windows | ✅ Locked |
| [[Physical Decline]] | How body deteriorates with age | 📝 Conceptual |
| [[Role Evolution]] | Transition to non-wrestling roles | 📝 Conceptual |

---

## Design Philosophy

Careers in wrestling are finite. The body cannot sustain the abuse indefinitely. The Aging System respects this reality while creating meaningful long-term gameplay. Players must:

- Develop young talent before veterans decline
- Manage declining stars' egos and expectations
- Plan for generational transitions
- Decide when to retire legends vs. let them fade

The goal is to create natural career narratives without scripting outcomes.

---

## Integration Points

**With Training System:**
- Young phase has highest development potential
- Peak phase sees slower skill growth
- Veteran phase focuses on mental stat maintenance
- Training cannot reverse physical decline

**With Injury System:**
- Injuries accelerate decline curves
- Accumulated wear creates permanent ceiling reduction
- Major injuries can force early retirement
- Working hurt compounds long-term damage

**With Retirement System:**
- Aging triggers retirement consideration
- Performance decline below threshold prompts retirement decisions
- Personality affects how workers handle decline
- Comeback mechanics address return attempts

**With Popularity System:**
- Long careers build legacy
- Decline can erode fan connection
- "Nostalgia pop" for returning legends
- Career achievements compound into legacy score

---

## Implementation Priority

**Phase 1 (MVP):** Career phases, basic decline curves
**Phase 2:** Arc templates, style-specific peaks
**Phase 3:** Role evolution, legacy calculation

---

**Document Status:** Index Complete, Templates Locked, Formulas Need Design
**Last Updated:** 2025-12-21
**Next Review:** Design decline curve formulas
