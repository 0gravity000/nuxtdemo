<template>
  <div>
    <h3>v-on（省略形 @）</h3>
    <p>{{ message }}</p>
    <button @click="reverseMessage">
      Reverse Message
    </button>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      message: 'Hello Vue.js!'
    }
  },
  methods: {
    reverseMessage () {
      this.message = this.message.split('').reverse().join('')
    }
  }
}
</script>
