# 問題1：部室備品リスト（forEach × テーブル）（20分）

このフォルダ（`week08-1`）で作業してください。

配列 `items` を **`forEach` で `<tbody>` に行追加**してください。

仕様表と `goal.png` を参考に実装します。`innerHTML` で一気に `tr` を組んでも、`createElement("tr")` でセルを足しても構いません。
**完成したら `goal.png` を開いて見比べてください。同じになっていれば OK です。**

作業前に、「データ形・ループ・DOM の親」を表に書いてから進めてください。

#### 仕様

| 項目 | Tailwindクラス / 内容 |
|---|---|
| ページ背景 | `bg-gray-50` |
| テーブル | `bg-white rounded-xl shadow overflow-hidden` |
| thead | `bg-gray-100` |
| 列 | 備品名 / 数量 / 借用者 |
| 借用者が「なし」の行 | `text-gray-400`（それ以外は `text-gray-800`） |

#### 掲載する内容

```js
const items = [
  { name: "プロジェクター", qty: 1, borrower: "田中" },
  { name: "ホワイトボード", qty: 2, borrower: "なし" },
  { name: "延長コード", qty: 3, borrower: "佐藤" },
  { name: "スピーカー", qty: 1, borrower: "なし" },
];
```

#### Step 1：`tbody#tableBody` を `getElementById` で取得し、初期は空のままにする

#### Step 2：`items.forEach` の中で `tr` を作り、3セル（name / qty / borrower）のデータを入れる。borrowerが「なし」かどうかで文字色クラスを切り替える

#### Step 3：`goal.png` と行数・文字・借用者の色を照合する
