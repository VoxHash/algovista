# AlgoVista

Interactive algorithm visualizer for sorting, pathfinding, and string matching — with real-time step-by-step animations.

[![CI](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/VoxHash/algovista)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Next.js](https://img.shields.io/badge/Next.js-14-black)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)](https://www.typescriptlang.org/)
[![GitHub stars](https://img.shields.io/github/stars/VoxHash/algovista?style=social)](https://github.com/VoxHash/algovista)

> **Live demo**: [https://algovista.voxhash.dev/](https://algovista.voxhash.dev/)

## Features

- **30+ algorithms** across sorting, pathfinding, and string matching
- **Real-time controls**: play, pause, step, and speed adjustment
- **Interactive grids and arrays** with independent per-algorithm cards
- **SEO & PWA assets**: sitemap, robots, manifest, Open Graph image
- **Modern stack**: Next.js 14, TypeScript, Tailwind CSS, Framer Motion

### Algorithms

| Category | Count | Examples |
|----------|------:|----------|
| Sorting | 10 | Quick Sort, Merge Sort, Heap Sort, Radix Sort |
| Pathfinding | 10 | Dijkstra, A*, BFS, DFS, Bellman-Ford, JPS |
| String matching | 10 | KMP, Rabin-Karp, Boyer-Moore, Aho-Corasick |

## Quick start

**Requirements**: Node.js 18+ (20 LTS recommended), npm 9+

```bash
git clone https://github.com/VoxHash/algovista.git
cd algovista
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

Optional environment variables (copy `.env.example` → `.env`):

| Variable | Required | Purpose |
|----------|----------|---------|
| `GOOGLE_VERIFICATION_CODE` | No | Google Search Console verification |
| `NEXT_PUBLIC_SITE_URL` | No | Canonical site URL override |
| `NEXT_PUBLIC_GA_ID` | No | Google Analytics |
| `NEXT_PUBLIC_GTM_ID` | No | Google Tag Manager |

No secrets are required to run the visualizer locally.

## Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Development server (`http://localhost:3000`) |
| `npm run build` | Production build |
| `npm start` | Serve production build |
| `npm run lint` | ESLint (Next.js core-web-vitals) |
| `npm test` | Jest unit tests |
| `npm run generate-images` | Build PNG icons / OG image from SVG sources |

## Documentation

- [Getting started](docs/getting-started.md)
- [Installation](docs/installation.md)
- [Configuration](docs/configuration.md)
- [Usage](docs/usage.md)
- [Architecture](docs/architecture.md)
- [API / algorithms](docs/api.md)
- [CLI / scripts](docs/cli.md)
- [Troubleshooting](docs/troubleshooting.md)
- [FAQ](docs/faq.md)
- [Examples](docs/examples/example-01.md)
- [Roadmap](ROADMAP.md)
- [Changelog](CHANGELOG.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)
- [Support](SUPPORT.md)

## Project structure

```
algovista/
├── app/                 # Next.js App Router pages
├── components/          # UI and algorithm cards
├── lib/                 # Algorithm generators and helpers
├── __tests__/           # Jest tests
├── public/              # Static assets (icons, OG image)
├── scripts/             # Image generation helpers
└── docs/                # Documentation kit
```

## Deployment

### Vercel

1. Import `VoxHash/algovista` in Vercel
2. Framework preset: Next.js
3. Deploy (no required env vars for core features)

Optional: set `GOOGLE_VERIFICATION_CODE` and analytics IDs in the Vercel project settings.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). By participating, you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

MIT © [VoxHash Technologies](https://voxhash.dev) — see [LICENSE](LICENSE).

## Contact

- GitHub: [@VoxHash](https://github.com/VoxHash)
- Email: [contact@voxhash.dev](mailto:contact@voxhash.dev)
- Portfolio: [voxhash.dev](https://voxhash.dev)
