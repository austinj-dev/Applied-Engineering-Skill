# Confidence Assessment — Applied Engineering

## Rating Scale
| Rating | Meaning | Action |
|--------|---------|--------|
| 95-98% | Everything locked, complete schemas, patterns, seeds, scripts | Ship it |
| 90-94% | Mostly complete, minor gaps Phase 0 catches | Ship with notes |
| 80-89% | Most decisions locked, some unknowns | Enhance before shipping |
| 70-79% | Major decisions locked but unknowns remain | Back to gap analysis |
| Below 70% | Too many unknowns | Back to questions |

## What Adds Confidence
1. Complete database schemas (actual SQL) → +5%
2. Complete RLS/permission policies → +5%
3. MEMORY.md system → +5%
4. Reference code patterns → +3%
5. Zod/validation schemas → +3%
6. Verification scripts per phase → +3%
7. Session splitting with handoff → +3%
8. Complete seed data SQL → +3%
9. Migration dependency chain → +2%
10. Component library selection with specific components → +2%
11. Competitive research completed → +2%
12. Security review completed → +2%
13. Cost estimate completed → +1%
14. Launch checklist completed → +1%

## If Below 90%
Identify what's dragging it down. Add it. Re-rate. Repeat until 90%+.
