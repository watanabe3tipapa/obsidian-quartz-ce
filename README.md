# 📂 obsidian-quartz-ce / GitHub Pages テンプレート

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-0.1.0-green.svg)

GitHub Pages で Obsidianノートブックを公開するためのテンプレートです。HTML 生成は Quartz を利用します。公開ページ（RSS配信）は以下の URL で確認できます。

公開URL: https://watanabe3tipapa.github.io/obsidian-quartz-ce/

---

## 主な内容

- Obsidian（または任意の Markdown）を source/content に置くことで、Quartz を用いて静的サイトとして公開できます。
- ビルドとデプロイは GitHub Actions を利用可能な設定になっています（Settings > Pages の Build and Deployment で GitHub Actions を選択します）。
- raw HTML を置けるディレクトリ（source/raw_html）も用意されています。

## 必要条件（前提）

- Node.js / npm がインストールされていること（ローカルでのプレビュー時）。
- GitHub リポジトリをフォークして Pages のビルド方法に GitHub Actions を選ぶこと（Actions が稼働するようにするため）。

## セットアップ（ローカルでの開発 / プレビュー）

1. フォークしたリポジトリをクローンし、source ディレクトリに移動します。

   ```bash
   cd source
   npm install
   ```

2. ローカルプレビュー用サーバーを起動します。

   ```bash
   npx quartz build --serve
   ```

   コマンド実行後、ブラウザで http://localhost:8080 にアクセスして確認してください。

## デプロイ（GitHub Pages）

- リポジトリ設定で GitHub Actions を有効にしておくと、ソース（source/content 内の Markdown）をコミットしてプッシュするだけで自動的にビルドとデプロイが実行されます。

## コンテンツの配置

- Markdown（Obsidian の Vault）: source/content に配置します。Obsidian の書庫をそのままここに設定すると扱いやすい構成です。
- raw HTML: source/raw_html にファイルを置くことで、直接参照できる HTML ページを追加できます。

例:
- https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-test.html
- https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-markdown-editor.html
- Example3: coming soon ...

## Quartz に関して

- HTML への変換は Quartz が行います。
- 主な設定は quartz.config.ts、レイアウトは quartz.layout.ts を編集することで調整できます。

## ライセンス

このリポジトリには LICENSE ファイルが含まれており、README のバッジから MIT ライセンスであることが示されています。

## 開発・保守状態

- リポジトリはアーカイブされていません（archived: false）。

---

README に記載された事実に基づき構成しています。追加の設定手順やカスタマイズ方法は、リポジトリ内の source ディレクトリや Quartz の公式ドキュメント（README 内記載のリンク）を参照してください。
