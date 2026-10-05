# Changelog

All notable changes to AlgoVista are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-10-05

First official GitHub release of AlgoVista (repository renamed from `algovista-next` to `algovista`).

### Added

- Interactive visualizer for 30+ sorting, pathfinding, and string matching algorithms
- Dedicated pages for Home, Sorting, Pathfinding, and String Matching with per-algorithm cards
- SEO support: sitemap, robots.txt, JSON-LD schema, Open Graph / Twitter metadata (`3f675b7`)
- PWA manifest and generated PNG icons / OG image (`og-image.png`, `icon-192.png`, `icon-512.png`)
- Image generation script (`npm run generate-images`) using Sharp (`24905f7`)
- Environment template (`.env.example`) including `GOOGLE_VERIFICATION_CODE` (`f2568cd`, `54620f7`)
- Jest unit tests for Quick Sort, Merge Sort, and KMP LPS construction
- Full documentation kit (`docs/`, CONTRIBUTING, SECURITY, SUPPORT, ROADMAP, GitHub issue/PR templates)
- MIT `LICENSE` and ESLint config (`next/core-web-vitals`) for a working `npm run lint` path

### Changed

- Repository brand/name aligned to **algovista** (package name was already `algovista`)
- Default KMP pattern set to `ababaca` to demonstrate non-zero LPS values (`805e877`)
- LPS table UI shows guidance when empty and only for KMP (`5da73b4`)
- English-only product surface (i18n removed in prior commits)

### Fixed

- Aho-Corasick infinite loop (`3f675b7`)
- Stale closure bugs in algorithm cards via `useRef` generator state (`8f65339`, `763cbeb`)
- Hydration mismatch from server-rendered dates (`dbe2c0b`)
- TypeScript `Link` `href` typing issues on Home and Navigation (`fe3b794`, `785756d`)

### Security

- No secrets required for local or production core usage; `.env` remains gitignored
- Optional verification / analytics IDs only — never commit real values

[1.0.0]: https://github.com/VoxHash/algovista/releases/tag/v1.0.0
