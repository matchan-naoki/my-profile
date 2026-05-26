# 問題3：Flex + Grid + レスポンシブを全部使う（20分）

このフォルダ（`week05-3`）で作業してください。

Week03 の Flex、Week04 の Grid、Week05 のレスポンシブを全部使って、イベント紹介ページを作ります。
**完成したら `goal.png` を開いて見比べてください。同じになっていれば OK です。**

#### 仕様

| 項目 | Tailwindクラス |
|---|---|
| ページ背景 | `bg-gray-50` |
| ヘッダー | `flex flex-col md:flex-row md:items-center md:justify-between gap-3 px-6 py-4` |
| ナビ | `flex flex-col md:flex-row gap-2 md:gap-5 text-sm` |
| メイン幅 | `max-w-5xl mx-auto px-6 py-8` |
| ヒーロー | `flex flex-col md:flex-row gap-6 items-center` |
| ヒーロー画像枠 | `w-full md:w-1/2 bg-indigo-100 rounded-2xl h-56` |
| ヒーロー本文 | `w-full md:w-1/2` |
| カード一覧 | `grid grid-cols-1 md:grid-cols-3 gap-4` |
| カード | `bg-white rounded-xl shadow p-5 hover:shadow-lg transition` |

#### 掲載する内容

- サイト名：POSSE Weekend
- ナビ：概要 / タイムテーブル / 申し込み
- メイン見出し：週末に小さなWebサービスを作ろう
- 本文：チームでアイデアを出し、HTML・Tailwind・JavaScriptで形にする1日イベントです。
- カード1：アイデア出し / 10:00
- カード2：実装タイム / 13:00
- カード3：発表会 / 17:00

#### Step 1：ヘッダーをスマホ縦並び、md以上横並びにする

ヘッダーとナビの両方に `flex flex-col md:flex-row` を使います。PC幅では `md:justify-between` で左右に分けます。

#### Step 2：ヒーローを `flex-col md:flex-row` で切り替える

スマホでは画像枠が上、本文が下。md以上では左右50%ずつになるように `w-full md:w-1/2` を使います。

#### Step 3：カード一覧を `grid-cols-1 md:grid-cols-3` で切り替える

375px ではカードが縦1列、768px 以上では3列になっているかを `goal.png` と DevTools で確認してください。
