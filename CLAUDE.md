# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of standalone web apps — each is a single self-contained HTML file with inline CSS and JavaScript. No build tools, no dependencies, no npm. Open any file directly in a browser.

## Git Workflow

**Commit and push after every change — no exceptions.** This ensures work is never lost and the repo always reflects the current state of the project.

- Remote: https://github.com/schoemanrenee-source/TutorialTechwithTim
- Branch: `main`
- Git identity configured locally (not globally): `schoemanrenee-source`

After completing any edit — no matter how small — run:

```
git add <files>
git commit -m "short description

- file.html: what changed

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>"
git push
```

Commit message style: imperative subject line, bullet-point body listing what changed per file. Never batch unrelated changes into one commit.

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
