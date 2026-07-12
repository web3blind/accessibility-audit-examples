# International accessibility audit examples

Примеры по проектам вне российской/русскоязычной подборки.

Это не «доска позора», а библиотека конкретных паттернов: что было найдено, почему это мешает пользователям клавиатуры/скринридеров, и какой upstream fix или proposal был подготовлен.

## Cases

| Case | Type | Target | Report | Summary | Upstream |
|---|---|---|---|---|---|
| Vaadin Web Components — non-modal overlays | Web components / TypeScript | https://github.com/vaadin/web-components | [audit](web-vaadin-non-modal-overlays/audit.md) | [summary](web-vaadin-non-modal-overlays/summary.md) | [upstream](web-vaadin-non-modal-overlays/pr-or-issue.md) |
| Hermes Desktop — accessibility semantics | Desktop / Electron-like React surfaces | https://github.com/NousResearch/hermes-agent | [audit](desktop-hermes-semantics/audit.md) | [summary](desktop-hermes-semantics/summary.md) | [upstream](desktop-hermes-semantics/pr-or-issue.md) |
| IBM MCP Context Forge — admin UI modal and validation semantics | Web app / Admin UI | https://github.com/IBM/mcp-context-forge | [audit](web-ibm-mcp-context-forge-admin-ui/audit.md) | [summary](web-ibm-mcp-context-forge-admin-ui/summary.md) | [upstream](web-ibm-mcp-context-forge-admin-ui/pr-or-issue.md) |
| Amnezia Client — QML accessible labels | Desktop/mobile / Qt Quick QML | https://github.com/amnezia-vpn/amnezia-client | [audit](desktop-amnezia-client-qml-labels/audit.md) | [summary](desktop-amnezia-client-qml-labels/summary.md) | [upstream](desktop-amnezia-client-qml-labels/pr-or-issue.md) |
| Quasar Framework — QInput/QField error semantics | Web component library / Vue | https://github.com/quasarframework/quasar | [audit](web-quasar-field-error-aria/audit.md) | [summary](web-quasar-field-error-aria/summary.md) | [upstream](web-quasar-field-error-aria/pr-or-issue.md) |
| Ride The Lightning — auth feedback announcements | Web app / Angular | https://github.com/Ride-The-Lightning/RTL | [audit](web-rtl-auth-feedback-announcements/audit.md) | [summary](web-rtl-auth-feedback-announcements/summary.md) | [upstream](web-rtl-auth-feedback-announcements/pr-or-issue.md) |
| Conducky — form feedback announcements | Web app | https://github.com/mattstratton/conducky | [audit](web-conducky-form-feedback/audit.md) | [summary](web-conducky-form-feedback/summary.md) | [upstream](web-conducky-form-feedback/pr-or-issue.md) |
| Eventra — common form input error wiring | Web app / React + Spring Boot | https://github.com/SandeepVashishtha/Eventra | [audit](web-eventra-form-input-errors/audit.md) | [summary](web-eventra-form-input-errors/summary.md) | [upstream](web-eventra-form-input-errors/pr-or-issue.md) |
| La Suite numérique Docs — export select focus stop | Web app / document editor | https://github.com/suitenumerique/docs | [audit](web-suitenumerique-docs-export-select-focus/audit.md) | [summary](web-suitenumerique-docs-export-select-focus/summary.md) | [upstream](web-suitenumerique-docs-export-select-focus/pr-or-issue.md) |
| La Suite numérique UI Kit — dropdown menu semantics | Web component library / React | https://github.com/suitenumerique/ui-kit | [audit](web-suitenumerique-ui-kit-dropdowns/audit.md) | [summary](web-suitenumerique-ui-kit-dropdowns/summary.md) | [upstream](web-suitenumerique-ui-kit-dropdowns/pr-or-issue.md) |
| WindoM — GlassSelect keyboard navigation | Web app / React | https://github.com/YehudaBriskman/WindoM | [audit](web-windowm-glassselect-keyboard/audit.md) | [summary](web-windowm-glassselect-keyboard/summary.md) | [upstream](web-windowm-glassselect-keyboard/pr-or-issue.md) |
| WindoM — clickable widgets keyboard access | Web app / React | https://github.com/YehudaBriskman/WindoM | [audit](web-windowm-clickable-widgets/audit.md) | [summary](web-windowm-clickable-widgets/summary.md) | [upstream](web-windowm-clickable-widgets/pr-or-issue.md) |
| Codeversehub Website — skip link | Website / React | https://github.com/TheCodeVerseHub/Codeversehub-Website | [audit](web-codeverse-skip-link/audit.md) | [summary](web-codeverse-skip-link/summary.md) | [upstream](web-codeverse-skip-link/pr-or-issue.md) |
| Artigen — action sheet focus | Web app / React | https://github.com/MukundaKatta/artigen | [audit](web-artigen-action-sheet-focus/audit.md) | [summary](web-artigen-action-sheet-focus/summary.md) | [upstream](web-artigen-action-sheet-focus/pr-or-issue.md) |
| Vets Who Code App — form error feedback | Web app / React | https://github.com/Vets-Who-Code/vets-who-code-app | [audit](web-vets-who-code-form-errors/audit.md) | [summary](web-vets-who-code-form-errors/summary.md) | [upstream](web-vets-who-code-form-errors/pr-or-issue.md) |
| smrt-svelte — form feedback relationships | Web component library / Svelte | https://github.com/happyvertical/smrt | [audit](web-smrt-svelte-form-feedback/audit.md) | [summary](web-smrt-svelte-form-feedback/summary.md) | [upstream](web-smrt-svelte-form-feedback/pr-or-issue.md) |
| MindTab — writing assistant live region scope | Web app / writing assistant | https://github.com/AetherAssembly/MindTab | [audit](web-mindtab-live-region-scope/audit.md) | [summary](web-mindtab-live-region-scope/summary.md) | [upstream](web-mindtab-live-region-scope/pr-or-issue.md) |
| Drinkup — form control accessibility | Web app | https://github.com/johnnymackcodes/drinkup | [audit](web-drinkup-form-controls/audit.md) | [summary](web-drinkup-form-controls/summary.md) | [upstream](web-drinkup-form-controls/pr-or-issue.md) |
| DevTrack — visible focus styles | Web app | https://github.com/Priyanshu-byte-coder/devtrack | [audit](web-devtrack-focus-visible/audit.md) | [summary](web-devtrack-focus-visible/summary.md) | [upstream](web-devtrack-focus-visible/pr-or-issue.md) |
| Joplin website — keyboard focus indicator | Website / documentation site | https://github.com/laurent22/joplin | [audit](web-joplin-website-focus-indicator/audit.md) | [summary](web-joplin-website-focus-indicator/summary.md) | [upstream](web-joplin-website-focus-indicator/pr-or-issue.md) |
| Personal Planner — icon-only control labels | Web app | https://github.com/TemaDeveloper/personal_planner | [audit](web-personal-planner-icon-labels/audit.md) | [summary](web-personal-planner-icon-labels/summary.md) | [upstream](web-personal-planner-icon-labels/pr-or-issue.md) |
| PKP pkp-lib — FormHandler validation focus and error relationships | Web app framework / JavaScript form controller | https://github.com/pkp/pkp-lib | [audit](web-pkp-lib-formhandler-validation/audit.md) | [summary](web-pkp-lib-formhandler-validation/summary.md) | [upstream](web-pkp-lib-formhandler-validation/pr-or-issue.md) |
| Nextcloud iOS — share extension folder picker | Mobile / iOS | https://github.com/nextcloud/ios | [audit](mobile-nextcloud-ios-folder-picker/audit.md) | [summary](mobile-nextcloud-ios-folder-picker/summary.md) | [upstream](mobile-nextcloud-ios-folder-picker/pr-or-issue.md) |

## Not included

Некоторые найденные PR/issue намеренно не добавлены: нерелевантные изменения, не-accessibility PR, а также чувствительные домены, где публичный учебный пример может выглядеть неуместно.
