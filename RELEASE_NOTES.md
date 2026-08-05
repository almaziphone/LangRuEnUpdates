# LangRuEn 0.3.0 Beta — сборка 28

## Что нового

- Добавлена отдельная настройка снимков экрана для PC-клавиатур: `Alt + Shift + 3/4/5` преобразуется в системные сочетания macOS.
- Поддержано копирование снимка в буфер обмена через дополнительный `Ctrl`.
- Исправлено случайное удаление слов: теперь русские, английские слова и исключения удаляются только по крестику.
- Плавная прокрутка обычного колеса мыши теперь работает по схеме Mos и синхронизируется с частотой экрана.
- Для вертикальной и горизонтальной осей можно отдельно включить плавную и обратную прокрутку.
- Добавлен режим `Симулировать трекпад (бета)` с фазами жеста и инерционным затуханием.
- Дополнительным кнопкам мыши можно назначить навигацию, средний клик, Mission Control, рабочий стол и переключение Spaces.
- Добавлены Windows-сочетания клавиш для PC-клавиатур и варианты переключения RU/EN через `Ctrl + Shift` и `Alt + Shift`.
- Исключения для приложений могут отключать весь модуль либо отдельно прокрутку, кнопки мыши и клавиатуру.
- Исправлено обучение новым словам после ручного переключения раскладки.
- Интерфейс прокрутки упрощён: технические ползунки убраны, оставлены понятные переключатели.

## Установка

1. Скачайте `LangRuEn-Beta.dmg` в разделе Assets.
2. Откройте DMG и перетащите `LangRuEn.app` в `Applications`.
3. Запускайте приложение только из `/Applications`.
4. Выдайте разрешения macOS:
   - `System Settings → Privacy & Security → Input Monitoring`
   - `System Settings → Privacy & Security → Accessibility`

## Если macOS пишет, что файл повреждён

Beta-сборка пока не notarized у Apple. Выполните в Terminal:

```bash
xattr -dr com.apple.quarantine ~/Downloads/LangRuEn-Beta.dmg
open ~/Downloads/LangRuEn-Beta.dmg
```

Если приложение уже находится в `/Applications`:

```bash
xattr -dr com.apple.quarantine /Applications/LangRuEn.app
open /Applications/LangRuEn.app
```

---

## What’s New

- Added a separate PC-keyboard screenshot option: `Alt + Shift + 3/4/5` now triggers the matching macOS screenshot shortcut.
- Holding `Ctrl` additionally copies supported screenshots to the clipboard.
- Fixed accidental dictionary deletion: Russian words, English words, and exclusions are now removed only with the `x` button.
- Mos-style smooth scrolling synchronized to the display refresh rate.
- Independent smooth and reverse scrolling switches for vertical and horizontal axes.
- Experimental `Simulate Trackpad (Beta)` mode with gesture phases and momentum.
- Configurable extra mouse buttons for navigation, Mission Control, desktop, and Spaces.
- Familiar Windows keyboard shortcuts and PC-style RU/EN switching.
- Full or partial per-application exclusions.
- Fixed new-word learning after manual keyboard layout switching.
- Simplified scrolling UI without technical sliders.
