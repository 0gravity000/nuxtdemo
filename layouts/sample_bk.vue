<template>
  <div>
    <NaviHeader />
    <div class="container">
      <div class="row my-2">
        <div class="col-4">
          <SampleMenu
            @clickedSamplePage="showSamplePage"
          />
        </div>
        <div class="col">
          <Nuxt
            :content="page"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      page: 'mustache'
    }
  },
  methods: {
    showSamplePage (page) {
      this.page = page
      // alert(page);
    }
  }
}
</script>
