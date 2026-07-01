# Suggested fixes for Культура.РФ

This file summarizes the first practical fixes derived from the automated audit.

1. **Headings:** Use one H1 for the page topic and lower heading levels for sections.
   - Evidence: `https://www.culture.ru/: h1 count: 0`
2. **Images:** Replace generic alt text with content-specific descriptions, or mark decorative images intentionally.
   - Evidence: `https://www.culture.ru/: 43 suspicious alt values; sample: <img alt="" loading="lazy" width="976" height="513" decoding="async" data-nimg="1" class="styles_img__fl4IZ styles_img__d_Yw2" style="color:transparent" sizes="976px" srcSet="/_next/image?url=https%3A%2F%2Fcdn.culture.ru`
3. **Bypass blocks:** Add a visible-on-focus skip link to the main content if absent.
   - Evidence: `https://www.culture.ru/: No obvious skip-link href/text found`
4. **Forms:** Associate every input/select/textarea with a visible label or aria-labelledby.
   - Evidence: `https://www.culture.ru/: controls: 1, labels: 0, aria labels on controls: 0`
5. **Language:** Add `<html lang="ru">` or the correct page language.
   - Evidence: `https://www.culture.ru/s/kurs-kak-chitat-russkuyu-klassiku/: <html>`
6. **Links:** Make link text self-contained, e.g. `Подробнее о спектакле ...` instead of `Подробнее`.
   - Evidence: `https://www.culture.ru/s/vopros/durochka-s-pereulochka/: generic link labels: ['читать']`
7. **Images:** Add meaningful alt text for informative images or `alt=""` for decorative images.
   - Evidence: `https://www.culture.ru/live: 68 images missing alt; sample: <img class="KRQ9s" src="https://cdn.culture.ru/images/e1a91bcf-8af7-5991-8f6f-4ca504fc75c2/w_324,h_200,c_fill,g_center/429ba7015377789918e4dd5a9f82fec5-jpg"/>`
