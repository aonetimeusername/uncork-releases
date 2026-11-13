# Uncork

Uncork — бесплатное приложение для Mac на Apple Silicon: запускает Windows-игры из Steam и Epic через слой совместимости, без аккаунта и без ограничения по времени. Дополнительные функции входят в Uncork Pro.

Актуальная версия — **1.7.1 от 13 ноября 2026** ([список версий](https://uncorkmac.com/changelog.html)). Эта страница сверена с сайтом **4 ноября 2026**.

Описание, цена и скачивание — на сайте **[uncorkmac.com](https://uncorkmac.com/)**. Этот репозиторий — страница-указатель на сайт: в нём нет ни исходного кода, ни сборок. Исходный код приложения не опубликован. Другие публичные проекты на GitHub с названием Uncork — не это приложение и не наши.

English version: [below](#uncork-english).

## Цена и доступ

Цена и состав функций — по [FAQ от 31 октября 2026](https://uncorkmac.com/faq.html) и [главной странице](https://uncorkmac.com/#access), сверенным 4 ноября 2026.

- **Бесплатно, без аккаунта и без срока:** запуск игр, Steam и Epic, бутылки, библиотека и история запусков, «Разобраться» и обратимые починки, компоненты Windows (.NET, DirectX, шрифты), рецепты под игры, оптимизации Steam и совместимый звук, Game Mode, режим геймпада и настройка контроллеров, проверка мыши, отчёты сообщества, игры как отдельные приложения для Mac, избранное и свои обложки. Также бесплатны перевод поверх игры (бета, macOS 15 или новее), пауза игр, консольный режим, импорт из Whisky и ярлыки игр в Steam для Mac.
- **Uncork Pro — 19 € разово**, без срока, все версии 1.x: мышь прямо с устройства, «Ровные кадры» для одиночных игр и ровные 60 от батареи, панель поверх игры, достройка кадров на MetalFX (бета, macOS 26, для одиночных игр), перемотка (бета, игры на DXMT), 4:3 на весь экран (для игр на Source 2, проверено в CS2), Content Manager в один клик и экран заезда Assetto Corsa, отдача руля Logitech G923. Купившие Pro получают новые версии раньше и прямую связь с разработчиком.
- **До 31 января 2027 включительно Pro открыт всем в раннем доступе.** В приложении нажмите «Включить Pro — до 31 января»: без аккаунта и без оплаты, в том числе на Mac, где проба уже была. Работают все функции Pro; ранние сборки и прямая связь с разработчиком остаются у купивших. Текст кнопки — из [заметки к версии 1.5.6 от 26 октября 2026](https://uncorkmac.com/changelog.html).
- **После этой даты** функции Pro выключатся у тех, кто его не купил; игры продолжат запускаться бесплатно. Новые маки получат обычную пробу Pro на 7 дней с момента, когда вы сами начнёте её в Uncork. Аккаунт для пробы не нужен, проба одна на Mac. При входе оставшиеся дни перейдут в аккаунт. Аккаунт нужен только для покупки Pro; автопродления нет.
- **Оплата Pro** — Telegram Stars или криптовалюта (USDT, TON, BTC и другие), картой пока нельзя. В первые 14 дней после оплаты деньги возвращаются без объяснений; остальные условия возврата — в [условиях](https://uncorkmac.com/terms.html).
- **Pro привязан к одному Mac.** Для переноса нажмите «Сменить мак» в профиле: привязка снимается сразу, если вы сами не меняли мак в последние 30 дней. Чаще — по письму на hello@uncork.win.
- **Ключ Pro** живёт неделю и продлевается автоматически, пока есть сеть. Без интернета дольше недели Pro выключится до выхода в сеть; сами игры ключа не требуют.

## Требования

По [FAQ от 31 октября 2026](https://uncorkmac.com/faq.html) и [требованиям на главной](https://uncorkmac.com/#req), сверенным 4 ноября 2026:

- Mac на Apple Silicon, M1 и новее. На Mac с процессором Intel Uncork не работает.
- macOS 14 или новее. Проверяем на текущей версии, на более старых не тестировали.
- Rosetta 2: пока её нет, приложение не даёт создать бутылку и показывает кнопку установки.
- Свой аккаунт Steam или Epic Games Store и купленные в нём игры. Пароль Steam и код Steam Guard вводятся только в окне самого Steam: Uncork их не спрашивает.
- Место на диске: около 3 ГБ под среду и Steam (замер автора на главной странице) плюс место под игры.

## Чем Uncork отличается

Мы не обещаем запустить всё подряд. Работа идёт над тем, как игра ощущается. Возможности и ограничения — по [FAQ от 31 октября 2026](https://uncorkmac.com/faq.html), [описанию работы](https://uncorkmac.com/how-uncork-works.html) и [списку версий](https://uncorkmac.com/changelog.html), сверенным 4 ноября 2026.

| Возможность | Что это |
|---|---|
| Мышь с устройства (Pro) | macOS отдаёт движения мыши пачками раз в кадр экрана; Uncork читает мышь прямо с устройства. Наш замер 25 сентября 2026, вне игры: мышь на 1000 Гц прислала 843 движения в секунду, а обычная программа получила их 119 пачками. Это запись на MacBook Pro с M3 Pro и экраном 120 Гц, а не замер влияния на прицел в игре. Разрешение «Мониторинг ввода» необязательно: без него мышь читается обычным путём. [Замер и условия](https://uncorkmac.com/mouse.html). |
| Ровные кадры (Pro) | Кадры выходят на экран через равные промежутки. Режим для одиночных игр. С версии 1.5.6 от 26 октября 2026 он не включается в CS2 и играх с EasyAntiCheat или BattlEye. |
| Game Mode | Бесплатно: macOS включает игровой режим и для Windows-игр; Uncork запускает каждую игру из её маленького приложения с категорией «Игры». |
| Режим геймпада и консольный режим | Бесплатно: геймпад водит курсор по маку, пока игра не запущена; кнопка PS или Xbox открывает список игр на весь экран. Управлению курсором нужно необязательное разрешение «Универсальный доступ». |
| Перевод и пауза | Бесплатно: перевод поверх игры — бета, macOS 15 или новее; после загрузки языков перевод работает без сети, кадры и текст не сохраняются и не отправляются. Пауза включается в Настройках: ⌘P останавливает игру, затем можно продолжить с того же места. CS2 не ставится на паузу, а онлайн-игра за время паузы теряет соединение с сервером. |
| Импорт из Whisky | Бесплатно: копирует бутылки вместе с установленными играми, оригинал не меняет. На бутылке, созданной самим Whisky, импорт ещё не проверяли: сохраните оригинал, пока игры не запустятся в Uncork. |
| Игры в Steam для Mac | Бесплатно: установленную игру можно добавить как сторонний ярлык через Настройки Uncork. Сначала закройте Steam для Mac. Его клиент не меняется; Windows-версия Steam внутри среды по-прежнему нужна. Steam Input, оверлей и учёт времени в Steam для Mac не гарантируются. |
| Отдача руля Logitech (Pro) | G923 для PlayStation и ПК проверен вживую в Assetto Corsa; G29 поддержан в коде, вживую не проверялся. Версия G923 для Xbox и другие рули не проверялись. |

Прямой ввод мыши есть и у других проектов; подробности — на [странице сравнения от 31 октября 2026](https://uncorkmac.com/compare.html). Скорость других приложений мы не сравнивали. Слой совместимости стоит кадров: Uncork не сделает из ноутбука игровой ПК.

## Что проверено

- **14 игр проверены нами**, а из магазинов — Steam и Epic Games Store (сам магазин, а не весь каталог). Большинство игр проверены только до меню или первого экрана. Это данные [сравнения от 31 октября 2026](https://uncorkmac.com/compare.html) и [FAQ той же даты](https://uncorkmac.com/faq.html); пределы каждой проверки, машина и дата — на странице [«Игры»](https://uncorkmac.com/games.html), машиночитаемая копия наших проверок — [games.json](https://uncorkmac.com/games.json).
- **Отчёты сообщества о ~540 играх** — из открытой базы highball-db (CC0), снимок 22 октября 2026 ([источник: сравнение от 31 октября 2026](https://uncorkmac.com/compare.html)). Это сведения о чужих маках и настройках, а не наши проверки и не обещание запуска.
- В [каталоге игр](https://uncorkmac.com/games.html) наши проверки, отчёты игроков, блокировки и указанные магазином версии для Mac помечены отдельно, с источниками и датами.
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy и Rockstar Games в приложении есть, но работу в них мы не проверяли.
- Если игра не проверена, это ещё не значит, что она не работает. Свою можно проверить бесплатно, без ограничения по времени.
- Замеры сделаны на одном MacBook Pro с M3 Pro; на другом Mac и в другой сцене числа будут другими. Условия и даты приведены в записях на странице «Игры».

## Что не запустится

Игры с античитом уровня ядра: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege и новые части Call of Duty. У macOS нет ядра Windows, куда можно поставить такой драйвер. Uncork защиту не обходит. Подробнее — на странице [«Игры с античитом»](https://uncorkmac.com/anti-cheat.html).

Valve не даёт гарантий для запуска CS2 через слой совместимости; матч под VAC мы не записывали и гарантий по блокировкам аккаунта не даём ([FAQ](https://uncorkmac.com/faq.html)).

## Что стоит знать до установки

- **Приложение подписано Developer ID и нотаризовано Apple** с версии 1.0.12 от 7 октября 2026 и открывается как обычная программа для Mac ([FAQ от 31 октября 2026](https://uncorkmac.com/faq.html)).
- **Код закрыт.** Если нужен открытый код или большая база наших проверок, посмотрите [сравнение](https://uncorkmac.com/compare.html).
- **Главный риск проекта — Rosetta.** По FAQ от 31 октября 2026, со ссылкой на Apple, macOS 27 — последняя версия с полной Rosetta, а в macOS 28 она остаётся только для старых игр. Uncork работает поверх неё и не обещает работу на macOS 28 и новее. Подробнее — [«Rosetta и macOS 27»](https://uncorkmac.com/rosetta-macos-27.html).

## Где скачать и как начать

1. Скачайте приложение кнопкой «Скачать» на **[uncorkmac.com](https://uncorkmac.com/)** — вход и регистрация не нужны.
2. Установите и откройте Uncork. Приложение подписано и нотаризовано Apple.
3. Войдите в Steam внутри Uncork и поставьте игру. Запуск игр бесплатный. Для раннего доступа к Pro нажмите «Включить Pro — до 31 января»; срок и условия приведены выше.

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

Uncork is a free Mac app for Apple Silicon: it runs Windows games from Steam and Epic through a compatibility layer, with no account and no time limit. Extra features are part of Uncork Pro.

The current version is **1.7.1, released on 13 November 2026** ([changelog](https://uncorkmac.com/en/changelog.html)). This page was checked against the website on **4 November 2026**.

The description, price and download are on **[uncorkmac.com](https://uncorkmac.com/en/)**. This repository is a pointer page to the site: it holds no source code and no builds. The app's source code is not published. Other public GitHub projects called Uncork are not this app and not ours.

## Price and access

Prices and features come from the [FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html) and the [home page](https://uncorkmac.com/en/#access), checked on 4 November 2026.

- **Free, no account and no time limit:** running games, Steam and Epic, bottles, the library and launch history, Find out why and repairs you can undo, Windows components (.NET, DirectX, fonts), game recipes, Steam optimisations and compatible audio, Game Mode, gamepad mode and controller settings, the mouse check, community reports, games as separate Mac apps, Favorites and your own covers. Translation over a game (beta, macOS 15 or newer), pausing games, console mode, Import from Whisky and game shortcuts in Steam for Mac are free too.
- **Uncork Pro is €19 once**, with no end date, every 1.x version: the mouse read straight from the device, Even frames for single-player games and an even 60 on battery, the in-game panel, MetalFX frame generation (beta, macOS 26, for single-player games), rewind (beta, games on DXMT), 4:3 on the whole screen (for Source 2 games, tested in CS2), one-click Content Manager and the race screen for Assetto Corsa, Logitech G923 force feedback. Buyers get new versions earlier and a direct line to the developer.
- **Until 31 January 2027 inclusive, Pro is open to everyone in early access.** Press “Turn on Pro — until 31 January” in the app: no account and no payment, including on a Mac that already had a trial. All Pro features work; early builds and the direct line to the developer stay with buyers. The button text comes from the [1.5.6 release note of 26 October 2026](https://uncorkmac.com/en/changelog.html).
- **After that date**, Pro features switch off for those who have not bought Pro; games keep launching for free. New Macs get the usual 7-day Pro trial, counted from the moment you start it yourself in Uncork. No account is needed for the trial, and there is one trial per Mac. Signing in moves the remaining days to your account. An account is needed only to buy Pro; there is no auto-renewal.
- **Paying for Pro** is by Telegram Stars or crypto (USDT, TON, BTC and more); cards are not accepted yet. Refunds need no explanation in the first 14 days after payment; the other refund conditions are in the [terms](https://uncorkmac.com/terms.html).
- **Pro is tied to one Mac.** To move it, press “Change Mac” in your profile: the binding is released at once if you have not changed Macs yourself in the last 30 days. For more frequent changes, write to hello@uncork.win.
- **The Pro key** lasts a week and renews automatically while there is a network. After more than a week offline, Pro switches off until you go online; games themselves need no key.

## Requirements

From the [FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html) and the [home page requirements](https://uncorkmac.com/en/#req), checked on 4 November 2026:

- An Apple Silicon Mac, M1 or later. Uncork does not run on Intel Macs.
- macOS 14 or later. We test on the current version; older ones are untested.
- Rosetta 2: until it is installed, the app will not let you create a bottle and shows an install button.
- Your own Steam or Epic Games Store account and games bought in it. Your Steam password and Steam Guard code are entered only in Steam's own window: Uncork does not ask for them.
- Disk space: about 3 GB for the environment and Steam (the author's measurement on the home page), plus space for games.

## What sets it apart

We do not promise to run everything. The work goes into how a game feels. Features and limits come from the [FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html), [How Uncork works](https://uncorkmac.com/en/how-uncork-works.html) and the [changelog](https://uncorkmac.com/en/changelog.html), checked on 4 November 2026.

| Feature | What it is |
|---|---|
| Mouse from the device (Pro) | macOS delivers mouse movement in batches once per display frame; Uncork reads the mouse straight from the device. Our measurement on 25 September 2026, outside a game: a 1000 Hz mouse sent 843 movements a second, reaching an ordinary app as 119 batches. This was recorded on a MacBook Pro with an M3 Pro and a 120 Hz display; it did not measure the effect on aim in a game. Input Monitoring is optional: without it, the mouse is read the usual way. [Measurement and conditions](https://uncorkmac.com/en/mouse.html). |
| Even frames (Pro) | Frames reach the screen at even intervals. For single-player games. Since version 1.5.6 of 26 October 2026, it does not turn on in CS2 or games with EasyAntiCheat or BattlEye. |
| Game Mode | Free: macOS turns Game Mode on for Windows games; Uncork launches each game from its own small app with the Games category. |
| Gamepad mode and console mode | Free: a controller moves the Mac's pointer while no game is running; the PS or Xbox button opens the game list full screen. Moving the pointer needs the optional Accessibility permission. |
| Translation and pause | Free: translation over a game is in beta and needs macOS 15 or newer; after downloading languages, it works offline and does not store or send frames or text. Enable pause in Settings: ⌘P stops a game, then you can carry on from the same moment. CS2 is never paused; an online game loses its server connection while paused. |
| Import from Whisky | Free: copies bottles with their installed games and leaves the original untouched. We have not tested the import on a bottle created by Whisky itself: keep the original until your games start in Uncork. |
| Games in Steam for Mac | Free: add an installed game as a non-Steam shortcut through Uncork's Settings. Close Steam for Mac first. Its client is not modified; Windows Steam is still needed inside the game environment. Steam Input, the overlay and playtime tracking in Steam for Mac are not guaranteed. |
| Logitech wheel force feedback (Pro) | The PlayStation and PC G923 is tested live in Assetto Corsa; the G29 is supported in code but not tested on real hardware. The Xbox G923 and other wheels have not been tested. |

Other projects also have direct mouse input; see the [comparison dated 31 October 2026](https://uncorkmac.com/en/compare.html). We have not compared other apps' speed. A compatibility layer costs frames: Uncork will not turn a laptop into a gaming PC.

## What has been tested

- **14 games tested by us**, and of the stores, Steam and the Epic Games Store (the store itself, not its whole catalogue). Most games were tested only to the menu or first screen. These are the figures in the [comparison dated 31 October 2026](https://uncorkmac.com/en/compare.html) and the [FAQ of the same date](https://uncorkmac.com/en/faq.html); each test's limits, machine and date are on the [Games page](https://uncorkmac.com/en/games.html). Our tests also have a machine-readable copy: [games.json](https://uncorkmac.com/games.json).
- **Community reports for ~540 games**, from the open highball-db database (CC0), snapshot of 22 October 2026 ([source: comparison dated 31 October 2026](https://uncorkmac.com/en/compare.html)). These describe other people's Macs and settings; they are not our tests or a promise that a game will run.
- The [game catalogue](https://uncorkmac.com/en/games.html) labels our tests, player reports, blocks and store-listed Mac versions separately, with sources and dates.
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy and Rockstar Games are in the app, but we have not tested them.
- An untested game may still work. You can try yours for free, with no time limit.
- Measurements were taken on one MacBook Pro with an M3 Pro; on another Mac or in another scene, numbers will differ. Conditions and dates are recorded on the Games page.

## What will not run

Games with kernel-level anti-cheat: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege and recent Call of Duty titles. macOS has no Windows kernel to put such a driver in. Uncork does not bypass that protection. Details are on the [anti-cheat page](https://uncorkmac.com/en/anti-cheat.html).

Valve gives no guarantees for running CS2 through a compatibility layer; we have not recorded a match under VAC and promise nothing about account bans ([FAQ](https://uncorkmac.com/en/faq.html)).

## Before you install

- **The app has been signed with Developer ID and notarized by Apple** since version 1.0.12 of 7 October 2026, and opens like an ordinary Mac app ([FAQ dated 31 October 2026](https://uncorkmac.com/en/faq.html)).
- **Closed source.** If you need open source or a large database of our own tests, see the [comparison](https://uncorkmac.com/en/compare.html).
- **The project's main risk is Rosetta.** The FAQ dated 31 October 2026, citing Apple, says macOS 27 is the last version with full Rosetta; macOS 28 keeps it only for older games. Uncork runs on top of it and does not promise to work on macOS 28 or later. More: [Rosetta and macOS 27](https://uncorkmac.com/en/rosetta-macos-27.html).

## Where to download and how to start

1. Download the app with the Download button on **[uncorkmac.com](https://uncorkmac.com/en/)** — no sign-in or sign-up needed.
2. Install and open Uncork. The app is signed and notarized by Apple.
3. Sign in to Steam inside Uncork and install a game. Running games is free. For Pro early access, press “Turn on Pro — until 31 January”; the dates and conditions are above.

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
