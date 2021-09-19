<template>
  <div>
    <h3>CSS その他</h3>
<pre>
2-11-1 直線状のグラデーション

linear-gradient(方向, 開始色, 終了色)

background: linear-gradient(#ddd, #333);
background: linear-gradient(to bottom, #ddd, #333);
background: linear-gradient(180deg, #ddd, #333);
background: linear-gradient(180deg, #ddd 0%, #333 100%);

2-11-2 放射状のグラデーション

radial-gradient(中心の位置, 中心の色, 外側の色)

background: radial-gradient(#ddd, #333);
background: radial-gradient(at center, #ddd, #333);
background: radial-gradient(at 50% 50%, #ddd, #333);

2-11-3 リスト関連のプロパティ

2-11-4 テーブル関連のプロパティ

2-11-5 内容を追加するプロパティ

body {
    counter-reset: chapter;
}
h1::before {
    counter-increment: chapter;
    content: "第" counter(chapter) "章 ";
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
