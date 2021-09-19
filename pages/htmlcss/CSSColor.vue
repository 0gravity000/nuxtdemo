<template>
  <div>
    <h3>CSS 色</h3>
<pre>
2-4-1 色を示す値：16進数

#ff0000

#f00

2-4-2 色を示す値：キーワード

2-4-3 色を示す値：rgb()、rgba()

rgb(255, 0, 0)

rgba(255, 0, 0, 0.5)

2-4-4 色を示す値：hsl()、hsla()

hsl(0, 100%, 50%)

hsla(0, 100%, 50%, 0.5)

2-4-5 colorプロパティ
テキストの文字色を設定するプロパティ

body { color: #333; }

2-4-6 opacityプロパティ
要素の不透明度を設定するプロパティ

h1 { opacity: 0.5; }
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
