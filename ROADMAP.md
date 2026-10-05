# Roadmap

Realistic near-term plan for AlgoVista based on the current Next.js 14 codebase (static educational visualizer, no backend).

## Now (v1.x)

- [x] 30+ algorithm visualizations (sorting, pathfinding, string matching)
- [x] Multi-page layout with independent algorithm cards
- [x] SEO basics (sitemap, robots, metadata, OG image)
- [x] Fresh-clone docs kit and MIT license
- [ ] Expand Jest coverage to more generators in `lib/algorithms.ts`
- [ ] Resolve `react-hooks/exhaustive-deps` warnings in algorithm cards
- [ ] Document complexity metrics shown in the UI with source references

## Next

- [ ] Accessibility pass (keyboard focus order, reduced-motion preferences)
- [ ] Shareable algorithm state via URL query params (array seed, grid walls, pattern)
- [ ] Optional dark/light theme toggle (feature flag already sketched in `.env.example`)
- [ ] Dependency hygiene: address high npm audit findings on a non-breaking path

## Later

- [ ] Additional algorithm families (graphs beyond grids, compression demos)
- [ ] Optional i18n reintroduction only if there is clear demand
- [ ] Export animation frames / GIF for teaching materials

## Non-goals (for now)

- User accounts, persistence, or server-side algorithm execution
- Paid features or API rate limits (the app is client-side)

Suggestions welcome via [GitHub Issues](https://github.com/VoxHash/algovista/issues) or [contact@voxhash.dev](mailto:contact@voxhash.dev).
