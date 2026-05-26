# 問題2：バグ診断（型変換・文字列と数値）（15分）

このフォルダ（`week06-2`）で作業してください。`index.html` を開いてください。

合計 **5000** 円・人数 **3** のとき、1人あたりは **1667** 円（切り上げ）になるはずですが、現状は `"50003"` のように**文字列の連結**になっています。原因を説明し、正しく計算されるよう修正してください。必要なら **`goal.png`** で表示の参考にします。

`index.html` のスクリプトには次のようなバグがあります。

```js
document.querySelector("#calcBtn").addEventListener("click", () => {
  const total = totalInput.value;
  const people = peopleInput.value;
  // バグ: 文字列のまま + してしまっている
  const perPerson = total + people;
  result.textContent = perPerson + " 円";
});
```

**ヒント:** `total + people` の `+` は、両方が文字列だと**足し算ではなく連結**になります。割り算には `Number(total)` と `Number(people)` を使い、結果に `Math.ceil` をかけます。

修正後、合計 5000・人数 3 で「1667 円」付近の正しい表示になることを確認してください。
