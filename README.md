🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**Public game data repository for the [Spyglass](https://github.com/beryndil/Spyglass) Android app.**

This repository contains hand-validated Minecraft Java Edition reference data used by the Spyglass app. Data is served via a CDN at `data.hardknocks.university` and synced automatically by the app every 12 hours.

## Disclaimer

**Spyglass is not affiliated with, endorsed by, or associated with Mojang Studios or Microsoft.** Minecraft is a trademark of Mojang Studios. All game data is used for informational and reference purposes only.

---

## Data Files

| File | Entries | Description |
|------|---------|-------------|
| `blocks.json` | 1,167 | All Java Edition blocks with descriptions, hardness, blast resistance, and drops |
| `items.json` | 502 | Items with durability, stack size, renewable/non-renewable flags |
| `recipes.json` | 1,291 | Crafting, smelting, blasting, smoking, campfire, stonecutting, and loom recipes |
| `mobs.json` | 81 | All mob types with health, attack damage, drops, and spawn conditions |
| `trades.json` | 231 | Villager trades for all 13 professions + wandering trader |
| `biomes.json` | 65 | All biomes with descriptions, building palettes, and spawn data |
| `structures.json` | 25 | Generated structures with loot tables and associated mobs |
| `enchants.json` | 43 | All enchantments including 1.21+ additions |
| `potions.json` | 130 | Base, splash, and lingering variants with brewing paths |
| `commands.json` | 85 | Full Java Edition command reference |
| `advancements.json` | 125 | All 5 advancement tabs with requirements and rewards |
| `version_tags.json` | 1,279 | Edition/version data with Java/Bedrock availability |
| `tips.json` | 87 | In-app tips with edition-specific tags |
| `texture_map.json` | — | Mapping of item/block IDs to texture filenames |
| `textures.zip` | ~696 | Downloadable texture pack (~1.3 MB) |
| `manifest.json` | — | Per-file version tracking for incremental sync |

## How Sync Works

The Spyglass app checks `manifest.json` periodically. Each data file has an independent version string. Only files with newer versions are downloaded — keeping updates small and fast.

Version format: `ZodiacName.MMDD.HHmm` (e.g., `FireHorse.0308.1430`)

## Data Quality

All data is validated against the [Minecraft Wiki](https://minecraft.wiki/). Cross-reference audits ensure accuracy across categories. See the Spyglass app repository for validation history.

---

## Related Projects

- **[Spyglass](https://github.com/beryndil/Spyglass)** — The Android companion app
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — Desktop companion for live world streaming

---

## Credits

**Spyglass Data** is maintained by **Beryndil**.

## License

Copyright (c) 2026 Beryndil. All rights reserved. The data in this repository is provided for use with the Spyglass application. Redistribution or use in other applications requires written permission.
