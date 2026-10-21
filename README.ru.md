> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="Скриншот MiniVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe — это **сборка MiniMax** из семейства _Vibe_ — форк ZCode, ориентированный на одного провайдера: **MiniMax**. Одна модель, одно рабочее пространство, партнёр — не агент.

Семейство _Vibe_ выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, MiniVibe для MiniMax, …), каждое со своим характером. Оно существует **наряду** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полный код проекта смотрите в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux доступны на [странице релизов](../../releases); самый новый релиз всегда помечен тегом **latest**:

| Платформа | Файлы |
| --- | --- |
| macOS (Apple Silicon) | `MiniVibe-<version>-mac-arm64.dmg` · `MiniVibe-<version>-mac-arm64.zip` |
| Windows | `MiniVibe-<version>-win-x64.exe` |
| Linux | `MiniVibe-<version>-linux-x86_64.AppImage` · `MiniVibe-<version>-linux-amd64.deb` · `MiniVibe-<version>-linux-x86_64.rpm` · `MiniVibe-<version>-linux-x64.pkg.tar.zst` |

Все приложения семейства *Vibe* выпускаются с **одинаковым номером версии** (сейчас 1.0.5). Встроенный механизм обновления проверяет последний релиз этого репозитория.

> **macOS (Apple Silicon):** сборка **неподписанная** (нет платной программы Apple Developer Program), поэтому Gatekeeper
> выдаёт предупреждение при первом запуске. Приложение подписано ad-hoc — откройте его один раз через **правый клик → Открыть** или выполните
> `xattr -dr com.apple.quarantine "/Applications/MiniVibe.app"`.

## Сборка из исходного кода

Требуются Git, Node.js **24.14.0** и pnpm **10.33.2** (см. `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Лицензия и атрибуция

Создано на основе ZCode (Apache-2.0); лицензия и NOTICE сохранены. MiniVibe — независимый проект, не связанный с ZCode/Z.ai или MiniMax. MiniMax является товарным знаком своего владельца; логотип используется с разрешения оператора.
