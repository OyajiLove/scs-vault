# SCS Systems Bible - ID Naming Convention

**Established:** 2025-12-22
**Status:** CANONICAL

---

## Standard Format

All entity IDs use **lowercase snake_case** with optional numeric suffix:

```
{entity_type}_{identifier}
```

---

## Entity ID Patterns

| Entity Type | Pattern | Example |
|-------------|---------|---------|
| Worker | `worker_{id}` | `worker_001`, `worker_12345` |
| Promotion | `promo_{id}` | `promo_001`, `promo_cca` |
| Faction | `faction_{id}` | `faction_001`, `faction_elite` |
| Title | `title_{id}` | `title_001`, `title_world` |
| Contract | `contract_{id}` | `contract_001` |
| Feud | `feud_{yyyy}_{seq}` | `feud_2024_001` |
| Turn | `turn_{yyyy}_{seq}` | `turn_2024_001` |
| Event | `evt_{yyyy_mm_dd}` | `evt_2024_05_15` |
| Show | `show_{id}` | `show_001`, `show_wrestlemania` |
| Match | `match_{id}` | `match_001` |
| Scandal | `scan_{id}` | `scan_001` |
| Gimmick | `gim_{id}` | `gim_001` |
| Snapshot | `snap_{id}` | `snap_001` |
| Trail | `tr_{id}` | `tr_001` |
| Territory | `terr_{id}` | `terr_south`, `terr_japan` |
| Arena | `arena_{id}` | `arena_msg`, `arena_001` |

---

## Rules

1. **Always lowercase** (never `WORK_001` or `Worker_001`)
2. **Use underscores** for word separation (never hyphens or camelCase)
3. **Prefix indicates entity type** for easy identification
4. **Numeric IDs** can be zero-padded (`001`) or plain (`1`)
5. **Semantic IDs** allowed where useful (`promo_cca`, `terr_japan`)
6. **Date-based IDs** use `yyyy_mm_dd` or `yyyy_seq` format

---

## Reference Examples

### Worker
```json
{
  "worker_id": "worker_001",
  "name": "Terry Funk"
}
```

### Feud
```json
{
  "feud_id": "feud_2024_001",
  "workers": ["worker_a", "worker_b"]
}
```

### Event
```json
{
  "event_id": "evt_2024_05_15",
  "promotion": "promo_001"
}
```

### Title
```json
{
  "title_id": "title_001",
  "current_champion": "worker_001"
}
```

---

## Why This Convention

1. **Consistency:** One pattern across all systems
2. **Readability:** Lowercase is easier to scan
3. **Debugging:** Prefix tells you entity type at a glance
4. **Flexibility:** Supports both numeric and semantic IDs
5. **Modern:** Aligns with standard API/database conventions

---

## Migration Notes

The following files were updated on 2025-12-22 to match this convention:

| File | Changes |
|------|---------|
| Worker_Skills.md | `WORK_12345` → `worker_12345` |
| Hidden_Personality.md | `WORK_12345` → `worker_12345` |
| Popularity_System.md | `WORK_12345` → `worker_12345` |
| Turn_Engine.md | `TURN_`, `WORK_A/B`, `FEUD_` → lowercase |
| Feud_Memory.md | `FEUD_`, `WORK_A/B` → lowercase |
| Crowd_Memory.md | `PROM_001`, `EVT_` → lowercase |
| Emotional_Show_Flow.md | `SHOW_` → `show_` |
| Predictability_Stakes.md | `MATCH_` → `match_` |
| Tags_System.md | `ANCH_` → `anchor_` |

---

**All new schemas must follow this convention.**

*Last Updated: 2025-12-22*
