# 問題2：バグ診断（`hover:` の使い方ミス）（15分）

このフォルダ（`week04-2`）で作業してください。`index.html` を開いてください。

次のコードは「ホバーしたらボタンの背景色を濃くする」つもりですが、ホバーしても変化しません。何が問題か説明し、修正してください。

`index.html` にはボタンに加え、同じ種類のバグがカードにも入っています。`hover:` の直後にスペースが入っていないか、全体を確認してください。

```html
<a href="#" class="bg-blue-600 text-white px-5 py-3 rounded-lg font-bold hover: bg-blue-700 transition">
  詳細を見る
</a>
```

#### 仕様

| 項目 | 正しい書き方 |
|---|---|
| 通常背景 | `bg-blue-600` |
| ホバー背景 | `hover:bg-blue-700` |
| 文字 | `text-white font-bold` |
| 角丸 | `rounded-lg` |
| 余白 | `px-5 py-3` |
| なめらかな変化 | `transition` |

#### 掲載する内容

- 見出し：ホバー診断カード
- 説明：マウスを乗せるとボタンの色が変わります
- ボタン：詳細を見る
- 修正対象：`hover: bg-blue-700` を `hover:bg-blue-700` に直す

#### Step 1：バグの原因を文章で書く

`hover:` と `bg-blue-700` の間にスペースがあると、Tailwind は `hover:bg-blue-700` という1つのクラスとして認識できません。

#### Step 2：クラス名を1つだけ直す

`hover: bg-blue-700` ではなく、スペースなしの `hover:bg-blue-700` にしてください。

#### Step 3：Chrome でホバーして確認する

ボタンにマウスを乗せたときだけ背景色が濃くなれば OK です。**`goal.png`** でも見た目を確認してください。
