# Accessibility audit examples

Репозиторий с примерами агентного аудита доступности реальных интерфейсов: desktop, mobile и web.

Цель — показать типовые проблемы, способы проверки и возможные исправления на реальных проектах, без формата «доски позора».

## Collections

- [Russian / русскоязычные и российские примеры](audits/russian/README.md)
- [International / другие проекты](audits/international/README.md)

## Current cases

| Collection | Case | Type | Target | Report | Summary | Upstream |
|---|---|---|---|---|---|---|
| Russian | School Table | Desktop / PyQt5 | https://github.com/EDeev/school_table | [audit](audits/russian/desktop-school-table/audit.md) | [summary](audits/russian/desktop-school-table/summary.md) | [PR #1](https://github.com/EDeev/school_table/pull/1) |
| Russian | TastyTales | Mobile / Flutter | https://gitflic.ru/project/tastytales/tastytales | [audit](audits/russian/mobile-tastytales/audit.md) | [summary](audits/russian/mobile-tastytales/summary.md) | [issue draft](audits/russian/mobile-tastytales/issue-draft.md) |
| Russian | Культура.РФ | Website | https://www.culture.ru/ | [audit](audits/russian/web-culture-ru/audit.md) | [summary](audits/russian/web-culture-ru/summary.md) | [contact draft](audits/russian/web-culture-ru/contact-draft.md) |

## Method

Аудиты выполнены агентом по доступному коду, HTML/CSS/JS, структуре интерфейса и публичным страницам. Проверяется всё, что можно проверить агентно по доступным источникам. Ручное тестирование со скринридером или физическим устройством — отдельный этап и не смешивается с этими отчётами.

