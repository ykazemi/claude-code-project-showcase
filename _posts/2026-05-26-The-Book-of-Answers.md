---
layout: post
title: "The Book of Answers"
date: 2026-05-25
team: "Sabrina Yan"
tools: "Claude Code, Python, Pygame 2, Pytest"
github_repo: "https://github.com/SabrinaYyy/The-Book-of-Answers"
demo_link: "https://canva.link/y9mjb0hzvmhryw7"
summary: "A psychological horror dialogue game where players silently think of a question and receive mysterious answers from a supernatural book."
categories: project
---

## Project Overview

The Book of Answers is a small 2D psychological horror experience inspired by *The Book of Answers*.

The player silently thinks of a question, opens a mysterious book, and receives one of three outcomes:
- a normal answer,
- a disturbing/spooky answer,
- or a rare jump scare event.

The goal of the project was not only to build the game itself, but also to explore a structured AI-assisted development workflow using Claude Code.

---

## Problem

Many beginner game projects become difficult to manage because they are built without clear planning, testing, or scope control.

I wanted to explore:
- how to break a game into small verifiable steps,
- how to use Claude Code effectively without over-engineering,
- and how simple visuals and timing can still create strong psychological atmosphere.

---

## What We Built

We built a state-driven 2D horror dialogue game using Python and Pygame 2.

Main features include:
- mysterious interactive book,
- random answer system,
- spooky dialogue events,
- rare jump scares,
- fade transitions,
- flickering horror effects,
- atmospheric audio,
- disclaimer screen,
- restart loop,
- and a full pytest-based verification workflow.

The game flow is controlled through explicit game states:
- START
- IDLE
- OPENING_BOOK
- NORMAL_ANSWER
- SPOOKY_ANSWER
- JUMPSCARE
- RESTART

---

## How We Used Claude Code

We used Claude Code as an AI coding assistant throughout the entire project.

Instead of asking Claude to "build the whole game," the project was broken into small plans:
- Plan 1 — Core window and game loop
- Plan 2 — State system
- Plan 3 — Book interaction and animation
- Plan 4 — Random answer selection
- Plan 5 — Answer display
- Plan 6 — Jump scare system
- Plan 7 — Restart loop and polish

For each feature:
1. A detailed `plan.md` was written first
2. Claude implemented only that plan
3. Pytest tests were added
4. Verification was performed before continuing

Claude Code helped with:
- project structure,
- debugging,
- test generation,
- refactoring,
- state management,
- animation timing,
- safe asset loading,
- and polishing the final experience.

---

## Development Workflow

The project used:
- `Design_Doc.md` for the overall game vision,
- `CLAUDE.md` for coding rules and architecture constraints,
- and individual feature plans for incremental implementation.

Important design rules included:
- no over-engineering,
- state-driven logic,
- minimal dependencies,
- no hardcoded magic numbers,
- graceful asset fallback handling,
- and keeping the game psychologically atmospheric rather than visually complex.

---

## Technical Highlights

Some technical systems implemented:
- state transition validation,
- animated book-opening sequence,
- probability-based outcome selection,
- text wrapping for book pages,
- fade transitions,
- flickering spooky backgrounds,
- jumpscare timing systems,
- audio switching between ambient music and horror sounds,
- and a fully testable modular architecture.

The project ended with over 90 automated tests passing.

---

## Screenshots

![Screenshot of The Book of Answers]({{ "/assets/images/the-book-of-answers/screenshot.png" | relative_url }})

---

## GitHub Repository

[View the project repository](https://github.com/SabrinaYyy/The-Book-of-Answers)

---

## Demo

https://canva.link/y9mjb0hzvmhryw7

---

## What We Learned

This project taught me:
- how to structure an AI-assisted development workflow,
- how to write better prompts for coding agents,
- how to break large ideas into testable tasks,
- and how small atmospheric details can create strong emotional effects.

One major lesson was that AI coding tools work best when:
- the architecture is clear,
- the task scope is small,
- and the verification criteria are explicit.

---

## Future Improvements

Possible future improvements:
- improved book artwork,
- additional jumpscare variations,
- dynamic page textures,
- more advanced sound design,
- save system for discovered answers,
- randomized visual glitches,
- and expanded psychological horror events.
