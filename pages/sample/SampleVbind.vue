<template>
  <div>
    <h3>v-bind（省略形 :）</h3>
    <span :title="message">
      マウスを数秒間、この文章の上に置くと、動的にバインドされたタイトルが表示されます。
    </span>
    <p>Mustache は、HTML 属性の内部で使用することはできません。代わりに、v-bind ディレクティブを使用する</p>
    <div :id="dynamicId" />
    <h4>属性が真偽値属性の場合</h4>
    <p>isButtonDisabled が null、undefined、または false の値を持つ場合、disabled属性は描画された button要素に含められません。</p>
    <button :disabled="isButtonDisabled">
      Button
    </button>
    <h4>動的引数 バージョン 2.6.0 から</h4>
    <p>角括弧で囲むことで JavaScript 式をディレクティブの引数に使うこともできます</p>
    <a :[attributeName]="url">リンク</a>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      message: 'title属性にバインドされたメッセージ',
      attributeName: 'href',
      url: 'https://jp.vuejs.org/v2/guide/syntax.html#%E5%8B%95%E7%9A%84%E5%BC%95%E6%95%B0',
      dynamicId: 'button-example01',
      isButtonDisabled: false
    }
  }
}
</script>
