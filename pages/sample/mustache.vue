<template>
  <div>
    <h3>マスタッシュ構文{{}} Mustache構文(二重中括弧)</h3>
    <p>2重中括弧の mustaches は、データを HTML ではなく、プレーンなテキストとして扱います。</p>
    <p>{{ message }}</p>
    <h4>v-once ディレクティブ</h4>
    <p>v-once ディレクティブを使用することで、データ変更時の更新はおこなわず、一度だけ展開することができます。</p>
    <p>ただし、同じノードのあらゆる他のバインディングが影響を受けることに注意してください</p>
    <span v-once>v-onceは、変化しない: {{ once_message }}</span>
    <h4>生のHTML v-html ディレクティブ</h4>
    <p>実際の HTML として出力するためには、v-html ディレクティブを使用する必要があります</p>
    <p>Using mustaches: {{ rawHtml }}</p>
    <p>Using v-html directive: <span v-html="rawHtml" /></p>
    <p>XSS 脆弱性を容易に引き起こすので、ウェブサイトで動的に任意のHTMLを描画することは、非常に危険です。</p>
    <p>信頼できるコンテンツにだけ HTML 展開を利用してください。ユーザーから提供されたコンテンツに対しては決して使用してはいけません。</p>
    <h4>JavaScript 式の使用</h4>
    <p>JavaScript 式を完全にサポートする。文は動作しない。</p>
    <p>テンプレート式はサンドボックスで、Math や Date といった ホワイトリストにあるグローバルオブジェクト だけにアクセスできます。</p>
    <p>テンプレート式内でユーザーが定義したグローバルオブジェクトにアクセスしようとしてはいけません。</p>
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
  }
}
</script>
