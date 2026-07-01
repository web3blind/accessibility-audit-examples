# Аудит доступности: Культура.РФ

## Объект проверки

- **Проект:** Культура.РФ
- **Тип:** сайт / публичный URL
- **URL:** https://www.culture.ru/
- **Дата:** 2026-07-01
- **Стандарты и ориентиры:** WCAG 2.1 AA, практические проверки WCAG 2.2, принципы ГОСТ Р 52872-2019.

## Область проверки

Выполнен агентный аудит доступности по доступному HTML/CSS/JS, структуре интерфейса и публичным страницам. Ручная проверка скринридером или физическим устройством относится к отдельному этапу и не смешивается с этим отчётом.

## Краткий итог

- **Оценка:** 59/100
- **Уровень:** F
- **Критичные проблемы:** 2
- **Предупреждения:** 4
- **Информационные замечания:** 1

Проверены главная и разные типы страниц, найденные внутренним обходом. Агент смотрел HTML-структуру, заголовки, язык документа, изображения, кнопки, ссылки, формы и признаки ссылки перехода к основному содержимому. Всего проверено страниц: 45.

## Критичные проблемы

### 1. На одной из страниц отсутствует язык HTML-документа

- **Категория:** язык страницы
- **Критерий:** WCAG 3.1.1
- **Доказательство:** `https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: <html>`
- **Рекомендация:** добавить `<html lang="ru">` или другой корректный язык страницы.

### 2. На страницах трансляций есть изображения без `alt`

- **Категория:** изображения
- **Критерий:** WCAG 1.1.1
- **Доказательство:** `https://www.culture.ru/live: 68 images missing alt; sample: <img class="KRQ9s" src="https://cdn.culture.ru/images/e1a91bcf-8af7-5991-8f6f-4ca504fc75c2/w_324,h_200,c_fill,g_center/429ba7015377789918e4dd5a9f82fec5-jpg"/>`
- **Рекомендация:** добавить содержательные `alt` для информативных изображений или `alt=""` для декоративных.

## Предупреждения

### 1. На части страниц нет ровно одного `h1`

- **Категория:** заголовки
- **Критерий:** WCAG 1.3.1 / 2.4.6
- **Доказательство:** `https://www.culture.ru/: h1 count: 0`
- **Рекомендация:** использовать один `h1` для основной темы страницы, а разделы размечать более низкими уровнями заголовков.

### 2. У части изображений подозрительно пустые или слишком общие `alt`

- **Категория:** изображения
- **Критерий:** WCAG 1.1.1
- **Доказательство:** `https://www.culture.ru/: 43 suspicious alt values; sample: <img alt="" loading="lazy" width="976" height="513" decoding="async" data-nimg="1" class="styles_img__fl4IZ styles_img__d_Yw2" style="color:transparent" sizes="976px" srcSet="/_next/image?url=https%3A%2F%2Fcdn.culture.ru`
- **Рекомендация:** заменить общие `alt` на описания по содержанию изображения или явно пометить декоративные изображения через `alt=""`.

### 3. У некоторых элементов форм могут отсутствовать подписи

- **Категория:** формы
- **Критерий:** WCAG 1.3.1 / 3.3.2 / 4.1.2
- **Доказательство:** `https://www.culture.ru/: controls: 1, labels: 0, aria labels on controls: 0`
- **Рекомендация:** связать каждый `input`, `select`, `textarea` с видимой подписью или `aria-labelledby`.

### 4. Есть слишком общий текст ссылок

- **Категория:** ссылки
- **Критерий:** WCAG 2.4.4
- **Доказательство:** `https://www.culture.ru/s/vopros/durochka-s-pereulochka/: generic link labels: ['читать']`
- **Рекомендация:** делать текст ссылок самодостаточным, например «Подробнее о спектакле ...» вместо короткого «Подробнее» или «читать» без контекста.

## Информационные замечания

### 1. Статический скан не нашёл ссылку перехода к основному содержимому

- **Категория:** обход повторяющихся блоков
- **Критерий:** WCAG 2.4.1
- **Доказательство:** `https://www.culture.ru/: не найдены очевидные href/text признаки ссылки перехода к основному содержимому`
- **Рекомендация:** добавить ссылку перехода к основному содержимому, видимую при фокусе, если такой ссылки действительно нет.

## Что проверено и выглядит нормально

- Проверены 45 публичных страниц разных типов: афиша, архитектура, кино, главная, литература, трансляции, материалы, музеи, музыка, новости, чтение, спецпроекты, темы, посещение, видео.
- https://www.culture.ru/: Найден содержательный title: Культура.РФ. Портал культурного наследия, традиций народов России
- https://www.culture.ru/: Атрибут языка HTML присутствует.
- https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: Найден содержательный title: Курс «Как читать русскую классику»
- https://www.culture.ru/s/slovo-dnya/kompilyatsiya/: Найден содержательный title: Что означает слово «компиляция» и когда оно появилось?
- https://www.culture.ru/s/vopros/durochka-s-pereulochka/: Найден содержательный title: Кто такая «дурочка с переулочка»?
- https://www.culture.ru/materials/259206/pamyatka-uchastnikam-svo-i-chlenam-ikh-semei-o-vozmozhnosti-besplatnogo-posesheniya-meropriyatii-v-sfere-kultury: Найден содержательный title: Памятка участникам СВО и членам их семей о возможности бесплатного посещения мероприятий в сфере культуры
- https://www.culture.ru/materials/259206/pamyatka-uchastnikam-svo-i-chlenam-ikh-semei-o-vozmozhnosti-besplatnogo-posesheniya-meropriyatii-v-sfere-kultury: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259258/test-ugadaite-spektakl-po-eskizu: Найден содержательный title: Тест: угадайте спектакль по эскизу
- https://www.culture.ru/materials/259258/test-ugadaite-spektakl-po-eskizu: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259248/danse-macabre-tema-smerti-v-muzyke: Найден содержательный title: Danse macabre: тема смерти в музыке
- https://www.culture.ru/materials/259248/danse-macabre-tema-smerti-v-muzyke: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259246/test-ugadaite-region-rossii-po-ego-flagu: Найден содержательный title: Тест: угадайте регион России по его флагу
- https://www.culture.ru/materials/259246/test-ugadaite-region-rossii-po-ego-flagu: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259241/letnie-festivali-2026-goda-kino-dzhaz-performansy-i-knizhnye-yarmarki: Найден содержательный title: Летние фестивали 2026 года: кино, джаз, перформансы и книжные ярмарки
- https://www.culture.ru/materials/259241/letnie-festivali-2026-goda-kino-dzhaz-performansy-i-knizhnye-yarmarki: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259236/test-ugadaite-region-rossii-po-blyudu-nacionalnoi-kukhni: Найден содержательный title: Тест: угадайте регион России по блюду национальной кухни
- https://www.culture.ru/materials/259236/test-ugadaite-region-rossii-po-blyudu-nacionalnoi-kukhni: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/259232/khrupkoe-iskusstvo-istoriya-gusevskogo-khrustalnogo-zavoda: Найден содержательный title: Хрупкое искусство: история Гусевского хрустального завода
- https://www.culture.ru/materials/259232/khrupkoe-iskusstvo-istoriya-gusevskogo-khrustalnogo-zavoda: Атрибут языка HTML присутствует.
- https://www.culture.ru/themes/259191/proshai-lyubit-ne-obyazuisya-stikhi-o-rasstavanii: Найден содержательный title: «Прощай, любить не обязуйся»: стихи о расставании
- https://www.culture.ru/themes/259191/proshai-lyubit-ne-obyazuisya-stikhi-o-rasstavanii: Атрибут языка HTML присутствует.
- https://www.culture.ru/materials/258333/vo-sne-i-nayavu-kto-pomogal-traktovat-sny-tatyane-larinoi: Найден содержательный title: Во сне и наяву: кто помогал трактовать сны Татьяне Лариной
- https://www.culture.ru/materials/258333/vo-sne-i-nayavu-kto-pomogal-traktovat-sny-tatyane-larinoi: Атрибут языка HTML присутствует.
- https://www.culture.ru/themes/259221/sila-kultury-ob-iskusstve-pod-grokhot-pushek: Найден содержательный title: «Сила культуры»: об искусстве под грохот пушек
- https://www.culture.ru/themes/259221/sila-kultury-ob-iskusstve-pod-grokhot-pushek: Атрибут языка HTML присутствует.
- https://www.culture.ru/news: Найден содержательный title: Новости культуры: кино, театры, литература, музыка России
- https://www.culture.ru/news: Атрибут языка HTML присутствует.
- https://www.culture.ru/news/259260/20-iyulya-startuet-mezhdunarodnyi-sankt-peterburgskii-dzhazovyi-festival: Найден содержательный title: 20 июля стартует Международный Санкт-Петербургский джазовый фестиваль
- https://www.culture.ru/news/259260/20-iyulya-startuet-mezhdunarodnyi-sankt-peterburgskii-dzhazovyi-festival: Атрибут языка HTML присутствует.
- ...и ещё 50 положительных проверок по `title` / `lang` в полном JSON.

## Первые исправления

1. Использовать один `h1` для основной темы страницы.
2. Заменить общие или пустые `alt` на содержательные описания, а декоративные изображения помечать намеренно.
3. Связать поля форм с видимыми подписями или `aria-labelledby`.
4. Добавить `<html lang="ru">` там, где язык документа отсутствует.
5. Сделать текст ссылок самодостаточным.
6. Добавить `alt` для изображений без альтернативного текста.

## Upstream

- Публичный сайт: https://www.culture.ru/
- Следующий шаг: использовать `suggested-fixes.md` как черновик сообщения команде сайта; публичный исходный репозиторий в этом запуске не найден.
