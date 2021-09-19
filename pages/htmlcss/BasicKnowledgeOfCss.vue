<template>
  <div>
    <h3>CSSの基礎知識</h3>
<pre>
2-1-1 基本的な書式と各部の名称

セレクタ、宣言ブロック
h1 {
    color: white;
    font-size: 24px;
    text-shadow: 1px 1px 2px black;
}

プロパティ、値
h1 { color: white }

セレクタはカンマで区切って、複数指定することが可能
h1, p, address, small {
    color: #333;
    background: #fff;
}

CSSのコメントは /* */

2-1-2 link要素でHTMLに組み込む

<!DOCTYPE html>
<html>
<head>
・・・
<link rel="stylesheet" href="style.css">
</head>
<body>
・・・
</body>
</html>

link要素のmedia属性

link要素のtype属性

2-1-3 style要素でHTMLに組み込む

style要素に指定できる属性
media、type、nonce

<!DOCTYPE html>
<html>
<head>
・・・
<style>
  body {
    color: #333;
    background: #fff;
  }
  p { font-size: 13px; }
</style>
</head>
<body>
・・・
</body>
</html>

2-1-4 style属性でHTMLに組み込む

<!DOCTYPE html>
<html>
<head>
・・・
</head>
<body style="color: #333; background: #fff;">
<p style="font-size: 13px;">
・・・
</p>
</body>
</html>

2-1-5 @importでCSSに組み込む
@importを使用することで、CSSの中でさらに外部スタイルシートを読み込ませることができる

@import "style.css";
@import url("style.css");
@import "style.css" screen, print;

2-1-6 ボックスの構造

マージン
ボーダー
パディング

2-1-7 長さをあらわす単位

フォントに対する相対的な長さを表す単位
em, rem, ex, ch

ビューポートに対するパーセンテージで表す単位
vw, vh, vmin, vmax

絶対的な長さを表す単位
px, pt, pc, in, cm, mm, q

calc関数による計算式の指定
font-size: calc(100vw / 35);
margin: calc(1rem - 2px) calc(1rem - 1px);
</pre>
  </div>
</template>

<script>
export default {
  layout: 'LayoutHtmlcss',
  data () {
    return {
    }
  }
}
</script>

<style scoped>
</style>
