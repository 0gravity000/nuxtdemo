<template>
  <div>
    <h3>スロット その2 親 名前付きスロット</h3>
    <p>v-slotの省略形は#</p>
    <p>slot要素にname属性で指定する</p>
    <SampleSlotBChile>
      <template #header>
        <p>ここにv-slot:headerを表示</p>
      </template>

      <p>name属性のないslot要素は、暗黙的に「default」という名前を持ちます。</p>
      <p>さらにもう1行</p>

      <template #footer>
        <p>ここにv-slot:footerを表示</p>
      </template>
    </SampleSlotBChile>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
    }
  }
}
</script>
