# GitHub MCP 使い方メモ

このファイルは、ChatGPT から GitHub MCP を使ってリポジトリを操作するテストとして作成しました。

## GitHub MCP でできること

GitHub MCP を接続すると、ChatGPT から GitHub リポジトリに対して次のような操作ができます。

- リポジトリ、ブランチ、ファイル、Issue、Pull Request の読み取り
- コード検索、コミット検索、Issue / PR 検索
- 新しいブランチの作成
- Markdown などのファイル作成・更新
- Issue の作成・更新、コメント追加
- Pull Request の作成・更新・マージ

## 安全な使い方

書き込み権限がある場合、直接 `main` ブランチに変更するよりも、次の流れにすると安全です。

1. 作業用ブランチを作成する
2. 作業用ブランチにファイルを追加・更新する
3. Pull Request を作成する
4. GitHub 上で内容を確認してからマージする

## 今回のテスト内容

今回は以下の操作を試しています。

1. `main` から `mcp-usage-test` ブランチを作成
2. `docs/github-mcp-usage.md` を作成
3. このMarkdownファイルに GitHub MCP の使い方を記録

## ChatGPT への依頼例

```text
GitHub MCPを使って、mainから新しいブランチを作成してください。
そのブランチに docs/research-note.md を追加し、内容はMarkdownでまとめてください。
最後にPull Requestを作成してください。
```

## 注意点

- APIキーやトークンなどの秘密情報は絶対に書き込まない
- 書き込み操作の前に対象リポジトリ・ブランチ・パスを確認する
- 本番リポジトリでは、まずPR作成までに留める
- MCPの権限は必要最小限にする
