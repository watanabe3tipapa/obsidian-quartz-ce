# 📂 obsidian-quartz-ce / GitHub Pages Template


### *GitHub Pagesで Obsidianノートブック を公開するためのテンプレート*




## ⚙️ このリポジトリの使い方

##### 要件（手順）

- このリポジトリをフォークします。（詳細省略）

- フォークしたリポジトリの "Settings" > "Pages" の "Build and Deployment" の事項でGitHub Actionsを選択します。　>> Actionsが動き出します

- フォークしたリポジトリをデバイスにクローンします。（詳細省略）

- Note（Obsidianまたテキストエディタで編集したマークダウンファイル）は [source/content](./source/content)に置きます。:（基本的に）Obsidianの書庫をここに設定すれば使い勝手が良いです

- HTMLへの変換は [Quartz](https://github.com/jackyzha0/quartz)　が行います。 

- ローカル環境へのHTML変換は`./source/`で次のコマンドで行います。

初回コマンドは、
  `cd source && npm install && npx quartz build --serve`

それ以降は必ず`./source`で次のコマンドを実行してください。
  `npx quartz build --serve`  
  

- 他に（Raw HTML pages）を実装できるようになっています。
 [source/raw_html](./source/raw_html) に該当ファイルを置いてください。  
Example1: https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-test.html  
Example2: https://watanabe3tipapa.github.io/obsidian-quartz-ce/raw-html-markdown-editor.html



#### Quartz の利点

Quartzは、コーディングを知らなくても、非常に設定しやすいように設計されています。
必要な設定のほとんどは、quartz.config.tsを編集するか、quartz.layout.tsでレイアウトを変更するだけでできるという点が推しです。


公開URL: https://watanabe3tipapa.github.io/obsidian-quartz-ce


---
