# 問題2：バグ診断（`md:` クラスが効かない）（15分）

このフォルダ（`week05-2`）で作業してください。`index.html` を開いてください。

次のコードは「スマホでは1列、md以上では2列」にしたいのに、期待通りに切り替わりません。何が問題か説明し、修正してください。

```html
<div class="grid grid-cols-1 md: grid-cols-2 gap-4">
  <div class="bg-white rounded-lg p-4">水</div>
  <div class="bg-white rounded-lg p-4">食料</div>
</div>
```

#### 仕様

| 項目 | 正しい書き方 |
|---|---|
| Grid有効化 | `grid` |
| スマホ幅 | `grid-cols-1` |
| md以上 | `md:grid-cols-2` |
| 余白 | `gap-4` |
| カード | `bg-white rounded-lg p-4 shadow` |

#### 掲載する内容

- 見出し：レスポンシブ診断
- 説明：375pxでは1列、768px以上では2列にします
- カード：水 / 食料
- 修正対象：`md: grid-cols-2` を `md:grid-cols-2` に直す

#### Step 1：バグの原因を文章で書く

`md:` と `grid-cols-2` の間にスペースがあると、Tailwind は `md:grid-cols-2` という1つのクラスとして認識できません。

#### Step 2：クラス名をスペースなしに直す

`md: grid-cols-2` ではなく `md:grid-cols-2` と書きます。

#### Step 3：375pxと768pxで表示を確認する

DevTools のレスポンシブモードで、375px では1列、768px 以上では2列になることを確認してください。**`goal.png`** も参考にしてください。
