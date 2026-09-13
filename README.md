# 新人バイトFAQ MVP v1.2

固定URL方式の実店舗テスト候補。

## 構成
- `index.html`: 固定UI、検索、安全文、店舗データ検証
- `data/<store_id>.json`: 店舗データ
- `schema.json`: 生成前のJSON Schema

## 固定URL
`https://公開先/index.html?id=marufuku`

## 安全設計
- AIは店舗ルールを推測・補完しない
- 未登録は未登録のまま表示
- 緊急・医療・食品安全等はFAQで判断させない
- 質問フォームURLはHTTPSのみ
- `innerHTML`不使用
- 外部CDNなし
- URLの店舗IDとJSONの`store_id`を一致確認
- 不明・不正データはエラー表示

## テスト状態
静的・構造テストは実施。iPhone Safari実機および公開URLでの実地確認は未実施。
