# 請求書メーカー

ブラウザだけで動く請求書作成ツールです（サーバー不要）。Word（.docx）ダウンロードと、印刷機能経由のPDF保存に対応しています。

## GitHub Pagesで公開する
1. このフォルダの中身（`index.html` と `vendor/`）をGitHubリポジトリに置く
2. Settings → Pages → Branch を `main` / `(root)` に設定して保存
3. 表示されたURLにアクセス

## 使い方
- 左のフォームに入力すると、右のプレビューにリアルタイムで反映されます
- 「Wordでダウンロード」でdocxを保存
- 「PDFで保存」で印刷画面が開くので、送信先を「PDFに保存」にしてください（余白は「なし」、ヘッダーとフッターはオフ推奨）
- 請求者情報・振込先・備考は、このブラウザのlocalStorageに保存されます（サーバーには送信されません）

`vendor/docx.iife.js` は [docx](https://github.com/dolanmiu/docx)（MIT License）です。
