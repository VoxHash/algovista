# Installation

## System dependencies

- **Node.js 18+** with npm
- Sufficient disk for `node_modules` (~600–700 MB)
- Network access to the npm registry on first install

## Clone

```bash
git clone https://github.com/VoxHash/algovista.git
cd algovista
```

## Install packages

```bash
npm install
```

This installs Next.js 14, React 18, Framer Motion, Tailwind, Jest, Sharp (for image generation), and related tooling.

## Environment file (optional)

```bash
cp .env.example .env
```

Edit only the variables you need. See [configuration.md](configuration.md).

## Regenerating PWA / OG images

PNG assets ship in `public/`. To regenerate from SVG sources:

```bash
npm run generate-images
```

Requires the `sharp` dev dependency (included after `npm install`).

## Fresh-environment checklist

1. `node -v` ≥ 18
2. `npm install` completes without registry auth (public packages only)
3. `npm test` passes
4. `npm run lint` completes (non-interactive; `.eslintrc.json` is committed)
5. `npm run build` succeeds
6. `npm run dev` serves `/`, `/sorting`, `/pathfinding`, `/string-matching`
