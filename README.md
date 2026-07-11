<p align="center">
  <img src="assets/logo.png" width="128" height="128" alt="LangRuEn logo">
</p>

# LangRuEn

LangRuEn — macOS-утилита в menu bar для автоматического исправления раскладки клавиатуры RU/EN.

Приложение следит за набранными словами, определяет текст, введенный в неправильной раскладке, аккуратно исправляет его и помогает быстрее переключаться между русским и английским языками. LangRuEn создается в первую очередь для русскоязычных пользователей macOS, которые часто печатают в двух раскладках.

## Скачать

Последняя beta-сборка DMG:

[LangRuEn-Beta.dmg](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/LangRuEn-Beta.dmg)

> **Если macOS пишет, что DMG или приложение повреждено**
>
> Это beta-сборка без Apple notarization. Скачайте DMG из этого репозитория и выполните в Terminal:
>
> ```bash
> xattr -dr com.apple.quarantine ~/Downloads/LangRuEn-Beta.dmg
> open ~/Downloads/LangRuEn-Beta.dmg
> ```
>
> Если `LangRuEn.app` уже скопирован в `/Applications`:
>
> ```bash
> xattr -dr com.apple.quarantine /Applications/LangRuEn.app
> open /Applications/LangRuEn.app
> ```

## Для тестеров

Дорогие друзья, прошу протестировать LangRuEn.

Это маленькая macOS-утилита в menu bar, которая помогает, когда вы набрали текст не в той раскладке. Например, написали русское слово на английской раскладке или наоборот — программа пытается аккуратно исправить это автоматически. Еще она умеет переключать раскладку в email, URL, login и технических полях.

Для PC-клавиатур можно включить ручное переключение RU/EN в разделе `Настройки -> Клавиатура и мышь -> Клавиатура`. Доступны `Ctrl + Shift`, обычный `Alt + Shift` и `Alt + Shift (Mac-режим)` для клавиатур, где физический Alt определяется macOS как Command. Активным может быть только один вариант; по умолчанию все выключены.

Раздел `Клавиатура и мышь` также добавляет Windows-подобную прокрутку, настраиваемые скорость,
ускорение и плавность, переназначение дополнительных кнопок мыши, Windows-сочетания клавиш и
полные или частичные исключения для выбранных приложений. Все параметры применяются сразу, а
встроенные тестовые области помогают проверить события колеса, кнопок и клавиатуры.

Важно: сейчас это beta-версия для теста. Приложение пока не подписано Apple Developer ID, поэтому macOS может предупреждать, что программа скачана из интернета или не может проверить разработчика. Это ожидаемо для текущей тестовой сборки.

## Установка

1. Откройте скачанный DMG.
2. Перетащите `LangRuEn.app` в `Applications`.
3. Если macOS пишет, что приложение не может быть открыто:
   - `System Settings -> Privacy & Security -> Open Anyway`
   - или правый клик по приложению -> `Open`
4. Запустите LangRuEn из `Applications`.
5. Выдайте разрешения Input Monitoring и Accessibility, когда macOS попросит.

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
- Переключение RU/EN через `Ctrl + Shift` или один из режимов `Alt + Shift` для PC-клавиатур.
- Индикатор текущей раскладки в menu bar.
- `Esc` отменяет последнее исправление.
- Пользовательские слова и исключения.
- Авто English в email, URL, login и технических полях.
- История исправлений.
- Настройки и диагностика в одном окне.
- Windows-подобное направление, скорость, ускорение и плавность прокрутки.
- Переназначение дополнительных кнопок мыши и переключение рабочих столов Spaces.
- Windows-сочетания клавиш для PC-клавиатуры.
- Полные и частичные исключения по приложениям для прокрутки, мыши и клавиатуры.
- Живая проверка событий ввода в настройках.
- Публичный beta update-feed.

## Обновления

LangRuEn проверяет beta-обновления через публичный feed:

[update.json](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/update.json)

Автор: [almazbek@me.com](mailto:almazbek@me.com)

---

## English

LangRuEn is a macOS menu bar utility for automatic RU/EN keyboard layout correction.

It watches typed words, detects when text was entered in the wrong keyboard layout, corrects it, and helps quickly switch between Russian and English input. The app is designed for Russian-speaking macOS users who often type in both layouts.

PC keyboard users can enable manual RU/EN switching under `Settings -> Keyboard and Mouse -> Keyboard`. Available choices are `Ctrl + Shift`, regular `Alt + Shift`, and `Alt + Shift (Mac mode)` for keyboards whose physical Alt key is reported by macOS as Command. Only one option can be active, and all are disabled by default.

The `Keyboard and Mouse` section also provides Windows-style scrolling direction, configurable
speed, acceleration and smoothing, extra mouse-button remapping, Windows keyboard shortcuts, and
full or partial per-application exclusions. Settings apply immediately, with live test areas for
wheel, button and keyboard events.

### Download

Download the latest beta DMG:

[LangRuEn-Beta.dmg](https://github.com/almaziphone/LangRuEnUpdates/releases/download/beta/LangRuEn-Beta.dmg)

> **If macOS says the DMG or app is damaged**
>
> This beta build is not Apple-notarized yet. Download the DMG from this repository and run:
>
> ```bash
> xattr -dr com.apple.quarantine ~/Downloads/LangRuEn-Beta.dmg
> open ~/Downloads/LangRuEn-Beta.dmg
> ```
>
> If `LangRuEn.app` is already copied to `/Applications`:
>
> ```bash
> xattr -dr com.apple.quarantine /Applications/LangRuEn.app
> open /Applications/LangRuEn.app
> ```

### Tester Note

This is a beta build for testing. The app is not signed with an Apple Developer ID yet, so macOS may warn that it cannot verify the developer.

### Installation

1. Open the downloaded DMG.
2. Drag `LangRuEn.app` into `Applications`.
3. Launch LangRuEn from `Applications`.
4. Grant Input Monitoring and Accessibility permissions when macOS asks.

If macOS says the app can’t be opened:

- Open `System Settings -> Privacy & Security -> Open Anyway`
- or Control-click `LangRuEn.app` in `Applications`, then choose `Open`.

If macOS says the app is damaged, run:

```bash
xattr -dr com.apple.quarantine /Applications/LangRuEn.app
open /Applications/LangRuEn.app
```

Only do this if you downloaded the DMG from this repository.

### Features

- Automatic RU/EN layout correction.
- Optional `Ctrl + Shift` or Mac-mode-aware `Alt + Shift` RU/EN switching for PC keyboards.
- Menu bar indicator for the current layout.
- `Esc` cancels the last correction.
- Personal words and exclusions.
- Auto English for email, URL, login, and technical fields.
- Correction history.
- Settings and diagnostics in one window.
- Windows-style scrolling direction, speed, acceleration, and smoothing.
- Configurable extra mouse buttons and Space switching.
- Windows keyboard shortcuts for PC keyboards.
- Full and partial per-application exclusions for scrolling, mouse buttons, and keyboard mappings.
- Live input-event testing in Settings.
- Public beta update feed.
