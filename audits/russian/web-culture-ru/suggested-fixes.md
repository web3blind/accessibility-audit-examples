# Рекомендованные исправления для Культура.РФ

Файл собирает первые практические исправления по результатам агентного аудита.

1. **Заголовки:** использовать один `h1` для основной темы страницы, а разделы размечать более низкими уровнями заголовков.
   - Доказательство: `https://www.culture.ru/: h1 count: 0`
2. **Изображения:** заменить общие или пустые `alt` на содержательные описания; декоративные изображения помечать намеренно через `alt=""`.
   - Доказательство: `https://www.culture.ru/: 43 suspicious alt values; sample: <img alt="" loading="lazy" width="976" height="513" decoding="async" data-nimg="1" class="styles_img__fl4IZ styles_img__d_Yw2" style="color:transparent" sizes="976px" srcSet="/_next/image?url=https%3A%2F%2Fcdn.culture.ru`
3. **Переход к основному содержимому:** добавить ссылку, видимую при фокусе, если её действительно нет.
   - Доказательство: `https://www.culture.ru/: не найдены очевидные href/text признаки ссылки перехода к основному содержимому`
4. **Формы:** связать каждый `input`, `select`, `textarea` с видимой подписью или `aria-labelledby`.
   - Доказательство: `https://www.culture.ru/: controls: 1, labels: 0, aria labels on controls: 0`
5. **Язык страницы:** добавить `<html lang="ru">` или другой корректный язык страницы.
   - Доказательство: `https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: <html>`
6. **Текст ссылок:** делать ссылки самодостаточными, например «Подробнее о спектакле ...» вместо короткого «Подробнее» или «читать» без контекста.
   - Доказательство: `https://www.culture.ru/s/vopros/durochka-s-pereulochka/: generic link labels: ['читать']`
7. **Изображения без `alt`:** добавить содержательный `alt` для информативных изображений или `alt=""` для декоративных.
   - Доказательство: `https://www.culture.ru/live: 68 images missing alt; sample: <img class="KRQ9s" src="https://cdn.culture.ru/images/e1a91bcf-8af7-5991-8f6f-4ca504fc75c2/w_324,h_200,c_fill,g_center/429ba7015377789918e4dd5a9f82fec5-jpg"/>`
