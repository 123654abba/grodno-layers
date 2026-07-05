# Grodno Layers

Одностраничный портфолио-проект о Гродно как городе исторических и архитектурных слоев. Сайт сделан без React, backend, сборщиков, внешних библиотек и внешних изображений. Визуальная часть построена на CSS: силуэт замка, карта маршрута, постеры-заглушки, glow-эффекты и карточки.

## Как открыть локально

Откройте файл `index.html` в браузере. Дополнительный сервер не нужен.

## Как опубликовать на GitHub Pages

1. Создайте репозиторий на GitHub.
2. Загрузите в него файлы `index.html`, `style.css`, `script.js`, `README.md`.
3. Откройте `Settings` → `Pages`.
4. В блоке `Build and deployment` выберите `Deploy from a branch`.
5. Выберите ветку `main` и папку `/root`, затем нажмите `Save`.

Через несколько минут GitHub Pages выдаст публичную ссылку на сайт.

## Где менять тексты

Основные тексты RU/EN находятся в `script.js`:

- объект `translations` отвечает за тексты на странице;
- объект `content` отвечает за подробные описания в модальных окнах.

Структура блоков страницы находится в `index.html`.

## Где менять контакты

Контакты находятся в футере файла `index.html`:

- `aihappyfuture@gmail.com`
- `@aihappyfuture`
- заглушки `GitHub: #` и `Telegram: #`

## Как добавить настоящие фотографии

Сейчас в галерее используются CSS-placeholder карточки. Чтобы заменить их на фотографии:

1. Создайте папку `images`.
2. Положите туда оптимизированные изображения, например `castle.jpg`, `kalozha.jpg`.
3. В `style.css` замените фон нужной карточки:

```css
.poster-castle {
  background:
    linear-gradient(180deg, transparent, rgba(0, 0, 0, 0.72)),
    url("images/castle.jpg") center / cover;
}
```

## Проверенные источники

Факты в проекте сформулированы осторожно и опираются на открытые источники:

- UNESCO Tentative Lists: SS. Boris and Gleb (Kalozha) Church in Hrodna — https://whc.unesco.org/en/tentativelists/1895/
- Belarus.by: Old Castle and New Castle in Grodno — https://www.belarus.by/en/travel/belarus-life/old-new-castles-grodno
- Grodno Museum: The Old Castle — https://grodno-museum.by/en/the-old-castle/
- Grodno Museum: The New Castle — https://grodno-museum.by/en/new-castle/
- Belarus.by: Architecture in Belarus — https://www.belarus.by/en/about-belarus/architecture

## Файлы проекта

- `index.html` — структура страницы.
- `style.css` — дизайн, адаптивность, CSS-иллюстрации и постеры.
- `script.js` — переключение RU/EN, модальные окна, активные точки маршрута, анимации появления, parallax.
- `README.md` — инструкция по запуску и публикации.
