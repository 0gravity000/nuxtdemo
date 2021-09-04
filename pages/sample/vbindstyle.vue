<template>
  <div>
    <h3>v-bind:style（省略形 :style）</h3>
    <p>CSS のプロパティ名には、キャメルケースまたはケバブケースのどちらでも使用することができます</p>
    <div :style="{ color: activeColor, fontSize: fontSize + 'px' }">
      スタイルの例1
    </div>
    <div :style="styleObject">
      スタイルの例2
    </div>

    <h4>配列構文</h4>
    <div :style="[baseStyles, overridingStyles]">
      配列でスタイル設定
    </div>
  </div>
</template>

<script>
export default {
  layout: 'sample',
  data () {
    return {
      activeColor: 'red',
      fontSize: 20,
      styleObject: {
        color: 'red',
        fontSize: '13px'
      }
    }
  }
}
</script>
