# 使い方

## 更新運用
更新は Claude Code セッションで手動実行する。
シェルスクリプトや CI 自動化は意図的に設けていない。

### 更新手順
1. `modsharp-catalog` ディレクトリで Claude Code を起動
2. 「カタログを更新して」等と指示する
3. Claude Code が `CLAUDE.md` の手順に従って自動で実行する
4. 変更内容を確認してコミット

## プラグインプロジェクトからの参照

### submoduleとして追加
```bash
cd my-plugin
git submodule add <this-repo-url> refs/modsharp-catalog
git commit -m "Add ModSharp catalog reference"
```

### プラグイン側 CLAUDE.md に参照を追加
```markdown
## 参照資料
ModSharp開発時は以下を参照:
- APIカタログ: @refs/modsharp-catalog/catalog/_index.md
- 検証済みパターン: refs/modsharp-catalog/patterns/
- ハマりどころ: @refs/modsharp-catalog/gotchas.md

## ワークフロー
1. _index.md で該当namespaceを特定
2. projects/Sharp.Shared/namespaces/ を読む
3. Source Generator生成型(エンティティ等)も同じく参照可能
4. patterns/ に類似例がないか確認
5. 実装前に gotchas.md をチェック
```

### 更新の取り込み
プラグイン側で必要になったタイミングで:
```bash
git submodule update --remote refs/modsharp-catalog
git commit -am "Update catalog reference"
```

## 新マシンでのclone
```bash
git clone --recurse-submodules <plugin-repo-url>
```

`--recurse-submodules` を忘れないこと。
`git config --global submodule.recurse true` で自動化可能。

## 備考: ローカルパスからの submodule テスト
動作確認のためにローカルファイルシステム上のrepoを submodule として追加したい場合、
modern git は `file://` 経由のクローンを既定で拒否する。ワンショットで許可するには:
```bash
git -c protocol.file.allow=always submodule add /path/to/modsharp-catalog refs/modsharp-catalog
```
通常運用(GitHub などのリモートURL)ではこの設定は不要。
