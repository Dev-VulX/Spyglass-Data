🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**Öffentliches Spieldaten-Repository für die [Spyglass](https://github.com/beryndil/Spyglass) Android-App.**

Dieses Repository enthält manuell validierte Minecraft Java Edition Referenzdaten, die von der Spyglass-App verwendet werden. Die Daten werden über ein CDN unter `data.hardknocks.university` bereitgestellt und alle 12 Stunden automatisch von der App synchronisiert.

## Haftungsausschluss

**Spyglass ist nicht mit Mojang Studios oder Microsoft verbunden, wird nicht von ihnen unterstützt oder ist mit ihnen assoziiert.** Minecraft ist eine Marke von Mojang Studios. Alle Spieldaten werden ausschließlich zu Informations- und Referenzzwecken verwendet.

---

## Datendateien

| Datei | Einträge | Beschreibung |
|-------|----------|--------------|
| `blocks.json` | 1,167 | Alle Java Edition Blöcke mit Beschreibungen, Härte, Explosionswiderstand und Drops |
| `items.json` | 502 | Gegenstände mit Haltbarkeit, Stapelgröße und Erneuerbar/Nicht-erneuerbar-Flags |
| `recipes.json` | 1,291 | Handwerks-, Schmelz-, Hochofen-, Räucher-, Lagerfeuer-, Steinmetz- und Webstuhl-Rezepte |
| `mobs.json` | 81 | Alle Mob-Typen mit Gesundheit, Angriffsschaden, Drops und Spawn-Bedingungen |
| `trades.json` | 231 | Dorfbewohner-Handel für alle 13 Berufe + wandernder Händler |
| `biomes.json` | 65 | Alle Biome mit Beschreibungen, Baupaletten und Spawn-Daten |
| `structures.json` | 25 | Generierte Strukturen mit Beutetabellen und zugehörigen Mobs |
| `enchants.json` | 43 | Alle Verzauberungen einschließlich 1.21+ Ergänzungen |
| `potions.json` | 130 | Basis-, Wurf- und Verweilende Varianten mit Brau-Pfaden |
| `commands.json` | 85 | Vollständige Java Edition Befehlsreferenz |
| `advancements.json` | 125 | Alle 5 Fortschritts-Tabs mit Anforderungen und Belohnungen |
| `version_tags.json` | 1,279 | Editions-/Versionsdaten mit Java/Bedrock-Verfügbarkeit |
| `tips.json` | 87 | In-App-Tipps mit editionsspezifischen Tags |
| `texture_map.json` | — | Zuordnung von Gegenstands-/Block-IDs zu Texturdateinamen |
| `textures.zip` | ~696 | Herunterladbares Texturpaket (~1,3 MB) |
| `manifest.json` | — | Versionsverfolgung pro Datei für inkrementelle Synchronisation |

## Wie die Synchronisation Funktioniert

Die Spyglass-App prüft `manifest.json` regelmäßig. Jede Datendatei hat einen unabhängigen Versionsstring. Nur Dateien mit neueren Versionen werden heruntergeladen — so bleiben Updates klein und schnell.

Versionsformat: `ZodiacName.MMDD.HHmm` (z.B., `FireHorse.0308.1430`)

## Datenqualität

Alle Daten werden gegen das [Minecraft Wiki](https://minecraft.wiki/) validiert. Kreuzreferenz-Audits stellen die Genauigkeit über alle Kategorien sicher. Siehe das Spyglass-App-Repository für die Validierungshistorie.

---

## Verwandte Projekte

- **[Spyglass](https://github.com/beryndil/Spyglass)** — Die Android-Begleiter-App
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — Desktop-Begleiter für Live-Welt-Streaming

---

## Danksagung

**Spyglass Data** wird von **Beryndil** gepflegt.

## Lizenz

Copyright (c) 2026 Beryndil. Alle Rechte vorbehalten. Die Daten in diesem Repository werden zur Verwendung mit der Spyglass-Anwendung bereitgestellt. Weiterverbreitung oder Nutzung in anderen Anwendungen erfordert eine schriftliche Genehmigung.
