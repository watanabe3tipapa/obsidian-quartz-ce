# 📂 obsidian-quartz-ce / GitHub Pages Template

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-0.1.0-green.svg)

### *GitHub Pagesで Obsidianノートブック を公開するためのテンプレート*




## ⚙️ このリポジトリの使い方

##### 要件（手順）

- このリポジトリをフォークします。（詳細省略）

- フォークしたリポジトリの "Settings" > "Pages" の "Build and Deployment" の事項でGitHub Actionsを選択します。　>> Actionsが動き出します

- フォークしたリポジトリをデバイスにクローンします。（詳細省略）

- Note（Obsidianまたテキストエディタで編集したマークダウンファイル）は [source/content](./source/content)に置きます。:（基本的に）Obsidianの書庫をここに設定すれば使い勝手が良いです

- HTMLへの変換は [Quartz](https://github.com/jackyzha0/quartz) が行います。 
- `source` ディレクトリが Quartz の本体です。

### 💻 ローカルでの開発（プレビュー）

ローカル環境でプレビューを行うには、`source` ディレクトリに移動してコマンドを実行します。

1. **初回セットアップ**: 依存関係をインストールします。
   ```bash
   cd source
   npm install
   ```

2. **プレビュー起動**: サーバーを立ち上げて変更を確認します。
   ```bash
   npx quartz build --serve
   ```
   コマンド実行後、ブラウザで `http://localhost:8080` にアクセスしてください。

### 🚀 デプロイ（GitHub Pages）

GitHub Actions が設定されているため、GitHub にプッシュするだけで自動的にビルドとデプロイが行われます。
`source/content` 内のマークダウンファイルを編集してプッシュしてください。
  

- 他に（Raw HTML pages）を実装できるようになっています。
 [source/raw_html](./source/raw_html) に該当ファイルを置いてください。  
Example1: https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-test.html  
Example2: https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-markdown-editor.html  

Example3:  coming soon ... 



#### Quartz の利点

Quartzは、コーディングを知らなくても、非常に設定しやすいように設計されています。
必要な設定のほとんどは、quartz.config.tsを編集するか、quartz.layout.tsでレイアウトを変更するだけでできるという点が推しです。


公開URL（RSS配信）: https://watanabe3tipapa.github.io/obsidian-quartz-ce


---
