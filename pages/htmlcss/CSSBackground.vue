<template>
  <div>
    <h3>CSS 背景</h3>
<pre>
2-5-1 background-color プロパティ
ボックスの背景色を設定するプロパティ

body { background-color: #fff; }

2-5-2 background-image プロパティ
背景に画像を表示させるプロパティ

body { background-image: url(a.png), url(b.png), url(c.png); }

body {
    background-image: url(a.png), url(b.png), url(c.png);
    background-repeat: no-repeat, repeat-x, repeat-y;
}

2-5-3 background-clip プロパティ
背景をボックスのどの領域に表示させるのかを設定するプロパティ

2-5-4 background-repeat プロパティ
背景画像を縦または横に繰り返して表示させるのかどうかを設定するプロパティ

2-5-5 background-size プロパティ
背景画像の表示サイズを設定するプロパティ

body {
    background-image: url(books.png);
    background-repeat: no-repeat;
    background-size: contain;
}

body {
    background-image: url(sky.jpg);
    background-size: cover;
}

2-5-6 background-origin プロパティ
背景画像の配置位置を指定する際の基準となる領域を設定するプロパティ

2-5-7 background-position プロパティ
背景画像を表示させる領域内での画像の配置位置を設定するプロパティ

body {
    background-image: url(logo.png);
    background-repeat: no-repeat;
    background-position: 100% 100%;
}

2-5-8 background-attachment プロパティ
背景画像を表示領域に固定して、ページの内容をスクロールしても動かないようにすることができる

2-5-9 background プロパティ
背景関連のプロパティの値をまとめて指定できるプロパティ

body {
    background: #ccc url(castle.jpg) bottom left / 100% auto no-repeat;
    /* 背景色が #ccc（グレー）、背景画像はcastle.jpg、背景画像の位置は左下を基準、表示領域に対して幅は100％、高さはautoで表示、画像の繰り返しはなし */
}

body {
    background: url(a.png) no-repeat, url(b.png) no-repeat, #ffffff url(c.png);
    /* 一番上（手前）の背景画像はa.pngで繰り返しはなし、真ん中の背景画像はb.pngで繰り返しはなし、一番下（後ろ）の背景画像はc.pngで背景色は#ffffff（白） */
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
