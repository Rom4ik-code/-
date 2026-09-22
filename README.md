# Фавиконки для HydraMan — 5 вариантов

Файл `preview.png` — картинка со всеми вариантами рядом, чтобы выбрать один.

1. **drop-square** — капля на фиолетовом квадрате со скруглёнными углами (максимально похоже на текущий логотип сайта).
2. **drop-circle** — та же капля, но фон — круг.
3. **drop-gradient** — капля на фиолетовом градиенте (более «живой» вариант).
4. **monogram-h** — буква «H» (HydraMan) на фиолетовом квадрате.
5. **drop-wrench** — капля с маленьким значком гаечного ключа — более явно про сантехнику.

В папке `sets/<название>/` для каждого варианта лежит полный комплект файлов:
- `favicon.ico` — классическая иконка (16/32/48 px, для старых браузеров и вкладки)
- `favicon-16x16.png`, `favicon-32x32.png`, `favicon-48x48.png`
- `apple-touch-icon.png` (180×180) — иконка при добавлении сайта на экран iPhone/iPad
- `android-chrome-192x192.png`, `android-chrome-512x512.png` — для Android и PWA

## Как подключить выбранный вариант к сайту

Просто скажите мне, какой вариант понравился (например «нравится вариант 1» или «drop-circle») — я сам добавлю нужные файлы и теги в `index.html` и опубликую обновлённую версию сайта.

Если захотите сделать это вручную самостоятельно (например, уже на GitHub):
1. Скопируйте файлы из папки `sets/<название>` в корень репозитория (рядом с `index.html`).
2. Добавьте в `<head>` файла `index.html` эти строки:

```html
<link rel="icon" href="favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="192x192" href="android-chrome-192x192.png">
```
