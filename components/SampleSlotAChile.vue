<template>
  <div>
    <h4>スロット その1 子</h4>
    <a
      :href="url"
      class="nav-link"
    >
      スロットを表示:<slot />
    </a>
  </div>
</template>

<script>
export default {
  data () {
    return {
      url: ''
    }
  }
}
</script>
