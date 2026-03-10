# Launch Checklist — Applied Engineering

## Build Verification
- [ ] Production build completes with zero errors
- [ ] TypeScript / type checking passes
- [ ] Linter passes with zero errors
- [ ] Zero mock data, placeholder, TODO in production code
- [ ] All environment variables configured for production
- [ ] Bundle size within acceptable limits

## Security
- [ ] All OWASP Top 10 vectors addressed
- [ ] Security headers configured (HSTS, CSP, X-Frame-Options)
- [ ] API routes have auth checks
- [ ] No secrets in client-side code
- [ ] Rate limiting configured
- [ ] CORS properly restricted
- [ ] Input validation on all forms and API endpoints
- [ ] SQL injection protection verified
- [ ] XSS protection verified

## Auth & Permissions
- [ ] All roles can login
- [ ] Permission matrix tested
- [ ] Cross-org isolation verified
- [ ] Session management working
- [ ] Password reset flow working
- [ ] Email verification working

## Data
- [ ] Database backups configured
- [ ] Seed data clean (no test data in production)
- [ ] RLS policies verified
- [ ] Data export capability working (GDPR)
- [ ] Migration chain runs cleanly from zero

## Monitoring
- [ ] Error tracking configured (Sentry or equivalent)
- [ ] Uptime monitoring configured
- [ ] Health check endpoint responding
- [ ] Alerting rules configured
- [ ] Logging working and accessible

## Performance
- [ ] Page load times acceptable (<3s LCP)
- [ ] No N+1 queries on critical paths
- [ ] Images optimized
- [ ] CDN configured for static assets
- [ ] Database indexes on frequently queried columns

## Legal
- [ ] Privacy policy published
- [ ] Terms of service published
- [ ] Cookie consent (if applicable)
- [ ] GDPR/CCPA compliance verified (if applicable)

## Documentation
- [ ] README updated
- [ ] API documentation published
- [ ] User documentation / help content available
- [ ] Architecture documentation current

## Operations
- [ ] Deployment process documented
- [ ] Rollback procedure documented
- [ ] Support channels configured
- [ ] Incident response plan documented
