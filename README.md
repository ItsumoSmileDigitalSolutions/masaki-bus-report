# 松前町ひまわりバス レポート (ver25 修正版)

## 公開ページ
- 集計レポート: [index.html](./index.html) - 住民要望調査集計レポート
- ルート地図: [map.html](./map.html) - Leafletベース地図・ver25（要注意区間ボタン修正版）

## ver24からの修正内容
- ver24で「⚠️ 要注意区間」ボタンをONにしても表示されなかった問題を修正
- 原因: POPUP_OPTS変数が未定義タイミングで参照されており JavaScript エラーで停止していた
- 修正: forEach内の POPUP_OPTS 参照を直接オブジェクトリテラルに置換
