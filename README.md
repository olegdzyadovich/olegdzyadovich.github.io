# Oleg Dzyadovich — Personal Portfolio

Минималистичный editorial-стайл портфолио-сайт на чистом HTML / CSS / JS. Без зависимостей и сборщиков.

## Локальный просмотр

```bash
cd portfolio
python3 -m http.server 8765
# открыть http://localhost:8765
```

## Деплой на GitHub Pages

1. Создать репо на GitHub: `olegdzyadovich.github.io` (именно такое имя — это user site).
2. Скопировать содержимое папки `portfolio/` в репо.
3. `git push` в `main`.
4. Settings → Pages → Source: `main` / root → Save.
5. Через ~1 минуту сайт откроется на `https://olegdzyadovich.github.io`.

## Свой домен (позже)

Settings → Pages → Custom domain → вписать `olegdzyadovich.com`. В DNS провайдере добавить CNAME на `olegdzyadovich.github.io`.

## Структура

- `index.html` — весь сайт одним файлом (HTML + inline CSS + inline JS)
- `Resume_Oleg_Dzyadovich.pdf` — PDF для скачивания

## Wow-эффекты (что где в коде)

| Эффект | Где |
|---|---|
| Cursor spotlight | `.spotlight` + `animateSpotlight()` |
| Reading progress bar | `.progress` + scroll listener |
| Role scramble / rotator | `scrambleTo()` + `rotateRoles()` |
| Scroll reveal | `.reveal` + `IntersectionObserver` |
| Timeline draw-on-scroll | `#timeline-line` + `updateTimeline()` |
| Magnetic buttons | `.magnetic` + mousemove listeners |
| Dark / Light theme | `data-theme` + `localStorage` |
