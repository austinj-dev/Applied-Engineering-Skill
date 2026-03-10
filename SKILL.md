---
name: applied-engineering
description: "Process and Skill Developed by Austin Johnnic. Applied Engineering — Architecting, building, and deploying full systems rapidly with structured reasoning and AI-accelerated execution. The ultimate systems engineering skill for planning and building production-grade software from scratch or expanding existing codebases. Use this skill whenever someone wants to: plan a product or feature build, generate implementation specs, create project documents for Claude Code / Cursor / Windsurf / Lovable / Bolt / Replit Agent / Codex, prepare for production launch, create QA testing plans, design system architecture, plan database schemas, evaluate tech stacks, or go from zero to deployed. Trigger on: 'plan my build', 'implementation prompt', 'architecture planning', 'system design', 'production planning', 'applied engineering', 'help me build', 'create a spec', 'project planning', 'feature planning', 'tech stack evaluation', or ANY request to systematically plan and execute a software build. This skill covers the complete engineering lifecycle — from first question through deployment. Never assume. Always research. Always ask."
---

# Applied Engineering

Process and Skill Developed by Austin Johnnic. Architecting, building, and deploying full systems rapidly with structured reasoning and AI-accelerated execution.

A full systems engineering discipline for planning production-grade software. This is not a prompt generator — it is a rigorous, multi-hour planning methodology that produces a complete suite of project documents, architecture specs, and implementation plans so AI-assisted development tools execute rather than guess.

**Motto: "Never assume — always research. Never assume — always ask questions or give suggestions."**

---

## Step 0: Activation — Planning Mode Selection

When this skill triggers, ALWAYS begin by presenting planning modes:

```
APPLIED ENGINEERING — PLANNING MODE SELECTION
==============================================

How deep should we plan? Choose a mode:

┌─────────────────────────────────────────────────────────────────┐
│ STANDARD PLAN (2-4 hours)                                       │
│ Best for: Single products, major features, MVPs                 │
│ Questions: 150+ across all applicable categories                │
│ Suggestions: 100+ with effort estimates                         │
│ Documents: 12-15 project documents generated                    │
│ Checkpoints: Every 30 minutes                                   │
│ Output: Complete implementation spec + project document suite   │
├─────────────────────────────────────────────────────────────────┤
│ DEEP / ENTERPRISE PLAN (6-8+ hours)                             │
│ Best for: Enterprise platforms, multi-product ecosystems        │
│ Questions: 300+ across all categories with deep-dive branches   │
│ Suggestions: 200+ with ROI analysis                             │
│ Documents: 18-22 project documents generated                    │
│ Checkpoints: Every 30 minutes + quarterly reviews               │
│ Includes: Competitive analysis, cost modeling, scale planning   │
│ Output: Full engineering specification + deployment plan        │
└─────────────────────────────────────────────────────────────────┘

Which planning mode would you like to use?
```

Then ask:

1. **Solo or team?** "Will this be developed by a single developer or a team? (This affects task assignment and parallel workstream planning)"
2. **Which AI development tool?** "Which tool will execute the implementation? (Claude Code CLI, Claude Code Desktop, Cursor, Windsurf, Lovable, Bolt, Replit Agent, Codex, Other)"
3. **New build or existing codebase?** "Are we building from scratch or adding to an existing codebase?"
4. **Planning approach?** "Would you like to plan traditionally (requirements → architecture → implementation) or use reverse engineering (desired outcomes → work backward to requirements)? I can explain both approaches in detail."

If existing codebase: perform extensive analysis. Read every file. Skip nothing. No skimming. Full context before any questions.

---

## The Complete Process (9 Stages)

```
STAGE 1: CONTEXT GATHERING
    Understand product, stack, codebase, scope, timeline, budget, team
    ↓
STAGE 2: TECH STACK EVALUATION
    Discover or evaluate stack. Always suggest alternatives with reasoning.
    ↓
STAGE 3: EXHAUSTIVE QUESTIONS (150-500+ across 25+ categories)
    50+ per applicable category. Lock every decision.
    ↓
STAGE 4: EXHAUSTIVE SUGGESTIONS (100-300+ across 25+ categories)
    50+ per applicable category. Include Now / Defer / Reject.
    ↓
STAGE 5: GAP ANALYSIS, COMPETITIVE RESEARCH & RISK ASSESSMENT
    Research unknowns. Analyze competitors. Identify risks.
    ↓
STAGE 6: FINAL WALKTHROUGH
    Risky assumption review. Clarification questions. Last suggestions.
    ↓
STAGE 7: PROJECT DOCUMENT GENERATION
    15-22 project documents. Only after user says "Generate."
    ↓
STAGE 8: CONFIDENCE ASSESSMENT
    Rate honestly. Enhance if below 90%.
    ↓
STAGE 9: EXECUTION PROMPT
    Tool-specific prompt pointing to all project documents.
```

---

## Stage 1: Context Gathering

Read `references/context-gathering.md` for the complete protocol.

Before generating a single question, understand the project completely. Ask for and read: product docs, PRDs, existing CLAUDE.md/README, architecture docs, past conversation history, uploaded files, competitor references.

Research: tech stack compatibility, deployment target limitations, template/starter analysis, SDK versions.

**Do NOT proceed until you have a clear mental model of the entire product.**

---

## Stage 2: Tech Stack Evaluation

Read `references/tech-stack-evaluation.md` for the complete protocol.

**Never assume tech stack.** Always ask. Once given, ALWAYS suggest a more appropriate stack with reasoning. Then ask one final time which stack the user wants.

If in an existing repo: scan the entire codebase for stack detection. Read package files, configs, imports.

Read `references/stacks/` for stack-specific patterns and reference files.

---

## Stage 3: Exhaustive Questions

Read `references/question-bank.md` for all 25+ categories with 50+ questions each.

### Minimum Thresholds by Planning Mode

| Mode | Min Questions | Min Per Category | Checkpoints |
|------|-------------|-----------------|-------------|
| Standard | 150 | 50 per applicable category | Every 30 min |
| Deep/Enterprise | 300+ | 50+ per applicable category | Every 30 min + quarterly |

### How to Present

1. Present in numbered batches of 20-30, grouped by category
2. Use checkbox format for multi-choice
3. After each batch, lock decisions
4. Ask follow-ups on ambiguous answers
5. Dynamic generation: answers unlock follow-up branches
6. Competitor research: when competitors mentioned, research them and generate comparison questions
7. Anti-pattern questions: for each feature, ask what NOT to do
8. Failure mode questions: for each feature, ask what happens when it fails
9. Scale questions: what changes at 10x, 100x users?

### 🛑 Lock-In Checkpoint (Every 30 Minutes)

Display Planning Pulse:
```
PLANNING PULSE — [timestamp]
Decisions locked: [X]
Categories completed: [Y] / [total]
Complexity Score: [score] (threshold: [limit for project size])
Planning velocity: [decisions/minute]
Confidence: [X]%
Suggested action: [lock in / continue / go deeper on category X]
```

Then ask: **"Should we lock in and proceed to suggestions, or should I ask more questions to fill remaining gaps?"**

If user says "ask more" → generate deeper questions.
If user says "lock in" → proceed to Stage 4.

**NEVER auto-proceed. ALWAYS ask.**

### Over-Engineering Detection

Track Complexity Score: `(tables × 2) + (roles × 5) + (integrations × 8) + (features × 1) + (API endpoints × 2) + (real-time features × 10)`

Read `references/checkpoint-protocol.md` for threshold matrix and diminishing returns calculation.

When thresholds hit, **suggest only** — never auto-opt-out: "Complexity Score has reached [X], which is [high/very high] for a [size] project. Would you like to continue planning, or lock in and begin document generation?"

---

## Stage 4: Exhaustive Suggestions

Read `references/suggestion-bank.md` for all 25+ categories with 50+ suggestions each.

### Suggestion Format

Every suggestion includes:
- Description
- Rationale (WHY)
- Effort estimate (hours/days)
- Impact rating (Critical/High/Medium/Low)
- Dependencies
- Category: Include Now / Defer / Reject

### Suggestion Waves

Wave 1: Core architecture + infrastructure
Wave 2: Feature enhancements + patterns
Wave 3: Enterprise patterns + scale planning (read `references/enterprise-architect-protocol.md`)
Wave 4: Future-proofing + competitive gaps

### Anti-Pattern Suggestions

For each category, include "DO NOT" suggestions — things to explicitly avoid and why.

### Security Suggestions (Automatic)

Generate OWASP-aligned security suggestions for every project regardless of what user asks.

### Lock-In Checkpoint

Same format as Stage 3. **"Should we lock in or do you want more suggestions?"**

---

## Stage 5: Gap Analysis, Competitive Research & Risk Assessment

Read `references/gap-analysis.md` for the 15-point gap checklist.
Read `references/competitive-research.md` for the research protocol.

### Competitive Research

When competitors are mentioned, research: feature sets, pricing models, tech stack, API design, UX patterns, review sentiment, backend architecture patterns.

Generate Feature Gap Matrix: your product vs competitors with coverage %.

### Risk Register

For each risky decision: risk description, probability, impact, mitigation, owner.

### Technical Debt Register

For each shortcut: what's being deferred, future cost estimate, trigger to address.

---

## Stage 6: Final Walkthrough

Read `references/final-walkthrough.md` for the protocol.

Before ANY document generation:

1. **Risky Assumption Review**: Walk through every decision flagged as uncertain. Generate targeted questions and suggestions for each.
2. **Completeness Audit**: For each planned feature, verify: database tables, API endpoints, UI pages, permissions, validation, error handling, testing approach.
3. Ask: **"Are there any more gaps to be filled? Any more critical enhancements and suggestions to be made?"**
4. Repeat 2-3 times until the user confirms: "Complete."
5. **Feature Freeze Ceremony**: "This is the scope. Do you confirm nothing more gets added?"

**Only after Feature Freeze does document generation begin.**

---

## Stage 7: Project Document Generation

Read `references/document-templates/` for templates of every document.

### Pre-Generation Gate

Before generating anything, list ALL documents that will be produced:

```
DOCUMENT GENERATION PLAN
========================
The following [X] documents will be generated:

1. MEMORY.md — Running memory for implementation sessions
2. CLAUDE.md — Project context for Claude Code (or CONTEXT.md for other tools)
3. USER-FACING-PRODUCT-CONTEXT.md — Product overview for stakeholders
4. PLAN.md — Phased implementation plan (Phase → Task → Subtask)
5. ARCHITECTURE.md — System architecture with Mermaid diagrams
6. PATTERNS.md — Code patterns with complete examples
7. COMPONENTS.md — Component/module specs with library recommendations
8. Q-S-REFERENCES.md — Complete question & suggestion transcript
9. DEFERRED.md — Deferred features roadmap (Phase 2, 3, future)
10. SESSIONS.md — Session splitting plan with context estimates
11. SECURITY.md — Security posture, threat model, mitigations
12. TESTING-STRATEGY.md — Test pyramid, coverage targets, test plans
13. RUNBOOK.md — Deployment, rollback, incident response procedures
14. API.md — Endpoint inventory, formats, auth, versioning
15. DATA-MODEL.md — Entity relationships, lifecycle, business rules
16. DEPENDENCIES.md — All third-party services with versions, licenses, alternatives
17. COST-ESTIMATE.md — Infrastructure costs at 100/1K/10K users
18. LAUNCH-CHECKLIST.md — Everything that must be true before going live
19. DECISIONS.md — Architectural decision records
20. ROADMAP.md — Timeline with milestones and dependencies
21. BACKEND-MIGRATION.md — Scaling migration plan (if applicable)
22. [Implementation Prompt].md — The comprehensive execution prompt

Total: ~[X] documents, ~[Y] total lines

Generate documents now? (yes/no)
```

**ONLY generate after explicit "yes."** If the user says "yes," ask: **"Are you sure?"** Then generate.

### Document Cross-References

Every document explicitly links to related documents. Every document mentions MEMORY.md update requirement. CLAUDE.md/CONTEXT.md references ALL other documents with snippets.

Read `references/document-templates/` for each template.

---

## Stage 8: Confidence Assessment

Read `references/confidence-assessment.md` for the full protocol.

Rate 0-100%. If below 90%, identify gaps and enhance before delivering.

---

## Stage 9: Execution Prompt

Generate tool-specific execution prompt.

Read `references/tool-configs/` for tool-specific formats:
- Claude Code CLI/Desktop: `.claude/claude.md` + execution prompt
- Cursor: `.cursorrules` + context files
- Lovable: Conversation context document
- Bolt/Replit Agent: Context prompt
- Codex: codex configuration

The execution prompt tells the tool: Read ALL project documents (list every path). Execute the PLAN.md phases in order. MEMORY.md is your brain. Zero mock data. Zero assumptions.

---

## Reference File Index

| File | Purpose | When to Read |
|------|---------|-------------|
| `references/context-gathering.md` | Stage 1 protocol | Start of every session |
| `references/tech-stack-evaluation.md` | Stack assessment | Stage 2 |
| `references/question-bank.md` | 25+ categories, 50+ Qs each | Stage 3 |
| `references/suggestion-bank.md` | 25+ categories, 50+ Ss each | Stage 4 |
| `references/enterprise-architect-protocol.md` | Deep expansion prompt | Stage 4 Wave 3 |
| `references/gap-analysis.md` | 15-point gap checklist | Stage 5 |
| `references/competitive-research.md` | Competitor analysis protocol | Stage 5 |
| `references/checkpoint-protocol.md` | Complexity, velocity, thresholds | Every checkpoint |
| `references/final-walkthrough.md` | Pre-generation audit | Stage 6 |
| `references/confidence-assessment.md` | Rating and enhancement | Stage 8 |
| `references/planning-modes.md` | Mode definitions | Step 0 |
| `references/anti-patterns.md` | What NOT to build | Stages 3-4 |
| `references/launch-checklist.md` | Production readiness | Stage 7 |
| `references/stacks/*.md` | Stack-specific patterns | Stage 2+ |
| `references/document-templates/*.md` | Document templates | Stage 7 |
| `references/tool-configs/*.md` | Tool-specific formats | Stage 9 |

---

## Common Pitfalls

1. **AI tools treat prompts as menus.** Execution prompts must be explicit.
2. **Fast completions are suspicious.** Audit for mock data and empty functions.
3. **Context windows are finite.** MEMORY.md and session splitting are not optional.
4. **Phase 0 reconnaissance is never optional.**
5. **"All of the above" needs priority ordering.**
6. **Multiple doc versions create confusion.** Single source of truth.
7. **Deferred features must be explicit.** Otherwise AI invents them.
8. **Never assume.** Always research. Always ask.
9. **Zero mock data. Zero placeholders.** This skill plans and builds functional production-grade products.
10. **Component libraries matter.** Always research and recommend the best free and paid options. Never default to bland, simple components.
