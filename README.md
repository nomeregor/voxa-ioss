# Voxa для iOS

Мессенджер Voxa в оболочке Capacitor. Вся логика приложения лежит в `www/index.html`.

## Как получить .ipa (без Mac)
1. Создай репозиторий на GitHub и загрузи в него всё содержимое этой папки (включая скрытую папку `.github`).
2. Вкладка **Actions** → **iOS unsigned build** → **Run workflow**.
3. Когда сборка станет зелёной, открой её и скачай артефакт **Voxa-ipa** (внутри `Voxa.ipa`).
4. На Windows установи iTunes и iCloud с apple.com (не из Microsoft Store) и Sideloadly (sideloadly.io).
5. Подключи iPhone, перетащи `Voxa.ipa` в Sideloadly, введи Apple ID, нажми Start.
6. На iPhone: Настройки → Основные → VPN и управление устройством → доверься профилю; включи Режим разработчика.

С бесплатным Apple ID приложение работает 7 дней, потом нужно переустановить. Push при закрытом приложении без платного аккаунта Apple Developer не работает.

## Обновление приложения
Замени `www/index.html` и снова запусти workflow.
