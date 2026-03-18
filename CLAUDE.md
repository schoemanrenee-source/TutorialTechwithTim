# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of standalone web apps — each is a single self-contained HTML file with inline CSS and JavaScript. No build tools, no dependencies, no npm. Open any file directly in a browser.

## Git Workflow

All changes must be committed and pushed to GitHub after every session.

- Remote: https://github.com/schoemanrenee-source/TutorialTechwithTim
- Branch: `main`
- Git identity configured locally (not globally): `schoemanrenee-source`

Commit message style: imperative subject line, bullet-point body listing what changed per file.

```
git add <files>
git commit -m "short description

- file.html: what changed"
git push
```

## Architecture

Each HTML file is fully self-contained:
- **Styles** — inline `<style>` block, dark theme (`#1a1a2e` background, `#e94560` accent)
- **State** — plain JS variables; `localStorage` used for persistence where needed
- **No frameworks** — vanilla HTML/CSS/JS only

### Files

| File | Description |
|---|---|
| `tictactoe.html` | 2-player Tic Tac Toe with score tracking across rounds |
| `daily-tasks.html` | Daily habit tracker — green ✓ / red ✗ per task, progress bar, end-of-day summary modal, inline task editing (double-click), localStorage persistence with automatic daily reset |

## Running

Open any `.html` file directly in a browser — no server needed.

```
start tictactoe.html
start daily-tasks.html
```
