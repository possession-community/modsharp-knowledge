# ModSharp Catalog

ModSharp (CS2/Source2 C# modding framework) のAPIカタログと開発知見集約リポジトリ。

## 目的
- AIアシスタント(Claude Code等)がModSharp APIを把握し適切に提案できるようにする
- Source Generatorで生成されるエンティティ情報等を含めた完全なAPIビューを提供する
- 動作検証済みの使用パターンを集約する
- ハマりどころを記録し再発を防ぐ

## ディレクトリ
- `external/modsharp/` - ModSharp本体 (submodule, commit固定)
- `catalog/` - 自動生成APIカタログ (Source Generator出力も含む)
- `patterns/` - 検証済み使用パターン(手動メンテ)
- `gotchas.md` - ハマりどころ集(手動メンテ)
- `CLAUDE.md` - Claude Code向けの更新手順書

## カタログ規模 (最新生成時点)
- Projects: 26 (Sharp.Shared / Sharp.Core / Sharp.Generator(.Sdk) / Sharp.Extensions.* / Sharp.Modules.*)
- Public Types: **1197** (うち Source Generator 由来: **64**)
- Public Methods: 9213
- Namespaces: 54
- プラグイン開発で最重要な `Sharp.Shared` は 1073 型 / 21 namespace

Source Generator 由来 64 型の一覧は `catalog/indexes/generated-types.md`。
protobuf メッセージの入れ子 `*.Types` がここに集約される。

## セットアップ (新マシン初回)
```bash
git clone --recurse-submodules <this-repo>
```
`--recurse-submodules` を忘れた場合は:
```bash
git submodule update --init --recursive
```

## 更新
このリポジトリで Claude Code セッションを起動し、
「カタログを更新して」等と指示する。
Claude Code が `CLAUDE.md` の手順に従って自動で実行する。

## 他プロジェクトからの参照
```bash
cd my-plugin
git submodule add <this-repo> refs/modsharp-catalog
```

CLAUDE.mdで:
```
ModSharp API: @refs/modsharp-catalog/catalog/_index.md
```

## ライセンス
- repo構造: MIT
- external/modsharp/: AGPL-3.0 (ModSharp本体)
- catalog/: ModSharpソース由来のためAGPL-3.0の影響を受ける可能性あり
