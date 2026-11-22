# Карта жизни: приложение для iPhone и Android

Сборку делает бесплатный сервер GitHub, Mac не нужен.

## Структура
- `www/index.html` — весь интерфейс (стартовые напоминания: поиск `rem:[`)
- `.github/workflows/build-apps.yml` — сборка iOS (.ipa) и Android (.apk)
- `package.json`, `capacitor.config.json` — настройки Capacitor

## 1. Собрать
1. Загрузите все файлы в репозиторий (Add file → Upload files).
   Если папка `.github` не загрузилась: Add file → Create new file, имя `.github/workflows/build-apps.yml`, вставьте содержимое файла.
2. Вкладка Actions → Build apps → Run workflow (5–10 минут).
3. Скачайте артефакты: `KartaZhizni-ipa` (iPhone) и `KartaZhizni-apk` (Android).

## 2. Установить
- iPhone: Sideloadly или AltStore, затем Режим разработчика и доверие профилю. С бесплатным Apple ID — 7 дней.
- Android: откройте .apk на телефоне и разрешите установку из неизвестных источников.
