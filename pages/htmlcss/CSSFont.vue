<template>
  <div>
    <h3>CSS フォント</h3>
<pre>
2-7-1 Webフォント
@font-faceでWeb上にあるフォントを指定することで、
そのフォントがインストールされていない環境でもそのフォントが表示させられるようになる

@font-face {
    font-family: mynaviFont;
    src: url(http://example.com/fonts/mynaviRegular.woff);
}
p { font-family: mynaviFont, serif; }

2-7-2 font-family プロパティ
フォントの種類を設定するプロパティ

p {
    font-family: "メイリオ", "ヒラギノ角ゴ Pro W3", Helvetica, sans-serif;
}

2-7-3 font-size プロパティ
フォントサイズを設定するプロパティ

2-7-4 font-weight プロパティ
同じフォントファミリーの中の太さの異なる書体を選択するためのプロパティ
単純に太字にしたい場合にも使用できる

2-7-5 font-style プロパティ
同じフォントファミリーの中のイタリックまたは社寺の書体を選択するためのプロパティ

2-7-6 font-variant プロパティ
同じフォントファミリーの中のスモールキャピタル（大文字を小さくしたような種類のフォント）の書体を選択する要素

2-7-7 font プロパティ
フォント関連プロパティの値をまとめて指定できるプロパティ

p {
    font: bold italic 13px/1.5 "メイリオ", "Meiryo", sans-serif;
}
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
