> Machine-translated from [README.md](README.md) into Deutsch — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="MiniVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe ist der **MiniMax-Build** der _Vibe_-Familie — ein Fork von ZCode, der sich auf einen einzigen Anbieter konzentriert: **MiniMax**. Ein Modell, ein Arbeitsbereich, ein Partner — kein Agent.

Die _Vibe_-Familie liefert eine fokussierte App pro Anbieter (DeepVibe für DeepSeek, KimiVibe für Kimi, LamaVibe für Ollama, MiniVibe für MiniMax, …), jede mit ihrem eigenen Charakter. Sie existiert **neben** ZCode, nicht an dessen Stelle: ZCode für den Multi-Provider-Workflow, die Vibe-Apps für Menschen, die ein Modell, einen Arbeitsbereich, einen Partner wollen. Siehe das Hauptquell-Repository für die vollständige Codebasis.

## Downloads

Installer für macOS, Windows und Linux werden unter [Releases](../../releases) veröffentlicht. Der integrierte Updater prüft dieses Repository.

## Aus dem Quellcode erstellen

Erfordert Git, Node.js **24.14.0** und pnpm **10.33.2** (siehe `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Lizenz & Namensnennung

Basiert auf ZCode (Apache-2.0); die Lizenz und NOTICE bleiben erhalten. MiniVibe ist ein unabhängiges Projekt und steht in keiner Verbindung zu ZCode/Z.ai oder MiniMax. MiniMax ist eine Marke ihres Inhabers; das Logo wird mit Erlaubnis des Betreibers verwendet.
