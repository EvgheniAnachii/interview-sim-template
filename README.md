# Interview Simulation Template

React + TypeScript + Tailwind + shadcn/ui, fully Dockerized.

## Stack

- Vite + React + TypeScript
- Tailwind CSS + shadcn/ui
- Biome (lint + format)
- Vitest + Testing Library
- Docker (all deps isolated in container)

## Usage

```bash
# Start app (runs in Docker, hot reload enabled)
npm run dev

# Stop
npm run docker:down

# Rebuild image (after adding new dependencies)
npm run docker:build

# Tests (runs locally)
npm run test:run

# Lint & format
npm run check
```

## Adding dependencies

Edit `package.json` directly, then rebuild:

```bash
npm run docker:build && npm run dev
```

## Adding shadcn components

```bash
npx shadcn@latest add <component>
npm run docker:build
```

## From template

1. Use this repo as a GitHub template
2. Clone your new repo
3. `npm run dev`
