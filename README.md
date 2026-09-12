# Uncork — сборки / builds

Бесплатная альтернатива CrossOver для Apple Silicon: Steam и игры (CS2 и другие) на Mac через Wine 10 и Apple D3DMetal.
Здесь только готовые сборки; исходный код пока закрыт.

## Установка

1. Скачай последний **Uncork-x.y.z.dmg** в разделе Releases и открой его.
2. Перетащи **Uncork** в «Программы».
3. Первый запуск: правый клик по Uncork → **Открыть** (сборка не нотаризована).
   Если macOS всё равно не пускает: Системные настройки → Конфиденциальность и безопасность → **Всё равно открыть**.
4. Внутри приложения: «Поставить Steam» — установщик качается с steampowered.com сам.

**Пишет «The application “Uncork” can't be opened»** (так бывает на macOS 26, если файл пришёл через Telegram, AirDrop или браузер): сними карантин одной командой в Terminal и открой снова:

```bash
xattr -dr com.apple.quarantine /Applications/Uncork.app && open /Applications/Uncork.app
```

**Нужно:** Apple Silicon (M1 и новее), macOS 14 или новее, Rosetta 2, Homebrew и каска `gcenx/wine/game-porting-toolkit` (приложение подскажет, чего не хватает).

## Install (English)

Download the latest **Uncork-x.y.z.dmg** from Releases, drag Uncork to Applications, then right-click → **Open** on first launch (the build is not notarized). If macOS still refuses: System Settings → Privacy & Security → **Open Anyway**. If it just says the app "can't be opened" (macOS 26, file received via Telegram/AirDrop/browser), clear the quarantine flag in Terminal: `xattr -dr com.apple.quarantine /Applications/Uncork.app && open /Applications/Uncork.app`. Requires Apple Silicon, macOS 14+, Rosetta 2, Homebrew and the `gcenx/wine/game-porting-toolkit` cask.

Uncork never asks for a Steam password or Steam Guard code: signing in stays inside Steam's own window.
