# Contributing to AlgoVista

Thanks for helping improve AlgoVista. This project is maintained by **VoxHash Technologies**.

## Development setup

```bash
git clone https://github.com/VoxHash/algovista.git
cd algovista
npm install
npm run dev
```

Before opening a PR:

```bash
npm test
npm run lint
npm run build
```

## Workflow

1. Open an issue describing the change (bug, feature, or docs).
2. Fork and create a branch: `feat/…`, `fix/…`, or `docs/…`.
3. Keep changes focused — one concern per PR.
4. Add or update tests when changing algorithm logic.
5. Use [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `chore:`).
6. Open a pull request using the template.

## Code guidelines

- TypeScript strictness: prefer explicit types at public boundaries.
- Algorithm generators live in `lib/algorithms.ts` / card components under `components/`.
- Do not commit `.env`, credentials, or generated `node_modules` / `.next`.
- Prefer real educational defaults (patterns, grids) over placeholder copy.

## Documentation

Update `docs/` and `CHANGELOG.md` when behavior or setup steps change.

## Conduct & security

- Follow the [Code of Conduct](CODE_OF_CONDUCT.md).
- Report vulnerabilities privately via [SECURITY.md](SECURITY.md).

Questions: [contact@voxhash.dev](mailto:contact@voxhash.dev).
