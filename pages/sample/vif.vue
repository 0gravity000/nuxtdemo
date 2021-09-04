<template>
  <div>
    <h3>v-if</h3>
    <span v-if="seen">Now you see me</span>
    <div>
      <button @click="clickBtn">
        クリックすると表示/非表示が切り替わる
      </button>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'sample',
  data () {
    return {
      seen: true
    }
  },
  methods: {
    clickBtn () {
      this.seen = !(this.seen)
    }
  }
}
</script>
