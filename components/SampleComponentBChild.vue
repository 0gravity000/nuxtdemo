<template>
  <div>
    <h4>コンポーネント その2 子</h4>
    <p>$emitの2番目のパラメータは引数</p>
    <button @click="$emit('enlarge-text', 0.1)">
      拡大
    </button>
    <button @click="$emit('shrink-text', 0.1)">
      縮小
    </button>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  props: {
  },
  data () {
    return {
    }
  }
}
</script>
