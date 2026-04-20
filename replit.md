# Workspace

## Overview

pnpm workspace monorepo using TypeScript. Each package manages its own dependencies.

Current main web artifact: `artifacts/zaky-portfolio`, a React/Vite single-page portfolio for M Zaky Mahid Ruwansyah with bilingual ID/EN content, a modern white background with subtle colorful animated movement, Poppins typography with lighter hero weight, glassmorphism exhibition cards with rounded corners, separated Graphic Design feed/story galleries, carousel media galleries with left/right navigation buttons, Ramoti and Kumata work sections, a vertical selected works library (Logo, 3D Mock-up, Gambar, Animasi), and a collaboration footer with email contact.

## Stack

- **Monorepo tool**: pnpm workspaces
- **Node.js version**: 24
- **Package manager**: pnpm
- **TypeScript version**: 5.9
- **API framework**: Express 5
- **Database**: PostgreSQL + Drizzle ORM
- **Validation**: Zod (`zod/v4`), `drizzle-zod`
- **API codegen**: Orval (from OpenAPI spec)
- **Build**: esbuild (CJS bundle)

## Key Commands

- `pnpm run typecheck` — full typecheck across all packages
- `pnpm run build` — typecheck + build all packages
- `pnpm --filter @workspace/api-spec run codegen` — regenerate API hooks and Zod schemas from OpenAPI spec
- `pnpm --filter @workspace/db run push` — push DB schema changes (dev only)
- `pnpm --filter @workspace/api-server run dev` — run API server locally

See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details.
