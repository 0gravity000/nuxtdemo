<template>
  <div>
    <h3>CSS アニメーション</h3>
<pre>
2-10-1 回転・拡大縮小・移動

2-10-2 transform プロパティ

div {
    width: 100px;
    height: 100px;
    color: #fff;
    background: #999;
    transform: translate(200px, 100px) scale(1.5, 1.5) rotate(45deg);
}

2-10-3 transform-origin プロパティ

transform-origin: top left;
transform: translate(200px, 100px) scale(1.5, 1.5) rotate(45deg);

2-10-4 CSS3のトランジションとは

2-10-5 transition-property プロパティ

#sample {
    transition-property: transform, opacity;
    transition-duration: 2s;
}

2-10-6 transition-duration プロパティ

#sample {
    transition-property: transform, opacity;
    transition-duration: 2s, 5s;
}

2-10-7 transition-timing-function プロパティ

2-10-8 transition-delay プロパティ

2-10-9 transition プロパティ

li {
    transition: background-color 3s;
    background-color: silver;
}
li:hover {
    background-color: red;
}

2-10-10 CSS3のアニメーションとは

2-10-11 @keyframes

@keyframes 名前 {
  0% {
    プロパティ: 値;
    プロパティ: 値;
    ・・・
  }
  x% {
    プロパティ: 値;
    プロパティ: 値;
    ・・・
  }

・・・

  x% {
    プロパティ: 値;
    プロパティ: 値;
    ・・・
  }

  100% {
    プロパティ: 値;
    プロパティ: 値;
    ・・・
  }
}

2-10-12 animation-name プロパティ

2-10-13 animation-duration プロパティ

#sample:hover {
    animation-name: jumping;
    animation-duration: 10s;
}

2-10-14 animation-timing-function プロパティ

2-10-15 animation-delay プロパティ

2-10-16 animation-iteration-count プロパティ

2-10-17 animation-direction プロパティ

2-10-18 animation-play-state プロパティ

2-10-19 animation-fill-mode プロパティ

2-10-20 animation プロパティ

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
