# NAS Card (FR)

Carte Home Assistant pour NAS Synology, au style verre, optimisée pour iPhone, iPad et kiosque en mode portrait.
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

## Licence

AGPL-3.0-only — voir [LICENSE](LICENSE). Auteur d'origine : BeGiBue.
