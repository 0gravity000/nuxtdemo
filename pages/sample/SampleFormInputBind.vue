<template>
  <div>
    <h3>フォーム入力バインディング</h3>
    <h4>テキスト</h4>
    <input v-model="message" placeholder="edit me">
    <p>Message is: {{ message }}</p>

    <h4>複数行テキスト</h4>
    <span>Multiline message is:</span>
    <p style="white-space: pre-line;">
      {{ message }}
    </p>
    <br>
    <textarea v-model="message" placeholder="add multiple lines" />

    <h4>チェックボックス 単体</h4>
    <input id="checkbox" v-model="checked" type="checkbox">
    <label for="checkbox">{{ checked }}</label>

    <h4>チェックボックス 複数</h4>
    <input id="jack" v-model="checkedNames" type="checkbox" value="Jack">
    <label for="jack">Jack</label>
    <input id="john" v-model="checkedNames" type="checkbox" value="John">
    <label for="john">John</label>
    <input id="mike" v-model="checkedNames" type="checkbox" value="Mike">
    <label for="mike">Mike</label>
    <br>
    <span>Checked names: {{ checkedNames }}</span>

    <h4>ラジオ</h4>
    <input id="one" v-model="picked" type="radio" value="One">
    <label for="one">One</label>
    <br>
    <input id="two" v-model="picked" type="radio" value="Two">
    <label for="two">Two</label>
    <br>
    <span>Picked: {{ picked }}</span>

    <h4>選択 単体</h4>
    <select v-model="selected">
      <option disabled value="">
        Please select one
      </option>
      <option>A</option>
      <option>B</option>
      <option>C</option>
    </select>
    <span>Selected: {{ selected }}</span>

    <h4>選択 複数（配列にバインド）</h4>
    <select v-model="selected" multiple>
      <option>A</option>
      <option>B</option>
      <option>C</option>
    </select>
    <br>
    <span>Selected: {{ selected }}</span>

    <h4>動的オプションは v-for で描画できます</h4>
    <select v-model="selected">
      <option v-for="option in options" :key="option.value" :value="option.value">
        {{ option.text }}
      </option>
    </select>
    <span>Selected: {{ selected }}</span>

    <h4>値のバインディング</h4>
    <!-- チェックされたとき、`picked` は文字列"a"になります -->
    <input v-model="picked" type="radio" value="a">

    <!-- `toggle` は true かまたは false のどちらかです -->
    <input v-model="toggle" type="checkbox">

    <!-- 最初のオプションが選択されたとき、`selected` は文字列"abc"です -->
    <select v-model="selected">
      <option value="abc">
        ABC
      </option>
    </select>

    <h4>チェックボックス</h4>
    <input
      v-model="toggle"
      type="checkbox"
      true-value="yes"
      false-value="no"
    >

    <h4>ラジオ</h4>
    <input v-model="pick" type="radio" :value="a">

    <h4>選択オプション</h4>
    <select v-model="selected">
      <!-- インラインオブジェクトリテラル -->
      <option :value="{ number: 123 }">
        123
      </option>
    </select>

    <h4>修飾子 .lazy</h4>
    <!-- "input" の代わりに "change" 後に同期します -->
    <input v-model.lazy="msg">

    <h4>修飾子 .number</h4>
    <input v-model.number="age" type="number">

    <h4>修飾子 .trim</h4>
    <input v-model.trim="msg">
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      checkedNames: [],
      selected: 'A',
      options: [
        { text: 'One', value: 'A' },
        { text: 'Two', value: 'B' },
        { text: 'Three', value: 'C' }
      ]
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
