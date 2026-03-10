# Gap Analysis — Applied Engineering (15-Point Checklist)

## Run After Stage 4 (Suggestions), Before Stage 6 (Final Walkthrough)

### Gap 1: Deployment Architecture
Check: Is deployment fully specified? Does framework run on target without limitations?
Research: Exact deployment path. Document config files needed.

### Gap 2: Template/Starter Specifics
Check: If using template, what does it ship with? Conflicts with plan?

### Gap 3: Email Infrastructure
Check: Provider, templates, env vars, bounce handling, unsubscribe?

### Gap 4: Webhook Handlers
Check: All inbound webhooks defined? Signature validation? Idempotency?

### Gap 5: Middleware
Check: CORS, security headers, CSP, auth validation, rate limiting?

### Gap 6: SDK/Runtime Compatibility
Check: AI SDK with deployment? DB client with edge? Version pins?

### Gap 7: Ecosystem Scope
Check: Product boundaries clear? What's in vs out?

### Gap 8: API Design
Check: Versioning? Pagination? Error format? Rate limit headers?

### Gap 9: Database Functions & Triggers
Check: Atomic operations? Timestamp triggers? Rate limit checks?

### Gap 10: Migration Ordering
Check: Dependency chain explicit? No FK violations in order?

### Gap 11: Observability (NEW)
Check: Logging? Error tracking? Monitoring? Health checks? Alerting?

### Gap 12: Caching Strategy (NEW)
Check: What's cached? TTL? Invalidation? CDN? Browser cache headers?

### Gap 13: Background Jobs (NEW)
Check: Queue system? Job types? Retry? Dead letter? Monitoring?

### Gap 14: Cost Projection (NEW)
Check: Estimated monthly at 3 scale tiers? Service costs identified?

### Gap 15: Legal & Compliance (NEW)
Check: Privacy policy? Terms? Cookie consent? GDPR? Data processing?

## For Each Gap Found
```
### Gap [N]: [Name]
**Problem**: [What's missing]
**Research**: [What was found]
**Fix**: [What's being added]
**Applied**: ✅
```
