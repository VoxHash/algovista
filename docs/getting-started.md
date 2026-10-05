# Getting started

## Prerequisites

| Dependency | Version | Notes |
|------------|---------|-------|
| Node.js | 18+ (20 LTS recommended) | Required |
| npm | 9+ | Ships with Node |
| Git | any recent | Clone the repo |
| Modern browser | Chromium / Firefox / Safari | Client-side animations |

No database, Docker, or cloud credentials are required for local use.

## First run

```bash
git clone https://github.com/VoxHash/algovista.git
cd algovista
npm install
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000).

## Verify

```bash
npm test
npm run lint
npm run build
```

## Optional configuration

Copy `.env.example` to `.env` only if you need Search Console verification or analytics. See [configuration.md](configuration.md).

Next: [quick-start.md](quick-start.md) or [usage.md](usage.md).
