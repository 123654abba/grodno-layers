# New Castle Grodno

Одностраничный портфолио-проект о Новом замке в Гродно. Концепт больше не работает как общий справочник по городу: главный герой сайта — одно здание, его политическая история, архитектурный замысел и современная музейная память.

## Что внутри

- история появления королевского дворца;
- строительство 1737–1742 годов;
- первый сейм во дворце в 1744 году;
- последний сейм Речи Посполитой в 1793 году;
- современное восприятие замка как музейного и исторического места;
- RU/EN-переключатель;
- интерактивные главы, модальные окна, хронология, визуальные CSS-постеры и схема чтения здания.

## Как открыть локально

Откройте `index.html` в браузере. Сборщик и backend не нужны.

## Как опубликовать на GitHub Pages

1. Загрузите `index.html`, `style.css`, `script.js`, `README.md` в репозиторий.
2. Откройте `Settings` → `Pages`.
3. Выберите `Deploy from a branch`.
4. Укажите ветку `main` и папку `/root`.
5. Сохраните настройки.

## Где менять тексты

Основные тексты находятся в `script.js`:

- `translations` — тексты интерфейса RU/EN;
- `content` — подробные тексты для модальных окон.

Структура страницы находится в `index.html`, визуальный стиль — в `style.css`.

## Как развивать визуал

Сейчас сайт не использует внешние изображения: все сделано через CSS, чтобы не было случайных или неподходящих картинок. Для следующего этапа можно заменить CSS-placeholder на настоящие фотографии Нового замка, планы, архивные изображения или авторские иллюстрации.

Пример замены постера:

```css
.poster-castle {
  background:
    linear-gradient(180deg, transparent, rgba(0, 0, 0, 0.72)),
    url("images/new-castle.jpg") center / cover;
}
```

## Проверенные источники

- Grodno Museum: The New Castle — https://grodno-museum.by/en/new-castle/
- Belarus.by: Old Castle and New Castle in Grodno — https://www.belarus.by/en/travel/belarus-life/old-new-castles-grodno
- Grodno Museum: The Old Castle — https://grodno-museum.by/en/the-old-castle/
- Belarus.by: Grodno Oblast Landmarks — https://www.belarus.by/en/travel/belarus-life/sightseeing/tourist-attraction-grodno

## Файлы

- `index.html` — структура сайта.
- `style.css` — визуальный стиль, адаптивность, CSS-иллюстрации.
- `script.js` — тексты, RU/EN, модалки, интерактивные точки, анимации.
- `README.md` — описание проекта и инструкция.
