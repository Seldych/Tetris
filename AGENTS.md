# AGENTS.md

## Project
Tetris — классическая игра на HTML5 Canvas

## Commands
No specific lint/typecheck/build commands available.

## Key Constants
- COLS=10, ROWS=20, BLOCK_SIZE=30
- LINES_PER_LEVEL=10
- LINE_POINTS=[0, 100, 300, 500, 800]
- FLASH_DURATION=300 (ms)
- EMPTY=0, EDGE_WIDTH=3
- Drop interval: max(80, 1000 - (level-1)*80) ms

## State Object: G
- `G` holds all game state (board, currentPiece, score, level, flags, timers)
- `G.pieceBag` — 7-bag shuffled array for fair random piece distribution
- DOM refs are top-level consts (not grouped — single-file pragmatism)

## Code Conventions
- Single HTML file (index.html) with embedded CSS and JS
- Russian locale for UI
- 4-space indentation
- JSDoc comments for all functions
- Inline `/** */` comments for constants (single-line)
- Section headers with `// ====` separator blocks
- camelCase for variables and functions
- UPPER_CASE for constants
