<template>
  <div>
    <h4>コンポーネント その2 子</h4>
    <button @click="$emit('enlarge-text')">
      拡大
    </button>
    <button @click="$emit('shrink-text')">
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
