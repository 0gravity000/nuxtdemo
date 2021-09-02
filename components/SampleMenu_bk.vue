<template>
  <div>
    <h4>サンプル</h4>
    <ul>
      <li>
        <button @click="clickSampleMustache">
          マスタッシュ構文 {{}}
        </button>
      </li>
      <li>
        Nested lists:
        <ul>
          <li>are unaffected by this style</li>
          <li>will still show a bullet</li>
          <li>and have appropriate left margin</li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      page: ''
    }
  },
  methods: {
    clickSampleMustache () {
      this.page = 'mustache'
      this.$emit('clickedSamplePage', this.page)
    }
  }
}
</script>

<style>
</style>
