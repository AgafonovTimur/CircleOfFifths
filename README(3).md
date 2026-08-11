# Circle of Fifths / Круг квинт / 五度圈

Interactive circle-of-fifths trainer — single self-contained HTML file, no build, no server, no dependencies.

## 🌐 Languages / Языки / 语言

- [🇷🇺 Русский](#ru)
- [🇬🇧 English](#en)
- [🇨🇳 中文](#zh)

---

<a id="ru"></a>
## 🇷🇺 Русский

### Что это

Одностраничное HTML-приложение (открывается в любом браузере, без установки) — интерактивный круг квинт для изучения аккордов и ладов, а также для тренировки слуха/памяти на ноты и аккорды. Работает мышью, с компьютерной клавиатуры и с настоящей MIDI-клавиатуры.

Три основных режима переключаются вкладками сверху экрана:

- **Обучение** — на круге стрелками или цветом показывается состав выбранного аккорда/лада относительно тоники.
- **Ноты** — тренировка на распознавание/выбор нот на мажорном и минорном кольце круга.
- **Аккорды/Лады** — тренировка на аккорды и лады с теми же способами ответа, что и в «Нотах».

### Функции приложения

- **Обучение**
  - Два независимых «варианта» показа подсказки — Вариант 1 и Вариант 2, каждый переключается между отображением **стрелками** и **цветом**.
  - 20 типов аккордов: обычные трезвучия (мажор/минор), sus2, sus4, доминантовые/большие/минорные септ-, нон-, ундецим- и терцдецимаккорды и их варианты (7, maj7, m7, m(Maj7), add9, m(add9), 9, maj9, m9, m(Maj9), add11, m(add11), 11, maj11, m11, 13, maj13, m13, m(Maj13)).
  - 7 диатонических ладов: лидийский, мажор (ионийский), миксолидийский, дорийский, минор (эолийский), фригийский, локрийский.
  - Клавиатура-подсказка (пианино) рядом с кругом, её можно скрыть/показать.
  - Подпись выбранного аккорда/лада по центру круга.
  - Поворот круга стрелками влево/вправо (шаг 30°).
- **Ноты и Аккорды/Лады (Практика)**
  - Ответ **кликом мыши** по кругу или игрой на **MIDI/компьютерной клавиатуре**.
  - Выбор набора нот (мажор/минор) или набора типов аккордов/ладов, по которым будут задаваться вопросы; кнопка «Убрать все».
  - Опциональный показ клавиатуры-пианино (в разделе «Аккорды/Лады»).
- **Общее**
  - Зум круга: клавиши **+/-**, жест тремя/четырьмя пальцами на тачскрине, либо кнопки в интерфейсе.
  - Панель настроек можно закрепить сбоку от круга (десктоп) или использовать как выезжающую снизу шторку (мобильные устройства) — открывается колесом мыши / свайпом / клавишей.
  - Подключение внешней **MIDI-клавиатуры** (до 7 входов одновременно) для ответа нотами/аккордами.
  - **Вывод в DAW**: проигрывание выбранного аккорда во внешний синтезатор/DAW — все ноты сразу или по очереди с заданным интервалом, с настраиваемой velocity, в формате MIDI 1.0 (1–127) или MIDI 2.0 (1–65536), с возможностью развести ноты аккорда по разным MIDI-каналам.
  - Переключение энгармонических альтернативных названий нот (например A♯/B♭) отдельно для мажорного и минорного колец.
  - Система названий нот: буквенная (ABC) или слоговая (до-ре-ми).
  - Интерфейс на 3 языках (русский/английский/китайский) и тёмная/светлая тема оформления.
  - Все настройки и выбранный язык/тема сохраняются в localStorage браузера и восстанавливаются при следующем открытии.

### Горячие клавиши

Работают по физическому расположению клавиш, поэтому одинаково действуют и на русской, и на английской раскладке.

| Клавиша | Действие |
|---|---|
| `A`…`G` | Выбрать ноту на круге (натуральная); повторное нажатие той же буквы переключает мажор ↔ минор |
| `Shift` + `A`…`G` | Выбрать диезную ноту (♯) |
| `Space`, затем `A`…`G` | Выбрать бемольную ноту (♭) |
| `1`…`9`, `0` | Выбрать тип аккорда (позиции 1–10 в списке) |
| `Space`, затем `1`…`9`/`0` | Выбрать тип аккорда из «второй страницы» (позиции 11–20) |
| `+` / `=` | Увеличить круг (зум) |
| `-` | Уменьшить круг (зум) |
| `Shift` + `-` | Сбросить зум |
| `Q` / `Й` | Обучение: Вариант 1 — «стрелками» |
| `W` / `Ц` | Обучение: Вариант 1 — «цветом» |
| `R` / `К` | Обучение: Вариант 2 — «стрелками» |
| `T` / `Е` | Обучение: Вариант 2 — «цветом» |
| `Y` / `Н` | Открыть/закрыть панель настроек |
| `Z` / `Я` | Аккорды/Лады: показать/скрыть подсказку (только в этом разделе) |
| `←` / `→` | Обучение: повернуть круг на 30° влево/вправо |
| Колесо мыши вверх/вниз | Открыть/закрыть панель настроек (десктоп) |
| Свайп вверх/вниз по экрану | Открыть/закрыть панель настроек (мобильные) |
| 2 пальца — короткий тап | Открыть/закрыть панель настроек (тачскрин) |
| 3 пальца — короткий тап | Увеличить круг (зум) |
| 4 пальца — короткий тап | Уменьшить круг (зум) |

Буквенные хоткеи нот работают в «Обучении» всегда, а в разделе «Ноты» — только если выбран способ ответа «На MIDI/ПК клавиатуре» (в режиме «Клик мыши» они отключены). Цифровые хоткеи аккордов работают в «Обучении» и в «Аккордах/Ладах».

### Что можно поменять через меню

Открывается клавишей `Y`/`Н`, колесом мыши, свайпом или значком настроек:

- Закрепить панель настроек сбоку от круга (только десктоп).
- Способ ответа: клик мыши / MIDI-ПК клавиатура (разделы «Ноты», «Аккорды/Лады»).
- Набор нот (мажор/минор), набор типов аккордов, набор ладов — какие именно варианты участвуют в тренировке.
- Показ/скрытие клавиатуры-пианино.
- Показ букв аккорда под нотами, показ ступеней аккорда, привязка тональности (в «Обучении»).
- Количество одновременных MIDI-входов (1–7), выбор конкретного MIDI-порта, выбор MIDI-выхода для DAW, подключение/переподключение MIDI-клавиатуры.
- Настройки вывода в DAW: играть аккорд сразу или по очереди, интервал между нотами (сек), velocity, формат MIDI 1.0/2.0, разделение сигнала по каналам.
- Альтернативные (энгармонические) названия нот — отдельно для мажорного и минорного кольца.
- Система названия нот: ABC или до-ре-ми.
- Язык интерфейса: русский / English / 中文.
- Тема оформления: тёмная / светлая.

### Что можно поменять через настройки внутри файла

Все параметры ниже — обычные константы/CSS-переменные в начале файла, отредактируйте их прямо в HTML-файле текстовым редактором:

- **Цвета и тема** — блок `:root{ ... }` в начале `<style>` (цвета фона, колец круга, кнопок, стрелок-подсказок и т.д.) и блок `body.theme-light{ ... }` для светлой темы — переменные подписаны комментариями.
- **Пределы зума круга** — константы `ZOOM_MIN`, `ZOOM_MAX`, `ZOOM_STEP` в `<script>`.
- **Нота в центре круга** (размер, цвет, шрифт) — объект `CENTER_NOTE_CONFIG`.
- **Подпись лада под нотой в центре круга** (размер, цвет, шрифт, отступ) — объект `CENTER_MODE_LABEL_CONFIG`.
- **Масштаб панели настроек на мобильных экранах** — константы `MOBILE_PANEL_BASE_WIDTH` / `MOBILE_PANEL_SIDE_MARGIN` / `MOBILE_PANEL_MAX_SCALE` рядом с функцией `updateMobilePanelScale()`.
- **Значения по умолчанию для вывода в DAW** — атрибуты `value` у полей `dawIntervalInput` (интервал, сек) и `dawVelocityInput` (velocity) в разметке.

[⬆ К списку языков](#-languages--языки--语言)

---

<a id="en"></a>
## 🇬🇧 English

### About

A single self-contained HTML app (opens in any browser, nothing to install) — an interactive circle of fifths for learning chords and modes, and for ear/memory training on notes and chords. Works with mouse, computer keyboard, and a real MIDI keyboard.

Three main modes, switched with the tabs at the top:

- **Training** — the circle shows the notes of the selected chord/mode relative to the root, using arrows or color.
- **Notes** — practice recognizing/picking notes on the major and minor rings of the circle.
- **Chords/Modes** — practice with chords and modes, using the same answer methods as in Notes.

### Features

- **Training**
  - Two independent hint "variants" — Variant 1 and Variant 2 — each switchable between **arrows** and **color** display.
  - 20 chord types: plain triads (major/minor), sus2, sus4, dominant/major/minor 7th, 9th, 11th and 13th chords and their variants (7, maj7, m7, m(Maj7), add9, m(add9), 9, maj9, m9, m(Maj9), add11, m(add11), 11, maj11, m11, 13, maj13, m13, m(Maj13)).
  - 7 diatonic modes: Lydian, Major (Ionian), Mixolydian, Dorian, Minor (Aeolian), Phrygian, Locrian.
  - An on-screen piano keyboard hint next to the circle, can be shown/hidden.
  - The chosen chord/mode is labelled in the center of the circle.
  - Rotate the circle left/right with the arrow keys (30° step).
- **Notes and Chords/Modes (Practice)**
  - Answer by **mouse click** on the circle or by playing on a **MIDI/computer keyboard**.
  - Choose which notes (major/minor) or which chord types/modes are used to generate questions; "Clear all" button.
  - Optional on-screen piano keyboard (in the Chords/Modes section).
- **General**
  - Zoom the circle: **+/-** keys, a three/four-finger touch gesture, or the on-screen buttons.
  - The settings panel can be pinned beside the circle (desktop) or used as a bottom sheet (mobile) — opened with the mouse wheel / a swipe / a hotkey.
  - Connect an external **MIDI keyboard** (up to 7 inputs at once) to answer with notes/chords.
  - **DAW output**: play the selected chord into an external synth/DAW — all notes at once or one after another with a set interval, with adjustable velocity, in MIDI 1.0 (1–127) or MIDI 2.0 (1–65536) format, and optionally split the chord's notes across separate MIDI channels.
  - Toggle alternate enharmonic note spellings (e.g. A♯/B♭) separately for the major and minor rings.
  - Note naming system: letter names (ABC) or solfège (do-re-mi).
  - Interface available in 3 languages (Russian/English/Chinese), with a dark/light theme.
  - All settings, the chosen language and theme are saved to the browser's localStorage and restored next time you open the app.

### Hotkeys

Hotkeys are matched by physical key position, so they work the same on a Russian or an English keyboard layout.

| Key | Action |
|---|---|
| `A`…`G` | Pick a note on the circle (natural); pressing the same letter again toggles major ↔ minor |
| `Shift` + `A`…`G` | Pick a sharp note (♯) |
| `Space`, then `A`…`G` | Pick a flat note (♭) |
| `1`…`9`, `0` | Pick a chord type (positions 1–10 in the list) |
| `Space`, then `1`…`9`/`0` | Pick a chord type from the "second page" (positions 11–20) |
| `+` / `=` | Zoom the circle in |
| `-` | Zoom the circle out |
| `Shift` + `-` | Reset zoom |
| `Q` | Training: Variant 1 — "arrows" |
| `W` | Training: Variant 1 — "color" |
| `R` | Training: Variant 2 — "arrows" |
| `T` | Training: Variant 2 — "color" |
| `Y` | Open/close the settings panel |
| `Z` | Chords/Modes: show/hide the hint (this section only) |
| `←` / `→` | Training: rotate the circle 30° left/right |
| Mouse wheel up/down | Open/close the settings panel (desktop) |
| Swipe up/down anywhere | Open/close the settings panel (mobile) |
| 2-finger short tap | Open/close the settings panel (touchscreen) |
| 3-finger short tap | Zoom the circle in |
| 4-finger short tap | Zoom the circle out |

Note-letter hotkeys always work in Training; in the Notes section they only work when "MIDI/computer keyboard" is selected as the answer method (they're disabled in "Mouse click" mode). Chord-number hotkeys work in Training and in Chords/Modes.

### What can be changed via the menu

Opened with `Y`, the mouse wheel, a swipe, or the settings icon:

- Pin the settings panel beside the circle (desktop only).
- Answer method: mouse click / MIDI-computer keyboard (Notes, Chords/Modes sections).
- Which notes (major/minor), which chord types, and which modes are included in practice.
- Show/hide the on-screen piano keyboard.
- Show chord letters under the notes, show chord degrees, lock the key (in Training).
- Number of simultaneous MIDI inputs (1–7), a specific MIDI port, the MIDI output for a DAW, connect/reconnect the MIDI keyboard.
- DAW output settings: play the chord together or in sequence, interval between notes (sec), velocity, MIDI 1.0/2.0 format, split the signal across channels.
- Alternate (enharmonic) note names — separately for the major and minor rings.
- Note naming system: ABC or do-re-mi.
- Interface language: Русский / English / 中文.
- Theme: dark / light.

### What can be changed in the file's settings

All of the below are plain constants/CSS variables near the top of the file — edit them directly in the HTML file with a text editor:

- **Colors and theme** — the `:root{ ... }` block at the top of `<style>` (background, circle rings, buttons, hint arrows, etc.) and the `body.theme-light{ ... }` block for the light theme — variables are documented with comments.
- **Circle zoom limits** — the `ZOOM_MIN`, `ZOOM_MAX`, `ZOOM_STEP` constants in `<script>`.
- **The note shown in the center of the circle** (size, color, font) — the `CENTER_NOTE_CONFIG` object.
- **The mode label under the center note** (size, color, font, spacing) — the `CENTER_MODE_LABEL_CONFIG` object.
- **The settings panel's scale on mobile screens** — the `MOBILE_PANEL_BASE_WIDTH` / `MOBILE_PANEL_SIDE_MARGIN` / `MOBILE_PANEL_MAX_SCALE` constants next to the `updateMobilePanelScale()` function.
- **Default values for DAW output** — the `value` attributes on the `dawIntervalInput` (interval, sec) and `dawVelocityInput` (velocity) fields in the markup.

[⬆ Back to language list](#-languages--языки--语言)

---

<a id="zh"></a>
## 🇨🇳 中文

### 简介

这是一个单文件 HTML 应用（在任意浏览器中打开即可使用，无需安装）——一个交互式五度圈工具，用于学习和弦与调式，也可用于训练对音符和和弦的听辨与记忆。支持鼠标、电脑键盘以及真实 MIDI 键盘操作。

顶部标签页可切换三种主要模式：

- **训练** —— 圆圈上通过箭头或颜色显示所选和弦/调式相对于根音的组成音。
- **音符** —— 在圆圈的大调环和小调环上进行音符辨认/选择练习。
- **和弦/调式** —— 与"音符"相同的作答方式，练习和弦与调式。

### 功能

- **训练**
  - 两套独立的提示"方案"——方案 1 和方案 2，每套都可在**箭头**显示和**颜色**显示之间切换。
  - 20 种和弦类型：普通三和弦（大调/小调）、sus2、sus4，以及属七/大七/小七、九、十一、十三和弦及其变体（7、maj7、m7、m(Maj7)、add9、m(add9)、9、maj9、m9、m(Maj9)、add11、m(add11)、11、maj11、m11、13、maj13、m13、m(Maj13)）。
  - 7 种自然调式：利底亚、大调（伊奥尼亚）、混合利底亚、多利亚、小调（爱奥利亚）、弗里几亚、洛克利亚。
  - 圆圈旁的钢琴键盘提示图，可显示/隐藏。
  - 圆圈中央显示当前所选和弦/调式的名称。
  - 使用左右方向键将圆圈旋转（每次 30°）。
- **音符 与 和弦/调式（练习）**
  - 可通过**鼠标点击**圆圈作答，或通过 **MIDI/电脑键盘**演奏作答。
  - 选择参与练习的音符集合（大调/小调）或和弦类型/调式集合；提供"全部清除"按钮。
  - 可选显示钢琴键盘（在"和弦/调式"部分）。
- **通用功能**
  - 圆圈缩放：**+/-** 键、触屏三指/四指手势，或界面上的按钮。
  - 设置面板可固定在圆圈旁边（桌面端），或作为从底部弹出的抽屉使用（移动端）——可通过鼠标滚轮、滑动手势或快捷键打开。
  - 连接外部 **MIDI 键盘**（最多同时 7 路输入）用于以音符/和弦作答。
  - **DAW 输出**：将所选和弦播放到外部合成器/DAW —— 可同时播放全部音符，或按设定的间隔依次播放，可调节 velocity（力度），支持 MIDI 1.0（1–127）或 MIDI 2.0（1–65536）格式，并可将和弦音符分配到不同的 MIDI 通道。
  - 分别为大调环和小调环切换等音异名（例如 A♯/B♭）的显示。
  - 音符命名方式：字母命名（ABC）或首调唱名法（do-re-mi）。
  - 界面支持 3 种语言（俄语/英语/中文），并提供深色/浅色主题。
  - 所有设置、所选语言和主题都会保存在浏览器的 localStorage 中，下次打开时自动恢复。

### 快捷键

快捷键按物理按键位置匹配，因此在俄语键盘布局和英语键盘布局下效果相同。

| 按键 | 操作 |
|---|---|
| `A`…`G` | 在圆圈上选择音符（本位音）；再次按同一字母可在大调/小调之间切换 |
| `Shift` + `A`…`G` | 选择升号音符（♯） |
| `Space`，然后按 `A`…`G` | 选择降号音符（♭） |
| `1`…`9`、`0` | 选择和弦类型（列表中第 1–10 项） |
| `Space`，然后按 `1`…`9`/`0` | 选择"第二页"中的和弦类型（第 11–20 项） |
| `+` / `=` | 放大圆圈 |
| `-` | 缩小圆圈 |
| `Shift` + `-` | 重置缩放 |
| `Q` | 训练：方案 1 —— "箭头" |
| `W` | 训练：方案 1 —— "颜色" |
| `R` | 训练：方案 2 —— "箭头" |
| `T` | 训练：方案 2 —— "颜色" |
| `Y` | 打开/关闭设置面板 |
| `Z` | 和弦/调式：显示/隐藏提示（仅该部分有效） |
| `←` / `→` | 训练：将圆圈向左/右旋转 30° |
| 鼠标滚轮上/下 | 打开/关闭设置面板（桌面端） |
| 屏幕任意位置上下滑动 | 打开/关闭设置面板（移动端） |
| 双指短按 | 打开/关闭设置面板（触屏） |
| 三指短按 | 放大圆圈 |
| 四指短按 | 缩小圆圈 |

音符字母快捷键在"训练"模式下始终可用；在"音符"部分，只有当作答方式选择为"MIDI/电脑键盘"时才可用（"鼠标点击"模式下不可用）。和弦数字快捷键在"训练"和"和弦/调式"中均可用。

### 可通过菜单更改的内容

通过按 `Y`、滚动鼠标滚轮、滑动手势或点击设置图标打开：

- 将设置面板固定在圆圈旁边（仅限桌面端）。
- 作答方式：鼠标点击 / MIDI-电脑键盘（"音符"、"和弦/调式"部分）。
- 参与练习的音符集合（大调/小调）、和弦类型集合、调式集合。
- 显示/隐藏钢琴键盘。
- 在音符下方显示和弦字母、显示和弦音级、锁定调性（训练模式中）。
- 同时使用的 MIDI 输入数量（1–7）、选择具体的 MIDI 端口、选择用于 DAW 的 MIDI 输出、连接/重新连接 MIDI 键盘。
- DAW 输出设置：同时播放和弦或依次播放、音符间隔（秒）、velocity（力度）、MIDI 1.0/2.0 格式、按通道拆分信号。
- 等音异名音符名称——分别针对大调环和小调环。
- 音符命名方式：ABC 或 do-re-mi。
- 界面语言：Русский / English / 中文。
- 主题：深色 / 浅色。

### 可在文件内部设置中更改的内容

以下均为文件顶部的普通常量/CSS 变量，可直接用文本编辑器在 HTML 文件中修改：

- **颜色与主题** —— `<style>` 开头的 `:root{ ... }` 代码块（背景色、圆环颜色、按钮颜色、提示箭头颜色等）以及浅色主题对应的 `body.theme-light{ ... }` 代码块——变量均附有注释说明。
- **圆圈缩放范围** —— `<script>` 中的 `ZOOM_MIN`、`ZOOM_MAX`、`ZOOM_STEP` 常量。
- **圆圈中央音符**的样式（大小、颜色、字体） —— `CENTER_NOTE_CONFIG` 对象。
- **中央音符下方调式名称标签**的样式（大小、颜色、字体、间距） —— `CENTER_MODE_LABEL_CONFIG` 对象。
- **移动端设置面板的缩放比例** —— 位于 `updateMobilePanelScale()` 函数旁边的 `MOBILE_PANEL_BASE_WIDTH` / `MOBILE_PANEL_SIDE_MARGIN` / `MOBILE_PANEL_MAX_SCALE` 常量。
- **DAW 输出的默认值** —— 标记中 `dawIntervalInput`（间隔，秒）和 `dawVelocityInput`（velocity）字段的 `value` 属性。

[⬆ 返回语言列表](#-languages--языки--语言)
