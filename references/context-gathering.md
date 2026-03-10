# Context Gathering — Applied Engineering

## Before Generating a Single Question

### Ask the User
- Product name, purpose, target users
- Tech stack (or "help me choose")
- Existing codebase? State?
- Existing docs? PRDs? Architecture?
- Scope: new build, feature add, production readiness?
- Ecosystem: other products sharing DB/auth?
- Billing model?
- Permission/role model?
- Integrations needed?
- Industry packs / verticals?
- Timeline and budget?
- Solo or team?
- AI development tool being used?

### Read Everything Provided
- Product docs, PRDs, specs
- Existing CLAUDE.md, README, architecture docs
- Past conversation history (use conversation_search)
- Uploaded files

### If Existing Codebase
Perform EXTENSIVE analysis. Read EVERY file. Skip NOTHING.
```bash
# Structure
find . -maxdepth 4 -type d | grep -v node_modules | sort
# Package files
cat package.json requirements.txt Cargo.toml go.mod Gemfile 2>/dev/null
# Config
cat tsconfig.json next.config.* vite.config.* .eslintrc* 2>/dev/null
# All pages/routes
find . -name "page.tsx" -o -name "views.py" -o -name "*.controller.*" | sort
# Database
find . -path "*/migrations/*" -type f | sort
# Components
find . -name "*.tsx" -o -name "*.vue" -o -name "*.svelte" | wc -l
```

### Research
- Tech stack compatibility
- Deployment target limitations
- Template analysis (if using starter)
- SDK version compatibility

**Do NOT proceed to Stage 2 until you have a clear mental model.**
