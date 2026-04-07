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

Commit and push after every meaningful change:

```bash
git add <file> && git commit -m "<message>" && git push
```

Remote: `https://github.com/steelandsilver/ClaudeTest`
