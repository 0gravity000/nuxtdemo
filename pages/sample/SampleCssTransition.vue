<template>
  <div>
    <h3>CSSトランジション</h3>
    <button @click="show = !show">
      Toggle render
    </button>
    <transition name="slide-fade">
      <p v-if="show">
        hello
      </p>
    </transition>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      show: true
    }
  }
}
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all 1.5s ease;
}
.slide-fade-leave-active {
  transition: all 1.5s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */ {
  transform: translateX(100px);
  opacity: 0;
}
</style>
