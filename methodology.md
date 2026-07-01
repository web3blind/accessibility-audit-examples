# Methodology

This repository uses an agent-driven accessibility audit workflow.

## Inputs

- Public source repositories for desktop and mobile apps.
- Public URLs and linked pages for websites.
- Platform-specific checklists: web WCAG/ARIA/HTML, Flutter/mobile semantics, PyQt/desktop accessible naming patterns.

## Audit boundary

The audit checks all accessibility evidence available from code, markup, styles, scripts, page structure and public HTTP responses. Manual screen-reader/device testing is intentionally a separate stage.

## Scoring

Score = `max(0, 100 - critical*10 - warning*5 - info)`.

Grades:
- A: 90–100
- B: 80–89
- C: 70–79
- D: 60–69
- F: below 60

## Public tone

These reports are learning examples and PR/issue starting points, not a public shaming list.
