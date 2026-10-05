# CLI and scripts

AlgoVista does not ship a standalone binary. Use npm scripts from the repo root.

| Script | Command | Purpose |
|--------|---------|---------|
| Dev server | `npm run dev` | Next.js development server |
| Build | `npm run build` | Production build to `.next/` |
| Start | `npm start` | Serve the production build |
| Lint | `npm run lint` | ESLint via `next lint` |
| Test | `npm test` | Jest |
| Images | `npm run generate-images` | SVG → PNG for OG / PWA icons |

## Examples

```bash
npm run dev -- --port 3010
npm test -- --watch
npm run build && npm start
```
