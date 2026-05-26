# 問題1：防災チェックリストLPを作る（25分）

このフォルダ（`week05-1`）で作業してください。

スマホでは上から順に読めて、PC幅では説明エリアとチェックリストが2カラムになる防災チェックリスト LP を作ります。
**完成したら `goal.png` を開いて見比べてください。同じになっていれば OK です。**

作業前に、スマホ幅と PC 幅（`md:` 以上）のレイアウトを表に書いてから進めてください。

#### 仕様

| 項目 | Tailwindクラス |
|---|---|
| ページ背景 | `bg-slate-100` |
| 全体幅 | `max-w-5xl mx-auto px-6 py-8` |
| ヘッダー | `flex flex-col md:flex-row md:items-center md:justify-between gap-3` |
| ナビ | `flex flex-col md:flex-row gap-2 md:gap-4 text-sm` |
| ヒーロー | `grid grid-cols-1 md:grid-cols-2 gap-6 items-stretch` |
| 左カラム | `bg-white rounded-2xl shadow p-6` |
| 右カラム | `bg-blue-900 text-white rounded-2xl shadow p-6` |
| チェックリスト | `space-y-3` |
| チェック項目 | `bg-white/10 rounded-lg p-3` |
| ボタン | `inline-block bg-orange-500 text-white px-5 py-3 rounded-lg font-bold hover:bg-orange-600 transition` |

#### 掲載する内容

- サイト名：防災スタート
- ナビ：備える / チェックリスト / 連絡先
- 見出し：今日からできる防災チェック
- 本文：水・食料・ライト・連絡手段を、家族で確認しておきましょう。
- ボタン：チェックを始める
- チェック項目：飲料水3日分 / モバイルバッテリー / 懐中電灯 / 家族の集合場所

#### Step 1：スマホ幅の順番を先に決める

接頭辞なしでは `grid-cols-1` にして、説明エリア → チェックリストの順に縦に積みます。

#### Step 2：PC幅の2カラムだけ `md:` で追加する

同じ親要素に `md:grid-cols-2` を追加します。`md:` は「768px以上で上書きする」指定です。

#### Step 3：DevTools で375pxと768pxを確認する

375px では1列、768px 以上では2列になっていれば OK です。横スクロールが出ていないかも確認してください。
