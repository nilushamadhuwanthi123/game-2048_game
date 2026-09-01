# 2048

A polished clone of the classic 2048 sliding-tile puzzle, built with vanilla JavaScript, DOM elements, and CSS Grid — no frameworks, no build step, no external dependencies.

It demonstrates core game-programming fundamentals outside of a canvas context: grid-based state management with immutable move resolution, once-per-move merge rules, CSS-transition-driven tile animation, unified keyboard/touch input handling, and accessibility patterns like live-region announcements and reduced-motion support.

## Features
- Standard 2048 merge logic with random 2 (90%) / 4 (10%) tile spawns
- Merge-once-per-move guarantee via a single generic line-collapse routine shared by all four directions
- Smooth CSS-transition tile slide/merge/spawn animations
- Keyboard (arrow keys / WASD) and touch (swipe) controls
- Win detection at the 2048 tile with a "keep playing" banner, and full lose detection (no empty cells, no adjacent equal tiles)
- Persistent best score, plus best-effort in-progress game state, via localStorage
- Reduced-motion support (`prefers-reduced-motion`)
- Screen-reader announcements via an `aria-live` region for score changes, merges, wins, and game over
- Visible focus states throughout, fully keyboard-operable

## Run it
Just open `index.html` in a browser — no build step, no install.

## Live version
Play it here: https://nilushamadhuwanthi123.github.io/game-2048_game/
