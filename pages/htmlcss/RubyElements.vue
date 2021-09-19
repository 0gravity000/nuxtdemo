<template>
  <div>
    <h3>ルビ関連の要素</h3>

<pre>
1-8-1 ruby要素

<ruby>漢字<rt>かんじ</rt></ruby>

1-8-2 rt要素

<ruby>漢字<rt>かんじ</rt></ruby>

1-8-3 rb要素

<ruby><rb>漢字</rb><rt>かんじ</rt></ruby>
<ruby><rb>漢</rb><rb>字</rb><rt>かん</rt><rt>じ</rt></ruby>

1-8-4 rp要素

<ruby>漢字<rp>（</rp><rt>かんじ</rt><rp>）</rp></ruby>
<ruby><rb>漢</rb><rb>字</rb><rp>（</rp><rt>かん</rt><rt>じ</rt><rp>）</rp></ruby>

1-8-5 rtc要素

<ruby>
    <rb>漢</rb><rb>字</rb>
    <rt>かん</rt><rt>じ</rt>
    <rtc><rt>kan</rt><rt>ji</rt></rtc>
</ruby>
</pre>

  </div>
</template>

<script>
export default {
  layout: 'LayoutHtmlcss',
  data () {
    return {
    }
  }
}
</script>

<style scoped>
</style>
