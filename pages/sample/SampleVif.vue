<template>
  <div>
    <h3>v-if</h3>
    <h4>v-if/v-else</h4>
    <p>v-else 要素は、v-if または v-else-if 要素の直後になければなりません。それ以外の場合は認識されません。</p>
    <span v-if="seen">seenは{{ seen }}</span>
    <span v-else>seenは{{ seen }}</span>
    <div>
      <button @click="clickBtn">
        クリックすると値が切り替わる
      </button>
    </div>

    <h4>v-else-if バージョン2.1.0 から</h4>
    <div v-if="type === 'A'">
      A
    </div>
    <div v-else-if="type === 'B'">
      B
    </div>
    <div v-else-if="type === 'C'">
      C
    </div>
    <div v-else>
      Not A/B/C
    </div>

    <h4>key属性による再利用可能な要素の制御</h4>
    <a :href="pagelink">
      リンク
    </a>
    <h4>v-if vs v-show</h4>
    <p>一般的に、v-if はより高い切り替えコストを持っているのに対して、 v-show はより高い初期描画コストを持っています。 </p>
    <p>とても頻繁に何かを切り替える必要があれば v-show を選び、条件が実行時に変更することがほとんどない場合は、v-if を選びます。</p>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      seen: true,
      type: 'A',
      pagelink: 'https://jp.vuejs.org/v2/guide/conditional.html#key-%E3%81%AB%E3%82%88%E3%82%8B%E5%86%8D%E5%88%A9%E7%94%A8%E5%8F%AF%E8%83%BD%E3%81%AA%E8%A6%81%E7%B4%A0%E3%81%AE%E5%88%B6%E5%BE%A1'
    }
  },
  methods: {
    clickBtn () {
      this.seen = !(this.seen)
    }
  }
}
</script>
