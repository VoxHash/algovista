# Quick start

End-to-end path validated on a clean install:

```bash
git clone https://github.com/VoxHash/algovista.git
cd algovista
npm install
npm test
npm run build
npm run dev
```

Then open:

- Home: `http://localhost:3000/`
- Sorting: `http://localhost:3000/sorting`
- Pathfinding: `http://localhost:3000/pathfinding`
- String matching: `http://localhost:3000/string-matching`

Production serve after build:

```bash
npm start
```

No `.env` file is required for the core visualizer.
