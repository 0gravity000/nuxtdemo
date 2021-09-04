<template>
  <div>
    <h3>v-bind:class（省略形 :class）</h3>
    <div :class="{ active: isActive }">
      isActiveの値：{{ isActive }}
    </div>
    <button @click="btnClicked">
      activeを切替
    </button>

    <h4>プレーンな class 属性と共存できる</h4>
    <div
      class="static"
      :class="{ active: isActive, 'text-danger': hasError }"
    >
      isActiveの値：{{ isActive }}、hasErrorの値：{{ hasError }}
    </div>

    <h4>束縛されるオブジェクトはインラインでなくてもOK</h4>
    <div :class="classObject">
      クラス属性のオブジェクト
    </div>

    <h4>オブジェクトを返す算出プロパティにbindすることもできる</h4>
    <div :class="computedClassObject">
      算出プロパティ クラス属性のオブジェクト
    </div>

    <h4>配列構文</h4>
    <p>配列を渡してクラスのリストを適用することができます</p>
    <div :class="[activeClass, errorClass]">
      配列クラスのオブジェクト
    </div>

    <h4>カスタムコンポーネントでclass 属性を使用</h4>
    <p>これらのクラスはコンポーネントの root 要素 に追加されます。この要素上に存在するクラスは、上書きされません。</p>
    <a :href="urlpath">リンク</a>
    <a href="https://jp.vuejs.org/v2/guide/class-and-style.html#%E3%82%B3%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%8D%E3%83%B3%E3%83%88%E3%81%AB%E3%81%8A%E3%81%84%E3%81%A6">リンク</a>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      classObject: {
        active: true,
        'text-danger': false
      },
      isActive: true,
      hasError: false,
      error: null,
      activeClass: 'active',
      errorClass: 'text-danger',
      urlpath: 'https://jp.vuejs.org/v2/guide/class-and-style.html#%E3%82%B3%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%8D%E3%83%B3%E3%83%88%E3%81%AB%E3%81%8A%E3%81%84%E3%81%A6'
    }
  },
  computed: {
    computedClassObject () {
      return {
        isActive: this.isActive && !this.error,
        'text-danger': this.error && this.error.type === 'fatal'
      }
    }
  },
  methods: {
    btnClicked () {
      this.isActive = !this.isActive
    }
  }
}
</script>

<style scoped>
  .active {
    color: red;
  }
</style>
