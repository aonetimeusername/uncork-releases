# Uncork

Uncork — платное приложение для Mac на Apple Silicon: запускает Windows-игры из Steam и Epic. Семь дней бесплатно и без регистрации, дальше 5 € в месяц или 50 € в год.

Это платное приложение, а не бесплатное: бесплатна только проба — семь дней. Нужен Mac с Apple Silicon (M1 и новее) и macOS 14 или новее. Приложение в бете (предварительная сборка), актуальная версия — **0.19.3** от 3 октября 2026. Эта страница сверена с сайтом **3 октября 2026**.

Описание, цена и скачивание — на сайте **[uncork.win](https://uncork.win)**. Этот репозиторий — страница-указатель на сайт: в нём нет ни исходного кода, ни сборок. Исходный код приложения не опубликован. Другие публичные проекты на GitHub с названием Uncork — не это приложение и не наши.

English version: [below](#uncork-english).

## Цена и доступ

- **5 € в месяц или 50 € в год.** Первые семь дней бесплатны и без аккаунта: отсчёт начинается с кнопки «Начать 7 дней бесплатно» в приложении на этом Mac. Проба одна на Mac — для этого приложение отправляет отпечаток Mac. Аккаунт нужен, когда решите остаться: оплата — в профиле на сайте, а оставшиеся пробные дни при входе переходят в аккаунт. Автопродления нет: ничего не списывается само.
- **Оплата** — Telegram Stars или TON, картой пока нельзя. В первые 14 дней после оплаты деньги возвращаются без объяснений ([условия](https://uncork.win/terms.html)).
- **Один доступ — один Mac.** Перенос на другой Mac — по письму на hello@uncork.win.
- **Ключ драйвера** живёт неделю и не переживает оплаченное время больше чем на час. Пока есть сеть, приложение продлевает его само, поэтому без интернета можно играть до семи дней. Когда оплаченное время кончается, игры не запускаются; приложение при этом открывается, а бутылка, Steam и игры на диске остаются вашими.

## Требования

- Mac на Apple Silicon, M1 и новее. На Mac с процессором Intel Uncork не работает.
- macOS 14 или новее. Проверяем на текущей версии, на более старых не тестировали.
- Rosetta 2: пока её нет, приложение не даёт создать бутылку и показывает кнопку установки.
- Свой аккаунт Steam или Epic Games Store и купленные в нём игры. Пароль Steam и код Steam Guard вводятся только в окне самого Steam: Uncork их не спрашивает.
- Место на диске: около 3 ГБ под среду и Steam (замерено у нас) плюс то, сколько весят игры.

## Чем Uncork отличается

Мы не обещаем запустить всё подряд. Работа идёт над тем, как игра ощущается.

| Возможность | Что это |
|---|---|
| Мышь с устройства | macOS отдаёт движение мыши пачками раз в кадр экрана; Uncork читает мышь прямо с устройства, до 1000 Гц (частота зависит от самой мыши). Наш замер 25 сентября 2026 (мышь 1000 Гц, MacBook Pro M3 Pro, вне игры): 843 движения в секунду против 119 пачек, которые доходят до обычной программы. Нужно необязательное разрешение «Мониторинг ввода»: без него мышь читается обычным путём. |
| Ровные кадры | Кадры выходят на экран через равные промежутки. Режим для одиночных игр: гонок, экшенов, открытых миров. В соревновательных матчах (в том числе в CS2) его включать не советуем. |
| Game Mode | macOS включает игровой режим и для Windows-игр, когда игра на весь экран и впереди: Uncork запускает каждую игру из её маленького приложения с категорией «Игры». |
| Режим геймпада | DualSense, DualShock 4 или геймпад Xbox водит курсор по маку, пока игра не запущена. Нужно необязательное разрешение «Универсальный доступ». |
| Отдача руля Logitech | G923 (версия для PlayStation и ПК) проверен вживую в Assetto Corsa; G29 поддержан в коде, вживую не проверялся. Версия G923 для Xbox и другие рули не проверялись. |

У других приложений, по прочитанным нами страницам на 29 сентября 2026, чтение мыши с устройства не упоминается; подробности и оговорки — на [странице сравнения](https://uncork.win/compare.html). Слой совместимости стоит кадров: Uncork не сделает из ноутбука игровой ПК, и мы не обещаем «как на Windows».

## Что проверено

- Семь игр мы запускали сами, а из магазинов проверены Steam и Epic Games Store (сам магазин, а не весь его каталог). Каждая игра — с замером или пометкой «кадры не измеряли», машиной и датой — на странице [«Игры»](https://uncork.win/games.html) (машиночитаемая копия: [games.json](https://uncork.win/games.json)). Counter-Strike 2: наш замер 30 сентября 2026 — 102–147 fps на Dust II на эталонной машине (ниже); условия и все записи с датами — на странице [CS2 на Mac](https://uncork.win/cs2.html).
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy и Rockstar Games в приложении есть, но работу в них мы не проверяли.
- Игры, которых нет в списке, — «не знаем», а не «не работает». Многие, вероятно, запустятся, но мы этого не обещаем: проверить свою можно за семь пробных дней.
- Все замеры кадров сняты на одной машине — эталонной: MacBook Pro 14″ (Mac15,6), Apple M3 Pro, 14-ядерный GPU, 18 ГБ, macOS 26. На другом Mac и в другой сцене числа будут другими. Подробные записи — на страницах CS2 и «Игры».

## Что не запустится

Игры с античитом уровня ядра: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege и новые части Call of Duty. Это не настройка и не ошибка, которую починят позже: у macOS нет ядра Windows, куда такой драйвер можно поставить. Uncork защиту не обходит и обходить не будет; в библиотеке такие игры помечаются, а перед скачиванием Uncork спрашивает, точно ли ставить. Список — на странице [«Игры с античитом»](https://uncork.win/anti-cheat.html).

Valve официально не поддерживает запуск через слой совместимости, поэтому гарантий по блокировкам аккаунта никто дать не может.

## Что стоит знать до установки

- **Приложение не нотаризовано Apple** (оно подписано сертификатом Apple Development, не Developer ID). Первый запуск macOS не разрешит: Системные настройки → Конфиденциальность и безопасность → «Всё равно открыть». Правый клик → «Открыть» в новых macOS не помогает. Пошагово — на странице [«Вопросы»](https://uncork.win/faq.html).
- **Код закрыт**, приложение платное. Если нужна бесплатная или открытая программа, программа с нотаризацией или большая база проверенных игр, Uncork не подойдёт; сравнение с датой проверки данных — на странице [«Сравнение»](https://uncork.win/compare.html).
- **Главный риск проекта — Rosetta.** По сообщениям Apple, macOS 27 — последняя версия с полной Rosetta; Uncork сегодня работает поверх неё. Что с этим делать — на странице [«Rosetta и macOS 27»](https://uncork.win/rosetta-macos-27.html).
- Подходит, если вы играете в одиночные игры или гонки, готовы платить и хотите мышь с устройства и ровные кадры. Скорость других приложений мы не сравнивали.

## Где скачать и как начать

1. Скачайте приложение кнопкой «Скачать» на **[uncork.win](https://uncork.win)** — вход и регистрация для этого не нужны.
2. Установите приложение и подтвердите первый запуск в системных настройках (см. выше).
3. Нажмите «Начать 7 дней бесплатно»: проба пойдёт на этом Mac без аккаунта. Затем войдите в Steam внутри Uncork и поставьте игру. Аккаунт на сайте понадобится, когда решите оплатить; «Войти» — для тех, у кого он уже есть.

## Страницы сайта

| Страница | RU | EN |
|---|---|---|
| Главная | [uncork.win](https://uncork.win/) | [uncork.win/en](https://uncork.win/en/) |
| Как играть в Windows-игры на Mac: все способы | [открыть](https://uncork.win/windows-games-on-mac.html) | [open](https://uncork.win/en/windows-games-on-mac.html) |
| Counter-Strike 2 на Mac | [открыть](https://uncork.win/cs2.html) | [open](https://uncork.win/en/cs2.html) |
| Почему прицел плавает на Mac (мышь) | [открыть](https://uncork.win/mouse.html) | [open](https://uncork.win/en/mouse.html) |
| Вопросы и ответы | [открыть](https://uncork.win/faq.html) | [open](https://uncork.win/en/faq.html) |
| Проверенные игры | [открыть](https://uncork.win/games.html) | [open](https://uncork.win/en/games.html) |
| Игры с античитом | [открыть](https://uncork.win/anti-cheat.html) | [open](https://uncork.win/en/anti-cheat.html) |
| Сравнение с другими приложениями | [открыть](https://uncork.win/compare.html) | [open](https://uncork.win/en/compare.html) |
| Чем заменить Whisky | [открыть](https://uncork.win/whisky-alternative.html) | [open](https://uncork.win/en/whisky-alternative.html) |
| Assetto Corsa на Mac | [открыть](https://uncork.win/assetto-corsa.html) | [open](https://uncork.win/en/assetto-corsa.html) |
| Rosetta и macOS 27 | [открыть](https://uncork.win/rosetta-macos-27.html) | [open](https://uncork.win/en/rosetta-macos-27.html) |
| Что Uncork отправляет | [открыть](https://uncork.win/what-uncork-sends.html) | [open](https://uncork.win/en/what-uncork-sends.html) |
| Что нового (по версиям) | [открыть](https://uncork.win/changelog.html) | [open](https://uncork.win/en/changelog.html) |

Политика конфиденциальности и условия: [privacy](https://uncork.win/privacy.html), [terms](https://uncork.win/terms.html) (русский и английский текст на одной странице).

## Приватность

Приложение обращается к нашему серверу ради доступа и обновлений; названия игр, время игры, файлы и пароль Steam не отправляются, сторонней аналитики нет, а сервер отмечает лишь служебные шаги (вышло на связь, выдан ключ драйвера, начат вход) — полный список соединений на странице [«Что Uncork отправляет»](https://uncork.win/what-uncork-sends.html).

## Лицензии

Драйвер, производный от компонента с лицензией LGPL (2.1), сопровождается лицензией и письменным предложением исходников: они входят в приложение (Настройки → Помощь → Лицензии компонентов). Запросить исходники драйвера по этому предложению можно по контактам ниже (в предложении указан Telegram @uncorkwin). Лицензии остальных компонентов — там же. Uncork не связан с Valve и Apple; названия игр и продуктов принадлежат их правообладателям.

## Связь

[hello@uncork.win](mailto:hello@uncork.win) · Telegram: [@uncorkwin](https://t.me/uncorkwin) (личные сообщения поддержке, это не канал).

Ранние сборки 0.4.x, лежавшие здесь раньше, сняты с публикации: они устарели и не поддерживаются. Актуальная версия — на сайте.

---

# Uncork (English)

Uncork is a paid Mac app for Apple Silicon: it runs Windows games from Steam and Epic. Seven days free with no sign-up, then €5 a month or €50 a year.

It is a paid app, not a free one: only the trial, seven days, is free. It needs a Mac with Apple Silicon (M1 and later) and macOS 14 or later. The app is in beta (a prerelease build); the current version is **0.19.3**, released on 3 October 2026. This page was checked against the website on **3 October 2026**.

The description, price and download are on **[uncork.win](https://uncork.win/en/)**. This repository is a pointer page to the site: it holds no source code and no builds. The app's source code is not published. Other public GitHub projects called Uncork are not this app and not ours.

## Price and access

- **5 € a month or 50 € a year.** The first seven days are free and need no account: the count starts when you press “Start 7 days free” in the app on this Mac. There is one trial per Mac — for that, the app sends a fingerprint of the Mac. You need an account once you decide to stay: you pay in your profile on the site, and signing in moves the trial days you have left to the account. There is no auto-renewal: nothing is charged by itself.
- **Payment** is by Telegram Stars or TON; a card is not available yet. For the first 14 days after a payment your money is returned with no reasons asked ([the terms](https://uncork.win/terms.html)).
- **One access, one Mac.** To move it to another Mac, write to hello@uncork.win.
- **The driver key** lives for a week and never outlives your paid time by more than an hour. While there is a network the app renews it by itself, so you can play offline for up to seven days. When the paid time runs out, games stop launching; the app itself still opens, and the bottle, Steam and games on disk stay yours.

## Requirements

- An Apple Silicon Mac, M1 and later. Uncork does not run on Intel Macs.
- macOS 14 or later. We test on the current version; older ones are untested.
- Rosetta 2: until it is installed, the app will not let you create a bottle and shows an install button.
- Your own Steam or Epic Games Store account and games bought in it. Your Steam password and Steam Guard code are entered only in the Steam window itself: Uncork does not ask for them.
- Disk space: about 3 GB for the environment and Steam (measured here), plus whatever the games weigh.

## What sets it apart

We do not promise to run everything. The work goes into how a game feels.

| Feature | What it is |
|---|---|
| Mouse from the device | macOS hands mouse movement over in batches once per display frame; Uncork reads the mouse straight from the device, up to 1000 Hz (the rate depends on the mouse itself). Our measurement on 25 September 2026 (a 1000 Hz mouse, MacBook Pro M3 Pro, outside a game): 843 movements a second versus 119 batches reaching an ordinary program. It uses the optional “Input Monitoring” permission: without it the mouse is read the usual way. |
| Even frames | Frames reach the screen at even intervals. A mode for single-player games: racing, action, open worlds. We do not recommend it in competitive matches (CS2 included). |
| Game Mode | macOS turns Game Mode on for Windows games too, when the game is full screen and in front: Uncork launches each game from its own small app with the “Games” category. |
| Gamepad mode | A DualSense, DualShock 4 or Xbox controller drives the Mac's pointer while no game is running. It uses the optional “Accessibility” permission. |
| Logitech wheel force feedback | The G923 (PlayStation and PC version) is tested live in Assetto Corsa; the G29 is supported in code but not tested on real hardware. The Xbox version of the G923 and other wheels have not been tested. |

In the pages of other apps we read on 29 September 2026, reading the mouse from the device is not mentioned; details and caveats are on [the Compare page](https://uncork.win/en/compare.html). A compatibility layer costs frames: Uncork will not turn a laptop into a gaming PC, and we do not promise “like on Windows”.

## What has been tested

- We have run seven games ourselves, and of the stores, Steam and the Epic Games Store are tested (the store itself, not its whole catalogue). Each game, with a measurement or a “frame rate not measured” note, the machine and the date, is on [the Games page](https://uncork.win/en/games.html) (machine-readable copy: [games.json](https://uncork.win/games.json)). Counter-Strike 2: our measurement on 30 September 2026 — 102–147 fps on Dust II on the reference machine (below); the conditions and all dated records are on [CS2 on a Mac](https://uncork.win/en/cs2.html).
- Ubisoft Connect, EA app, Battle.net, GOG Galaxy and Rockstar Games are in the app, but we have not tested them.
- A game that is not on the list is “unknown”, not “broken”. Many will probably start, but we do not promise it: you can check yours during the seven trial days.
- All frame-rate measurements were taken on one machine, the reference one: a MacBook Pro 14″ (Mac15,6), Apple M3 Pro, 14-core GPU, 18 GB, macOS 26. On another Mac and in another scene the numbers will differ. Detailed records are on the CS2 and Games pages.

## What will not run

Games with kernel-level anti-cheat: Valorant, Fortnite, Apex Legends, Destiny 2, PUBG, Rainbow Six Siege and recent Call of Duty titles. It is not a setting or a bug that will be fixed later: macOS has no Windows kernel to put such a driver in. Uncork does not bypass such protection and will not; the library marks such games, and before downloading one Uncork asks whether you really want it. The list is on [the anti-cheat page](https://uncork.win/en/anti-cheat.html).

Valve does not officially support running the game through a compatibility layer, so nobody can promise you against account bans.

## Before you install

- **The app is not notarized by Apple** (it is signed with an Apple Development certificate, not Developer ID). macOS will not open it the first time: System Settings → Privacy & Security → “Open Anyway”. Right-click → “Open” no longer helps in recent versions of macOS. Step by step on [the FAQ page](https://uncork.win/en/faq.html).
- **Closed source**, and paid. If you need a free or open-source app, a notarized one, or a large database of tested games, Uncork does not fit; the comparison, with its date of checking, is on [the Compare page](https://uncork.win/en/compare.html).
- **The project's main risk is Rosetta.** According to Apple, macOS 27 is the last version with full Rosetta; Uncork runs on top of it today. What to do about it: [Rosetta and macOS 27](https://uncork.win/en/rosetta-macos-27.html).
- It fits if you play single-player games or racing games, are ready to pay, and want the mouse read from the device and evened-out frames. We have not compared other apps' speed.

## Where to download and how to start

1. Download the app with the Download button on **[uncork.win](https://uncork.win/en/)** — no sign-in or sign-up needed.
2. Install the app and confirm the first launch in System Settings (see above).
3. Press “Start 7 days free”: the trial runs on this Mac with no account. Then sign in to Steam inside Uncork and install a game. You will need an account on the site when you decide to pay; “Sign in” is for those who already have one.

## Pages of the site

| Page | RU | EN |
|---|---|---|
| Home | [uncork.win](https://uncork.win/) | [uncork.win/en](https://uncork.win/en/) |
| How to play Windows games on a Mac: every method | [RU](https://uncork.win/windows-games-on-mac.html) | [EN](https://uncork.win/en/windows-games-on-mac.html) |
| Counter-Strike 2 on a Mac | [RU](https://uncork.win/cs2.html) | [EN](https://uncork.win/en/cs2.html) |
| Why aim feels floaty on a Mac (the mouse) | [RU](https://uncork.win/mouse.html) | [EN](https://uncork.win/en/mouse.html) |
| FAQ | [RU](https://uncork.win/faq.html) | [EN](https://uncork.win/en/faq.html) |
| Games we have tested | [RU](https://uncork.win/games.html) | [EN](https://uncork.win/en/games.html) |
| Anti-cheat games | [RU](https://uncork.win/anti-cheat.html) | [EN](https://uncork.win/en/anti-cheat.html) |
| Comparison with other apps | [RU](https://uncork.win/compare.html) | [EN](https://uncork.win/en/compare.html) |
| What to use instead of Whisky | [RU](https://uncork.win/whisky-alternative.html) | [EN](https://uncork.win/en/whisky-alternative.html) |
| Assetto Corsa on a Mac | [RU](https://uncork.win/assetto-corsa.html) | [EN](https://uncork.win/en/assetto-corsa.html) |
| Rosetta and macOS 27 | [RU](https://uncork.win/rosetta-macos-27.html) | [EN](https://uncork.win/en/rosetta-macos-27.html) |
| What Uncork sends | [RU](https://uncork.win/what-uncork-sends.html) | [EN](https://uncork.win/en/what-uncork-sends.html) |
| Changelog | [RU](https://uncork.win/changelog.html) | [EN](https://uncork.win/en/changelog.html) |

Privacy policy and terms: [privacy](https://uncork.win/privacy.html), [terms](https://uncork.win/terms.html) (Russian and English text on one page).

## Privacy

The app talks to our server for access and updates; game titles, play time, files and your Steam password are not sent, there is no third-party analytics, and the server notes only service steps (the app got in touch, a driver key was issued, a sign-in was started) — the full list of connections is on [What Uncork sends](https://uncork.win/en/what-uncork-sends.html).

## Licences

The driver, derived from a component under the LGPL (2.1), ships with the licence and a written offer of its source, both included in the app (Settings → Help → Component licences). You can request the driver's source under that offer through the contacts below (the offer names Telegram @uncorkwin). The licences of the other components are in the same place. Uncork is not affiliated with Valve or Apple; game and product names belong to their owners.

## Contact

[hello@uncork.win](mailto:hello@uncork.win) · Telegram: [@uncorkwin](https://t.me/uncorkwin) (direct messages to support, not a channel).

The early 0.4.x builds that used to be here have been withdrawn: they are outdated and unsupported. The current version is on the site.
