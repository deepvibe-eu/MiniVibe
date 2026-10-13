> Machine-translated from [README.md](README.md) into Deutsch — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="MiniVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe ist der **MiniMax-Build** der _Vibe_-Familie — ein Fork von ZCode, der sich auf einen einzigen Anbieter konzentriert: **MiniMax**. Ein Modell, ein Arbeitsbereich, ein Partner — kein Agent.

Die _Vibe_-Familie liefert eine fokussierte App pro Anbieter (DeepVibe für DeepSeek, KimiVibe für Kimi, LamaVibe für Ollama, MiniVibe für MiniMax, …), jede mit ihrem eigenen Charakter. Sie existiert **neben** ZCode, nicht an dessen Stelle: ZCode für den Multi-Provider-Workflow, die Vibe-Apps für Menschen, die ein Modell, einen Arbeitsbereich, einen Partner wollen. Den vollständigen Codebestand findest du im Hauptquellcode-Repository.

## Downloads

Installer für macOS, Windows und Linux findest du auf der [Releases-Seite](../../releases); das neueste Release ist immer mit **latest** getaggt:

| Plattform | Dateien |
| --- | --- |
| macOS (Apple Silicon) | `MiniVibe-<version>-mac-arm64.dmg` · `MiniVibe-<version>-mac-arm64.zip` |
| Windows | `MiniVibe-<version>-win-x64.exe` |
| Linux | `MiniVibe-<version>-linux-x86_64.AppImage` · `MiniVibe-<version>-linux-amd64.deb` · `MiniVibe-<version>-linux-x86_64.rpm` · `MiniVibe-<version>-linux-x64.pkg.tar.zst` |

Jede App der *Vibe*-Familie wird mit der **gleichen Versionsnummer** veröffentlicht (derzeit 1.0.3). Der integrierte Updater prüft das neueste Release dieses Repositorys.

> **macOS (Apple Silicon):** Der Build ist **unsigniert** (kein kostenpflichtiges Apple Developer Program), daher warnt Gatekeeper
> beim ersten Start. Die App ist ad-hoc signiert — öffne sie einmal über **Rechtsklick → Öffnen** oder führe
> `xattr -dr com.apple.quarantine "/Applications/MiniVibe.app"` aus.

## Aus dem Quellcode bauen

Erfordert Git, Node.js **24.14.0** und pnpm **10.33.2** (siehe `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Lizenz & Namensnennung

Basiert auf ZCode (Apache-2.0); die Lizenz und der NOTICE-Hinweis bleiben erhalten. MiniVibe ist ein unabhängiges Projekt und steht in keiner Verbindung zu ZCode/Z.ai oder MiniMax. MiniMax ist eine Marke ihres Inhabers; das Logo wird mit Erlaubnis des Betreibers verwendet.
