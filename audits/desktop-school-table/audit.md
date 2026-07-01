# Accessibility audit: School Table desktop app

## Target

- **Project:** EDeev/school_table
- **Type:** desktop / PyQt5
- **Source:** https://github.com/EDeev/school_table
- **Date:** 2026-07-01
- **Standards:** WCAG 2.1 AA principles, Desktop accessibility checklist, Qt/PyQt accessible naming patterns

## Scope

Полный агентный аудит доступности по доступному коду, HTML/CSS/JS, структуре интерфейса и публичным страницам/ресурсам. Ручное тестирование со скринридером или физическим устройством относится к отдельному этапу и не смешивается с этим отчётом.

## Executive summary

- **Score:** 88/100
- **Grade:** B
- **Critical issues:** 0
- **Warnings:** 2
- **Informational:** 2

Небольшое PyQt-приложение: хороший кандидат для первого upstream PR с доступными именами, связью label→field и явным tab order там, где это нужно.

## Critical issues

No findings in this severity group.

## Warnings

### 1. No explicit accessible names are set for widgets

- **Category:** Desktop / PyQt

- **Criterion:** WCAG 4.1.2 / desktop UIA/AT-SPI naming

- **Evidence:** `setAccessibleName occurrences: 0`

- **Suggested fix:** Add setAccessibleName() to icon-only, ambiguous, or dynamically created controls; keep visible text for normal QPushButton/QLabel controls.

### 2. Form labels are not programmatically associated with inputs

- **Category:** Forms

- **Criterion:** WCAG 1.3.1 / 3.3.2

- **Evidence:** `QLabel.setBuddy occurrences: 0`

- **Suggested fix:** Use QLabel.setBuddy(inputWidget) for form labels, or set accessibleName on each field.


## Informational findings

### 1. No accessible descriptions are provided

- **Category:** Desktop / PyQt

- **Criterion:** WCAG 3.3.2 / 4.1.2

- **Evidence:** `setAccessibleDescription occurrences: 0`

- **Suggested fix:** Add setAccessibleDescription() for fields or buttons whose purpose is not fully clear from their visible label.

### 2. No explicit tab order is declared

- **Category:** Keyboard navigation

- **Criterion:** WCAG 2.4.3

- **Evidence:** `setTabOrder occurrences: 0`

- **Suggested fix:** If the UI order is non-trivial, define setTabOrder() for forms and table/editing workflows.


## Passed checks

- Source inspected: 1 Python files and 1 Qt Designer .ui files.
- Table widgets were identified and included in the desktop audit surface.

## Suggested first fixes

1. Add setAccessibleName() to icon-only, ambiguous, or dynamically created controls; keep visible text for normal QPushButton/QLabel controls.
2. Use QLabel.setBuddy(inputWidget) for form labels, or set accessibleName on each field.

## Upstream work

- Repository: https://github.com/EDeev/school_table
- Suggested next action: prepare a small PR after manually reviewing widget names in `main.py` and `rasp.ui`.
