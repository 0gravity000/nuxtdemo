<template>
  <div>
    <h3>全体構造とメタ情報</h3>
<pre>
1-4-1 html要素

<!DOCTYPE html>
<html lang="ja">
<head>
・・・
</head>
<body>
・・・
</body>
</html>

1-4-2 head要素

1-4-3 body要素

1-4-4 title要素

<!DOCTYPE html>
<head>
<title>会社概要 | マイナビ</title>
</head>
<body>
・・・
<h1>会社概要</h1>
・・・
</body>

1-4-5 meta要素

<!DOCTYPE html>
<head>
<meta charset="UTF-8">
<title>meta要素の使用例</title>
<meta name="author" content="大藤 幹">
<meta name="description" content="meta要素のサンプルソースです。">
<meta name="keywords" content="meta, メタデータ, プラグマディレクティブ">
<!-- <meta http-equiv="refresh" content="10; URL=page2.html">   10秒後にpage2.htmlに移動-->
・・・
</head>

1-4-6 link要素

<head>
・・・
<link rel="stylesheet" href="style.css">
<link rel="icon" href="favicon.png" sizes="16x16" type="image/png">
<link rel="alternate" href="en.html" hreflang="en" type="text/html" title="EnglishVersion">
<link rel="alternate" href="fr.html" hreflang="fr" type="text/html" title="FrenchVersion">
・・・
</head>

1-4-7 base要素

<!DOCTYPE html>
<html lang="ja">
<head>
<title>マイナビブックス</title>
<!-- <base href="http://www.mynavi.com/books/index.html"> -->
</head>
<body>
<!-- <p><a href="new.html">新刊情報</a></p> -->
<!-- 上のリンクは「http://www.mynavi.com/books/new.html」となります -->
</body>
</html>

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
