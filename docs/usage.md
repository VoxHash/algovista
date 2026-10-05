# Usage

## As a learner

1. Open the [live demo](https://algovista.voxhash.dev/) or local server.
2. Choose **Sorting**, **Pathfinding**, or **String Matching** from the navigation.
3. Pick an algorithm card.
4. Adjust size / speed / pattern / grid as available.
5. Use play, pause, and step controls to walk through the generator.

## Sorting

Each card owns its own array and controls. Typical flow: shuffle or resize → play → watch comparisons and swaps highlight.

## Pathfinding

Interact with the grid (walls, start/goal depending on the card). Run Dijkstra, A*, BFS, and related algorithms and observe explored cells versus the final path.

## String matching

Provide text and pattern inputs. For KMP, inspect the LPS table when the algorithm builds it (default pattern `ababaca` shows non-zero LPS values).

## Edge cases to try

- Empty or single-element arrays for sorting
- Pattern longer than text for string matching
- Fully blocked grids for pathfinding (no path)
- Very high animation speed (UI should remain controllable via pause)
