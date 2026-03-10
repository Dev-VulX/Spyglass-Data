🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**Repositório público de dados de jogo para o aplicativo Android [Spyglass](https://github.com/beryndil/Spyglass).**

Este repositório contém dados de referência do Minecraft Java Edition validados manualmente e utilizados pelo aplicativo Spyglass. Os dados são servidos via CDN em `data.hardknocks.university` e sincronizados automaticamente pelo aplicativo a cada 12 horas.

## Aviso Legal

**Spyglass não é afiliado, endossado ou associado à Mojang Studios ou Microsoft.** Minecraft é uma marca registrada da Mojang Studios. Todos os dados do jogo são utilizados apenas para fins informativos e de referência.

---

## Arquivos de Dados

| Arquivo | Entradas | Descrição |
|---------|----------|-----------|
| `blocks.json` | 1,167 | Todos os blocos da Java Edition com descrições, dureza, resistência a explosões e drops |
| `items.json` | 502 | Itens com durabilidade, tamanho de pilha e flags de renovável/não renovável |
| `recipes.json` | 1,291 | Receitas de crafting, fundição, alto-forno, defumador, fogueira, cortador de pedra e tear |
| `mobs.json` | 81 | Todos os tipos de mobs com vida, dano de ataque, drops e condições de spawn |
| `trades.json` | 231 | Trocas de aldeões para todas as 13 profissões + comerciante errante |
| `biomes.json` | 65 | Todos os biomas com descrições, paletas de construção e dados de spawn |
| `structures.json` | 25 | Estruturas geradas com tabelas de saque e mobs associados |
| `enchants.json` | 43 | Todos os encantamentos incluindo adições da 1.21+ |
| `potions.json` | 130 | Variantes base, arremessável e persistente com caminhos de preparação |
| `commands.json` | 85 | Referência completa de comandos da Java Edition |
| `advancements.json` | 125 | Todas as 5 abas de progressos com requisitos e recompensas |
| `version_tags.json` | 1,279 | Dados de edição/versão com disponibilidade Java/Bedrock |
| `tips.json` | 87 | Dicas no aplicativo com tags específicas de edição |
| `texture_map.json` | — | Mapeamento de IDs de itens/blocos para nomes de arquivo de texturas |
| `textures.zip` | ~696 | Pacote de texturas para download (~1.3 MB) |
| `manifest.json` | — | Rastreamento de versão por arquivo para sincronização incremental |

## Como a Sincronização Funciona

O aplicativo Spyglass verifica o `manifest.json` periodicamente. Cada arquivo de dados tem uma string de versão independente. Apenas arquivos com versões mais recentes são baixados — mantendo as atualizações pequenas e rápidas.

Formato de versão: `ZodiacName.MMDD.HHmm` (ex., `FireHorse.0308.1430`)

## Qualidade dos Dados

Todos os dados são validados contra a [Minecraft Wiki](https://minecraft.wiki/). Auditorias de referência cruzada garantem a precisão entre categorias. Consulte o repositório do aplicativo Spyglass para o histórico de validação.

---

## Projetos Relacionados

- **[Spyglass](https://github.com/beryndil/Spyglass)** — O aplicativo companheiro para Android
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — Companheiro desktop para streaming de mundos ao vivo

---

## Créditos

**Spyglass Data** é mantido por **Beryndil**.

## Licença

Copyright (c) 2026 Beryndil. Todos os direitos reservados. Os dados neste repositório são fornecidos para uso com o aplicativo Spyglass. Redistribuição ou uso em outros aplicativos requer permissão por escrito.
