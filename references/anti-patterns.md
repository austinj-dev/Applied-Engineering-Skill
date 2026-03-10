# Anti-Patterns — Applied Engineering

## Per-Category Anti-Patterns

### Auth
- DO NOT build custom auth when Supabase Auth / Clerk / Auth0 handles it
- DO NOT store passwords in plaintext or reversible encryption
- DO NOT use JWTs without refresh token rotation
- DO NOT skip rate limiting on login endpoints

### Database
- DO NOT store files in the database (use object storage)
- DO NOT skip indexes "because it's small now"
- DO NOT use soft deletes without filtering them from all queries
- DO NOT skip RLS/authorization at the database level
- DO NOT use TEXT for fields that should be ENUM/CHECK

### Frontend
- DO NOT use default/bland components when the library has rich alternatives
- DO NOT skip empty states, loading states, and error states
- DO NOT use alert() or window.confirm() in production
- DO NOT skip dark mode if the component library supports it
- DO NOT use localStorage for sensitive data (tokens, keys)

### API
- DO NOT return stack traces in production error responses
- DO NOT skip pagination on list endpoints
- DO NOT use GET for state-changing operations
- DO NOT skip API versioning from day one
- DO NOT expose internal IDs without authorization checks

### Security
- DO NOT skip HTTPS enforcement
- DO NOT skip CORS configuration
- DO NOT put API keys in client-side code
- DO NOT trust client-side validation alone
- DO NOT skip input sanitization

### Infrastructure
- DO NOT deploy without health check endpoints
- DO NOT skip structured logging
- DO NOT skip error tracking (Sentry or equivalent)
- DO NOT hard-code environment-specific values
- DO NOT skip backup verification

### General
- DO NOT use mock data in production code
- DO NOT leave TODO/FIXME without implementation
- DO NOT leave console.log in production
- DO NOT skip type safety (use TypeScript strict or equivalent)
- DO NOT skip documentation
