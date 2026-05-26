# 問題2：バグ診断（map の return）（15分）

このフォルダ（`week08-2`）で作業してください。`index.html` を開いてください。

Console に **`undefined`** が混ざったリストになっています。

`map` のコールバックで**値を返していない**のが原因です。「名前 · 役割」の文字列を **return** して表示を直してください。

`index.html` には次のようなバグがあります。

```js
const lines = members.map((m) => {
  m.name + " · " + m.role;
});
```

**ヒント:** `map` は**新しい配列の要素になる値を `return` する**のが必須です。`forEach` だと戻り値は使われません。今回は `return m.name + " · " + m.role;` のように書きます。

修正後、リストに `undefined` が出ないことを確認してください。**`goal.png`** も参考にしてください。
