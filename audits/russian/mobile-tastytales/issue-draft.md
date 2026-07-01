# Черновик предложения по доступности для TastyTales

## Кратко

Статический аудит Flutter-кода показал, что в приложении есть кастомные области нажатия через `GestureDetector`, но не найдены соответствующие обёртки `Semantics`. Также есть риск, что элементы только с иконками не получают понятные доступные имена для TalkBack/VoiceOver.

## Доказательства

- `lib/screens/loginScreen.dart`: области навигации по нажатию используют `GestureDetector`.
- `lib/screens/profileScreen.dart`: действия в профиле используют `GestureDetector`.
- `lib/screens/myrecipesScreen.dart`: действие с рецептом использует `GestureDetector`.
- Поиск по проекту: `GestureDetector` найден, а `Semantics(` / `semanticLabel` в `lib/` не найдены.

## Предлагаемое исправление

- По возможности использовать семантические виджеты: `IconButton`, `ElevatedButton`, `ListTile`.
- Если `GestureDetector` действительно нужен, оборачивать область нажатия в `Semantics(label: ..., button: true, child: ...)`.
- Для кнопок только с иконкой добавлять `tooltip` или явную подпись через `Semantics`.

## Проверка

Это предложение основано на агентном аудите исходного кода. Ручную проверку TalkBack/VoiceOver можно провести отдельным последующим этапом.
