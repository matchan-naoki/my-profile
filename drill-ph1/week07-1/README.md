# 問題1：数量カウンター（20分）

このフォルダ（`week07-1`）で作業してください。

`-` / `+` ボタンで数量を変え、**0 未満にならない**こと、**在庫上限 10** で止まること、単価980円で**合計金額を更新**することがゴールです。
**完成したら `goal.png` を開いて見比べてください。同じになっていれば OK です。**

作業前に、「取得する要素・イベント・処理内容」を表に書いてから進めてください。

#### 仕様

| 項目 | Tailwindクラス / 内容 |
|---|---|
| ページ背景 | `bg-gray-100` |
| カード | `max-w-xs mx-auto bg-white rounded-xl shadow-lg p-8 text-center` |
| h2 | `text-xl font-bold text-gray-900 mb-1` |
| 在庫テキスト | `text-gray-500 text-sm mb-6` |
| ボタンエリア | `flex items-center justify-center gap-4 mb-6` |
| マイナスボタン | `bg-gray-200 w-10 h-10 rounded-full text-xl font-bold text-gray-700`（0以下に行かない） |
| 数値表示 | `id="count"` `text-3xl font-bold text-gray-900` |
| プラスボタン | `bg-blue-600 text-white w-10 h-10 rounded-full text-xl font-bold`（在庫上限10） |
| 合計 | `id="total"` `text-gray-700 font-semibold` |

#### 掲載する内容

- h2：商品名（「プログラミング入門書」など）
- 在庫テキスト：在庫: 10個
- 初期値：1、上限 `const MAX = 10`、単価 `const PRICE = 980`
- 合計：「合計: ¥〇〇」（`count * PRICE` を `toLocaleString()` で表示）

#### Step 1：`let count = 1` と `const MAX = 10` `const PRICE = 980` を決め、HTML にボタンと表示枠を置く

#### Step 2：`refresh()` で `count` の表示と合計金額をまとめて更新する。`disabled` も付けると上限・下限の挙動が分かりやすくなる

#### Step 3：`goal.png` と操作感を照合する（0 と 10 のときの挙動は必ず確認）
