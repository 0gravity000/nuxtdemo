<template>
  <div>
    <h3>マスタッシュ構文{{}}</h3>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  layout: 'sample',
  data () {
    return {
      message: 'これはメッセージ'
    }
  }
}
</script>
