# ejs-amp-generator
EJS+gulpを使って、HTMLとAMP HTMLを同時に生成可能なHTMLジェネレータです

※このツールは現在未完成です。より精度を上げるため、今後も改修予定です。

## フォルダ構造
- html：通常のHTMLの出力先フォルダです。
- amp-html：AMP HTMLの出力先フォルダです。
- contents：HTMLの中身を管理するフォルダとなります。
  - amp-html-tmp：AMP HTML用の共通ファイルをまとめたファイル
  - normal-html-tmp：通常HTML用の共通ファイルをまとめたファイル
  - inner：各ページのコンテンツ用ファイルをまとめたフォルダ
  - css：サイトのCSSをまとめたフォルダ
  - image：サイト内で使う画像をまとめたフォルダ
  - json：EJSで変数箇所に挿入する内容をまとめたjsonファイル
- gulpfile.js：gulpでHTMLを生成するために色々書いたツールです。

## 使い方
※node.jsやEJS、gulpのインストールは説明割愛。

1. contentsの中身を編集
2. 「gulpfile.js」と同じ階層で下記のコマンドを実装
```
gulp ejs
```
3. 「html」と「amp-html」に出力されたファイルが格納される。
