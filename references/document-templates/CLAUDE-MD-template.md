# [PROJECT] — Project Context

## Project Overview
[1-2 paragraphs: what this is, who it's for, core problem solved]

## Tech Stack
| Layer | Technology | Version |
|-------|-----------|---------|
| Frontend | [framework] | [version] |
| UI Library | [library] | [version] |
| Backend | [framework] | [version] |
| Database | [database] | [version] |
| Auth | [provider] | |
| Deployment | [target] | |

## Architecture Summary
[High-level: monolith vs microservices, key architectural patterns, data flow]

## Directory Structure
```
[Annotated file tree — key directories with purpose]
```

## Conventions
- Naming: [conventions]
- Files: [organization pattern]
- Imports: [pattern]
- Error handling: [pattern — see PATTERNS.md for full examples]
- State management: [approach]

## Commands
```bash
# Dev server
[command]
# Production build
[command]
# Type check
[command]
# Lint
[command]
# Test
[command]
# Database migrations
[command]
# Seed data
[command]
```

## Project Documents — READ ALL BEFORE CODING
Every document below is part of this project specification. Read each one completely — no skimming, no skipping sections.

| Document | Purpose | Key Content |
|----------|---------|-------------|
| MEMORY.md | Implementation status | Current phase, files created, known issues |
| PLAN.md | What to build and in what order | Phases, tasks, gates, session boundaries |
| PATTERNS.md | How to write code | Hook patterns, component patterns, API patterns (WITH CODE EXAMPLES) |
| COMPONENTS.md | Which components to use | Specific library components per UI element |
| ARCHITECTURE.md | System design | Mermaid diagrams, data flow, relationships |
| SECURITY.md | Security requirements | Auth model, OWASP mitigations, headers |
| API.md | API design | Endpoints, formats, auth, rate limits |
| DATA-MODEL.md | Database design | Entities, relationships, business rules |
| DEFERRED.md | What NOT to build | Features excluded from this implementation |
| SESSIONS.md | Session boundaries | Which phases in which session |

**After every phase: UPDATE MEMORY.md.**
**Before implementing anything: CHECK DEFERRED.md to ensure it's in scope.**

## Critical Rules
1. MEMORY.md is your brain. Create first. Read before every phase. Update after.
2. Zero mock data. Zero placeholders. Zero empty function bodies.
3. Follow PATTERNS.md exactly — do not invent new patterns.
4. Use components specified in COMPONENTS.md — do not substitute.
5. Every phase has a GATE in PLAN.md. Verify before proceeding.
6. If something isn't in PLAN.md or is in DEFERRED.md, do not build it.
