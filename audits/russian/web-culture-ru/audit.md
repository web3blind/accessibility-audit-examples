# Accessibility audit: Культура.РФ website

## Target

- **Project:** Культура.РФ
- **Type:** website / public URL
- **URL:** https://www.culture.ru/
- **Date:** 2026-07-01
- **Standards:** WCAG 2.1 AA, WCAG 2.2 practical checks, ГОСТ Р 52872-2019 principles

## Scope

Полный агентный аудит доступности по доступному коду, HTML/CSS/JS, структуре интерфейса и публичным страницам/ресурсам. Ручное тестирование со скринридером или физическим устройством относится к отдельному этапу и не смешивается с этим отчётом.

## Executive summary

- **Score:** 59/100
- **Grade:** F
- **Critical issues:** 2
- **Warnings:** 4
- **Informational:** 1

Многостраничный аудит: главная и разные типы страниц, найденные внутренним crawl. Проверены HTML-структура, заголовки, язык, изображения, кнопки, ссылки, формы и skip-link признаки. Всего страниц: 45.

## Critical issues

### 1. HTML document language is missing

- **Category:** Language

- **Criterion:** WCAG 3.1.1

- **Evidence:** `https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: <html>`

- **Suggested fix:** Add `<html lang="ru">` or the correct page language.

### 2. Images without alt attributes

- **Category:** Images

- **Criterion:** WCAG 1.1.1

- **Evidence:** `https://www.culture.ru/live: 68 images missing alt; sample: <img class="KRQ9s" src="https://cdn.culture.ru/images/e1a91bcf-8af7-5991-8f6f-4ca504fc75c2/w_324,h_200,c_fill,g_center/429ba7015377789918e4dd5a9f82fec5-jpg"/>`

- **Suggested fix:** Add meaningful alt text for informative images or `alt=""` for decorative images.


## Warnings

### 1. Page should have exactly one H1

- **Category:** Headings

- **Criterion:** WCAG 1.3.1 / 2.4.6

- **Evidence:** `https://www.culture.ru/: h1 count: 0`

- **Suggested fix:** Use one H1 for the page topic and lower heading levels for sections.

### 2. Images have generic or empty-looking alt text

- **Category:** Images

- **Criterion:** WCAG 1.1.1

- **Evidence:** `https://www.culture.ru/: 43 suspicious alt values; sample: <img alt="" loading="lazy" width="976" height="513" decoding="async" data-nimg="1" class="styles_img__fl4IZ styles_img__d_Yw2" style="color:transparent" sizes="976px" srcSet="/_next/image?url=https%3A%2F%2Fcdn.culture.ru`

- **Suggested fix:** Replace generic alt text with content-specific descriptions, or mark decorative images intentionally.

### 3. Some form controls may not have labels

- **Category:** Forms

- **Criterion:** WCAG 1.3.1 / 3.3.2 / 4.1.2

- **Evidence:** `https://www.culture.ru/: controls: 1, labels: 0, aria labels on controls: 0`

- **Suggested fix:** Associate every input/select/textarea with a visible label or aria-labelledby.

### 4. Generic link text is present

- **Category:** Links

- **Criterion:** WCAG 2.4.4

- **Evidence:** `https://www.culture.ru/s/vopros/durochka-s-pereulochka/: generic link labels: ['читать']`

- **Suggested fix:** Make link text self-contained, e.g. `Подробнее о спектакле ...` instead of `Подробнее`.


## Informational findings

### 1. Skip link was not detected by static scan

- **Category:** Bypass blocks

- **Criterion:** WCAG 2.4.1

- **Evidence:** `https://www.culture.ru/: No obvious skip-link href/text found`

- **Suggested fix:** Add a visible-on-focus skip link to the main content if absent.


## Passed checks

- Crawled 45 public pages across URL types: afisha, architecture, cinema, home, literature, live, materials, museums, music, news, read, s, themes, visit, watch.
- https://www.culture.ru/: Descriptive title present: Культура.РФ. Портал культурного наследия, традиций народов России
- https://www.culture.ru/: HTML lang attribute is present.
- https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: Descriptive title present: Курс «Как читать русскую классику»
- https://www.culture.ru/s/slovo-dnya/kompilyatsiya/: Descriptive title present: Что означает слово «компиляция» и когда оно появилось?
- https://www.culture.ru/s/vopros/durochka-s-pereulochka/: Descriptive title present: Кто такая «дурочка с переулочка»?
- https://www.culture.ru/materials/259206/pamyatka-uchastnikam-svo-i-chlenam-ikh-semei-o-vozmozhnosti-besplatnogo-posesheniya-meropriyatii-v-sfere-kultury: Descriptive title present: Памятка участникам СВО и членам их семей о возможности бесплатного посещения мероприятий в сфере культуры
- https://www.culture.ru/materials/259206/pamyatka-uchastnikam-svo-i-chlenam-ikh-semei-o-vozmozhnosti-besplatnogo-posesheniya-meropriyatii-v-sfere-kultury: HTML lang attribute is present.
- https://www.culture.ru/materials/259258/test-ugadaite-spektakl-po-eskizu: Descriptive title present: Тест: угадайте спектакль по эскизу
- https://www.culture.ru/materials/259258/test-ugadaite-spektakl-po-eskizu: HTML lang attribute is present.
- https://www.culture.ru/materials/259248/danse-macabre-tema-smerti-v-muzyke: Descriptive title present: Danse macabre: тема смерти в музыке
- https://www.culture.ru/materials/259248/danse-macabre-tema-smerti-v-muzyke: HTML lang attribute is present.
- https://www.culture.ru/materials/259246/test-ugadaite-region-rossii-po-ego-flagu: Descriptive title present: Тест: угадайте регион России по его флагу
- https://www.culture.ru/materials/259246/test-ugadaite-region-rossii-po-ego-flagu: HTML lang attribute is present.
- https://www.culture.ru/materials/259241/letnie-festivali-2026-goda-kino-dzhaz-performansy-i-knizhnye-yarmarki: Descriptive title present: Летние фестивали 2026 года: кино, джаз, перформансы и книжные ярмарки
- https://www.culture.ru/materials/259241/letnie-festivali-2026-goda-kino-dzhaz-performansy-i-knizhnye-yarmarki: HTML lang attribute is present.
- https://www.culture.ru/materials/259236/test-ugadaite-region-rossii-po-blyudu-nacionalnoi-kukhni: Descriptive title present: Тест: угадайте регион России по блюду национальной кухни
- https://www.culture.ru/materials/259236/test-ugadaite-region-rossii-po-blyudu-nacionalnoi-kukhni: HTML lang attribute is present.
- https://www.culture.ru/materials/259232/khrupkoe-iskusstvo-istoriya-gusevskogo-khrustalnogo-zavoda: Descriptive title present: Хрупкое искусство: история Гусевского хрустального завода
- https://www.culture.ru/materials/259232/khrupkoe-iskusstvo-istoriya-gusevskogo-khrustalnogo-zavoda: HTML lang attribute is present.
- https://www.culture.ru/themes/259191/proshai-lyubit-ne-obyazuisya-stikhi-o-rasstavanii: Descriptive title present: «Прощай, любить не обязуйся»: стихи о расставании
- https://www.culture.ru/themes/259191/proshai-lyubit-ne-obyazuisya-stikhi-o-rasstavanii: HTML lang attribute is present.
- https://www.culture.ru/materials/258333/vo-sne-i-nayavu-kto-pomogal-traktovat-sny-tatyane-larinoi: Descriptive title present: Во сне и наяву: кто помогал трактовать сны Татьяне Лариной
- https://www.culture.ru/materials/258333/vo-sne-i-nayavu-kto-pomogal-traktovat-sny-tatyane-larinoi: HTML lang attribute is present.
- https://www.culture.ru/themes/259221/sila-kultury-ob-iskusstve-pod-grokhot-pushek: Descriptive title present: «Сила культуры»: об искусстве под грохот пушек
- https://www.culture.ru/themes/259221/sila-kultury-ob-iskusstve-pod-grokhot-pushek: HTML lang attribute is present.
- https://www.culture.ru/news: Descriptive title present: Новости культуры: кино, театры, литература, музыка России
- https://www.culture.ru/news: HTML lang attribute is present.
- https://www.culture.ru/news/259260/20-iyulya-startuet-mezhdunarodnyi-sankt-peterburgskii-dzhazovyi-festival: Descriptive title present: 20 июля стартует Международный Санкт-Петербургский джазовый фестиваль
- https://www.culture.ru/news/259260/20-iyulya-startuet-mezhdunarodnyi-sankt-peterburgskii-dzhazovyi-festival: HTML lang attribute is present.
- https://www.culture.ru/news/259259/mamt-predstavlyaet-premeru-baleta-anna-karenina: Descriptive title present: МАМТ представляет премьеру балета «Анна Каренина»
- https://www.culture.ru/news/259259/mamt-predstavlyaet-premeru-baleta-anna-karenina: HTML lang attribute is present.
- https://www.culture.ru/news/259256/gid-po-festivalyu-leto-muzyka-muzei: Descriptive title present: Гид по фестивалю «Лето. Музыка. Музей»
- https://www.culture.ru/news/259256/gid-po-festivalyu-leto-muzyka-muzei: HTML lang attribute is present.
- https://www.culture.ru/news/259255/24-iyunya-v-ufe-sostoitsya-otkrytie-iii-vserossiiskoi-detskoi-folkloriady: Descriptive title present: 24 июня в Уфе состоится открытие III Всероссийской детской фольклориады
- https://www.culture.ru/news/259255/24-iyunya-v-ufe-sostoitsya-otkrytie-iii-vserossiiskoi-detskoi-folkloriady: HTML lang attribute is present.
- https://www.culture.ru/news/259254/v-muzee-arkhitektury-otkrylas-vystavka-fedor-shekhtel-grezy-russkogo-moderna: Descriptive title present: В Музее архитектуры открылась выставка «Федор Шехтель. Грезы русского модерна»
- https://www.culture.ru/news/259254/v-muzee-arkhitektury-otkrylas-vystavka-fedor-shekhtel-grezy-russkogo-moderna: HTML lang attribute is present.
- https://www.culture.ru/news/259252/stali-izvestny-pobediteli-konkursnoi-programmy-festivalya-arkhitekturnoe-nasledie: Descriptive title present: Стали известны победители конкурсной программы фестиваля «Архитектурное наследие»
- https://www.culture.ru/news/259252/stali-izvestny-pobediteli-konkursnoi-programmy-festivalya-arkhitekturnoe-nasledie: HTML lang attribute is present.
- https://www.culture.ru/visit: Descriptive title present: Посетить культурные объекты России
- https://www.culture.ru/visit: HTML lang attribute is present.
- https://www.culture.ru/read: Descriptive title present: Читать о культурном наследии России
- https://www.culture.ru/read: HTML lang attribute is present.
- https://www.culture.ru/watch: Descriptive title present: Смотреть лучшие фильмы, спектакли, лекции онлайн
- https://www.culture.ru/watch: HTML lang attribute is present.
- https://www.culture.ru/live: Descriptive title present: Смотреть прямые трансляции концертов, театров, лекций, фестивалей и экскурсий бесплатно. Видео трансляции онлайн. Культу
- https://www.culture.ru/live: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/162236/progulka-skvoz-vremya-lekciya-ob-istorii-kazanskogo-zoobotsada: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/162236/progulka-skvoz-vremya-lekciya-ob-istorii-kazanskogo-zoobotsada: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/161997/skazochnica-marfa-chitaet-skazki: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/161997/skazochnica-marfa-chitaet-skazki: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/162484/teatry-v-epokhu-cifrovykh-tekhnologii: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/162484/teatry-v-epokhu-cifrovykh-tekhnologii: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/162012/roza-i-solovei: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/162012/roza-i-solovei: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/162625/teatralnyi-arkhiv-intervyu-s-artistami: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/162625/teatralnyi-arkhiv-intervyu-s-artistami: HTML lang attribute is present.
- https://www.culture.ru/live/broadcast/162427/don-zhuan-seichas: Descriptive title present: Прямые трансляции: смотреть онлайн и бесплатно трансляции и записи концертов, лекций, фестивалей в разделе «Культурный с
- https://www.culture.ru/live/broadcast/162427/don-zhuan-seichas: HTML lang attribute is present.
- https://www.culture.ru/live/cinema/movies: Descriptive title present: Список фильмов: смотреть онлайн и бесплатно лучшие советские и зарубежные фильмы. Каталог классических фильмов.
- https://www.culture.ru/live/cinema/movies: HTML lang attribute is present.
- https://www.culture.ru/live/theaters/performances: Descriptive title present: Спектакли — смотреть бесплатно онлайн в хорошем качестве. Лучшие советские и российские спектакли на портале «Культура.Р
- https://www.culture.ru/live/theaters/performances: HTML lang attribute is present.
- https://www.culture.ru/live/music/concerts: Descriptive title present: Концерты онлайн
- https://www.culture.ru/live/music/concerts: HTML lang attribute is present.
- https://www.culture.ru/live/lectures/movies: Descriptive title present: Лекции онлайн бесплатно. Слушать интересные лекции. Видео на портале «Культура.РФ»
- https://www.culture.ru/live/lectures/movies: HTML lang attribute is present.
- https://www.culture.ru/museums/institutes/location-russia: Descriptive title present: Музеи России - список с фото, названиями и описаниями. Интересные музеи России на портале «Культура.РФ»
- https://www.culture.ru/museums/institutes/location-russia: HTML lang attribute is present.
- https://www.culture.ru/literature/books: Descriptive title present: Произведения российских писателей читать онлайн бесплатно. Скачать художественные книги русских авторов бесплатно на пор
- https://www.culture.ru/literature/books: HTML lang attribute is present.
- https://www.culture.ru/architecture/institutes/location-russia: Descriptive title present: Архитектурные объекты России - список с фото, названиями и описаниями. Интересные архитектурные объекты России на портал
- https://www.culture.ru/architecture/institutes/location-russia: HTML lang attribute is present.
- https://www.culture.ru/s/narody-rossii/: Descriptive title present: Народы России
- https://www.culture.ru/s/: Descriptive title present: Спецпроекты: лучшее о культурном наследии России
- https://www.culture.ru/s/mikhail-vrubel/: Descriptive title present: Михаил Врубель: «чертежи, похищенные у Вечности»
- https://www.culture.ru/afisha/russia: Descriptive title present: Афиша мероприятий России. Куда сходить в России — интересные культурные события и мероприятия
- https://www.culture.ru/afisha/russia: HTML lang attribute is present.
- https://www.culture.ru/cinema: Descriptive title present: Кино — смотреть фильмы онлайн бесплатно, без регистрации и смс. Видео фильмы в хорошем качестве прямо сейчас!

## Suggested first fixes

1. Use one H1 for the page topic and lower heading levels for sections.
2. Replace generic alt text with content-specific descriptions, or mark decorative images intentionally.
3. Associate every input/select/textarea with a visible label or aria-labelledby.
4. Add `<html lang="ru">` or the correct page language.
5. Make link text self-contained, e.g. `Подробнее о спектакле ...` instead of `Подробнее`.
6. Add meaningful alt text for informative images or `alt=""` for decorative images.

## Upstream work

- Public website: https://www.culture.ru/
- Suggested next action: use `suggested-fixes.md` as a message to the site team; no public source repository was found in this run.
