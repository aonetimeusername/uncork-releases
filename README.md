# Uncork

**Запуск совместимых Windows-игр в Uncork бесплатен и останется бесплатным.** Играйте из своей библиотеки Steam на Mac с Apple Silicon и macOS 14 или новее. Аккаунт Uncork и подписка для этого не нужны. Для Epic Games Store мы проверили установку клиента, вход и установку игр. Наши проверки запуска игр относятся к версиям из Steam. [Установка](https://uncorkmac.com/install.html) · [Проверить игру в каталоге](https://uncorkmac.com/games.html)

Публичная версия на 20 ноября 2026 года — **1.7.3.1** от 16 ноября. Образ подписан Developer ID и прошёл нотарификацию Apple. [Версия и SHA-256](https://uncorkmac.com/latest.json) · [История выпусков](https://uncorkmac.com/changelog.html)

Сведения о приложении и ссылка для скачивания — на сайте **[uncorkmac.com](https://uncorkmac.com/)**. Этот репозиторий — страница-указатель на сайт: в нём нет ни исходного кода, ни сборок. Исходный код приложения не опубликован. Другие публичные проекты на GitHub с названием Uncork — не это приложение и не наши.

English version: [below](#uncork-english).

## Бесплатный запуск и дополнительные функции

Запускайте купленные игры и бесплатные игры из своей библиотеки Steam без оплаты Uncork. У каждой игры свои системные требования и условия магазина. В бесплатную версию входят установка Steam и компонентов Windows, выбор графики, диагностика запуска и проверка мыши. Перевод видимого текста доступен бесплатно на macOS 15 и новее.

Дополнительные игровые функции, включая прямой ввод мыши и экран заезда Assetto Corsa, сейчас можно включить бесплатно в разделе Pro. В будущем отдельные дополнительные функции могут стать платными. Бесплатное использование не создаёт подписку и не влечёт автоматического списания.

Новые покупки Pro временно закрыты. Ранее приобретённые лицензии Pro сохраняют права на версии 1.x на условиях покупки. Владельцам по-прежнему доступны вход в аккаунт и восстановление доступа. [Условия](https://uncorkmac.com/terms.html) · [Ответы на вопросы](https://uncorkmac.com/faq.html)

## Требования

По [FAQ от 31 октября 2026](https://uncorkmac.com/faq.html) и [требованиям на главной](https://uncorkmac.com/#req), сверенным 4 ноября 2026:

- Mac на Apple Silicon, M1 и новее. На Mac с процессором Intel Uncork не работает.
- macOS 14 или новее. Проверяем на текущей версии, на более старых не тестировали.
- Rosetta 2: пока её нет, приложение не даёт создать бутылку и показывает кнопку установки.
- Свой аккаунт Steam или Epic Games Store и купленные в нём игры. Пароль Steam и код Steam Guard вводятся только в окне самого Steam: Uncork их не спрашивает.
- Место на диске: около 3 ГБ под среду и Steam (замер автора на главной странице) плюс место под игры.

## Чем Uncork отличается

### Графика в версии 1.7.3.1

Uncork использует Wine 10.0 ревизии 6 от Sikarugir с комплектом драйверов Uncork и нашу сборку DXMT на базе v0.80. D3DMetal 3.0 от Apple загружается отдельно после принятия лицензии. При ручном выборе DXVK Uncork использует DXVK-macOS для Direct3D 10–11 и d9vk для Direct3D 9. Для игр на Direct3D 9 с выбранным DXVK мы исправили ошибку отрисовки, из-за которой в меню и игровом интерфейсе появлялись чёрные треугольники. [Как устроен Uncork](https://uncorkmac.com/how-uncork-works.html) · [Исправление Direct3D 9](https://uncorkmac.com/changelog.html#v1-6-2) · [Версии компонентов и лицензии](https://uncorkmac.com/licenses/third-party-notices.txt)

**Assetto Corsa 2014.** Бесплатная версия готовит компоненты Windows для купленной игры. Дальше заезд можно начать из её лаунчера в Steam. В Pro есть Content Manager и экран заезда. При запуске заезда из Uncork Pro используется DXMT. На D3DMetal при проверке с Custom Shaders Patch 0.3 мы увидели розовые квадраты по краям и в бликах. [Настройка и результаты](https://uncorkmac.com/assetto-corsa.html)

| Возможность | Что это |
|---|---|
| Прямой ввод мыши и CS2 | Проверка мыши бесплатна. В Pro драйвер читает движение внешней мыши напрямую, пока активная игра скрывает курсор над своим окном. Требуется «Мониторинг ввода». На MacBook Pro M3 Pro с экраном 120 Гц и Logitech G309, настроенной на 1000 Гц, вне игры мы измерили 843 события движения в секунду на системном уровне и 119 в обычном окне macOS. [Повторить замер](https://uncorkmac.com/mouse.html) · [Условия теста CS2](https://uncorkmac.com/cs2.html) |
| Ровные кадры (Pro) | Кадры выходят на экран через равные промежутки. Режим для одиночных игр. С версии 1.5.6 от 26 октября 2026 он не включается в CS2 и играх с EasyAntiCheat или BattlEye. |
| Game Mode | Бесплатно: macOS включает игровой режим и для Windows-игр; Uncork запускает каждую игру из её маленького приложения с категорией «Игры». |
| Режим геймпада и консольный режим | Бесплатно: геймпад водит курсор по маку, пока игра не запущена; кнопка PS или Xbox открывает список игр на весь экран. Управлению курсором нужно необязательное разрешение «Универсальный доступ». |
| Перевод поверх игры | Бесплатная бета для macOS 15 и новее. Включите перевод в настройках и загрузите языковую пару. В игре нажмите Control–Option–T (сочетание по умолчанию), чтобы перевести меню, подсказки и видимые субтитры. Перевод работает локально. Языки результата — русский, английский, японский, немецкий, французский и испанский. [Меню Portal 2 до и после перевода и настройка](https://uncorkmac.com/translate-games.html) |
| Пауза | Бесплатно. Включите паузу в настройках и нажмите ⌘P в игре. В CS2 функция отключена, в других сетевых играх при паузе возможно отключение от сервера. |
| Импорт из Whisky | Бесплатно: копирует бутылки вместе с установленными играми, оригинал не меняет. На бутылке, созданной самим Whisky, импорт ещё не проверяли: сохраните оригинал, пока игры не запустятся в Uncork. |
| Игры в Steam для Mac | Бесплатно: установленную игру можно добавить как сторонний ярлык через Настройки Uncork. Сначала закройте Steam для Mac. Его клиент не меняется; Windows-версия Steam внутри среды по-прежнему нужна. Steam Input, оверлей и учёт времени в Steam для Mac не гарантируются. |
| Отдача руля Logitech (Pro) | G923 для PlayStation и ПК проверен вживую в Assetto Corsa; G29 поддержан в коде, вживую не проверялся. Версия G923 для Xbox и другие рули не проверялись. |

Прямой ввод мыши есть и у других проектов; подробности — на [странице сравнения от 31 октября 2026](https://uncorkmac.com/compare.html). Скорость других приложений мы не сравнивали. Слой совместимости стоит кадров: Uncork не сделает из ноутбука игровой ПК.

## Что проверено

- В каталоге на 20 ноября 2026 года **596 записей** с указанием источника и статуса. В наших проверках указаны машина и достигнутая стадия, например меню, заезд или матч. [Каталог совместимости](https://uncorkmac.com/games.html) · [Выборка проверок проекта в JSON](https://uncorkmac.com/games.json)
- Во встроенном снимке базы highball-db от 22 октября 2026 года около 540 записей (CC0). В них игроки рассказывают о своих Mac и настройках. [Источники каталога](https://uncorkmac.com/compare.html)
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy и Rockstar Games в приложении есть, но работу в них мы не проверяли.
- Если игра не проверена, это ещё не значит, что она не работает. Свою можно проверить бесплатно, без ограничения по времени.
- Замеры сделаны на одном MacBook Pro с M3 Pro; на другом Mac и в другой сцене числа будут другими. Условия и даты приведены в записях на странице «Игры».

## Что не запустится

Игры с античитом уровня ядра: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege и новые части Call of Duty. У macOS нет ядра Windows, куда можно поставить такой драйвер. Uncork защиту не обходит. Подробнее — на странице [«Игры с античитом»](https://uncorkmac.com/anti-cheat.html).

В сентябре 2026 года разработчик проверил официальный матчмейкинг CS2 на одном аккаунте. Для Premier отдельной проверки нет. Условия и ограничения указаны в карточке игры. [Counter-Strike 2 на Mac](https://uncorkmac.com/cs2.html)

## Что стоит знать до установки

- **Приложение подписано Developer ID и нотаризовано Apple** с версии 1.0.12 от 7 октября 2026 и открывается как обычная программа для Mac ([FAQ от 31 октября 2026](https://uncorkmac.com/faq.html)).
- **Код закрыт.** Если нужен открытый код или большая база наших проверок, посмотрите [сравнение](https://uncorkmac.com/compare.html).
- **Главный риск проекта — Rosetta.** По FAQ от 31 октября 2026, со ссылкой на Apple, macOS 27 — последняя версия с полной Rosetta, а в macOS 28 она остаётся только для старых игр. Uncork работает поверх неё и не обещает работу на macOS 28 и новее. Подробнее — [«Rosetta и macOS 27»](https://uncorkmac.com/rosetta-macos-27.html).

## Где скачать и как начать

1. Скачайте приложение кнопкой «Скачать» на **[uncorkmac.com](https://uncorkmac.com/)** — вход и регистрация не нужны.
2. Установите и откройте Uncork. Приложение подписано и нотаризовано Apple.
3. Войдите в Steam внутри Uncork, установите игру из своей библиотеки и нажмите «Играть».

### Одна команда в Терминале

```sh
curl -fsSL https://uncorkmac.com/install.sh | sh
```

Скрипт скачивает образ с uncorkmac.com, сверяет SHA-256, проверяет подпись Developer ID (команда PJC7K6A3U5) и нотаризацию Apple, копирует Uncork в «Программы» и открывает его. Без sudo и без аккаунта; установленную копию не трогает. Что делает каждая строка и что нужно знать ИИ-агенту — на странице [Установка из Терминала](https://uncorkmac.com/install.html).

### Homebrew

```sh
brew tap aonetimeusername/uncork
brew trust aonetimeusername/uncork
brew install --cask uncork
```

Это наш tap: он указывает на тот же нотаризованный DMG с uncorkmac.com. Команда `brew trust` нужна один раз: свежий Homebrew загружает формулы из сторонних tap только после неё.

## Страницы сайта

| Страница | RU | EN |
|---|---|---|
| Главная | [uncorkmac.com](https://uncorkmac.com/) | [uncorkmac.com/en](https://uncorkmac.com/en/) |
| Как играть в Windows-игры на Mac: все способы | [открыть](https://uncorkmac.com/windows-games-on-mac.html) | [open](https://uncorkmac.com/en/windows-games-on-mac.html) |
| Counter-Strike 2 на Mac | [открыть](https://uncorkmac.com/cs2.html) | [open](https://uncorkmac.com/en/cs2.html) |
| Почему мышь плавает в играх на Mac | [открыть](https://uncorkmac.com/mouse.html) | [open](https://uncorkmac.com/en/mouse.html) |
| Игры Valve на Mac | [открыть](https://uncorkmac.com/valve-games.html) | [open](https://uncorkmac.com/en/valve-games.html) |
| Вопросы и ответы | [открыть](https://uncorkmac.com/faq.html) | [open](https://uncorkmac.com/en/faq.html) |
| Каталог игр | [открыть](https://uncorkmac.com/games.html) | [open](https://uncorkmac.com/en/games.html) |
| Игры с античитом | [открыть](https://uncorkmac.com/anti-cheat.html) | [open](https://uncorkmac.com/en/anti-cheat.html) |
| Сравнение с другими приложениями | [открыть](https://uncorkmac.com/compare.html) | [open](https://uncorkmac.com/en/compare.html) |
| Чем заменить Whisky | [открыть](https://uncorkmac.com/whisky-alternative.html) | [open](https://uncorkmac.com/en/whisky-alternative.html) |
| Assetto Corsa на Mac | [открыть](https://uncorkmac.com/assetto-corsa.html) | [open](https://uncorkmac.com/en/assetto-corsa.html) |
| Rosetta и macOS 27 | [открыть](https://uncorkmac.com/rosetta-macos-27.html) | [open](https://uncorkmac.com/en/rosetta-macos-27.html) |
| Что Uncork отправляет | [открыть](https://uncorkmac.com/what-uncork-sends.html) | [open](https://uncorkmac.com/en/what-uncork-sends.html) |
| Что нового (по версиям) | [открыть](https://uncorkmac.com/changelog.html) | [open](https://uncorkmac.com/en/changelog.html) |

Политика конфиденциальности и условия: [privacy](https://uncorkmac.com/privacy.html), [terms](https://uncorkmac.com/terms.html) (русский и английский текст на одной странице).

## Приватность

Сторонней аналитики нет. Приложение обращается к нашему серверу для Pro и обновлений, а также отправляет служебные отметки установки и запуска с отпечатком Mac и версией приложения; в этих отметках нет названия игры, пароля Steam, путей к файлам или времени игры. Отдельно можно согласиться отправлять ответы «Как прошла игра?» — тогда передаются игра, ответ, модель Mac и версии macOS и Uncork. Перевод поверх игры обрабатывает кадры и текст на самом Mac и не отправляет их. Подробности — на странице [«Что Uncork отправляет»](https://uncorkmac.com/what-uncork-sends.html) и в [политике конфиденциальности](https://uncorkmac.com/privacy.html).

## Лицензии

Драйвер, производный от открытого слоя совместимости, распространяется по LGPL 2.1: лицензия и письменное предложение исходников входят в приложение (Настройки → Помощь → Лицензии компонентов). Лицензии остальных компонентов — там же ([главная страница](https://uncorkmac.com/#honest) и [FAQ](https://uncorkmac.com/faq.html), сверены 4 ноября 2026). По вопросам исходников драйвера можно написать по контактам ниже. Uncork не связан с Valve и Apple; названия игр и продуктов принадлежат их правообладателям.

## Связь

[hello@uncork.win](mailto:hello@uncork.win) · Telegram: [@uncorkwin](https://t.me/uncorkwin).

Актуальная версия приложения — на сайте.

---

# Uncork (English)

**Launching compatible Windows games with Uncork is free and will stay free.** Play from your Steam library on an Apple Silicon Mac running macOS 14 or later. You do not need an Uncork account or subscription to play. For the Epic Games Store, we tested client installation, sign-in and game installation. Our game-launch tests cover Steam versions. [Installation guide](https://uncorkmac.com/en/install.html) · [Check a game](https://uncorkmac.com/en/games.html)

The public version on 20 November 2026 is **1.7.3.1**, released on 16 November. The disk image is Developer ID signed and notarized by Apple. [Version and SHA-256](https://uncorkmac.com/latest.json) · [Release notes](https://uncorkmac.com/en/changelog.html)

For details and downloads, visit **[uncorkmac.com](https://uncorkmac.com/en/)**. This repository is a pointer page to the site: it holds no source code and no builds. The app's source code is not published. Other public GitHub projects called Uncork are not this app and not ours.

## Free game launching and optional features

Use Uncork to launch games you own on Steam and free-to-play Steam games without paying for the launcher. Each game's store terms and system requirements still apply. Steam and Windows component setup, graphics selection, launch diagnostics and the mouse check are included for free. On-screen text translation is free on macOS 15 or later.

Optional gameplay features, including direct mouse input and the Assetto Corsa race setup screen, can currently be enabled for free in the Pro section. Some optional features may be offered for a fee in the future. Using them for free does not start a subscription or create an automatic charge.

New Pro purchases are paused. Existing Pro licences retain their 1.x entitlements under the terms of purchase. Owners can still sign in and restore access. [Terms](https://uncorkmac.com/terms.html) · [FAQ](https://uncorkmac.com/en/faq.html)

## Requirements

From the [FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html) and the [home page requirements](https://uncorkmac.com/en/#req), checked on 4 November 2026:

- An Apple Silicon Mac, M1 or later. Uncork does not run on Intel Macs.
- macOS 14 or later. We test on the current version; older ones are untested.
- Rosetta 2: until it is installed, the app will not let you create a bottle and shows an install button.
- Your own Steam or Epic Games Store account and games bought in it. Your Steam password and Steam Guard code are entered only in Steam's own window: Uncork does not ask for them.
- Disk space: about 3 GB for the environment and Steam (the author's measurement on the home page), plus space for games.

## What sets it apart

### Graphics in version 1.7.3.1

Uncork uses Sikarugir Wine 10.0 revision 6 with Uncork's driver package and our build of DXMT based on v0.80. Apple's D3DMetal 3.0 downloads separately after you accept its licence. If you select DXVK manually, Uncork uses DXVK-macOS for Direct3D 10–11 and d9vk for Direct3D 9. For Direct3D 9 games using DXVK, we fixed a rendering issue that drew large black triangles across menus and the in-game interface. [How Uncork works](https://uncorkmac.com/en/how-uncork-works.html) · [Direct3D 9 fix](https://uncorkmac.com/en/changelog.html#v1-6-2) · [Component versions and licences](https://uncorkmac.com/licenses/third-party-notices.txt)

**Assetto Corsa (2014).** Free setup installs the Windows components for your Steam copy. You can then start a race from the game's own launcher. Pro adds Content Manager and a race setup screen. Races launched from Uncork Pro use DXMT. When we tested Custom Shaders Patch 0.3 with D3DMetal, pink squares appeared on edges and highlights. [Setup and test results](https://uncorkmac.com/en/assetto-corsa.html)

| Feature | What it is |
|---|---|
| Direct mouse input and CS2 | The mouse check is free. With Pro and Input Monitoring enabled, the driver reads movement directly from an external mouse while the active game hides the pointer over its window. Outside the game, a Logitech G309 set to 1000 Hz on an M3 Pro MacBook Pro with a 120 Hz display produced 843 movement events per second at the system event tap and 119 in an ordinary macOS window. [Repeat the test](https://uncorkmac.com/en/mouse.html) · [CS2 test conditions](https://uncorkmac.com/en/cs2.html) |
| Even frames (Pro) | Frames reach the screen at even intervals. For single-player games. Since version 1.5.6 of 26 October 2026, it does not turn on in CS2 or games with EasyAntiCheat or BattlEye. |
| Game Mode | Free: macOS turns Game Mode on for Windows games; Uncork launches each game from its own small app with the Games category. |
| Gamepad mode and console mode | Free: a controller moves the Mac's pointer while no game is running; the PS or Xbox button opens the game list full screen. Moving the pointer needs the optional Accessibility permission. |
| On-screen text translation | Free beta for macOS 15 or later. Enable translation in Settings and download the language pair. In the game, press Control–Option–T (the default shortcut) to translate menus, prompts and visible subtitles. Translation runs locally. The six output languages are English, Russian, Japanese, German, French and Spanish. [Portal 2 menu before and after translation, with setup steps](https://uncorkmac.com/en/translate-games.html) |
| Pause | Free. Enable pause in Settings, then press ⌘P in the game. Pause is disabled in CS2. Other online games can lose their server connection while paused. |
| Import from Whisky | Free: copies bottles with their installed games and leaves the original untouched. We have not tested the import on a bottle created by Whisky itself: keep the original until your games start in Uncork. |
| Games in Steam for Mac | Free: add an installed game as a non-Steam shortcut through Uncork's Settings. Close Steam for Mac first. Its client is not modified; Windows Steam is still needed inside the game environment. Steam Input, the overlay and playtime tracking in Steam for Mac are not guaranteed. |
| Logitech wheel force feedback (Pro) | The PlayStation and PC G923 is tested live in Assetto Corsa; the G29 is supported in code but not tested on real hardware. The Xbox G923 and other wheels have not been tested. |

Other projects also have direct mouse input; see the [comparison dated 31 October 2026](https://uncorkmac.com/en/compare.html). We have not compared other apps' speed. A compatibility layer costs frames: Uncork will not turn a laptop into a gaming PC.

## What has been tested

- On 20 November 2026 the website catalogue lists **596 entries**, each labelled by source and status. Our test records name the Mac and the stage reached, such as a menu, a race or a match. [Compatibility catalogue](https://uncorkmac.com/en/games.html) · [Selected project test records in JSON](https://uncorkmac.com/games.json)
- The in-app highball-db snapshot from 22 October 2026 contains about 540 entries (CC0). Players report their own Macs and settings. [Catalogue sources](https://uncorkmac.com/en/compare.html)
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy and Rockstar Games are in the app, but we have not tested them.
- An untested game may still work. You can try yours for free, with no time limit.
- Measurements were taken on one MacBook Pro with an M3 Pro; on another Mac or in another scene, numbers will differ. Conditions and dates are recorded on the Games page.

## What will not run

Games with kernel-level anti-cheat: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege and recent Call of Duty titles. macOS has no Windows kernel to put such a driver in. Uncork does not bypass that protection. Details are on the [anti-cheat page](https://uncorkmac.com/en/anti-cheat.html).

In September 2026 the developer tested official CS2 matchmaking on one account. Premier has no separate test on record. See the game page for the test conditions and limitations. [Counter-Strike 2 on Mac](https://uncorkmac.com/en/cs2.html)

## Before you install

- **The app has been signed with Developer ID and notarized by Apple** since version 1.0.12 of 7 October 2026, and opens like an ordinary Mac app ([FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html)).
- **Closed source.** If you need open source or a large database of our own tests, see the [comparison](https://uncorkmac.com/en/compare.html).
- **The project's main risk is Rosetta.** The FAQ dated 31 October 2026, citing Apple, says macOS 27 is the last version with full Rosetta; macOS 28 keeps it only for older games. Uncork runs on top of it and does not promise to work on macOS 28 or later. More: [Rosetta and macOS 27](https://uncorkmac.com/en/rosetta-macos-27.html).

## Where to download and how to start

1. Download the app with the Download button on **[uncorkmac.com](https://uncorkmac.com/en/)** — no sign-in or sign-up needed.
2. Install and open Uncork. The app is signed and notarized by Apple.
3. Sign in to Steam inside Uncork, install a game from your library, then press Play.

### One Terminal command

```sh
curl -fsSL https://uncorkmac.com/install.sh | sh
```

The script downloads the image from uncorkmac.com, compares its SHA-256, checks the Developer ID signature (team PJC7K6A3U5) and Apple's notarization, copies Uncork to Applications and opens it. No sudo and no account; an installed copy is left alone. What each step does, and what an AI agent needs to know, is on the page [Install from the Terminal](https://uncorkmac.com/en/install.html).

### Homebrew

```sh
brew tap aonetimeusername/uncork
brew trust aonetimeusername/uncork
brew install --cask uncork
```

This is our tap: it points to the same notarized DMG from uncorkmac.com. `brew trust` is needed once: current Homebrew loads casks from third-party taps only after it.

## Pages of the site

| Page | RU | EN |
|---|---|---|
| Home | [uncorkmac.com](https://uncorkmac.com/) | [uncorkmac.com/en](https://uncorkmac.com/en/) |
| How to play Windows games on a Mac: every method | [RU](https://uncorkmac.com/windows-games-on-mac.html) | [EN](https://uncorkmac.com/en/windows-games-on-mac.html) |
| Counter-Strike 2 on a Mac | [RU](https://uncorkmac.com/cs2.html) | [EN](https://uncorkmac.com/en/cs2.html) |
| Why the mouse feels floaty in games on a Mac | [RU](https://uncorkmac.com/mouse.html) | [EN](https://uncorkmac.com/en/mouse.html) |
| Valve games on Mac | [RU](https://uncorkmac.com/valve-games.html) | [EN](https://uncorkmac.com/en/valve-games.html) |
| FAQ | [RU](https://uncorkmac.com/faq.html) | [EN](https://uncorkmac.com/en/faq.html) |
| Game catalogue | [RU](https://uncorkmac.com/games.html) | [EN](https://uncorkmac.com/en/games.html) |
| Anti-cheat games | [RU](https://uncorkmac.com/anti-cheat.html) | [EN](https://uncorkmac.com/en/anti-cheat.html) |
| Comparison with other apps | [RU](https://uncorkmac.com/compare.html) | [EN](https://uncorkmac.com/en/compare.html) |
| What to use instead of Whisky | [RU](https://uncorkmac.com/whisky-alternative.html) | [EN](https://uncorkmac.com/en/whisky-alternative.html) |
| Assetto Corsa on a Mac | [RU](https://uncorkmac.com/assetto-corsa.html) | [EN](https://uncorkmac.com/en/assetto-corsa.html) |
| Rosetta and macOS 27 | [RU](https://uncorkmac.com/rosetta-macos-27.html) | [EN](https://uncorkmac.com/en/rosetta-macos-27.html) |
| What Uncork sends | [RU](https://uncorkmac.com/what-uncork-sends.html) | [EN](https://uncorkmac.com/en/what-uncork-sends.html) |
| Changelog | [RU](https://uncorkmac.com/changelog.html) | [EN](https://uncorkmac.com/en/changelog.html) |

Privacy policy and terms: [privacy](https://uncorkmac.com/privacy.html), [terms](https://uncorkmac.com/terms.html) (Russian and English text on one page).

## Privacy

There is no third-party analytics. The app contacts our server for Pro and updates, and sends setup and launch step marks with the Mac's fingerprint and app version; those marks contain no game title, Steam password, file paths or play time. Separately, you can opt in to share “How did the game go?” answers: those include the game, your answer, Mac model, macOS and Uncork versions. Translation over a game processes frames and text on the Mac and does not send them. Details are on [What Uncork sends](https://uncorkmac.com/en/what-uncork-sends.html) and in the [privacy policy](https://uncorkmac.com/privacy.html).

## Licences

The driver, derived from the open-source compatibility layer, is distributed under LGPL 2.1: its licence and a written source offer are included in the app (Settings → Help → Component licences). Other component licences are in the same place ([home page](https://uncorkmac.com/en/#honest) and [FAQ](https://uncorkmac.com/en/faq.html), checked on 4 November 2026). For questions about the driver's source, use the contacts below. Uncork is not affiliated with Valve or Apple; game and product names belong to their owners.

## Contact

[hello@uncork.win](mailto:hello@uncork.win) · Telegram: [@uncorkwin](https://t.me/uncorkwin).

The current version of the app is on the site.
