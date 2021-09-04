<template>
  <div>
    <h3>ライフサイクルフック</h3>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      message: '調査中'
    }
  }
  /*
  beforeCreate () {
    this.message = 'beforeCreate'
  },
  created () {
    this.message = 'created'
  }
  beforeMount () {
    this.message = 'beforeMount'
  },
  mounted () {
    this.message = 'mounted'
  },
  beforeUpdate () {
    this.message = 'beforeUpdate'
  },
  updated () {
    this.message = 'updated'
  },
  beforeDestroy () {
    this.message = 'beforeDestroy'
  },
  destroyed () {
    this.message = 'destroyed'
  }
  */
}
</script>
