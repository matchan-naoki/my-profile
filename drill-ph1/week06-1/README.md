# 問題1：割り勘計算ツール（20分）

このフォルダ（`week06-1`）で作業してください。

`index.html` に骨組みがあります。**この README の仕様表**と **`goal.png`** を見比べて、同じレイアウトになれば OK です（完成答えの HTML は配布していません）。

作業前に、「入力 → 処理 → 出力」の分解表を埋めてから進めてください。

#### 仕様

| 項目 | Tailwindクラス / 内容 |
|---|---|
| ページ背景 | `bg-gray-50` |
| カード | `max-w-sm w-full mx-auto bg-white rounded-xl shadow-lg p-8` |
| h1 | `text-2xl font-bold text-gray-900 mb-6`、テキスト「割り勘計算」 |
| 入力 | 「合計金額（円）」「人数」の `type="number"` |
| ボタン | `bg-blue-600 text-white w-full py-2 rounded-lg font-semibold hover:bg-blue-700`、テキスト「計算する」 |
| 結果表示 | `id="result"` — 「1人あたり: ¥〇〇」`text-3xl font-bold text-center`。**端数は切り上げ**（`Math.ceil`） |
| ガード | 未入力・0以下は「入力を確認してください」などで表示 |
| JS | `.value` は文字列なので `Number(...)` で数値へ変換してから計算 |

#### Step 1：分解表と仕様表を見ながら、ラベル・入力・ボタン・結果の構造を `index.html` に実装する

#### Step 2：`addEventListener` でクリック時に `Number` → 割り算 → `Math.ceil` の順で実装する

#### Step 3：`goal.png` と並べて表示を確認する（情報の並びが揃っていれば OK）
