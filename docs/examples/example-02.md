# Example 02 — Trace A* pathfinding

## Goal

Watch A* explore a grid and produce a path.

## Steps

1. Start the app (`npm run dev`).
2. Open [http://localhost:3000/pathfinding](http://localhost:3000/pathfinding).
3. Open the **A\*** card.
4. Draw walls on the grid (if the card supports clicking cells).
5. Run the algorithm and observe the frontier versus the final path.
6. Compare with **Dijkstra** on the same layout to discuss heuristics.

## Teaching tip

Ask learners why A* expands fewer nodes than Dijkstra when the heuristic is admissible (Manhattan distance on a uniform grid).
