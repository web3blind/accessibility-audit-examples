# Summary: TastyTales mobile app

- **Target:** tastytales/TastyTales
- **Type:** mobile / Flutter
- **Score:** 85/100 (B)
- **Critical:** 1
- **Warnings:** 1
- **Info:** 0

## Top findings

1. **critical:** GestureDetector is used without any Semantics wrappers in the app code — Wrap custom tap targets in Semantics(label: ..., button: true, child: ...), or replace with semantic controls such as ElevatedButton/IconButton/ListTile where appropriate.
2. **warning:** Icon-only controls may lack accessible names — Use IconButton tooltip, Semantics labels, or visible text for icon-only actions.

## Public framing

Это пример агентного аудита: проверяется всё, что доступно по коду/структуре/публичным страницам. Ручная проверка скринридером — отдельный этап.
