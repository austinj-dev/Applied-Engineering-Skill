# Checkpoint Protocol — Applied Engineering

## Planning Pulse (Every 30 Minutes)

Display after every 30 minutes of planning time OR after completing 2 categories:

```
PLANNING PULSE — [timestamp] ([X] min elapsed)
═══════════════════════════════════════════════
Decisions locked:     [X] / estimated [Y]
Categories completed: [X] / [Y] applicable
Complexity Score:     [score] [■■■■■□□□□□] [threshold note]
Planning velocity:    [X] decisions/min (trend: ↑/↓/→)
Confidence:           [X]%
Deferred items:       [X] (ratio to included: [X:Y])

Suggested action: [lock in / continue / deep-dive category X / consider MVP gate]
```

## Complexity Score Formula

```
Score = (tables × 2)
      + (roles × 5)
      + (integrations × 8)
      + (features × 1)
      + (API endpoints × 2)
      + (real-time features × 10)
      + (industry packs × 15)
      + (portal types × 10)
      + (subscription tiers × 3)
      + (background jobs × 5)
```

### Threshold Matrix

| Project Size | Score Range | Flag |
|-------------|------------|------|
| Small | 0-100 | Normal |
| Medium | 101-250 | ⚠️ "Getting complex for a medium project" |
| Large | 251-500 | Normal for large |
| Enterprise | 501-1000 | Normal for enterprise |
| Any | >1000 | 🔴 "Extremely high complexity. Consider splitting into multiple products or phased launches." |

When threshold hit, **suggest only**: "Complexity Score has reached [X]. Would you like to continue planning, consider an MVP gate, or lock in?"

**NEVER auto-opt-out of planning.** Always present as suggestion. Always continue if user says continue.

## Diminishing Returns Detector

After each batch, calculate: `new_decisions / questions_asked` for this batch.

| Ratio | Signal |
|-------|--------|
| >0.7 | High yield — keep going |
| 0.4-0.7 | Normal — continue |
| 0.2-0.4 | Diminishing — suggest lock-in |
| <0.2 | Very low — strongly suggest lock-in |

Display: "Last batch: [X] new decisions from [Y] questions ([Z]% yield). Previous batch: [A]%. Trend: [↑/↓/→]."

If diminishing: "We're seeing diminishing returns. Consider locking in — or I can go deeper on specific categories that yielded high results."

## MVP Gate (Optional, User-Triggered or Suggested)

Trigger when: complexity score exceeds threshold OR user requests OR halfway through planning.

Present:
```
MVP GATE CHECKPOINT
===================
If you launched TODAY with only these features, would it be viable?

TOP 10 HIGHEST-IMPACT FEATURES:
1. [feature] — [why it matters]
2. [feature] — [why it matters]
...10. [feature] — [why it matters]

Options:
A) Plan for MVP only — defer everything else to Phase 2+
B) Continue full planning — build the complete vision
C) Review what we've added beyond original scope
```

**Always ask. Never auto-select.**

## Scope Creep Alert

Track features added during planning vs original scope. If >40% expansion:

"You've expanded scope by [X]% since we started ([Y] features added beyond original description). Want to review what was added and decide what to keep vs defer?"

## Feature Freeze Ceremony

Before ANY document generation:

```
FEATURE FREEZE
==============
Total features planned: [X] (Include Now)
Total features deferred: [Y] (Phase 2+)
Total features rejected: [Z]

This is the final scope. Nothing more gets added after this point.
Do you confirm the feature freeze? (yes/no)
```

Only after "yes" → proceed to document generation.

## Over-Engineering Detection (Hybrid Approach)

Three signals combined:
1. **Complexity Score** exceeds threshold for project size
2. **Diminishing Returns** ratio drops below 0.3 for 2+ consecutive batches
3. **Deferred:Included ratio** exceeds 2:1

When 2 of 3 signals trigger:
"I'm noticing signs that we may be approaching over-engineering: [list which signals triggered]. This isn't a problem if it's intentional — enterprise systems are naturally complex. Would you like to: continue planning, lock in, or review the deferred items?"

## Planning Time Tracker

After 4+ hours: "We've been planning for [X] hours. The spec is at [Y]% confidence with [Z] decisions locked. Want to ship what we have or keep going?"

After 6+ hours: "This is a deep planning session — [X] hours. We've covered [Y] categories with [Z] decisions. Most projects at this depth are 90%+ confident. Ready to generate documents?"

After 8+ hours: "We're at [X] hours — this is enterprise-level planning. Let's ensure we're not in a planning loop. Here's what we have vs what's left: [summary]. Recommend generating documents now and iterating on gaps during implementation."

## Readiness Assessment (Before Document Generation)

Score 0-100:
- Questions answered: [X] / [Y] (weight: 40%)
- Suggestions categorized: [X] / [Y] (weight: 20%)
- Gaps identified and filled: [X] / [Y] (weight: 20%)
- Reference implementations provided: [X] (weight: 10%)
- Confidence rating: [X]% (weight: 10%)

Must hit 80+ to proceed. If below 80, identify what's dragging it down.
