<template>
  <div>
    <h3>HTMLの基礎知識</h3>
<pre>
1-1-1 基本的な書式と各部の名称
要素    Element
開始タグ
終了タグ

<br>
<br />

属性    Attribute
属性名
属性値

1-1-2 HTMLの全体構造
HTML文書の先頭には、DOCTYPE宣言をする必要がある
DOCTYPE宣言のあとには、html要素を配置し、
その中にheadとbody要素を順にはとつづつ配置する

<!DOCTYPE html>
<html>
    <head>
    ・・・
    <title>文書タイトル</title>
    ・・・
    </head>
    <body>

    ・・・

    </body>
</html>

1-1-3 DOCTYPE宣言

標準モード
後方互換モード

<!DOCTYPE html>
<!DOCTYPE HTML>
<!-- <!doctype html> -->

1-1-4 文字参照
名前指定文字参照    &lt;、&gt;
10進数数値文字参照  &#60;
16進数数値文字参照  &#x3C;

1-1-5 コメント

<!--コメント-->

<!--
コメント
-->

1-2 HTML5.1の要素とカテゴリー
1-2-1 HTML5の要素と種類
7つのカテゴリー

フローコンテンツ（Flow content）
見出しコンテンツ（Heading content）
セクショニングコンテンツ（Sectioning content）
フレージングコンテンツ（Phrasing content）
組み込みコンテンツ（Embedded content）
インタラクティブコンテンツ（Interactive content）
メタデータコンテンツ（Metadata content）
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
