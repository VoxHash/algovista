# Troubleshooting

## `npm run lint` prompts for ESLint setup

**Cause**: Missing `.eslintrc.json` in older checkouts.

**Fix**: Ensure you are on a commit that includes `.eslintrc.json` extending `next/core-web-vitals`, or recreate:

```json
{ "extends": "next/core-web-vitals" }
```

## Build succeeds but OG / PWA icons 404

**Cause**: PNG files missing from `public/`.

**Fix**:

```bash
npm run generate-images
```

## Hydration warnings around dates

Header date formatting must stay client-only (`useEffect`). Do not compute `toLocaleDateString` during SSR.

## Pathfinding or string matching appears stuck

Pause and reset the card. Historical bugs (Aho-Corasick infinite loop, stale generator closures) were fixed in the 1.0.0 line — upgrade if you are on an older fork.

## Corrupt local `.git` objects

External-drive sync can corrupt loose objects. Re-clone from GitHub:

```bash
git clone https://github.com/VoxHash/algovista.git
```

## Port already in use

```bash
npm run dev -- --port 3010
```

## Still stuck?

See [SUPPORT.md](../SUPPORT.md) and open a bug report.
