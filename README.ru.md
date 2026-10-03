> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="Скриншот MiniVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe — это **сборка MiniMax** из семейства _Vibe_ — форк ZCode, ориентированный на одного провайдера: **MiniMax**. Одна модель, одно рабочее пространство, партнёр — не агент.

Семейство _Vibe_ выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, MiniVibe для MiniMax, …), каждое со своим характером. Оно существует **наряду** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полный код можно найти в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux публикуются в разделе [Releases](../../releases). Встроенное средство обновления проверяет этот репозиторий.

## Сборка из исходного кода

Требуются Git, Node.js **24.14.0** и pnpm **10.33.2** (см. `mise.toml`).

```bash
pnpm bootstrap
# запустить вариант MiniVibe в режиме разработки
pnpm dev:desktop:mini
# упаковать (вариант MiniVibe)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Лицензия и указание авторства

Создано на основе ZCode (Apache-2.0); лицензия и NOTICE сохранены. MiniVibe — независимый проект, не связанный с ZCode/Z.ai или MiniMax. MiniMax является товарным знаком своего владельца; логотип используется с разрешения оператора.
