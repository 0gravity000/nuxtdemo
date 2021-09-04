<template>
  <div>
    <h3>トランジションクラス</h3>
    <a :href="pagelink">リンク</a>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      pagelink: 'https://jp.vuejs.org/v2/guide/transitions.html#%E3%83%88%E3%83%A9%E3%83%B3%E3%82%B8%E3%82%B7%E3%83%A7%E3%83%B3%E3%82%AF%E3%83%A9%E3%82%B9'
    }
  }
}
</script>

<style scoped>
</style>
