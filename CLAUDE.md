# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **GitHub profile repository** (`penafortee/penafortee`). Its sole purpose is to render a personal profile page on [github.com/penafortee](https://github.com/penafortee). There is no application code, build system, or test suite.

## Structure

- **README.md** — The profile content displayed on GitHub. Uses HTML/Markdown with external badge/widget services:
  - [readme-typing-svg.demolab.com](https://readme-typing-svg.demolab.com) for animated typing header
  - [github-readme-streak-stats.herokuapp.com](https://github-readme-streak-stats.herokuapp.com) for contribution streak stats
  - [visitor-badge.laobi.icu](https://visitor-badge.laobi.icu) for visitor counter
- **img/** — Static image assets referenced by the README
- **.github/workflows/main.yml** — GitHub Actions workflow that generates a contribution grid snake animation SVG every 12 hours using `Platane/snk`, publishing output to the `output` branch

## Notes

- The snake animation embed in README.md is currently commented out (line 33).
- The snake SVG is published to `output` branch at `github-contribution-grid-snake.svg`.
- All changes to the profile are made by editing README.md directly — no build step is needed locally.
