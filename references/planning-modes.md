# Planning Modes — Applied Engineering

## Mode Definitions

### Standard Plan (2-4 hours)

**Best for**: Single products, major features, MVPs, startups
**Questions**: 150+ across applicable categories (50 per category minimum)
**Suggestions**: 100+ with effort estimates
**Documents generated**: 12-15
**Checkpoints**: Planning Pulse every 30 minutes
**Competitive research**: Feature-level comparison
**Cost modeling**: Basic (monthly estimate at 3 scale tiers)
**Complexity Score cap**: Suggest lock-in at 250+
**MVP Gate**: Optional, suggested at midpoint

### Deep / Enterprise Plan (6-8+ hours)

**Best for**: Enterprise platforms, multi-product ecosystems, regulated industries
**Questions**: 300+ across ALL categories (50+ per category with deep-dive branches)
**Suggestions**: 200+ with ROI analysis and effort estimates
**Documents generated**: 18-22
**Checkpoints**: Planning Pulse every 30 minutes + quarterly deep reviews
**Competitive research**: Full analysis (features, pricing, tech stack, API, UX, reviews)
**Cost modeling**: Detailed (per-service breakdown at 5 scale tiers with growth projections)
**Complexity Score cap**: Suggest lock-in at 750+
**MVP Gate**: Mandatory at midpoint, optional at quartiles
**Includes**: DDD assessment, event storming prompts, CQRS evaluation

## Mode Selection Prompt

Present at skill activation. Include descriptions. Let user choose. Never assume.

## Mode Escalation

If Standard mode hits Enterprise complexity (score >500), suggest: "This project has grown beyond Standard scope. Would you like to escalate to Deep/Enterprise mode for the remaining categories? This adds: [list of additional coverage]."

## Mode De-escalation

If Deep/Enterprise mode shows diminishing returns early (velocity <0.3 by hour 3), suggest: "We may not need full Enterprise-depth planning. Would you like to complete the current categories and move to document generation?"
