# Architecture

## Overview

```
Browser
  └── Next.js 14 App Router (static pages)
        ├── Header / Navigation
        ├── HomePage
        └── Algorithm cards (client components)
              └── Generators in lib/algorithms.ts + AlgoVista.tsx
```

## Routing

| Route | Page |
|-------|------|
| `/` | Home |
| `/sorting` | Sorting algorithm cards |
| `/pathfinding` | Pathfinding algorithm cards |
| `/string-matching` | String matching cards |
| `/sitemap.xml` | Generated sitemap |
| `/robots.txt` | Robots rules |
| `/manifest.webmanifest` | PWA manifest |

## Rendering

- App shell and metadata are server-friendly.
- Visualizer cards are client components (`'use client'`) for animation state.
- No backend database; all computation runs in the browser.

## Styling & motion

- Tailwind CSS + glassmorphism utilities in `app/globals.css`
- Framer Motion for transitions
- Lucide icons

## Deploy target

Designed for Vercel (or any Node host that can run `next start`). Live site: `https://algovista.voxhash.dev`.
