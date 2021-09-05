<template>
  <div>
    <h3>コンポーネント その1 親</h3>
    <h4>親->子へデータ受け渡し プロパティ props</h4>
    <SampleComponentAChild
      :comptitle="ptitle"
      :compposts="posts"
    />
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      ptitle: '親タイトル',
      posts: [
        { id: 1, title: 'My journey with Vue' },
        { id: 2, title: 'Blogging with Vue' },
        { id: 3, title: 'Why Vue is so fun' }
      ]
    }
  }
}
</script>
