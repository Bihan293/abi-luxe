# Темы сайта

Внешний вид сайта полностью собран в этой папке. Логика, база и бот
(`app/`) не зависят от темы.

## Как переключить тему

В начале `site/theme.css` есть одна строка:

```css
@import url("themes/mono-noir.css");
```

Поменяйте её на нужный файл из папки `themes/`.

Всё. Для нового салона можно скопировать любой пресет в
`site/themes/my-theme.css` и менять только его.

## Что менять в теме

Готовые пресеты:

- `mono-noir.css` — текущий чёрно-белый стиль Abi Luxe;
- `dark-gold.css` — тёмный вариант шаблона;
- `light-pink.css` — светлый вариант шаблона.

В каждом файле меняются:

- `--font-body`, `--font-display` — шрифты;
- `--accent`, `--accent-rgb`, `--accent-light`, `--on-accent` — акцент и текст на нём;
- `--bg`, `--bg-deep`, `--bg-soft` — фон страницы;
- `--text`, `--text-rgb`, `--muted`, `--faint` — текст;
- `--line`, `--line-soft` — линии и рамки;
- `--surface*`, `--modal-bg`, `--select-bg` — карточки, поля, окна;
- `--hero-bg`, `--section-from`, `--section-to` — фоны секций;
- `--panel-rgb`, `--backdrop-rgb`, `--shadow-rgb` — прозрачные слои и тени;
- `--highlight-rgb` — светлые/тёмные блики на карточках;
- `--danger*`, `--success*` — ошибки и успешные статусы;
- `--card-bg*` — градиенты карточек;
- `--shot-1` … `--shot-6` — заглушки галереи.

Если меняете шрифт, обновите ссылку на Google Fonts в `site/index.html`
и `site/privacy.html`.
