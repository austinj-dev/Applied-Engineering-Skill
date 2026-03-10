# Tech Stack Evaluation — Applied Engineering

## Protocol

1. **Never assume tech stack.** Always ask.
2. If in existing repo: scan ENTIRE codebase for detection (package.json, requirements.txt, Cargo.toml, go.mod, Gemfile, etc.)
3. After user states their stack: **ALWAYS suggest an alternative with reasoning.**
4. Ask one final time: "Which stack do you want to use?"
5. Load the appropriate stack reference from `references/stacks/`

## Modern Tech Stack Reference (2025-2026)

### Full-Stack Web Frameworks

| Framework | Language | Best For | DB Pairing | Deploy Target |
|-----------|----------|----------|-----------|---------------|
| Next.js 15 | TypeScript | SaaS, dashboards, content | Supabase, Neon, PlanetScale | Vercel, Cloudflare Workers |
| Nuxt 3 | TypeScript/Vue | SaaS, content sites | Supabase, Prisma+Postgres | Vercel, Cloudflare, Netlify |
| SvelteKit 2 | TypeScript/Svelte | Fast UIs, SPAs, dashboards | Supabase, Drizzle+Postgres | Vercel, Cloudflare |
| Remix/React Router 7 | TypeScript | Data-heavy apps, forms | Prisma, Drizzle | Vercel, Fly.io, Cloudflare |
| Astro 5 | TypeScript | Content sites, docs, blogs | Any via API | Vercel, Cloudflare, Netlify |
| Django 5 | Python | Enterprise, data-heavy, admin | PostgreSQL, MySQL | Railway, Fly.io, AWS, self-hosted |
| FastAPI | Python | APIs, ML services, microservices | SQLAlchemy+Postgres, MongoDB | Railway, Fly.io, AWS Lambda |
| Rails 8 | Ruby | Rapid prototyping, SaaS, CRUD | PostgreSQL, SQLite | Fly.io, Railway, Heroku, self-hosted |
| Laravel 12 | PHP | SaaS, CMS, e-commerce | MySQL, PostgreSQL | Forge, Vapor, self-hosted |
| Phoenix | Elixir | Real-time, high concurrency | PostgreSQL | Fly.io, self-hosted |
| Go + htmx | Go | High-performance APIs, internal tools | PostgreSQL, SQLite | Any (single binary) |
| Rust (Actix/Axum) | Rust | Performance-critical APIs | PostgreSQL, SQLite | Any |
| Spring Boot | Java/Kotlin | Enterprise, banking, healthcare | PostgreSQL, MySQL, Oracle | AWS, Azure, self-hosted |
| .NET 9 | C# | Enterprise, Windows ecosystem | SQL Server, PostgreSQL | Azure, AWS, self-hosted |

### Frontend-Only Frameworks

| Framework | Best For | State Management |
|-----------|----------|-----------------|
| React 19 | Complex UIs, ecosystem | Zustand, Jotai, React Query |
| Vue 3 | Progressive enhancement | Pinia, Vue Query |
| Svelte 5 | Performance, simplicity | Built-in runes |
| Solid.js | Fine-grained reactivity | Built-in signals |
| Angular 19 | Enterprise, large teams | RxJS, NgRx, Signals |
| htmx + Alpine.js | Server-rendered, simple interactivity | Minimal client state |

### Databases

| Database | Type | Best For | Hosting Options |
|----------|------|----------|----------------|
| PostgreSQL | Relational | General purpose, SaaS, enterprise | Supabase, Neon, Railway, AWS RDS, self-hosted |
| MySQL | Relational | Traditional web apps, WordPress | PlanetScale, AWS RDS, self-hosted |
| SQLite | Embedded relational | Edge, single-server, Electron | Turso (distributed), local |
| MongoDB | Document | Flexible schemas, rapid prototyping | Atlas, self-hosted |
| Redis | Key-value/cache | Caching, sessions, queues, pub/sub | Upstash, AWS ElastiCache, self-hosted |
| DynamoDB | Key-value | AWS-native, serverless | AWS only |
| CockroachDB | Distributed SQL | Global distribution, strong consistency | CockroachDB Cloud, self-hosted |
| ClickHouse | Columnar | Analytics, time-series, logs | ClickHouse Cloud, self-hosted |
| Neo4j | Graph | Relationships, recommendations | AuraDB, self-hosted |
| Elasticsearch | Search | Full-text search, log analysis | Elastic Cloud, self-hosted |

### UI Component Libraries (Research-Based Recommendations)

| Library | Framework | Tier | Highlights |
|---------|-----------|------|-----------|
| Mantine 7 | React | Free | 100+ components, hooks, form integration, dark mode |
| shadcn/ui | React | Free | Radix primitives, copy-paste, fully customizable |
| Ant Design 5 | React | Free | Enterprise-grade, 60+ components, data-heavy |
| MUI 6 | React | Free/Paid | Most popular React lib, comprehensive |
| Chakra UI 3 | React | Free | Accessible, composable, dark mode |
| Headless UI | React/Vue | Free | Unstyled, accessible primitives |
| Radix UI | React | Free | Low-level accessible primitives |
| PrimeReact/Vue/Angular | Multi | Free/Paid | 90+ components per framework |
| Vuetify 3 | Vue | Free | Material Design, comprehensive |
| Naive UI | Vue | Free | TypeScript-first, 80+ components |
| Element Plus | Vue | Free | Enterprise, data tables, forms |
| Skeleton | Svelte | Free | Tailwind-based, Svelte-native |
| Angular Material | Angular | Free | Official Material Design |
| daisyUI | Tailwind | Free | Tailwind component classes |
| Tremor | React | Free | Dashboard components, charts |
| Aceternity UI | React | Free | Animated, modern, premium feel |

### Paid Component Libraries (When Free Isn't Enough)

| Library | Price | Why It's Worth It |
|---------|-------|-------------------|
| Syncfusion | $995/yr | 80+ components, grids, schedulers, Gantt, PDF |
| Telerik (Progress) | $1,299/yr | Enterprise data grids, charts, schedulers |
| AG Grid | $999+/yr | The best data grid. Period. |
| DevExtreme | $1,495/yr | Complex dashboards, pivots, schedulers |
| Retool | $10+/user/mo | Internal tool builder with pre-built components |

### Deployment Targets

| Target | Best For | Limitations |
|--------|----------|-----------|
| Vercel | Next.js, frontend-heavy | Serverless limits, cold starts |
| Cloudflare Workers | Edge-first, global | Worker size limits (10MB paid) |
| Fly.io | Containers, databases, global | More ops overhead than Vercel |
| Railway | Full-stack, databases, queues | Less edge optimization |
| AWS (ECS/Lambda/Amplify) | Enterprise, compliance, scale | Complexity, cost management |
| GCP (Cloud Run) | Containers, ML, Firebase integration | Ecosystem lock-in |
| Azure | .NET, enterprise, hybrid cloud | Complexity |
| DigitalOcean App Platform | Simple deployments, cost-effective | Limited edge features |
| Render | Simple full-stack | Similar to Railway |
| Self-hosted (VPS) | Full control, compliance | All ops on you |

### Mobile Stacks

| Stack | Language | Best For |
|-------|----------|----------|
| React Native | TypeScript | Cross-platform, web devs transitioning |
| Expo | TypeScript | React Native with managed services |
| Flutter | Dart | High-performance cross-platform |
| Swift/SwiftUI | Swift | iOS-only, best native experience |
| Kotlin/Jetpack Compose | Kotlin | Android-only, best native experience |
| Capacitor (Ionic) | TypeScript | Web app → mobile wrapper |
| Tauri Mobile | Rust + Web | Lightweight, new but promising |

## Alternative Suggestion Template

After user states their stack:

```
TECH STACK EVALUATION
=====================
Your choice: [user's stack]

Alternative recommendation: [suggested stack]

Reasoning:
- [advantage 1 of alternative]
- [advantage 2 of alternative]
- [trade-off / what you'd lose]

For your specific use case ([product description]):
- [why alternative fits better OR why user's choice is actually good]

Which stack do you want to proceed with?
```
