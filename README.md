# NAS Card (FR)

Carte Home Assistant pour NAS Synology, au style verre avec nuance de couleur au choix, optimisée pour iPhone, iPad et kiosque en mode portrait.
Traduction française de [home-assistant-nas-card](https://github.com/BeGiBue/home-assistant-nas-card) de BeGiBue (licence AGPL-3.0-only).

## Installation via HACS (dépôt personnalisé)

1. HACS → ⋮ (en haut à droite) → **Dépôts personnalisés**.
2. Collez l'URL de ce dépôt, choisissez la catégorie **Tableau de bord** (Dashboard), puis **Ajouter**.
3. Recherchez « NAS Card (FR) », cliquez sur **Télécharger**.
4. Rechargez le navigateur (Ctrl+Maj+R). HACS ajoute la ressource automatiquement.

## Utilisation

```yaml
type: custom:nas-card
title: DS720+
subtitle: Synology NAS
```

Toutes les options (entités, taille, disposition, image) se règlent dans l'éditeur visuel de la carte.
Les entités par défaut correspondent à l'intégration Synology DSM avec Home Assistant en allemand : adaptez-les si les vôtres sont nommées autrement.

## Apparence : thème et nuance de couleur

Dans l'éditeur visuel, section **Apparence** :

| Option | Valeurs |
|---|---|
| `theme` | `auto` (suit Home Assistant), `light`, `dark` |
| `nuance` | `theme` (par défaut), `braise`, `ocean`, `lagon`, `foret`, `lavande`, `framboise`, `ambre`, `ardoise`, `perso` |
| `nuance_perso` | Couleur au choix (sélecteur de couleur), utilisée avec `nuance: perso` |
| `intensite` | De `0` (neutre) à `2` (très coloré), `1` par défaut |

La nuance teinte le dégradé de fond et la couleur principale des tuiles ; les couleurs d'alerte (vert, orange, rouge) restent identiques.

**Une seule nuance pour toutes tes cartes** : laisse `nuance: theme` et ajoute cette ligne à ton thème Home Assistant (sans thème, c'est la nuance braise) :

```yaml
carte-nuance: "#2f8fd8"
```

## Historique des versions

- **2.1.0** : style verre propre à la carte (fond dégradé, panneaux en verre), thème clair/sombre automatique ou forcé, nuance de couleur au choix (8 nuances, couleur personnalisée, intensité, ou nuance commune via le thème) ; `validate.yml` déplacé dans `.github/workflows/`.
- **2.0.0** : version initiale.

## Licence

AGPL-3.0-only — voir [LICENSE](LICENSE). Auteur d'origine : BeGiBue.
