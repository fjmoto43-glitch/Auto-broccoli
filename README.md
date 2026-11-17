# TierBoard

ブラウザで使えるティア表メーカー。GitHub Pagesで公開できます。

## 機能
- 8段階（SS〜F）のティア表
- ドラッグ＆ドロップでカードを移動
- 改行区切りで一括追加
- ダブルクリックで名前変更、右クリックで削除
- Undo / Redo、ダークモード、PNG出力
- タイトル・作成者設定、ランク名編集
- localStorageによるブラウザ内自動保存
- 共有URL（作成時点のスナップショット）

## GitHub Pages
Settings → Pages → Build and deployment で「Deploy from a branch」を選び、Branch: main / Folder: /(root) を指定してください。

## 保存と共有の注意
現在は各ブラウザ内への保存です。端末間同期はありません。共有リンクはその時点のデータをURLに含めるコピー方式で、共同編集やリアルタイム同期ではありません。

## Firebase連携
firestore.rules は匿名認証を使う場合のルール案です。現時点のindex.htmlにはFirebase SDKは未接続です。Firebase ConsoleでAuthenticationのAnonymous providerとFirestoreを有効化し、ルールを適用した後にクラウド保存機能を実装してください。