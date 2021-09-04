<template>
  <div>
    <h3>v-model</h3>
    <p>{{ message }}</p>
    <input v-model="message" size="50">
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      message: 'v-modelは「双方向バインディング」です'
    }
  }
}
</script>
