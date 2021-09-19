<template>
  <div>
    <h3>CSS セレクタ</h3>
<pre>
2-2-1 セレクタの種類と組み合わせのルール

2-2-2 タイプセレクタ（要素名）

h1 { color: #333; }

2-2-3 ユニバーサルセレクタ（*）

* { color: #333; }

2-2-4 クラスセレクタ（.）

p.subtitle { color: #333; }

2-2-5 IDセレクタ（*）

ul#footnav { color: #333; }

2-2-6 属性セレクタ（[属性名]）
7種類の属性セレクタ
[属性名]
[属性名="属性値"]
[属性名~="属性値"]
[属性名|="属性値"]
[属性名^="属性値の始め"]
[属性名$="属性値の終り"]
[属性名*="属性値の一部"]

img[src$=".jpg"] { border: 3px solid #f00; }

2-2-7 リンク関連の擬似クラス（:）

使用頻度が高い4個。通常、この順番で指定する
a:link  リンク先をまだ見ていない状態のa要素
a:visited   リンク先を既に見た状態のa要素
a:hover カーソルが上にある状態の要素
a:active    マウスボタン等がおされている状態の要素

a:link { color: blue; }
a:visited { color: purple; }
a:hover { color: red; }
a:active { color: yellow; }

2-2-8 その他の擬似クラス（:）

残りの19個
:nth-child(式)
:nth-last-child(式)
:nth-of-type(式)
:nth-last-of-type(式)
:first-child
:last-child
:first-of-type
:last-of-type
:only-child
:only-of-type
:focus
:checked
:disabled
:enabled
:root
:empty
:target
:lang(言語コード)
:not(シンプルセレクタ)

tr:nth-child(odd) { background: #ccc; }

2-2-9 疑似要素（::）

::first-line    ブロックレベル要素の1行目
::first-letter  ブロックレベル要素の1文字目
::before    要素内容の先頭にコンテンツを追加
::after 要素内容の最後にコンテンツを追加

2-2-10 結合子
セレクタA 空白文字 セレクタB    Aの子孫のB
セレクタA > セレクタB   Aの直接の子のB
セレクタA + セレクタB
セレクタA ~ セレクタB
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
