# おはなし どっかい（試作版）

GitHub Pagesで動く、AI API不要の四択読解ゲームです。既存の5w1h-readingとは別リポジトリで公開してください。

## 公開手順
1. 新規GitHubリポジトリを作成し、このフォルダ内のファイルと `stories` フォルダを配置します。
2. Settings → Pages → Deploy from a branch → main / (root) → Save を選びます。
3. 公開URLで動作確認します。`index.html` を端末から直接開く方式では JSON 読み込みが失敗する場合があります。

## 問題追加
1. `stories/story002.json` のように新しい問題セットを追加します。
2. `stories/index.json` の `stories` 配列にタイトルとファイル名を追加します。
3. JSONの `correct` は0～3の番号、`evidence` は原文に完全一致する文の配列です。
4. 問題は5～8問、選択肢は各4個です。根拠文が本文に存在しないと読み込みを停止します。

※最初の問題は画面の動作確認用のサンプルであり、教材としての最終承認済み問題ではありません。
