🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**Repositorio público de datos de juego para la aplicación Android [Spyglass](https://github.com/beryndil/Spyglass).**

Este repositorio contiene datos de referencia de Minecraft Java Edition validados manualmente y utilizados por la aplicación Spyglass. Los datos se sirven a través de un CDN en `data.hardknocks.university` y se sincronizan automáticamente con la aplicación cada 12 horas.

## Aviso Legal

**Spyglass no está afiliado, respaldado ni asociado con Mojang Studios o Microsoft.** Minecraft es una marca registrada de Mojang Studios. Todos los datos del juego se utilizan únicamente con fines informativos y de referencia.

---

## Archivos de Datos

| Archivo | Entradas | Descripción |
|---------|----------|-------------|
| `blocks.json` | 1,167 | Todos los bloques de Java Edition con descripciones, dureza, resistencia a explosiones y drops |
| `items.json` | 502 | Objetos con durabilidad, tamaño de pila y flags de renovable/no renovable |
| `recipes.json` | 1,291 | Recetas de crafteo, fundición, alto horno, ahumado, fogata, cortapiedras y telar |
| `mobs.json` | 81 | Todos los tipos de mobs con salud, daño de ataque, drops y condiciones de aparición |
| `trades.json` | 231 | Intercambios de aldeanos para las 13 profesiones + comerciante errante |
| `biomes.json` | 65 | Todos los biomas con descripciones, paletas de construcción y datos de aparición |
| `structures.json` | 25 | Estructuras generadas con tablas de botín y mobs asociados |
| `enchants.json` | 43 | Todos los encantamientos incluyendo las adiciones de 1.21+ |
| `potions.json` | 130 | Variantes base, arrojadiza y persistente con rutas de elaboración |
| `commands.json` | 85 | Referencia completa de comandos de Java Edition |
| `advancements.json` | 125 | Las 5 pestañas de logros con requisitos y recompensas |
| `version_tags.json` | 1,279 | Datos de edición/versión con disponibilidad en Java/Bedrock |
| `tips.json` | 87 | Consejos dentro de la aplicación con etiquetas específicas de edición |
| `texture_map.json` | — | Mapeo de IDs de objetos/bloques a nombres de archivo de texturas |
| `textures.zip` | ~696 | Paquete de texturas descargable (~1.3 MB) |
| `manifest.json` | — | Seguimiento de versiones por archivo para sincronización incremental |

## Cómo Funciona la Sincronización

La aplicación Spyglass verifica `manifest.json` periódicamente. Cada archivo de datos tiene una cadena de versión independiente. Solo se descargan los archivos con versiones más recientes, manteniendo las actualizaciones pequeñas y rápidas.

Formato de versión: `ZodiacName.MMDD.HHmm` (ej., `FireHorse.0308.1430`)

## Calidad de los Datos

Todos los datos están validados contra la [Minecraft Wiki](https://minecraft.wiki/). Las auditorías de referencia cruzada aseguran la precisión entre categorías. Consulta el repositorio de la aplicación Spyglass para ver el historial de validación.

---

## Proyectos Relacionados

- **[Spyglass](https://github.com/beryndil/Spyglass)** — La aplicación compañera para Android
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — Compañero de escritorio para transmisión de mundos en vivo

---

## Créditos

**Spyglass Data** es mantenido por **Beryndil**.

## Licencia

Copyright (c) 2026 Beryndil. Todos los derechos reservados. Los datos en este repositorio se proporcionan para uso con la aplicación Spyglass. La redistribución o el uso en otras aplicaciones requiere permiso por escrito.
