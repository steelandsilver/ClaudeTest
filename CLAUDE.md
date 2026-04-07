# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

A browser-based Tic Tac Toe game. Single self-contained file — no build step, no dependencies, no package manager.

## Running

Open `tictactoe.html` directly in a browser:

```bash
start "D:\ClaudeTest\tictactoe.html"
```

## Architecture

Everything lives in `tictactoe.html`:

- **HTML** — game board (`#board`) built dynamically via JS; score display; reset button
- **CSS** — dark theme (`#1a1a2e` background), grid layout, cell hover/win animations
- **JS** — flat state (`board[]`, `current`, `over`, `scores`); `play(i)` handles all game logic; `WINS` array defines the 8 winning lines; no frameworks or modules

## Git workflow

**After every meaningful unit of work, commit and push.** This keeps GitHub as a reliable snapshot of current progress and ensures no work is ever lost.

- Commit when a feature is added, a bug is fixed, or any notable change is made — don't batch unrelated changes into one commit
- Write clean, descriptive commit messages that explain *what* changed and *why*
- Always push immediately after committing

```bash
git add <file> && git commit -m "<message>" && git push
```

Remote: `https://github.com/steelandsilver/ClaudeTest` (private)
