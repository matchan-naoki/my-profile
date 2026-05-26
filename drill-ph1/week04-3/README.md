# 問題3：ヘッダー + Grid + 画像の復習ページを作る（20分）

このフォルダ（`week04-3`）で作業してください。`images/team.svg` が同梱されています。

Week01〜03 の復習として、画像・ヘッダーの Flexbox・メインコンテンツの Grid を組み合わせたページを作ります。
**完成したら `goal.png` を開いて見比べてください。同じになっていれば OK です。**

#### 仕様

| 項目 | Tailwindクラス |
|---|---|
| ページ背景 | `bg-slate-100` |
| ヘッダー | `bg-white shadow` |
| ヘッダー内レイアウト | `flex justify-between items-center px-6 py-4` |
| ナビ | `flex gap-4 text-sm` |
| メイン幅 | `max-w-5xl mx-auto px-6 py-8` |
| メインGrid | `grid grid-cols-3 gap-4` |
| メインカード | `col-span-2 bg-white rounded-xl shadow p-6` |
| サイドカード | `bg-white rounded-xl shadow p-6` |
| 画像 | `<img src="./images/team.svg" alt="学習チームのイラスト" class="w-full h-48 object-cover rounded-lg">` |
| カードホバー | `hover:shadow-lg transition` |

#### 掲載する内容

- ヘッダーロゴ：POSSE Studio
- ナビ：About / Works / Contact
- メイン見出し：仲間と作るWebページ
- 本文：HTMLの構造、Flexboxの横並び、Gridのカード配置を組み合わせて練習します。
- サイドカード3つ：HTML復習 / Flex復習 / Grid練習

#### Step 1：ヘッダーだけ作り、`flex justify-between` が効いているか確認する

左にロゴ、右にナビが分かれていれば OK です。ナビの中も `flex gap-4` で横並びにします。

#### Step 2：メインコンテンツの親に `grid grid-cols-3 gap-4` を付ける

大きい紹介カードには `col-span-2`、右側の小さいカードエリアは1列分にします。

#### Step 3：画像パスと Grid の列幅を確認する

画像が表示されているか、メインカードが2列分・サイドカードが1列分になっているかを `goal.png` と見比べてください。
