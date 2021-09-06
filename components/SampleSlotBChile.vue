<template>
  <div>
    <h4>スロット その2 子</h4>
    <div class="container">
      <header>
        <slot name="header" />
      </header>
      <main>
        <slot />
      </main>
      <footer>
        <slot name="footer" />
      </footer>
    </div>
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
