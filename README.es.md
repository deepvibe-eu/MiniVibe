> Machine-translated from [README.md](README.md) into Español — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="MiniVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe es la **build de MiniMax** de la familia _Vibe_ — un fork de ZCode enfocado en un único proveedor: **MiniMax**. Un modelo, un espacio de trabajo, un compañero — no un agente.

La familia _Vibe_ distribuye una aplicación enfocada por proveedor (DeepVibe para DeepSeek, KimiVibe para Kimi, LamaVibe para Ollama, MiniVibe para MiniMax, …), cada una con su propio carácter. Existe **junto a** ZCode, no en su lugar: ZCode para el flujo de trabajo multiproveedor, las aplicaciones Vibe para quienes quieren un modelo, un espacio de trabajo, un compañero. Consulta el repositorio principal del código fuente para ver la base de código completa.

## Descargas

Los instaladores para macOS, Windows y Linux están en la [página de releases](../../releases); la versión más reciente siempre lleva la etiqueta **latest**:

| Plataforma | Archivos |
| --- | --- |
| macOS (Apple Silicon) | `MiniVibe-<version>-mac-arm64.dmg` · `MiniVibe-<version>-mac-arm64.zip` |
| Windows | `MiniVibe-<version>-win-x64.exe` |
| Linux | `MiniVibe-<version>-linux-x86_64.AppImage` · `MiniVibe-<version>-linux-amd64.deb` · `MiniVibe-<version>-linux-x86_64.rpm` · `MiniVibe-<version>-linux-x64.pkg.tar.zst` |

Cada aplicación de la familia *Vibe* se publica con el **mismo número de versión** (actualmente 1.0.3). El actualizador integrado comprueba la última release de este repositorio.

> **macOS (Apple Silicon):** la build **no está firmada** (sin Apple Developer Program de pago), por lo que Gatekeeper
> avisa en el primer arranque. La aplicación está firmada ad-hoc — ábrela una vez con **clic derecho → Abrir**, o ejecuta
> `xattr -dr com.apple.quarantine "/Applications/MiniVibe.app"`.

## Compilar desde el código fuente

Requiere Git, Node.js **24.14.0** y pnpm **10.33.2** (consulta `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licencia y atribución

Construido sobre ZCode (Apache-2.0); la licencia y el NOTICE se conservan. MiniVibe es un proyecto independiente y no está afiliado a ZCode/Z.ai ni a MiniMax. MiniMax es una marca registrada de su propietario; el logotipo se usa con el permiso del operador.
