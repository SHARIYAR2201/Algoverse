# AlgoVerse AI (front-end vertical slice)

A single-file, no-build web app. Open `index.html` in a browser, or run it with Docker.

Needs an internet connection: Tailwind CSS and Google Fonts load from CDNs.

## Run
- Browser: double-click `index.html`.
- Docker: `docker compose up --build`, then open http://localhost:8080
  (the Docker files are untested; they only serve `index.html` with nginx).

## Implemented
- Visualizer: Bubble, Insertion, Selection, Merge Sort, Binary Search and Linear Search, driven by one execution trace.
  Play/pause, step, rewind, scrub, speed, random or custom input, synced pseudocode, counted metrics.
- Complexity table per algorithm, toggleable growth curves, scaling counts, in-page self-tests.
- Comparison lab: two sorts or two searches on the same input, side by side.
- Stack and queue demo, 8-question quiz (best score kept in this browser's localStorage).
- Tutor: rule-based, answers only from the loaded algorithm, trace and analyzer. No LLM is called.
- Code analyzer: pattern-based bug checks and complexity estimates for pasted code. It never runs your code,
  cannot prove correctness, and only has rewrites for a few known patterns.

## Not implemented
FastAPI backend, PostgreSQL, accounts, Redis, CI, LLM provider integration, hash tables, trees, graphs,
DP, backtracking, greedy and bit-manipulation visualizers, learning paths and progress sync.
