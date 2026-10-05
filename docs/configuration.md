# Configuration

AlgoVista runs with zero required environment variables. Optional values are documented in `.env.example`.

## Environment variables

| Variable | Required | Default / notes |
|----------|----------|-----------------|
| `GOOGLE_VERIFICATION_CODE` | No | Injected into Next.js `metadata.verification.google` in `app/layout.tsx` |
| `BING_VERIFICATION_CODE` | No | Documented for future use; not wired in layout yet |
| `NEXT_PUBLIC_SITE_URL` | No | Documented; site URL currently hardcoded to `https://algovista.voxhash.dev` in metadata |
| `NEXT_PUBLIC_SITE_NAME` | No | Documented optional branding override |
| `NEXT_PUBLIC_GA_ID` | No | Optional analytics |
| `NEXT_PUBLIC_GTM_ID` | No | Optional tag manager |
| `NEXT_PUBLIC_TWITTER_HANDLE` | No | Optional social |
| `NEXT_PUBLIC_GITHUB_URL` | No | Defaults conceptually to `https://github.com/VoxHash/algovista` |
| `NEXT_PUBLIC_ENABLE_ANALYTICS` | No | Feature-flag placeholder |
| `NEXT_PUBLIC_ENABLE_PWA` | No | Feature-flag placeholder |
| `NEXT_PUBLIC_ENABLE_DARK_MODE` | No | Feature-flag placeholder |
| `NEXT_PUBLIC_DEBUG` | No | Development aid |

## Secrets

- Do **not** commit `.env`
- Core algorithms and UI do not call paid APIs
- Treat verification codes and analytics IDs as private project settings

## Next.js config

`next.config.mjs` enables `reactStrictMode` and experimental `typedRoutes`. No custom env loading beyond Next.js defaults.
