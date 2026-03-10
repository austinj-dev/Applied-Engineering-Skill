# Question Bank — Applied Engineering

## Usage Rules

- **Per-category minimum**: 50 questions in Standard mode. 75+ in Deep/Enterprise.
- **Dynamic generation**: After answers, generate follow-ups specific to responses.
- **Every category ends with**: "What else in this area haven't I asked about?"
- **Lock-In Checkpoint**: After every 2 categories or 30 minutes.
- **Competitor questions**: When competitors mentioned, research and generate comparison questions.
- **Anti-pattern questions**: For each feature, ask what NOT to do.
- **Failure mode questions**: For each feature, ask what happens when it fails.
- **Scale questions**: What changes at 10x, 100x users?

---

## Category 1: Product Identity & Vision (60 questions)

1. Product name?
2. One-line elevator pitch?
3. Primary target users (roles, industries, demographics)?
4. Secondary users?
5. Core problem solved?
6. What happens if users DON'T have this? (pain without solution)
7. B2B, B2C, B2B2C, or internal tool?
8. Standalone product or ecosystem?
9. If ecosystem: other products? Shared auth? Shared DB?
10. How do users access it? (subdomain, path, separate app, embedded)
11. Relationship to competitors?
12. Name 3-5 competing products.
13. Key differentiator vs every competitor?
14. Pricing model? (freemium, flat, tiered, usage-based, per-seat)
15. Free tier? What's included?
16. Monetization timeline?
17. Target market? (SMB, mid-market, enterprise, consumer)
18. MVP vs full vision?
19. If you could only ship 5 features, which 5?
20. Launch date or deadline?
21. External deadlines? (investor demo, conference, contract)
22. Infrastructure budget?
23. Venture-backed, bootstrapped, or side project?
24. Single-tenant or multi-tenant?
25. Multi-tenant isolation strategy?
26. White-labeling needed?
27. Industry-specific customization?
28. How many verticals at launch?
29. Existing branding? (colors, fonts, logo)
30. Domain/URL structure?
31. Existing user base to migrate?
32. Data migration requirements?
33. Expected user count at launch? 6mo? 12mo?
34. Geographic regions?
35. Multi-language/i18n?
36. Accessibility requirements (WCAG level)?
37. Compliance? (GDPR, CCPA, HIPAA, SOC2, PCI)
38. Beta testing plan?
39. Who maintains after launch?
40. Support model? (email, chat, phone, self-service)
41. Key analytics/KPIs?
42. Success metrics at 30d? 90d? 1yr?
43. Brand guide or design system?
44. Marketing/landing page needed?
45. Blog or CMS needed?
46. Documentation needed? (user docs, API docs)
47. Development methodology?
48. Release management? (continuous, scheduled)
49. Staging environment?
50. Risk tolerance for initial launch?
51. Revenue model beyond subscriptions? (marketplace, transactions, add-ons)
52. Partner/affiliate program planned?
53. API as a product? (developers building on your platform)
54. Embed/widget capability? (your product embedded in other sites)
55. Notification strategy? (email frequency, in-app, push, SMS)
56. Data ownership model? (who owns the data, export rights)
57. SLA commitments at launch?
58. Uptime target?
59. Customer onboarding approach? (self-serve, guided, white-glove)
60. What else about the product vision haven't I asked?

---

## Category 2: Tech Stack (55 questions)

1. Frontend framework + version?
2. UI component library?
3. CSS approach?
4. State management?
5. Form management?
6. Validation library?
7. Backend framework?
8. Runtime?
9. Database?
10. Database hosting?
11. ORM/query builder?
12. Auth system?
13. Deployment target?
14. Edge/serverless vs traditional server?
15. Package manager?
16. Monorepo or polyrepo?
17. If monorepo: which tool?
18. TypeScript or JavaScript? Strict mode?
19. Test framework?
20. Linter?
21. Formatter?
22. API architecture?
23. Real-time technology?
24. File storage?
25. CDN?
26. Email provider?
27. Search engine?
28. Background jobs?
29. Caching?
30. Analytics?
31. Error tracking?
32. Monitoring?
33. CI/CD?
34. Feature flags?
35. Payment processing?
36. AI/ML providers?
37. AI SDK?
38. Vector database?
39. CMS?
40. Mobile approach?
41. Desktop approach?
42. API documentation?
43. Secrets management?
44. DNS/Domain?
45. SSL/TLS?
46. Logging?
47. Image processing?
48. PDF generation?
49. Charts/visualization?
50. Rich text editor?
51. Date/time library?
52. Internationalization?
53. Queue/job system?
54. Rate limiting library?
55. What else about the stack haven't I considered?

**After answers: ALWAYS suggest alternative stack with reasoning. Ask one final time.**

---

## Category 3: Database Architecture (55 questions)

1. Shared DB or separate per service?
2. Table naming convention?
3. Column naming convention?
4. Primary key type? (UUID v4, v7, CUID, serial)
5. Soft deletes or hard deletes?
6. Soft delete column name?
7. Audit trail requirements?
8. Timestamp columns on every table?
9. Who updates updated_at? (trigger or app)
10. Multi-tenancy approach?
11. Organization/tenant model?
12. User multi-org membership?
13. JSONB vs strict columns?
14. When to use JSONB?
15. Full-text search approach?
16. Vector embeddings needed?
17. File storage approach?
18. File references: URL column or attachments table?
19. Migration strategy?
20. Migration tooling?
21. Seed data strategy? (dev, test, demo, staging)
22. Initial accounts to seed?
23. Initial organizations to seed?
24. Enum columns vs lookup tables vs CHECK?
25. Connection pooling?
26. Read replicas needed?
27. Database branching?
28. Backup strategy + frequency?
29. Point-in-time recovery?
30. Data retention policy?
31. GDPR right-to-erasure?
32. Data export capability?
33. Database extensions needed?
34. RLS strategy?
35. RLS policy pattern?
36. Database functions needed?
37. Database triggers needed?
38. Materialized views?
39. Partitioning strategy?
40. Index strategy?
41. Cross-database references?
42. Table prefix per domain?
43. Junction table naming?
44. Polymorphic associations?
45. Entity versioning?
46. Archival strategy?
47. DB-level vs app-level validation?
48. Custom types/domains?
49. Schema organization?
50. Database documentation approach?
51. Most complex relationships? Describe them.
52. Estimated row counts for largest tables at 12 months?
53. Time-series data needs? (metrics, logs, events)
54. Geographic/spatial data needs? (PostGIS)
55. What else about the database haven't I considered?

---

## Category 4: Auth & Permissions (55 questions)

1. Auth provider?
2. Login methods?
3. OAuth providers?
4. SSO/SAML support?
5. 2FA/MFA support?
6. Password requirements?
7. Password reset flow?
8. Email verification?
9. Role model? (RBAC, ABAC)
10. All roles with descriptions?
11. Permission granularity?
12. Role hierarchy?
13. Custom roles per org?
14. Custom permissions per role?
15. Multi-org support?
16. Org-scoped roles?
17. Default role for new users?
18. Invitation system?
19. Invitation expiration?
20. Self-registration?
21. Session management?
22. Session duration?
23. Multi-device sessions?
24. Remember me?
25. Account lockout?
26. IP rate limiting on auth?
27. Geo-blocking?
28. Admin impersonation?
29. API key strategy?
30. API key scoping?
31. Webhook authentication?
32. Portal auth model?
33. Portal registration?
34. Portal roles?
35. Guest access?
36. Anonymous usage?
37. Account deletion/deactivation?
38. Data export on deletion?
39. Cross-product auth?
40. Service-to-service auth?
41. Middleware auth strategy?
42. Auth error handling? (401 vs 403)
43. Token refresh strategy?
44. CORS for auth?
45. Cookie security flags?
46. CSRF protection?
47. Bot protection?
48. Auth event logging?
49. Auth compliance requirements?
50. Auth migration from existing?
51. Device trust / device management?
52. Session revocation (admin force-logout)?
53. Passwordless options? (passkeys, WebAuthn)
54. Social login data: what profile data to store?
55. What else about auth haven't I considered?

---

## Category 5: Feature Scope (50+ per feature area — dynamic)

*Generate 50+ questions per feature area the user describes. Use the per-feature template from the skill. Include competitor-inspired questions, anti-pattern questions, failure mode questions, and scale questions.*

---

## Category 6: UI/UX & Component Library (60 questions)

1. Dark mode?
2. Default theme?
3. System preference detection?
4. Responsive design approach?
5. Target breakpoints?
6. Mobile-specific layouts?
7. Component library choice? Why?
8. Have you evaluated alternatives?
9. Which specific data table component? (sorting, filtering, pagination, selection, inline edit, column resize, virtualization)
10. Which form components? (multi-step, conditional fields, validation display, file upload)
11. Which navigation components? (sidebar, breadcrumbs, tabs, command palette)
12. Which modal/dialog components?
13. Which date/time picker? (range, recurring, timezone)
14. Which rich text editor?
15. Which file upload component? (drag-drop, multi, progress, preview)
16. Which chart/visualization library?
17. Which notification/toast system?
18. Which command palette/search?
19. Are there paid libraries that would be better? (research and suggest)
20. Are there free alternatives more feature-rich? (research and suggest)
21. Icon library?
22. Font choices?
23. Animation library?
24. Brand colors?
25. Spacing system?
26. Border radius tokens?
27. Shadow tokens?
28. Typography scale?
29. Layout approach?
30. Sidebar behavior?
31. Header behavior?
32. Breadcrumb strategy?
33. Page title strategy?
34. Keyboard shortcuts?
35. Drag-and-drop interactions?
36. Onboarding flow design?
37. Empty state design?
38. Loading state design?
39. Error state design?
40. Toast design? (position, duration, actions, stacking)
41. Confirmation dialog patterns?
42. Form layout?
43. Form validation display?
44. Table design? (striped, bordered, compact, expandable)
45. Card design?
46. Modal vs drawer vs full-page?
47. Detail view layout?
48. Dashboard layout?
49. Print stylesheet?
50. PDF export design?
51. Email template design?
52. Portal design?
53. Landing page design?
54. WCAG level target?
55. Screen reader testing?
56. Keyboard navigation?
57. Focus management?
58. Color contrast?
59. ARIA strategy?
60. What UI patterns in competitors do you admire? Which do you hate?

---

## Category 7: AI / ML (55 questions)

1. AI/ML features needed? Describe each.
2. Which AI providers?
3. Default model per provider?
4. BYOK support?
5. Streaming responses?
6. Multi-agent or single agent?
7. Agent modes/personas?
8. Memory system? (short-term, long-term, knowledge base)
9. RAG/knowledge base?
10. Document types supported for RAG?
11. Chunking strategy? (size, overlap, method)
12. Vector embedding model?
13. Vector storage?
14. Tool/function calling?
15. What tools available to AI?
16. Safety/content filtering?
17. Cost management?
18. Usage limits per tier?
19. Free tier AI approach? (free models, limited usage, no AI)
20. Fallback chain? (BYOK → paid → free providers)
21. Model routing? (simple→cheap, complex→capable)
22. Conversation history storage?
23. Conversation branching/forking?
24. File/image input support?
25. Code execution/interpreter?
26. Web search integration?
27. Citation/source tracking?
28. AI-generated content labeling?
29. Approval gates for AI actions?
30. Auto-execute vs confirm-first vs explicit-approval?
31. AI widget for external embedding?
32. AI in portals?
33. Custom prompts/system prompts per feature?
34. Prompt template management?
35. A/B testing for prompts?
36. AI analytics? (usage, cost, quality, latency)
37. Feedback collection on AI responses?
38. AI moderation/review?
39. Batch/bulk AI operations?
40. Scheduled AI tasks?
41. AI-powered search?
42. AI-powered categorization/tagging?
43. AI-powered summarization?
44. AI-powered translation?
45. AI-powered data extraction?
46. Custom model fine-tuning?
47. Local/self-hosted model support?
48. AI API for external developers?
49. Rate limiting per AI endpoint?
50. AI error handling and graceful degradation?
51. What happens when all AI providers are down?
52. AI data privacy (where does data go)?
53. AI compliance (GDPR for AI processing)?
54. Which competitor's AI features do you admire?
55. What else about AI haven't I considered?

---

## Category 8: Subscription & Billing (55 questions)

1. What tiers exist with pricing?
2. Features gated per tier?
3. Limits per tier? (users, storage, API calls)
4. Billing provider?
5. Free tier?
6. Trial period? Length? Payment upfront?
7. Annual vs monthly? Discount?
8. Usage-based or flat?
9. Add-on pricing?
10. Per-seat pricing?
11. Stripe webhook events to handle?
12. Subscription lifecycle? (create, upgrade, downgrade, cancel, reactivate)
13. Proration on plan change?
14. Cancellation flow? (immediate vs end-of-period)
15. Refund policy?
16. Invoice generation?
17. Tax handling? (Stripe Tax, manual)
18. Currency support?
19. Payment methods? (card, ACH, wire, PayPal)
20. Failed payment handling? (retry, grace period, suspension)
21. Dunning emails?
22. Usage metering implementation?
23. Usage alerts? (80%, 90%, 100% of limit)
24. Overage handling? (hard limit, soft limit, charge overage)
25. Subscription analytics? (MRR, ARR, churn, LTV)
26. Coupon/discount system?
27. Referral program?
28. Grandfathering for price changes?
29. Enterprise custom pricing?
30. Self-serve vs sales-led for enterprise?
31. Billing portal for customers?
32. Subscription API for programmatic access?
33. Multi-currency support?
34. Volume discounts?
35. Commitment discounts? (annual commitment)
36. Free-to-paid conversion tracking?
37. Expansion revenue tracking?
38. Net revenue retention calculation?
39. Billing event audit logging?
40. PCI compliance approach?
41. Checkout page design? (hosted, embedded, custom)
42. Pricing page design? (comparison table, calculator)
43. Upgrade prompts strategy? (where, when, how)
44. Downgrade friction? (what do they lose?)
45. Cancellation survey?
46. Win-back campaigns?
47. Payment failure notification UX?
48. Invoice customization? (logo, address, tax ID)
49. Multi-org billing? (per org or per user across orgs)
50. Marketplace/add-on billing? (revenue share)
51. Billing migration from existing system?
52. Free tier to paid conversion funnel?
53. What billing UX in competitors do you like?
54. What billing anti-patterns should we avoid?
55. What else about billing haven't I considered?

---

## Category 9: Integrations (55 questions)

1. What third-party services integrate?
2. OAuth flows needed? Which providers?
3. Inbound webhooks? (from which services, event types)
4. Outbound webhooks? (to where, event types)
5. Webhook signature verification?
6. Webhook retry/failure handling?
7. Webhook idempotency?
8. Email integration? (send, receive, parse)
9. Calendar integration? (Google Cal, Outlook, CalDAV)
10. Two-way calendar sync?
11. Payment integration? (Stripe, PayPal, Plaid)
12. Accounting integration? (QuickBooks, Xero, FreshBooks)
13. Communication? (Twilio SMS, voice, WhatsApp)
14. Slack/Teams integration?
15. CRM integration? (if building non-CRM)
16. Project management integration?
17. Shipping integration?
18. Social media integration?
19. Analytics integration?
20. Storage/file integration? (Google Drive, Dropbox, OneDrive)
21. Zapier/Make/n8n connection?
22. REST API for external developers?
23. GraphQL API?
24. API rate limiting per integration?
25. API key management for partners?
26. SDK generation? (JS, Python, Ruby, Go)
27. Integration marketplace?
28. Custom integration framework?
29. iPaaS readiness?
30. SSO provider integration?
31. Import capabilities? (CSV, Excel, API, migration tools)
32. Export capabilities? (CSV, PDF, Excel, API, bulk)
33. Data sync frequency? (real-time, hourly, daily)
34. Conflict resolution for synced data?
35. Integration monitoring/health dashboard?
36. Integration error handling and retry?
37. Integration logging and audit trail?
38. OAuth token refresh handling?
39. Integration testing strategy?
40. Sandbox/test environments for integrations?
41. Integration documentation for partners?
42. Rate limit handling when calling external APIs?
43. Circuit breaker for external service calls?
44. Fallback behavior when integration is down?
45. Data mapping between systems?
46. Field mapping configuration UI?
47. Batch/bulk API operations?
48. Pagination handling for external APIs?
49. Integration versioning?
50. Deprecation strategy for old integrations?
51. White-label integration support?
52. Embedded integration (your product in theirs)?
53. Native mobile deep linking?
54. Browser extension integration?
55. What else about integrations haven't I considered?

---

## Category 10: Deployment & Infrastructure (55 questions)

1. Deployment target?
2. CI/CD pipeline?
3. Environments? (dev, staging, production)
4. Preview deployments? (per PR)
5. Deployment strategy? (blue-green, canary, rolling, recreate)
6. Rollback procedure?
7. Infrastructure as code?
8. Container strategy? (Docker, Kubernetes, serverless)
9. Edge computing needs?
10. Multi-region deployment?
11. CDN configuration?
12. SSL/TLS certificate management?
13. DNS management?
14. Domain strategy? (custom domains per tenant?)
15. Load balancing?
16. Auto-scaling rules?
17. Resource limits? (CPU, memory, bandwidth)
18. Cost monitoring and alerts?
19. Uptime monitoring?
20. Health check endpoints?
21. Liveness vs readiness probes?
22. Log aggregation?
23. Log retention policy?
24. Secret management in CI/CD?
25. Environment variable strategy?
26. Database migration in CI/CD?
27. Seed data in CI/CD?
28. Build caching?
29. Artifact storage?
30. Dependency caching?
31. Build time target?
32. Deploy time target?
33. Zero-downtime deployment?
34. Database backup in deployment pipeline?
35. Smoke tests post-deploy?
36. Canary analysis?
37. Feature flag-controlled rollout?
38. Hotfix process?
39. Emergency rollback process?
40. On-call rotation?
41. Incident response playbook?
42. Post-mortem process?
43. SLA monitoring?
44. Error budget tracking?
45. Capacity planning?
46. Cost optimization strategy?
47. Reserved instances/committed use?
48. Spot/preemptible instances?
49. Cold start mitigation? (for serverless)
50. Connection warming?
51. Static asset optimization?
52. Image/media CDN strategy?
53. Geographic routing?
54. DDoS protection?
55. What else about infrastructure haven't I considered?

---

## Category 11: Security (60 questions — OWASP-aligned)

1. OWASP Top 10 2025 assessment planned?
2. A01 Broken Access Control: IDOR testing planned?
3. Horizontal privilege escalation prevention?
4. Vertical privilege escalation prevention?
5. Force browsing prevention?
6. A02 Security Misconfiguration: security headers configured?
7. HSTS, CSP, X-Frame-Options, X-Content-Type-Options?
8. Server info leakage prevention?
9. Debug mode disabled in production?
10. Default credentials removed?
11. Directory listing disabled?
12. A05 Injection: XSS prevention strategy?
13. SQL injection prevention?
14. Input sanitization approach?
15. Output encoding approach?
16. Content Security Policy?
17. A04 Cryptographic Failures: encryption at rest?
18. Encryption in transit? (TLS 1.2+)
19. Key management strategy?
20. Password hashing algorithm? (bcrypt, argon2)
21. Sensitive data identification?
22. PII handling procedures?
23. A03 Supply Chain: dependency scanning?
24. Lock file enforcement?
25. NPM/pip audit in CI?
26. SBOM generation?
27. License compliance checking?
28. A06 Insecure Design: threat modeling?
29. Security requirements in each feature?
30. Abuse case analysis?
31. A07 Auth Failures: credential stuffing prevention?
32. Brute force protection?
33. Session fixation prevention?
34. Token leakage prevention?
35. A08 Data Integrity Failures: CI/CD pipeline security?
36. Code signing?
37. Deployment verification?
38. A09 Logging Failures: security event logging?
39. Audit log immutability?
40. Log access controls?
41. SIEM integration?
42. A10 SSRF: outbound request filtering?
43. Internal network access prevention?
44. URL validation?
45. Secrets in source code prevention?
46. Secret scanning in CI?
47. Environment variable validation?
48. API authentication on every route?
49. Rate limiting strategy?
50. CORS configuration?
51. Cookie security attributes?
52. CSRF protection?
53. File upload security? (type validation, size limits, virus scanning)
54. Subdomain takeover prevention?
55. DNS security? (DNSSEC, CAA records)
56. Penetration testing planned?
57. Bug bounty program?
58. Security incident response plan?
59. Vulnerability disclosure policy?
60. What else about security haven't I considered?

---

## Category 12: Observability & Monitoring (50 questions)

1. Structured logging format? (JSON, plaintext)
2. Log levels strategy? (debug, info, warn, error, fatal)
3. Correlation ID implementation?
4. Request/response logging?
5. PII redaction in logs?
6. Log aggregation service?
7. Log retention period?
8. Log search and analysis?
9. Error tracking service?
10. Error grouping strategy?
11. Error alert thresholds?
12. Source map upload for error tracking?
13. User context in errors?
14. Breadcrumb logging?
15. Uptime monitoring service?
16. Monitoring frequency?
17. Health check endpoint design?
18. Liveness check vs readiness check?
19. Synthetic monitoring? (critical user paths)
20. Real User Monitoring (RUM)?
21. Core Web Vitals tracking?
22. Performance budgets per route?
23. Alerting rules?
24. Alert channels? (email, Slack, PagerDuty, SMS)
25. Alert escalation?
26. On-call rotation?
27. SLI definitions? (latency, error rate, throughput)
28. SLO targets?
29. Error budget tracking?
30. Dashboard design? (ops dashboard, business dashboard)
31. Database monitoring? (slow queries, connections, replication lag)
32. API latency tracking?
33. Background job monitoring?
34. Queue depth monitoring?
35. Cache hit/miss rates?
36. Third-party service health tracking?
37. Dependency health dashboard?
38. Cost monitoring per service?
39. Resource utilization monitoring?
40. Anomaly detection?
41. Incident response automation?
42. Post-mortem template?
43. Status page?
44. Status page integration? (Statuspage.io, Instatus, custom)
45. Downtime notification to users?
46. Scheduled maintenance windows?
47. Deployment tracking in monitoring?
48. Feature flag change tracking?
49. User-facing error reporting? (report a bug button)
50. What else about observability haven't I considered?

---

## Category 13: Error Handling & Recovery (50 questions)

1. Error boundary strategy? (React error boundaries, Vue errorCaptured, etc.)
2. Global error handler?
3. Per-route error pages?
4. 404 page design?
5. 500 page design?
6. Network error handling?
7. Timeout handling?
8. Retry logic strategy? (exponential backoff, max retries)
9. Circuit breaker implementation?
10. Graceful degradation approach?
11. Offline detection and handling?
12. Reconnection strategy?
13. Stale data handling?
14. Optimistic update rollback?
15. Form submission error recovery?
16. File upload error recovery? (resume upload)
17. Payment failure recovery?
18. Auth error recovery? (token expired, session invalid)
19. API error response format?
20. Error codes taxonomy?
21. User-facing error messages (tone, format)?
22. Technical vs user-friendly error separation?
23. Error message localization?
24. Help links in error messages?
25. Retry actions in error UI?
26. Contact support from error page?
27. Error reporting (user reports a bug)?
28. Automatic error screenshot?
29. Error context collection? (URL, user, browser, session)
30. Database error handling? (constraint violations, deadlocks)
31. Migration error handling?
32. Background job error handling?
33. Webhook delivery failure handling?
34. Email sending failure handling?
35. Third-party API failure handling?
36. Rate limit error handling? (429 responses)
37. Storage quota exceeded handling?
38. Browser compatibility errors?
39. JavaScript runtime error handling?
40. Memory pressure handling?
41. Large payload handling?
42. Malformed data handling?
43. Concurrent modification conflict handling?
44. Data corruption detection and recovery?
45. Backup restoration testing?
46. Disaster recovery testing?
47. Chaos engineering approach?
48. Error handling documentation?
49. Error handling testing strategy?
50. What else about error handling haven't I considered?

---

## Category 14: Caching Strategy (50 questions)

1. What data to cache?
2. Cache provider? (Redis, Upstash, in-memory, CDN)
3. TTL per resource type?
4. Cache invalidation strategy?
5. Stale-while-revalidate?
6. Cache warming strategy?
7. CDN caching for static assets?
8. CDN caching for API responses?
9. Browser caching headers?
10. Service worker caching? (for PWA)
11. Database query caching?
12. ORM-level caching?
13. Application-level caching?
14. Session caching?
15. Full-page caching?
16. Fragment caching?
17. API response caching?
18. Computed value caching?
19. Search result caching?
20. Image/media caching?
21. Cache key naming convention?
22. Cache size limits?
23. Cache eviction policy? (LRU, LFU, TTL)
24. Multi-tier caching? (L1 memory, L2 Redis, L3 CDN)
25. Cache consistency across instances?
26. Cache stampede prevention?
27. Cache bypass for authenticated data?
28. Cache per-tenant isolation?
29. Cache debugging/inspection?
30. Cache hit/miss monitoring?
31. Cache performance impact measurement?
32. Lazy loading vs eager caching?
33. Write-through vs write-behind?
34. Read-through caching?
35. Cache preloading on deploy?
36. Cache clear on deploy?
37. Feature flag for cache bypass?
38. A/B test cache isolation?
39. Real-time data: never cache vs short TTL?
40. User-specific vs shared cache?
41. Geographic cache distribution?
42. Cache serialization format?
43. Cache compression?
44. Cache encryption for sensitive data?
45. Cache failover strategy?
46. Cache capacity planning?
47. Cache cost estimation?
48. Cache testing strategy?
49. Cache documentation?
50. What else about caching haven't I considered?

---

## Category 15: Search Architecture (50 questions)

1. Search engine choice?
2. What's searchable? (entities, content, files)
3. Global search (cross-module)?
4. Module-specific search?
5. Full-text search?
6. Fuzzy matching?
7. Autocomplete/typeahead?
8. Search suggestions?
9. Recent searches?
10. Saved searches?
11. Search filters? (faceted)
12. Filter UI design?
13. Sort options in search?
14. Search result ranking algorithm?
15. Search result highlighting?
16. Search result grouping? (by type, by module)
17. Search analytics? (popular queries, zero-result queries)
18. Search indexing strategy?
19. Real-time indexing vs batch?
20. Index update on CRUD operations?
21. Search across relationships?
22. Search permission scoping?
23. Multi-tenant search isolation?
24. Search pagination?
25. Search performance targets?
26. Search result caching?
27. Synonym handling?
28. Stop word handling?
29. Language-specific search?
30. Search within file contents? (PDF, DOCX)
31. Command palette integration?
32. Keyboard shortcut to search? (Cmd+K, /)
33. Search URL format? (shareable search links)
34. Advanced search syntax? (operators, boolean)
35. Natural language search?
36. AI-powered search?
37. Vector/semantic search?
38. Hybrid search? (keyword + semantic)
39. Search API for external access?
40. Search rate limiting?
41. Search result click tracking?
42. Search A/B testing?
43. Zero-result page design?
44. Search error handling?
45. Search index backup?
46. Search index rebuild strategy?
47. Search migration strategy?
48. Search cost per query?
49. Search scalability plan?
50. What else about search haven't I considered?

---

## Categories 16-30 (50+ questions each)

## Category 16: File & Media Handling (50 Qs)
Upload limits, storage provider, CDN delivery, image processing pipeline, virus scanning, signed URLs, video handling, document preview, bulk upload, drag-drop, progress tracking, resume upload, file versioning, file sharing, access control per file, storage quotas per tier, file type validation, thumbnail generation, responsive images, lazy loading images, WebP/AVIF conversion, metadata extraction, EXIF stripping for privacy, file deduplication, trash/recovery, permanent deletion, file search, file tagging, file organization (folders, tags, collections), S3-compatible API, presigned URLs, multipart upload, chunk upload for large files, bandwidth optimization, cost per GB estimation.

## Category 17: Background Jobs & Queues (50 Qs)
Job types, queue system, retry strategy (exponential backoff, max retries, dead letter), monitoring/alerting, scheduled/cron jobs, webhook processing, email sending, report generation, data import/export, cleanup jobs, cache warming, search indexing, notification delivery, billing/metering, analytics aggregation, AI processing, file processing, video transcoding, PDF generation, data migration, job priorities, job cancellation, job progress tracking, job result storage, job dependencies/chains, fan-out/fan-in, rate-limited jobs, tenant-isolated queues, job logging, job replay, idempotency, concurrency limits, worker scaling, job timeout, long-running job handling.

## Category 18: Real-time Features (50 Qs)
Technology choice, connection management, reconnection strategy, presence indicators, typing indicators, live cursors, real-time notifications, live data updates, collaborative editing, live chat, live dashboards/metrics, event streaming, pub/sub channels, channel authorization, message ordering, at-most-once vs at-least-once delivery, offline queue, state synchronization, conflict resolution, bandwidth optimization, mobile real-time (battery/data), scalability per connection, connection limits per tier, real-time debugging, event replay, real-time analytics.

## Category 19: Analytics & Telemetry (50 Qs)
Event taxonomy, naming convention, required properties per event, funnels, KPI dashboards, user behavior tracking, feature usage tracking, A/B testing framework, conversion tracking, cohort analysis, retention analysis, churn prediction, revenue analytics, performance analytics, error rate analytics, search analytics, AI usage analytics, integration usage, custom reports, scheduled reports, data export, privacy-compliant analytics, anonymization, consent tracking, server-side vs client-side tracking.

## Category 20: Data Architecture (50 Qs)
Data lifecycle, archival strategy, ETL/ELT pipelines, reporting database, data warehouse, event sourcing evaluation, CQRS evaluation, eventual consistency areas, data lake, data catalog, data lineage, data quality checks, data validation rules, data transformation, data aggregation, materialized views, denormalization strategy, read models, write models, data versioning, data migration paths, backward compatibility.

## Category 21: Testing Architecture (50 Qs)
Test pyramid strategy, unit test coverage targets, integration test scope, E2E test scenarios, load testing plan, security testing plan, accessibility testing plan, visual regression testing, contract testing, test data management, test environment management, CI test pipeline, test parallelization, flaky test handling, test reporting, test monitoring, mutation testing, property-based testing, snapshot testing, API testing, database testing, email testing, webhook testing, real-time testing, mobile testing, cross-browser testing, performance testing, chaos testing, canary testing, smoke testing.

## Category 22: DevOps & CI/CD (50 Qs)
Build pipeline, test pipeline, deploy pipeline, environment promotion, secret management, infrastructure as code, container registry, deployment strategy, rollback automation, preview environments, branch strategy, merge strategy, code review automation, dependency updates automation, security scanning in CI, license scanning, SBOM generation, build caching, artifact management, deployment notifications, deploy locks, concurrent deploy prevention, database migration in CI, seed data in CI.

## Category 23: Legal & Compliance (50 Qs)
GDPR requirements, CCPA requirements, HIPAA requirements (if applicable), SOC 2 readiness, PCI DSS (if payment), cookie consent implementation, privacy policy content, terms of service content, data processing agreements, data residency requirements, age verification, COPPA (if children), accessibility compliance (ADA/EAA), open source license compliance, third-party data sharing agreements, data breach notification plan, right to erasure implementation, right to portability, consent management, audit trail for compliance, data retention schedules, cross-border data transfer.

## Category 24: Cost & Budget (50 Qs)
Infrastructure cost per 100/1K/10K users, database hosting cost, file storage cost, CDN cost, email sending cost, AI/ML cost per user, search service cost, monitoring/logging cost, error tracking cost, CI/CD cost, domain/SSL cost, third-party API costs, payment processing fees, development time estimate per phase, ongoing maintenance cost estimate, total monthly burn rate, break-even user count, cost optimization opportunities, reserved capacity discounts, free tier costs (what does the free tier cost YOU).

## Category 25: Growth & Scalability (50 Qs)
Horizontal vs vertical scaling, database scaling strategy, read replica strategy, connection pooling at scale, sharding strategy, CDN at scale, queue scaling, cache scaling, search scaling, file storage scaling, real-time at scale, API rate limiting at scale, multi-region strategy, data replication, consistency vs availability trade-offs, load balancing strategy, auto-scaling triggers, capacity planning, load testing plan, performance benchmarks, degradation plan under load.

## Category 26: Support & Operations (50 Qs)
Support channels, SLA tiers, escalation paths, incident response plan, status page, changelog, release notes format, user feedback collection, bug report flow, feature request flow, knowledge base/help center, video tutorials, community forum, in-app support widget, support ticket system, support analytics, response time targets, resolution time targets, on-call rotation, runbook maintenance.

## Category 27: Multi-Tenancy Deep-Dive (50 Qs, if applicable)
Isolation strategy, data partitioning, tenant customization (branding, fields, workflows), tenant onboarding automation, tenant migration between tiers, resource quotas per tenant, noisy neighbor prevention, tenant-specific feature flags, tenant admin capabilities, super-admin cross-tenant access, tenant data export, tenant deletion and cleanup, tenant billing, tenant analytics, tenant health monitoring.

## Category 28: Mobile-Specific (50 Qs, if applicable)
Responsive vs native vs hybrid, PWA capabilities, push notifications, deep linking, app store submission, app review guidelines compliance, offline support, local storage, sync strategy, biometric auth, camera/photo access, GPS/location, device testing matrix, platform-specific UI guidelines, app size optimization, background processing, battery optimization.

## Category 29: Onboarding & First-Run (50 Qs)
Signup flow steps, required fields, optional fields, social signup, email verification, org creation, team invite, industry/vertical selection, plan selection, first-run dashboard, empty state design, quick-start actions, onboarding checklist, guided tours, progressive disclosure, activation metrics, time-to-value targets, onboarding email sequence, onboarding analytics, drop-off tracking, A/B testing onboarding variants.

## Category 30: Deferred Features & Roadmap (50 Qs)
What's NOT being built? Why? Target phase? Dependencies? Cost of deferral? Trigger to build? Migration path? Impact of deferral on launch? User expectations for missing features? Communication plan for "coming soon"? Placeholder UI needed? Feature voting/request system?
