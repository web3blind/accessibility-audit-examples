# Accessibility audit examples

Репозиторий с примерами агентного аудита доступности реальных интерфейсов: desktop, mobile и web.

Цель — показать типовые проблемы, способы проверки и возможные исправления на реальных русскоязычных/российских проектах, без формата «доски позора».

## Cases

| Case | Type | Target | Report | Summary | Upstream |
|---|---|---|---|---|---|
| School Table | Desktop / PyQt5 | https://github.com/EDeev/school_table | [audit](audits/desktop-school-table/audit.md) | [summary](audits/desktop-school-table/summary.md) | PR candidate |
| TastyTales | Mobile / Flutter | https://gitflic.ru/project/tastytales/tastytales | [audit](audits/mobile-tastytales/audit.md) | [summary](audits/mobile-tastytales/summary.md) | issue/PR candidate |
| Культура.РФ | Website | https://www.culture.ru/ | [audit](audits/web-culture-ru/audit.md) | [summary](audits/web-culture-ru/summary.md) | suggested fixes |

## Method

Аудиты выполнены агентом по доступному коду, HTML/CSS/JS, структуре интерфейса и публичным страницам. Проверяется всё, что можно проверить агентно по доступным источникам. Ручное тестирование со скринридером или физическим устройством — отдельный этап и не смешивается с этими отчётами.

## Status

Generated on 2026-07-01. Upstream PR/issue links will be added after review of the generated reports and minimal patches.
