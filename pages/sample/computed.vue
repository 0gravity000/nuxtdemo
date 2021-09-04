<template>
  <div>
    <h3>算出プロパティ</h3>
    <p>もとのメッセージ: "{{ message }}"</p>
    <p>算出プロパティでリバースしたメッセージ: "{{ reversedMessage }}"</p>

    <h4>算出プロパティ vs メソッド</h4>
    <p>算出プロパティの代わりに、同じような関数をメソッドとして定義することも可能です。</p>
    <p>算出プロパティ：</p>
    <p>message が変わらない限りは、reversedMessage に何度アクセスしても、関数を再び実行することなく以前計算された結果を即時に返すということです。</p>
    <p>算出プロパティは、リアクティブな依存関係が更新されたときにだけ再評価されます。</p>
    <p>メソッド：</p>
    <p>対称的に、メソッド呼び出しは、再描画が起きると常に関数を実行します。</p>
  </div>
</template>

<script>
export default {
  layout: 'sample',
  data () {
    return {
      message: 'これはメッセージ',
      once_message: 'これはv-onceのメッセージ',
      rawHtml: '<span style="color:red">これは赤色</span>'
    }
  },
  computed: {
    // 算出 getter 関数
    reversedMessage () {
      // `this` は vm インスタンスを指します
      return this.message.split('').reverse().join('')
    }
  }
}
</script>
