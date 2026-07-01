# Accessibility audit: TastyTales mobile app

## Target

- **Project:** tastytales/TastyTales
- **Type:** mobile / Flutter
- **Source:** https://gitflic.ru/project/tastytales/tastytales
- **Date:** 2026-07-01
- **Standards:** WCAG 2.1 AA principles, Mobile accessibility checklist, Flutter Semantics patterns

## Scope

Полный агентный аудит доступности по доступному коду, HTML/CSS/JS, структуре интерфейса и публичным страницам/ресурсам. Ручное тестирование со скринридером или физическим устройством относится к отдельному этапу и не смешивается с этим отчётом.

## Executive summary

- **Score:** 85/100
- **Grade:** B
- **Critical issues:** 1
- **Warnings:** 1
- **Informational:** 0

Flutter-приложение рецептов: нейтральный пример для демонстрации, как агент ищет риски в виджетах, формах, изображениях и кастомных tap targets.

## Critical issues

### 1. GestureDetector is used without any Semantics wrappers in the app code

- **Category:** Flutter semantics

- **Criterion:** WCAG 4.1.2 / mobile screen reader semantics

- **Evidence:** `GestureDetector: 10; Semantics: 0`

- **Suggested fix:** Wrap custom tap targets in Semantics(label: ..., button: true, child: ...), or replace with semantic controls such as ElevatedButton/IconButton/ListTile where appropriate.


## Warnings

### 1. Icon-only controls may lack accessible names

- **Category:** Controls

- **Criterion:** WCAG 4.1.2

- **Evidence:** `Icon widgets: 13; Tooltip: 0; Semantics: 0`

- **Suggested fix:** Use IconButton tooltip, Semantics labels, or visible text for icon-only actions.


## Informational findings

No findings in this severity group.

## Passed checks

- Text fields use InputDecoration/labelText patterns in the source.
- Source inspected: 18 Dart files under Flutter app code.
- Project has Flutter structure (`pubspec.yaml`, `lib/`, Android/iOS folders) suitable for static mobile audit.

## Suggested first fixes

1. Wrap custom tap targets in Semantics(label: ..., button: true, child: ...), or replace with semantic controls such as ElevatedButton/IconButton/ListTile where appropriate.
2. Use IconButton tooltip, Semantics labels, or visible text for icon-only actions.

## Upstream work

- Repository: https://gitflic.ru/project/tastytales/tastytales
- Suggested next action: open GitFlic issue or PR with Semantics/label improvements after reviewing exact screens.
