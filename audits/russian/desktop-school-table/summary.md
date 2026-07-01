# Summary: School Table desktop app

- **Target:** EDeev/school_table
- **Type:** desktop / PyQt5
- **Score:** 88/100 (B)
- **Critical:** 0
- **Warnings:** 2
- **Info:** 2

## Top findings

1. **warning:** No explicit accessible names are set for widgets — Add setAccessibleName() to icon-only, ambiguous, or dynamically created controls; keep visible text for normal QPushButton/QLabel controls.
2. **info:** No accessible descriptions are provided — Add setAccessibleDescription() for fields or buttons whose purpose is not fully clear from their visible label.
3. **warning:** Form labels are not programmatically associated with inputs — Use QLabel.setBuddy(inputWidget) for form labels, or set accessibleName on each field.
4. **info:** No explicit tab order is declared — If the UI order is non-trivial, define setTabOrder() for forms and table/editing workflows.

## Public framing

Это пример агентного аудита: проверяется всё, что доступно по коду/структуре/публичным страницам. Ручная проверка скринридером — отдельный этап.

## Upstream

- PR: https://github.com/EDeev/school_table/pull/1
- Status: opened
