🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**Dépôt public de données de jeu pour l'application Android [Spyglass](https://github.com/beryndil/Spyglass).**

Ce dépôt contient des données de référence Minecraft Java Edition validées manuellement et utilisées par l'application Spyglass. Les données sont servies via un CDN à `data.hardknocks.university` et synchronisées automatiquement par l'application toutes les 12 heures.

## Avertissement

**Spyglass n'est pas affilié, approuvé ou associé à Mojang Studios ou Microsoft.** Minecraft est une marque déposée de Mojang Studios. Toutes les données du jeu sont utilisées à des fins d'information et de référence uniquement.

---

## Fichiers de Données

| Fichier | Entrées | Description |
|---------|---------|-------------|
| `blocks.json` | 1,167 | Tous les blocs Java Edition avec descriptions, dureté, résistance aux explosions et drops |
| `items.json` | 502 | Objets avec durabilité, taille de pile et indicateurs renouvelable/non renouvelable |
| `recipes.json` | 1,291 | Recettes d'artisanat, de fonte, de haut fourneau, de fumoir, de feu de camp, de tailleur de pierre et de métier à tisser |
| `mobs.json` | 81 | Tous les types de mobs avec santé, dégâts d'attaque, drops et conditions d'apparition |
| `trades.json` | 231 | Échanges de villageois pour les 13 professions + marchand ambulant |
| `biomes.json` | 65 | Tous les biomes avec descriptions, palettes de construction et données d'apparition |
| `structures.json` | 25 | Structures générées avec tables de butin et mobs associés |
| `enchants.json` | 43 | Tous les enchantements y compris les ajouts 1.21+ |
| `potions.json` | 130 | Variantes de base, jetable et persistante avec chemins de préparation |
| `commands.json` | 85 | Référence complète des commandes Java Edition |
| `advancements.json` | 125 | Les 5 onglets de progrès avec exigences et récompenses |
| `version_tags.json` | 1,279 | Données d'édition/version avec disponibilité Java/Bedrock |
| `tips.json` | 87 | Conseils dans l'application avec tags spécifiques à l'édition |
| `texture_map.json` | — | Correspondance des IDs d'objets/blocs aux noms de fichiers de textures |
| `textures.zip` | ~696 | Pack de textures téléchargeable (~1.3 Mo) |
| `manifest.json` | — | Suivi de version par fichier pour la synchronisation incrémentale |

## Comment Fonctionne la Synchronisation

L'application Spyglass vérifie `manifest.json` périodiquement. Chaque fichier de données a une chaîne de version indépendante. Seuls les fichiers avec des versions plus récentes sont téléchargés — gardant les mises à jour petites et rapides.

Format de version : `ZodiacName.MMDD.HHmm` (ex., `FireHorse.0308.1430`)

## Qualité des Données

Toutes les données sont validées contre le [Minecraft Wiki](https://minecraft.wiki/). Des audits de références croisées assurent la précision entre les catégories. Consultez le dépôt de l'application Spyglass pour l'historique de validation.

---

## Projets Associés

- **[Spyglass](https://github.com/beryndil/Spyglass)** — L'application compagnon Android
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — Compagnon bureau pour le streaming de mondes en direct

---

## Crédits

**Spyglass Data** est maintenu par **Beryndil**.

## Licence

Copyright (c) 2026 Beryndil. Tous droits réservés. Les données de ce dépôt sont fournies pour une utilisation avec l'application Spyglass. La redistribution ou l'utilisation dans d'autres applications nécessite une autorisation écrite.
