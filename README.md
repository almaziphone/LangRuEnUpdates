<p align="center">
  <img src="assets/logo.png" width="128" height="128" alt="LangRuEn logo">
</p>

# LangRuEn

LangRuEn — macOS-утилита в menu bar для автоматического исправления раскладки клавиатуры RU/EN.

Приложение следит за набранными словами, определяет текст, введенный в неправильной раскладке, аккуратно исправляет его и помогает быстрее переключаться между русским и английским языками. LangRuEn создается в первую очередь для русскоязычных пользователей macOS, которые часто печатают в двух раскладках.

## Скачать

Последняя beta-сборка DMG:

[LangRuEn-Beta.dmg](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/LangRuEn-Beta.dmg)

## Для тестеров

Дорогие друзья, прошу протестировать LangRuEn.

Это маленькая macOS-утилита в menu bar, которая помогает, когда вы набрали текст не в той раскладке. Например, написали русское слово на английской раскладке или наоборот — программа пытается аккуратно исправить это автоматически. Еще она умеет переключать раскладку в email, URL, login и технических полях.

Важно: сейчас это beta-версия для теста. Приложение пока не подписано Apple Developer ID, поэтому macOS может предупреждать, что программа скачана из интернета или не может проверить разработчика. Это ожидаемо для текущей тестовой сборки.

## Установка

1. Откройте скачанный DMG.
2. Перетащите `LangRuEn.app` в `Applications`.
3. Запустите LangRuEn из `Applications`.
4. Выдайте разрешения Input Monitoring и Accessibility, когда macOS попросит.

## Если macOS ругается

Так как сборка пока неподписанная, macOS может показать предупреждение.

Попробуйте сначала обычный способ:

1. Откройте `Applications`.
2. Найдите `LangRuEn.app`.
3. Нажмите по приложению с зажатым `Control` или правой кнопкой.
4. Выберите `Open / Открыть`.
5. В появившемся окне снова нажмите `Open / Открыть`.

Если macOS пишет, что приложение повреждено или не может быть открыто, выполните в Terminal:

```bash
xattr -dr com.apple.quarantine /Applications/LangRuEn.app
open /Applications/LangRuEn.app
```

Используйте эту команду только если скачали `LangRuEn-Beta.dmg` отсюда, из этого репозитория.

После первого запуска macOS попросит разрешения:

- `Input Monitoring` — чтобы LangRuEn видел нажатия клавиш и мог понять, что раскладка была неверной.
- `Accessibility` — чтобы программа могла аккуратно исправлять уже набранный текст.

Без этих разрешений автоисправление работать не будет.

## Возможности

- Автоматическое исправление раскладки RU/EN.
- Индикатор текущей раскладки в menu bar.
- `Esc` отменяет последнее исправление.
- Пользовательские слова и исключения.
- Авто English в email, URL, login и технических полях.
- История исправлений.
- Настройки и диагностика в одном окне.
- Публичный beta update-feed.

## Обновления

LangRuEn проверяет beta-обновления через публичный feed:

[update.json](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/update.json)

Автор: [almazbek@me.com](mailto:almazbek@me.com)

---

## English

LangRuEn is a macOS menu bar utility for automatic RU/EN keyboard layout correction.

It watches typed words, detects when text was entered in the wrong keyboard layout, corrects it, and helps quickly switch between Russian and English input. The app is designed for Russian-speaking macOS users who often type in both layouts.

### Download

Download the latest beta DMG:

[LangRuEn-Beta.dmg](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/LangRuEn-Beta.dmg)

### Tester Note

This is a beta build for testing. The app is not signed with an Apple Developer ID yet, so macOS may warn that it cannot verify the developer.

### Installation

1. Open the downloaded DMG.
2. Drag `LangRuEn.app` into `Applications`.
3. Launch LangRuEn from `Applications`.
4. Grant Input Monitoring and Accessibility permissions when macOS asks.

If macOS refuses to open the app, try Control-clicking `LangRuEn.app` in `Applications`, then choose `Open`.

If macOS says the app is damaged, run:

```bash
xattr -dr com.apple.quarantine /Applications/LangRuEn.app
open /Applications/LangRuEn.app
```

Only do this if you downloaded the DMG from this repository.

### Features

- Automatic RU/EN layout correction.
- Menu bar indicator for the current layout.
- `Esc` cancels the last correction.
- Personal words and exclusions.
- Auto English for email, URL, login, and technical fields.
- Correction history.
- Settings and diagnostics in one window.
- Public beta update feed.
