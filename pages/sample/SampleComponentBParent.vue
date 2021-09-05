<template>
  <div>
    <h3>コンポーネント その2 親</h3>
    <h4>子->親へデータ受け渡し $emitメソッド</h4>
    <SampleComponentBChild
      @enlarge-text="postFontSize += $event"
      @shrink-text="onShrinkText"
    />
    <div :style="{ fontSize: postFontSize + 'em' }">
      テキスト
    </div>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      postFontSize: 1
    }
  },
  methods: {
    onEnlargeText (enlargeAmount) {
      this.postFontSize += enlargeAmount
    },
    onShrinkText (enlargeAmount) {
      this.postFontSize -= enlargeAmount
    }
  }
}
</script>
