<template>
  <div>
    <h3>v-bind（省略形 :）</h3>
    <span :title="message">
      マウスを数秒間、この文章の上に置くと、動的にバインドされたタイトルが表示されます。
    </span>
  </div>
</template>

<script>
export default {
  layout: 'sample',
  data () {
    return {
      message: 'title属性にバインドされたメッセージ'
    }
  }
}
</script>
