# 問題2：バグ診断（querySelector）（15分）

このフォルダ（`week07-2`）で作業してください。`index.html` を開いてください。

Console に **Cannot read properties of null** が出ます。

ボタンを押すと文言が差し代わるのが正しい動きです。`querySelector` の**セレクター文字列**のどこが間違いか説明し、修正してください。

`index.html` には次のようなバグがあります。

```js
// バグ: ID なのに # を付けていない
const btn = document.querySelector("swapBtn");
```

**ヒント:** `document.querySelector("swapBtn")` は **タグ名 `swapBtn` を探している**状態です。`id="swapBtn"` を取りたいときは `document.querySelector("#swapBtn")` とし、ID には `#` が必要です。

修正後、ボタンクリックで見出しとメッセージが差し替わることを確認してください。**`goal.png`** も参考にしてください。
