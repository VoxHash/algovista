# API / algorithm surfaces

There is no HTTP API. Algorithms are TypeScript generator functions consumed by React cards.

## Primary modules

| Path | Role |
|------|------|
| `lib/algorithms.ts` | Core algorithm generators and helpers |
| `lib/utils.ts` | Shared utilities (`cn`, etc.) |
| `components/AlgoVista.tsx` | Shared UI primitives and algorithm card implementations |
| `components/HomePage.tsx` | Landing content |
| `components/Header.tsx` / `Navigation.tsx` | Chrome |

## Generator pattern

Visualizers typically:

1. Create a generator that `yield`s intermediate states (arrays, grids, indices).
2. Store the generator in a `useRef` so play/pause/step closures stay current.
3. Render the latest yielded state in the card UI.

## Tests

`__tests__/algorithms.test.ts` covers pure Quick Sort, Merge Sort, and KMP LPS construction. Prefer adding pure-function tests alongside generator changes.

## Metadata “API”

Next.js metadata in `app/layout.tsx` reads `process.env.GOOGLE_VERIFICATION_CODE` at build/request time for Search Console verification.
