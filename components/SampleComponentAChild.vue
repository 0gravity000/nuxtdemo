<template>
  <div>
    <h4>コンポーネント その1 子</h4>
    {{ comptitle }}

    {{ compposts }}

    <div v-for="post in compposts" :key="post.id">
      {{ post.id }}:{{ post.title }}
    </div>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  props: {
    comptitle: {
      type: String,
      required: true
    },
    compposts: {
      type: Array,
      required: true
    }
  },
  data () {
    return {
    }
  }
}
</script>
