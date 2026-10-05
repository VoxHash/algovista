# Example 01 — Visualize Quick Sort

## Goal

Run Quick Sort locally and confirm the card animates partitions.

## Steps

1. Install and start the app (`npm install && npm run dev`).
2. Open [http://localhost:3000/sorting](http://localhost:3000/sorting).
3. Find the **Quick Sort** card.
4. Set a moderate array size and medium speed.
5. Click **Play** and observe pivot/partition highlights.
6. Use **Pause** / step controls to inspect intermediate states.

## Verify correctness offline

```bash
npm test
```

The Jest suite asserts Quick Sort output for a fixed unsorted array.
