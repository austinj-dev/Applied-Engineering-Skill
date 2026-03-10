# Final Walkthrough Protocol — Applied Engineering

## Purpose
Last chance to catch gaps before document generation. This is the "measure twice, cut once" step.

## Steps

### 1. Risky Assumption Review
Walk through EVERY decision flagged as uncertain or dependent on codebase state.
For each: generate targeted questions and suggestions.

### 2. Completeness Audit
For EACH planned feature verify it has:
- [ ] Database tables defined
- [ ] API endpoints defined
- [ ] UI pages/components defined
- [ ] Permission model defined
- [ ] Validation rules defined
- [ ] Error handling defined
- [ ] Testing approach defined
If any are missing, flag and ask.

### 3. Cross-Feature Dependency Check
Verify no circular dependencies. Verify shared data models are consistent.

### 4. "Are There Any More Gaps?" (Repeat 2-3 times)
Ask: "Are there any more gaps to be filled? Any more critical enhancements and suggestions?"
Continue until user confirms: "Complete."

### 5. Feature Freeze Ceremony
Present final scope. Get explicit confirmation. Then — and only then — proceed to document generation.
