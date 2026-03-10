🌐 [English](README.md) | [Español](README.es.md) | [Português](README.pt.md) | [Français](README.fr.md) | [Deutsch](README.de.md) | [日本語](README.ja.md)

# Spyglass Data

**[Spyglass](https://github.com/beryndil/Spyglass) Androidアプリのための公開ゲームデータリポジトリ。**

このリポジトリには、Spyglassアプリで使用される、手動で検証されたMinecraft Java Editionのリファレンスデータが含まれています。データは `data.hardknocks.university` のCDN経由で配信され、アプリによって12時間ごとに自動同期されます。

## 免責事項

**SpyglassはMojang StudiosまたはMicrosoftとは一切関係がなく、承認や提携もされていません。** MinecraftはMojang Studiosの商標です。すべてのゲームデータは情報提供および参照目的のみに使用されています。

---

## データファイル

| ファイル | エントリ数 | 説明 |
|----------|-----------|------|
| `blocks.json` | 1,167 | 説明、硬度、爆破耐性、ドロップを含むJava Editionの全ブロック |
| `items.json` | 502 | 耐久値、スタックサイズ、再生可能/再生不可フラグを含むアイテム |
| `recipes.json` | 1,291 | クラフト、製錬、溶鉱炉、燻製器、焚き火、石切台、機織り機のレシピ |
| `mobs.json` | 81 | 体力、攻撃力、ドロップ、スポーン条件を含む全モブタイプ |
| `trades.json` | 231 | 13の職業すべて＋行商人の村人取引 |
| `biomes.json` | 65 | 説明、建築パレット、スポーンデータを含む全バイオーム |
| `structures.json` | 25 | 戦利品テーブルと関連モブを含む生成構造物 |
| `enchants.json` | 43 | 1.21+の追加を含む全エンチャント |
| `potions.json` | 130 | 醸造パスを含む通常、スプラッシュ、残留バリアント |
| `commands.json` | 85 | Java Editionコマンドの完全リファレンス |
| `advancements.json` | 125 | 要件と報酬を含む全5つの進捗タブ |
| `version_tags.json` | 1,279 | Java/Bedrock対応状況を含むエディション/バージョンデータ |
| `tips.json` | 87 | エディション固有のタグ付きアプリ内ヒント |
| `texture_map.json` | — | アイテム/ブロックIDからテクスチャファイル名へのマッピング |
| `textures.zip` | ~696 | ダウンロード可能なテクスチャパック（約1.3 MB） |
| `manifest.json` | — | 増分同期のためのファイルごとのバージョン追跡 |

## 同期の仕組み

Spyglassアプリは定期的に `manifest.json` を確認します。各データファイルには独立したバージョン文字列があります。新しいバージョンのファイルのみがダウンロードされ、更新を小さく高速に保ちます。

バージョン形式: `ZodiacName.MMDD.HHmm`（例: `FireHorse.0308.1430`）

## データ品質

すべてのデータは [Minecraft Wiki](https://minecraft.wiki/) に対して検証されています。クロスリファレンス監査により、カテゴリ間の正確性が保証されています。検証履歴についてはSpyglassアプリのリポジトリを参照してください。

---

## 関連プロジェクト

- **[Spyglass](https://github.com/beryndil/Spyglass)** — Androidコンパニオンアプリ
- **[Spyglass Connect](https://github.com/beryndil/Spyglass-Connect)** — ライブワールドストリーミング用デスクトップコンパニオン

---

## クレジット

**Spyglass Data** は **Beryndil** によって管理されています。

## ライセンス

Copyright (c) 2026 Beryndil. All rights reserved. このリポジトリのデータはSpyglassアプリケーションでの使用のために提供されています。他のアプリケーションでの再配布または使用には書面による許可が必要です。
