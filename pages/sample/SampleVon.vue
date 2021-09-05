<template>
  <div>
    <h3>v-on（省略形 @）</h3>
    <p>{{ message }}</p>
    <button @click="reverseMessage">
      Reverse Message
    </button>

    <h4>イベント その1</h4>
    <button @click="counter += 1">
      Add 1
    </button>
    <p>The button above has been clicked {{ counter }} times.</p>

    <h4>イベント その2</h4>
    <!-- `greet` は、あらかじめ定義したメソッドの名前 -->
    <button @click="greet">
      Greet
    </button>

    <h4>イベント その3</h4>
    <button @click="say('hi')">
      Say hi
    </button>
    <button @click="say('what')">
      Say what
    </button>

    <h4>イベント その4</h4>
    <button @click="warn('Form cannot be submitted yet.', $event)">
      Submit
    </button>

    <h4>イベント修飾子</h4>
    <!-- クリックイベントの伝搬が止まります -->
    <a @click.stop="doThis">
      stop
    </a>
    <!-- submit イベントによってページがリロードされません -->
    <form @submit.prevent="onSubmit">
      prevent
    </form>
    <!-- 修飾子は繋げることができます -->
    <a @click.stop.prevent="doThat">
      stop.prevent
    </a>
    <!-- 値を指定せず、修飾子だけ利用することもできます -->
    <form @submit.prevent>
      submit.prevent
    </form>
    <!-- イベントリスナーを追加するときにキャプチャモードで使います -->
    <!-- 言い換えれば、内部要素を対象とするイベントは、その要素によって処理される前にここで処理されます -->
    <div @click.capture="doThis">
      capture
    </div>
    <!-- event.target が要素自身のときだけ、ハンドラが呼び出されます -->
    <!-- 言い換えると子要素のときは呼び出されません -->
    <div @click.self="doThat">
      self
    </div>
    <!-- 2.1.4 から新規 -->
    <!-- 最大1回、クリックイベントはトリガされます -->
    <a @click.once="doThis">
      once
    </a>
    <!-- 2.3.0 で新規追加 -->
    <!-- addEventListener の passive オプションに対応する .passive 修飾子も提供しています。 -->
    <!-- `onScroll` が `event.preventDefault()` を含んでいたとしても -->
    <!-- スクロールイベントのデフォルトの挙動(つまりスクロール)は -->
    <!-- イベントの完了を待つことなくただちに発生するようになります -->
    <div @scroll.passive="onScroll">
      scroll.passive
    </div>

    <h4>キー修飾子</h4>
    <!-- `key` が `Enter` のときだけ、`vm.submit()` が呼ばれます  -->
    <input @keyup.enter="submit">
    <!-- KeyboardEvent.key で公開されている任意のキー名は、ケバブケースに変換することで修飾子として直接使用できます。  -->
    <!-- ハンドラは $event.key が 'PageDown' に等しい場合だけ呼ばれます。  -->
    <input @keyup.page-down="onPageDown">

    <h4>キーコード</h4>
    .enter
    .tab
    .delete (“Delete” と “Backspace” キー両方をキャプチャします)
    .esc
    .space
    .up
    .down
    .left
    .right
    <input @keyup.13="submit">

    <h4>システム修飾子キー</h4>
    .ctrl
    .alt
    .shift
    .meta
    <!-- Alt + C -->
    <input @keyup.alt.67="clear">
    <!-- Ctrl + Click -->
    <div @click.ctrl="doSomething">
      Do something
    </div>

    <h4>.exact 修飾子 2.5.0 で新規追加</h4>
    <!-- これは Ctrl に加えて Alt や Shift キーが押されていても発行されます -->
    <button @click.ctrl="onClick">
      A
    </button>
    <!-- これは Ctrl キーが押され、他のキーが押されてないときだけ発行されます -->
    <button @click.ctrl.exact="onCtrlClick">
      A
    </button>
    <!-- これは システム修飾子が押されてないときだけ発行されます -->
    <button @click.exact="onClick">
      A
    </button>

    <h4>マウスボタンの修飾子 2.2.0 からの新機能</h4>
    .left
    .right
    .middle
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      message: 'Hello Vue.js!',
      counter: 0,
      name: 'Vue.js'
    }
  },
  methods: {
    reverseMessage () {
      this.message = this.message.split('').reverse().join('')
    },
    greet (event) {
      // メソッド内の `this` は、 Vue インスタンスを参照します
      alert('Hello ' + this.name + '!')
      // `event` は、ネイティブ DOM イベントです
      if (event) {
        alert(event.target.tagName)
      }
    },
    say (message) {
      alert(message)
    },
    warn (message, event) {
      // ネイティブイベントを参照しています
      if (event) {
        event.preventDefault()
      }
      alert(message)
    }
  }
}
</script>
