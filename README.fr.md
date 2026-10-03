> Machine-translated from [README.md](README.md) into Français — corrections welcome.

# MiniVibe

<div align="center">
  <img src="packages/desktop/build/README-images/MiniVibe.png" alt="Capture d'écran de MiniVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/minivibe">minivibe.eu</a>
</p>

MiniVibe est la **version MiniMax** de la famille _Vibe_ — un fork de ZCode centré sur un seul fournisseur : **MiniMax**. Un modèle, un espace de travail, un partenaire — pas un agent.

La famille _Vibe_ propose une application dédiée par fournisseur (DeepVibe pour DeepSeek, KimiVibe pour Kimi, LamaVibe pour Ollama, MiniVibe pour MiniMax, …), chacune avec son propre caractère. Elle existe **aux côtés** de ZCode, et non à sa place : ZCode pour le flux de travail multi-fournisseurs, les applications Vibe pour celles et ceux qui veulent un modèle, un espace de travail, un partenaire. Consultez le dépôt source principal pour l'intégralité du code.

## Téléchargements

Les installateurs pour macOS, Windows et Linux sont publiés dans [Releases](../../releases). Le programme de mise à jour intégré vérifie ce dépôt.

## Compilation depuis les sources

Nécessite Git, Node.js **24.14.0** et pnpm **10.33.2** (voir `mise.toml`).

```bash
pnpm bootstrap
# run the MiniVibe flavor in dev
pnpm dev:desktop:mini
# package (MiniVibe flavor)
ZCODE_MINI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licence et attribution

Basé sur ZCode (Apache-2.0) ; la licence et le fichier NOTICE sont conservés. MiniVibe est un projet indépendant et n'est affilié ni à ZCode/Z.ai ni à MiniMax. MiniMax est une marque déposée de son propriétaire ; le logo est utilisé avec l'autorisation de l'exploitant.
