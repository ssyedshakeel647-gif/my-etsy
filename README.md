# Etsy TrendScout

Etsy shop discovery, trending listing research, and keyword intelligence tool.

Phase 1 ships a Next.js dashboard with **demo data only**. Metrics are labeled verified/estimated/unavailable. Missing values are never fabricated.

## Stack

- Next.js (App Router) + TypeScript
- Tailwind CSS
- Zod-ready validation layer
- Modular data-provider interface (demo now; live providers later)
- Supabase/Postgres planned for Phase 3

## Getting started

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Scripts

- `npm run dev` — local development
- `npm run build` — production build
- `npm run lint` — ESLint
- `npm run typecheck` — TypeScript check

## Demo mode

The active provider is `demo`. Records are fictional and labeled **DEMO DATA**.

Swap providers later through `src/lib/providers/` without rewriting the UI.

## Phase roadmap

1. **Done in this MVP slice:** project setup, dashboard, New Shop Finder, Trending Listing Finder, filters, sorting, CSV export
2. Keyword Explorer, Tag Generator, SEO Analyzer
3. Database, auth, saved research, competitor comparison
4. Authorized live integrations, opportunity scoring refinements, usage limits

## Environment

Copy `.env.example` to `.env.local` when adding live credentials. Keep API keys server-side only.
