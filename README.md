# amoCRM API v2 documentation

![amoCRM logo](./assets/amocrm-logo.png)  

Архив документации в формате HTML по REST API [amoCRM](https://www.amocrm.ru) **v2** (запросы к API отправляются на /api/v2/).  
В настоящее время актуальной версией является [REST API amoCRM **v4**](https://www.amocrm.ru/developers/content/crm_platform/api-reference) (запросы к API отправляются на /api/v4/).  

Данный архив был создан в связи с тем, что документация по REST API **v2** теперь недоступна на русскоязычной версии сайта amoCRM.
На англоязычной версии сайта эта документация перенесена в раздел [API V2 GENERAL METHODS](https://www.amocrm.com/developers/).

## Чтение в браузере

В корне репозитория лежит [`index.html`](./index.html) — просмотрщик архива:

- список всех разделов с фильтром (клавиша <kbd>/</kbd>);
- автоматическое оглавление текущей страницы с подсветкой раздела, на котором вы находитесь;
- «режим чтения»: скрывает шапку, меню, формы и виджеты сайта amoCRM (переключается кнопкой, выбор запоминается);
- ссылки между разделами (например, со страницы «Сделки» на «Контакты») и якорные ссылки открываются внутри архива, а не ведут на сайт amoCRM;
- прямые ссылки на раздел и место в нём: `#leads`, `#leads/8` (пункт оглавления), `#notes/note_types` (якорь);
- адаптивная вёрстка для телефона и тёмная тема интерфейса.

### Онлайн (GitHub Pages)

Документация доступна по адресу: **https://patriot.github.io/amocrm-api-v2-docs/**

Чтобы сайт заработал, GitHub Pages нужно один раз включить в настройках репозитория:
**Settings → Pages → Build and deployment → Source: Deploy from a branch**, ветка `master`, папка `/ (root)`.
Файл `.nojekyll` отключает обработку Jekyll, страницы публикуются как есть.

### Локально

```bash
git clone https://github.com/patriot/amocrm-api-v2-docs.git
cd amocrm-api-v2-docs
python3 -m http.server 8000
```

Затем откройте http://localhost:8000/ в браузере.
Можно открыть `index.html` и просто двойным щелчком, но тогда браузер запрещает просмотрщику доступ к содержимому страниц
(ограничение `file://`), и оглавление, режим чтения и переходы по внутренним ссылкам работать не будут.

## Документация по REST API amoCRM **v2**

Архив документации по REST API amoCRM **v2** в формате HTML (файлы лежат в папке [`docs`](./docs)):

- [Аккаунт](https://patriot.github.io/amocrm-api-v2-docs/#account) 
- [Авторизация](https://patriot.github.io/amocrm-api-v2-docs/#auth)
- [Компании](https://patriot.github.io/amocrm-api-v2-docs/#companies)
- [Контакты](https://patriot.github.io/amocrm-api-v2-docs/#contacts)
- [Сделки](https://patriot.github.io/amocrm-api-v2-docs/#leads)
- [События](https://patriot.github.io/amocrm-api-v2-docs/#notes)
- [Задачи](https://patriot.github.io/amocrm-api-v2-docs/#tasks)
- [Списки](https://patriot.github.io/amocrm-api-v2-docs/#catalogs)
- [Элементы списков](https://patriot.github.io/amocrm-api-v2-docs/#catalog-elements)
- [Неразобранное](https://patriot.github.io/amocrm-api-v2-docs/#unsorted)
- [Webhooks](https://patriot.github.io/amocrm-api-v2-docs/#webhooks)
- [Покупатели](https://patriot.github.io/amocrm-api-v2-docs/#customers)
- [Дополнительные поля](https://patriot.github.io/amocrm-api-v2-docs/#custom_fields)
- [Виджеты](https://patriot.github.io/amocrm-api-v2-docs/#widgets)
- [Товары](https://patriot.github.io/amocrm-api-v2-docs/#products)
- [Воронки и этапы продаж](https://patriot.github.io/amocrm-api-v2-docs/#pipelines)
- [Логирование звонков](https://patriot.github.io/amocrm-api-v2-docs/#calls-add)
- [Уведомление о звонке](https://patriot.github.io/amocrm-api-v2-docs/#call-event)
- [Коды ошибок](https://patriot.github.io/amocrm-api-v2-docs/#errors)
- [Ограничения и рекомендации](https://patriot.github.io/amocrm-api-v2-docs/#recommendations)

<a id="%D0%90%D0%B2%D1%82%D0%BE%D1%80"></a>
## Автор архива

© 2020 andrey-tech

<a id="%D0%9B%D0%B8%D1%86%D0%B5%D0%BD%D0%B7%D0%B8%D1%8F"></a>
## Лицензия

Данный архив документации распространяется на условиях лицензии [MIT](./LICENSE).
