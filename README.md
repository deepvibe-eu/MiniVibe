# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="MiniVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe is the **MiniMax build** of the _Vibe_ family — a fork of ZCode focused on a single provider: **MiniMax**. One model, one workspace, a partner — not an agent.

The _Vibe_ family ships one focused app per provider (DeepVibe for DeepSeek, KimiVibe for Kimi, LamaVibe for Ollama, MiniVibe for MiniMax, …), each with its own character. It exists **alongside** ZCode, not instead of it: ZCode for the multi-provider workflow, the Vibe apps for people who want one model, one workspace, one partner. See the main source repository for the full codebase.

## Downloads

Installers for macOS, Windows and Linux are on the [releases page](../../releases); the newest release is always tagged **latest**:

| Platform | Files |
| --- | --- |
| macOS (Apple Silicon) | `MiniVibe-<version>-mac-arm64.dmg` · `MiniVibe-<version>-mac-arm64.zip` |
| Windows | `MiniVibe-<version>-win-x64.exe` |
| Linux | `MiniVibe-<version>-linux-x86_64.AppImage` · `MiniVibe-<version>-linux-amd64.deb` · `MiniVibe-<version>-linux-x86_64.rpm` · `MiniVibe-<version>-linux-x64.pkg.tar.zst` |

Every app in the *Vibe* family is released with the **same version number** (currently 1.0.3). The built-in updater checks this repository's latest release.

> **macOS (Apple Silicon):** the build is **unsigned** (no paid Apple Developer Program), so Gatekeeper
> warns on first launch. The app is ad-hoc signed — open it once via **right-click → Open**, or run
> `xattr -dr com.apple.quarantine "/Applications/MiniVibe.app"`.

## Building from source

Requires Git, Node.js **24.14.0** and pnpm **10.33.2** (see `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## License & attribution

Built on ZCode (Apache-2.0); the license and NOTICE are preserved. MiniVibe is an independent project and is not affiliated with ZCode/Z.ai or MiniMax. MiniMax is a trademark of its owner; the logo is used with the operator's permission.
