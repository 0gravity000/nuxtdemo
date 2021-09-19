<template>
  <div>
    <h3>CSS適用の優先順位</h3>
<pre>
2-3-1 CSSの指定元による優先順位

優先度高
    製作者
    ユーザー
    ユーザーエージェント
        Chrome、Firefoxなどのブラウザ
優先度低

2-3-2 !importantで優先順位を高くする

優先度高
    ユーザーエージェント    !important付き
    ユーザー    !important付き
    製作者  !important付き
    製作者
    ユーザー
    ユーザーエージェント
        Chrome、Firefoxなどのブラウザ
優先度低

p {
    font-size: 24pt !important;
}

2-3-3 セレクタの詳細度による優先順位の計算方法
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
